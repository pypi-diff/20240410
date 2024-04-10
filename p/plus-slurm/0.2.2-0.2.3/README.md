# Comparing `tmp/plus_slurm-0.2.2.tar.gz` & `tmp/plus_slurm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plus_slurm-0.2.2.tar", last modified: Mon Apr  8 14:16:00 2024, max compression
+gzip compressed data, was "plus_slurm-0.2.3.tar", last modified: Tue Apr  9 12:07:36 2024, max compression
```

## Comparing `plus_slurm-0.2.2.tar` & `plus_slurm-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.266187 plus_slurm-0.2.2/
--rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.2.2/LICENSE
--rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.2.2/MANIFEST.in
--rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-08 14:16:00.265187 plus_slurm-0.2.2/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.2.2/README.md
--rw-r--r--   0 th        (1011) th        (1011)        5 2024-04-08 14:15:44.000000 plus_slurm-0.2.2/VERSION
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.263187 plus_slurm-0.2.2/plus_slurm/
--rw-r--r--   0 th        (1011) th        (1011)      949 2023-05-05 12:37:55.000000 plus_slurm-0.2.2/plus_slurm/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.264187 plus_slurm-0.2.2/plus_slurm/jinja2_templates/
--rw-r--r--   0 th        (1011) th        (1011)     3040 2023-04-27 11:56:08.000000 plus_slurm-0.2.2/plus_slurm/jinja2_templates/runner.py
--rw-r--r--   0 th        (1011) th        (1011)      521 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/plus_slurm/jinja2_templates/submit.sh
--rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.2.2/plus_slurm/job.py
--rw-r--r--   0 th        (1011) th        (1011)    17289 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/plus_slurm/jobcluster.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.263187 plus_slurm-0.2.2/plus_slurm.egg-info/
--rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      408 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1011) th        (1011)        1 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1011) th        (1011)       45 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/requires.txt
--rw-r--r--   0 th        (1011) th        (1011)       11 2024-04-08 14:16:00.000000 plus_slurm-0.2.2/plus_slurm.egg-info/top_level.txt
--rw-r--r--   0 th        (1011) th        (1011)       38 2024-04-08 14:16:00.266187 plus_slurm-0.2.2/setup.cfg
--rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.2.2/setup.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-08 14:16:00.265187 plus_slurm-0.2.2/tests/
--rw-r--r--   0 th        (1011) th        (1011)     1392 2023-04-27 11:52:36.000000 plus_slurm-0.2.2/tests/test_nested_jobs.py
--rw-r--r--   0 th        (1011) th        (1011)     8453 2024-04-08 14:15:25.000000 plus_slurm-0.2.2/tests/test_plus_slurm.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-09 12:07:36.509960 plus_slurm-0.2.3/
+-rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.2.3/LICENSE
+-rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.2.3/MANIFEST.in
+-rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-09 12:07:36.509960 plus_slurm-0.2.3/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.2.3/README.md
+-rw-r--r--   0 th        (1011) th        (1011)        5 2024-04-09 12:07:22.000000 plus_slurm-0.2.3/VERSION
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-09 12:07:36.507959 plus_slurm-0.2.3/plus_slurm/
+-rw-r--r--   0 th        (1011) th        (1011)      949 2023-05-05 12:37:55.000000 plus_slurm-0.2.3/plus_slurm/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-09 12:07:36.507959 plus_slurm-0.2.3/plus_slurm/jinja2_templates/
+-rw-r--r--   0 th        (1011) th        (1011)     3040 2023-04-27 11:56:08.000000 plus_slurm-0.2.3/plus_slurm/jinja2_templates/runner.py
+-rw-r--r--   0 th        (1011) th        (1011)      521 2024-04-08 14:15:25.000000 plus_slurm-0.2.3/plus_slurm/jinja2_templates/submit.sh
+-rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.2.3/plus_slurm/job.py
+-rw-r--r--   0 th        (1011) th        (1011)    17523 2024-04-09 12:07:14.000000 plus_slurm-0.2.3/plus_slurm/jobcluster.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-09 12:07:36.507959 plus_slurm-0.2.3/plus_slurm.egg-info/
+-rw-r--r--   0 th        (1011) th        (1011)     1170 2024-04-09 12:07:36.000000 plus_slurm-0.2.3/plus_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      408 2024-04-09 12:07:36.000000 plus_slurm-0.2.3/plus_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1011) th        (1011)        1 2024-04-09 12:07:36.000000 plus_slurm-0.2.3/plus_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1011) th        (1011)       45 2024-04-09 12:07:36.000000 plus_slurm-0.2.3/plus_slurm.egg-info/requires.txt
+-rw-r--r--   0 th        (1011) th        (1011)       11 2024-04-09 12:07:36.000000 plus_slurm-0.2.3/plus_slurm.egg-info/top_level.txt
+-rw-r--r--   0 th        (1011) th        (1011)       38 2024-04-09 12:07:36.509960 plus_slurm-0.2.3/setup.cfg
+-rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.2.3/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2024-04-09 12:07:36.508959 plus_slurm-0.2.3/tests/
+-rw-r--r--   0 th        (1011) th        (1011)     1392 2023-04-27 11:52:36.000000 plus_slurm-0.2.3/tests/test_nested_jobs.py
+-rw-r--r--   0 th        (1011) th        (1011)     8453 2024-04-08 14:15:25.000000 plus_slurm-0.2.3/tests/test_plus_slurm.py
```

### Comparing `plus_slurm-0.2.2/LICENSE` & `plus_slurm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/PKG-INFO` & `plus_slurm-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plus_slurm
-Version: 0.2.2
+Version: 0.2.3
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plus_slurm-0.2.2/plus_slurm/__init__.py` & `plus_slurm-0.2.3/plus_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/plus_slurm/jinja2_templates/runner.py` & `plus_slurm-0.2.3/plus_slurm/jinja2_templates/runner.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/plus_slurm/jinja2_templates/submit.sh` & `plus_slurm-0.2.3/plus_slurm/jinja2_templates/submit.sh`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/plus_slurm/job.py` & `plus_slurm-0.2.3/plus_slurm/job.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/plus_slurm/jobcluster.py` & `plus_slurm-0.2.3/plus_slurm/jobcluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     max_jobs_per_jobcluster : :class:`int`, optional
         Slurm only allows a certain number of jobs per array job
         (1000 by default).
         If the number of jobs to be submitted is higher that this number, jobs
         will be split in more than one array job.
     append_to_path : :class:`str`, optional
         Path to append to the python module search path.
-    extra_slurm_args : class:`list`, optional
+    extra_slurm_args :class:`list`, optional
         Extra arguments for slurm sbatch. These get appended as is with
         the `#SBATCH` prefix.
     """
 
     _slurm_submit = '/usr/bin/sbatch'
     _runner_template = 'runner.py'
     _submit_template = 'submit.sh'
@@ -457,15 +457,20 @@
         if mount_slurm_folders:
             for mnt in self._slurm_folders:
                 if mnt not in self._mounts:
                     self._mounts.append(mnt)
 
     @property
     def apptainer_command(self):
-        return '/usr/bin/singularity'
+        if Path('/usr/bin/apptainer').is_file():
+            return '/usr/bin/apptainer'
+        elif Path('/usr/bin/singularity').is_file():
+            return '/usr/bin/singularity'
+        else:
+            raise RuntimeError('Neither apptainer nor singularity found.')
 
     @property
     def apptainer_arguments(self):
         cmd_list = ['exec']
         for mnt in self._mounts:
             cmd_list.append(f'-B {mnt}')
```

### Comparing `plus_slurm-0.2.2/plus_slurm.egg-info/PKG-INFO` & `plus_slurm-0.2.3/plus_slurm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plus-slurm
-Version: 0.2.2
+Version: 0.2.3
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plus_slurm-0.2.2/setup.py` & `plus_slurm-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/tests/test_nested_jobs.py` & `plus_slurm-0.2.3/tests/test_nested_jobs.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.2.2/tests/test_plus_slurm.py` & `plus_slurm-0.2.3/tests/test_plus_slurm.py`

 * *Files identical despite different names*

