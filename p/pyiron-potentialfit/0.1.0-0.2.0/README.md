# Comparing `tmp/pyiron_potentialfit-0.1.0.tar.gz` & `tmp/pyiron_potentialfit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_potentialfit-0.1.0.tar", last modified: Thu Feb 22 09:43:05 2024, max compression
+gzip compressed data, was "pyiron_potentialfit-0.2.0.tar", last modified: Wed Apr 10 09:12:40 2024, max compression
```

## Comparing `pyiron_potentialfit-0.1.0.tar` & `pyiron_potentialfit-0.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.289207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.293207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/atomicrex_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/function_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/general_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/potential_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    33964 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/structure_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.293207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.293207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.293207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/meamfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/meamfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/meamfit/meamfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.293207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/ml/potentialfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/cfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/masters.py
--rw-r--r--   0 runner    (1001) docker     (127)    30229 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/mlip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/mlipdescriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/pacemaker/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/storageclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-22 09:43:05.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-22 09:43:05.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 09:43:05.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 09:43:05.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-22 09:43:05.000000 pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-22 09:43:05.297207 pyiron_potentialfit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-22 09:43:04.000000 pyiron_potentialfit-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-02-22 09:43:00.000000 pyiron_potentialfit-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/pyiron_potentialfit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/atomicrex_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/function_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/general_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/potential_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33964 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/structure_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.404718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/meamfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/potentialfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/masters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlipdescriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/storageclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:12:40.408718 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-10 09:12:40.412719 pyiron_potentialfit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 09:12:40.000000 pyiron_potentialfit-0.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-10 09:12:38.000000 pyiron_potentialfit-0.2.0/versioneer.py
```

### Comparing `pyiron_potentialfit-0.1.0/LICENSE` & `pyiron_potentialfit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/PKG-INFO` & `pyiron_potentialfit-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
 Requires-Dist: pyiron_atomistics>=0.4.16
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyiron_base>=0.7.9
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: runnerase>=0.3.3
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/__init__.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/base.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/fit_properties.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/fit_properties.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/function_factory.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/function_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/general_input.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/general_input.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/interactive.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/parameter_constraints.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/potential_factory.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/potential_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/structure_list.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/structure_list.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomicrex/utility_functions.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomicrex/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/atomistics/job/trainingcontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/meamfit/meamfit.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/meamfit/meamfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/ml/potentialfit.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/ml/potentialfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/cfgs.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/cfgs.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/lammps.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/lammps.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         if self.input.mlip["mtp-filename"] == "auto":
             self.input.mlip["mtp-filename"] = os.path.basename(
                 self.potential["Filename"][0][0]
             )
         self.input.mlip.write_file(file_name="mlip.ini", cwd=self.working_directory)
 
     def convergence_check(self):
-        for line in self["error.out"]:
+        if self.files["error.out"] is None:
+            return True
+        for line in self.files["error.out"]:
             if line.startswith("MLIP: Breaking threshold exceeded"):
                 return False
         return True
 
     def enable_active_learning(self, threshold=2.0, threshold_break=5.0):
         """
         Enable active learning during MD run.
@@ -165,35 +167,23 @@
 
 
 class MlipInput(Input):
     def __init__(self):
         self.mlip = MlipParameter()
         super(MlipInput, self).__init__()
 
-    def to_hdf(self, hdf5):
-        """
-
-        Args:
-            hdf5:
-        Returns:
-        """
-        with hdf5.open("input") as hdf5_input:
-            self.mlip.to_hdf(hdf5_input)
-        super(MlipInput, self).to_hdf(hdf5)
-
-    def from_hdf(self, hdf5):
-        """
-
-        Args:
-            hdf5:
-        Returns:
-        """
-        with hdf5.open("input") as hdf5_input:
-            self.mlip.from_hdf(hdf5_input)
-        super(MlipInput, self).from_hdf(hdf5)
+    def to_dict(self):
+        data_dict = super().to_dict()
+        for k, v in self.mlip.to_dict().items():
+            data_dict[self.mlip.table_name + "/" + k] = v
+        return data_dict
+
+    def from_dict(self, data_dict):
+        super().from_dict(data_dict)
+        self.mlip.from_dict(data_dict[self.mlip.table_name])
 
 
 class MlipParameter(GenericParameters):
     def __init__(self, separator_char=" ", comment_char="#", table_name="mlip_inp"):
         super(MlipParameter, self).__init__(
             separator_char=separator_char,
             comment_char=comment_char,
```

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/masters.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/masters.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/mlip.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlip.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         if self.status.finished:
             return pd.DataFrame(
                 {
                     "Name": ["".join(elements)],
                     "Filename": [self.potential_files],
                     "Model": ["Custom"],
-                    "Species": [elements],
+                    "Species": [list(map(str, elements))],
                     "Config": [["pair_style mlip mlip.ini\n", "pair_coeff * *\n"]],
                 }
             )
         else:
             raise ValueError(
                 f"Potential only available after job is finished, not {self.status}!"
             )
```

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/mlipdescriptors.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/mlipdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/parser.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/mlip/potential.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/mlip/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/pacemaker/job.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/pacemaker/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             )
 
         with self.project_hdf5.open("output") as hdf5_output:
             training_data_ts.to_hdf(hdf=hdf5_output, group_name="training_data")
             predicted_data_fs.to_hdf(hdf=hdf5_output, group_name="predicted_data")
 
     def get_lammps_potential(self):
-        elements_name = self["output/potential/elements_name"]
+        elements_name = self.project_hdf5["output/potential/elements_name"]
         elem = " ".join(elements_name)
         pot_file_name = self.get_final_potential_filename_ace()
         pot_dict = {
             "Config": [
                 [
                     "pair_style pace\n",
                     "pair_coeff  * * {} {}\n".format(pot_file_name, elem),
@@ -424,18 +424,18 @@
     def _add_training_data(self, container: TrainingContainer) -> None:
         self.add_job_to_fitting(container.id)
 
     def add_job_to_fitting(self, job_id, *args, **kwargs):
         self._train_job_id_list.append(job_id)
 
     def _get_training_data(self) -> TrainingStorage:
-        return self["output/training_data"].to_object()
+        return self.project_hdf5["output/training_data"].to_object()
 
     def _get_predicted_data(self) -> FlattenedStorage:
-        return self["output/predicted_data"].to_object()
+        return self.project_hdf5["output/predicted_data"].to_object()
 
     # copied/adapted from mlip.py
     def create_training_dataframe(
         self, _train_job_id_list: List = None
     ) -> pd.DataFrame:
         if _train_job_id_list is None:
             _train_job_id_list = self._train_job_id_list
```

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/job.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/storageclasses.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/storageclasses.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit/runner/utils.py` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit/runner/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/PKG-INFO` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: ase>=3.22.1
 Requires-Dist: pyiron_atomistics>=0.4.16
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyiron_base>=0.7.9
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: runnerase>=0.3.3
 
 http://pyiron.org
```

### Comparing `pyiron_potentialfit-0.1.0/pyiron_potentialfit.egg-info/SOURCES.txt` & `pyiron_potentialfit-0.2.0/pyiron_potentialfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.1.0/setup.py` & `pyiron_potentialfit-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
         'ase>=3.22.1',
         'pyiron_atomistics>=0.4.16',
-        'matplotlib>=3.8.2',
-        'numpy>=1.26.2',
+        'matplotlib>=3.8.3',
+        'numpy>=1.26.4',
         'pyiron_base>=0.7.9',
         'scipy>=1.11.4',
         'runnerase>=0.3.3',
     ],
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pyiron_potentialfit-0.1.0/versioneer.py` & `pyiron_potentialfit-0.2.0/versioneer.py`

 * *Files identical despite different names*

