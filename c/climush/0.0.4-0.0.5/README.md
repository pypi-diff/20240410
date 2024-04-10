# Comparing `tmp/climush-0.0.4.tar.gz` & `tmp/climush-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climush-0.0.4.tar", last modified: Sun Apr  7 03:02:36 2024, max compression
+gzip compressed data, was "climush-0.0.5.tar", last modified: Wed Apr 10 18:24:23 2024, max compression
```

## Comparing `climush-0.0.4.tar` & `climush-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 03:02:36.691966 climush-0.0.4/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2135 2024-04-07 03:02:36.691713 climush-0.0.4/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.4/README.md
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 03:02:36.690319 climush-0.0.4/climush/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.4/climush/__init__.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.4/climush/binfo_old.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    64710 2024-04-04 05:28:28.000000 climush-0.0.4/climush/bioinfo.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.4/climush/config.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.4/climush/constants.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    43925 2024-03-21 06:50:22.000000 climush-0.0.4/climush/utilities.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.4/climush/viz.py
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 03:02:36.691454 climush-0.0.4/climush.egg-info/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2135 2024-04-07 03:02:36.000000 climush-0.0.4/climush.egg-info/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      313 2024-04-07 03:02:36.000000 climush-0.0.4/climush.egg-info/SOURCES.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-04-07 03:02:36.000000 climush-0.0.4/climush.egg-info/dependency_links.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       50 2024-04-07 03:02:36.000000 climush-0.0.4/climush.egg-info/requires.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-04-07 03:02:36.000000 climush-0.0.4/climush.egg-info/top_level.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      929 2024-04-07 03:01:07.000000 climush-0.0.4/pyproject.toml
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-04-07 03:02:36.692020 climush-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:24:23.775665 climush-0.0.5/
+-rw-r--r--   0 root         (0) staff       (20)     2135 2024-04-10 18:24:23.775481 climush-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:24:23.774556 climush-0.0.5/climush/
+-rw-r--r--   0 root         (0) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.5/climush/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.5/climush/binfo_old.py
+-rw-r--r--   0 root         (0) staff       (20)    64734 2024-04-10 02:05:17.000000 climush-0.0.5/climush/bioinfo.py
+-rw-r--r--   0 root         (0) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.5/climush/config.py
+-rw-r--r--   0 root         (0) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.5/climush/constants.py
+-rw-r--r--   0 root         (0) staff       (20)    44339 2024-04-10 09:04:59.000000 climush-0.0.5/climush/utilities.py
+-rw-r--r--   0 root         (0) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.5/climush/viz.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-10 18:24:23.775297 climush-0.0.5/climush.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     2135 2024-04-10 18:24:23.000000 climush-0.0.5/climush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      313 2024-04-10 18:24:23.000000 climush-0.0.5/climush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-10 18:24:23.000000 climush-0.0.5/climush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       50 2024-04-10 18:24:23.000000 climush-0.0.5/climush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        8 2024-04-10 18:24:23.000000 climush-0.0.5/climush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      929 2024-04-10 18:22:47.000000 climush-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-10 18:24:23.775702 climush-0.0.5/setup.cfg
```

### Comparing `climush-0.0.4/PKG-INFO` & `climush-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `climush-0.0.4/README.md` & `climush-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `climush-0.0.4/climush/binfo_old.py` & `climush-0.0.5/climush/binfo_old.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.4/climush/bioinfo.py` & `climush-0.0.5/climush/bioinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,26 +602,26 @@
                             '-a', f'^{rev_primer}...{fwd_revcomp_primer}$',
                             '-n', '2', '-e', str(max_err), untrim_cmd, '-o', trim_out, file]
 
             # create or append to cutadapt stderr/stdout, all output goes to one file (not one per sample)
             run_subprocess(cutadapt_cmd, dest_dir=trim_primers_parent)
 
     # quantify proportion untrimmed
-    with open((trim_primers_parent / 'cutadapt.out'), 'r') as fin:
-        cutadapt_df = pd.read_table(fin)
-        sum_in = cutadapt_df['in_reads'].sum(0)
-        sum_out = cutadapt_df['out_reads'].sum(0)
-        percent_lost = ((sum_in - sum_out) / (sum_in)) * 100
-        if percent_lost > max_untrimmed:
-            msg = f'After primer trimming, {percent_lost:.2f}% of the input reads were lost, which is ' \
-                  f'above the user-defined maximum threshold of {max_untrimmed}%.\n'
-            exit_process(message=msg)
-        else:
-            print(f'{percent_lost:.2f}% of input reads were lost to primer trimming. This is above the user-provided '
-                  f'input of {max_untrimmed}%, so proceeding to next step...\n')
+    # with open((trim_primers_parent / 'cutadapt.out'), 'r') as fin:
+    #     cutadapt_df = pd.read_table(fin)
+    #     sum_in = cutadapt_df['in_reads'].sum(0)
+    #     sum_out = cutadapt_df['out_reads'].sum(0)
+    #     percent_lost = ((sum_in - sum_out) / (sum_in)) * 100
+    #     if percent_lost > max_untrimmed:
+    #         msg = f'After primer trimming, {percent_lost:.2f}% of the input reads were lost, which is ' \
+    #               f'above the user-defined maximum threshold of {max_untrimmed}%.\n'
+    #         exit_process(message=msg)
+    #     else:
+    #         print(f'{percent_lost:.2f}% of input reads were lost to primer trimming. This is above the user-provided '
+    #               f'input of {max_untrimmed}%, so proceeding to next step...\n')
 
     return None
 
 def merge_reads(input_files, file_map):
     settings = import_config_as_dict(file_path=file_map['config']['main'], file_handle='pipeline-settings')
     run_name = settings['run_details']['run_name']
```

### Comparing `climush-0.0.4/climush/constants.py` & `climush-0.0.5/climush/constants.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.4/climush/utilities.py` & `climush-0.0.5/climush/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import subprocess, re, sys, pathlib, tomlkit
+import subprocess, re, sys, pathlib, shutil, json
+# import tomlkit
 from pathlib import Path
 from datetime import datetime
 from functools import wraps
-import shutil
 import pandas as pd
 from climush.constants import *
 
 # tried to order by category but some required specific order due to dependencies on other functions
 
 #######################
 # MISC UTILITIES ######
@@ -114,14 +114,28 @@
         if re.search(AFFIRM_REGEX, to_next, re.I):
             print(f'\n\nRunning next step, {next_script.name}...\n')
             subprocess.run(['python3', next_script])
             return None
         else:
             return print(f'\n\nExiting the completed step, {current_script}.\n')
 
+# log progress of bioinformatics pipeline
+def log_progress(file_map, run_name):
+    log_file = file_map['pipeline-output']['summary'] / f'log_{run_name}.json'
+
+    log_dict = {'run_name': run_name,
+                'error': {'script':'04_quality-filtering',
+                          'function':''}
+                }
+
+    with open(log_file, 'at') as log_out:
+        log_out.write(json.dumps(log_dict))
+
+
+
 # exit current script due to error, save script and timestamp of where error occurred
 def exit_process(message, config_section='error.message'):
     script_name = sys.argv[0]  # unsure if will get name of script it is executed in or the one it is compiled in
     exit_time = datetime.today().strftime('%Y-%m-%d %H:%M:%S')
     # write_to_config(config_section=config_section, script=script_name, timestamp=exit_time, details=message)
     print(f'Exiting {script_name}...\n')
     return sys.exit()
```

### Comparing `climush-0.0.4/climush/viz.py` & `climush-0.0.5/climush/viz.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.4/climush.egg-info/PKG-INFO` & `climush-0.0.5/climush.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `climush-0.0.4/pyproject.toml` & `climush-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'climush'
-version = '0.0.4'
+version = '0.0.5'
 authors = [
     { name='Carolyn Delevich', email='cdelevic@uoregon.edu' }]
 description = 'Tools to run the CliMush bioinformatics pipeline.'
 readme = 'README.md'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
```

