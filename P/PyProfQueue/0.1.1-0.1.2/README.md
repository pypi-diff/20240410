# Comparing `tmp/PyProfQueue-0.1.1.tar.gz` & `tmp/PyProfQueue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.1.tar", last modified: Tue Apr  9 14:34:15 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.2.tar", last modified: Wed Apr 10 08:23:49 2024, max compression
```

## Comparing `PyProfQueue-0.1.1.tar` & `PyProfQueue-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3815 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.1/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1435 2024-03-27 13:45:25.000000 PyProfQueue-0.1.1/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      732 2024-04-04 13:48:15.000000 PyProfQueue-0.1.1/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.1/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33503 2024-04-09 14:32:49.000000 PyProfQueue-0.1.1/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.1/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     3815 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-09 14:34:15.000000 PyProfQueue-0.1.1/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3115 2024-04-09 09:02:52.000000 PyProfQueue-0.1.1/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-09 14:34:15.983359 PyProfQueue-0.1.1/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-09 14:34:10.000000 PyProfQueue-0.1.1/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.461137 PyProfQueue-0.1.2/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.2/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1435 2024-03-27 13:45:25.000000 PyProfQueue-0.1.2/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      809 2024-04-10 07:50:21.000000 PyProfQueue-0.1.2/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.2/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33688 2024-04-10 07:50:21.000000 PyProfQueue-0.1.2/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.2/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4981 2024-04-10 08:22:46.000000 PyProfQueue-0.1.2/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-10 07:51:41.000000 PyProfQueue-0.1.2/setup.py
```

### Comparing `PyProfQueue-0.1.1/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.2/PyProfQueue/data/likwid_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.1/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.2/PyProfQueue/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.1/PyProfQueue/script.py` & `PyProfQueue-0.1.2/PyProfQueue/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,19 @@
         prometheus : bool = False
             bool determining if prometheus should be used to measure the metrics of the node on which
             the script is being run.
         prometheus_output: str = None
             str of the path and name of the file to which the prometheus values should be written to
         prometheus_req: list = None
             list of the required lines that need to be added to a bash script in order to allow prometheus
-            to be used. In order to run prometheus this list will need at least two entries. These are:
+            to be used. In order to run prometheus this list will need at least one entry:
                 'export PROMETHEUS_SOFTWARE=<path to the Prometheus software to be used>'
-                'export PROMPYTHON=<path to the Python version to be used to scrape the prometheus database>'
+            with an optional entry to change the python executable to use by declaring:
+                'export PROMETHEUS_PYTHON=<path to the Python version to be used to scrape the prometheus database>'
+            any additional entries will be added, but are at users discretion
 
         Notes
         -----
         The Script class is intended to manage the components necessary in order to take an existing bash script,
         extract any options for a queue system it has, add any desired options, and initiate the information needed
         for prometheus and likwid to perform their metric collections. This object can then be passed on to the
         submit() function in order to create the profiling bash script and submit it to the queue that it is
@@ -189,23 +191,23 @@
     def add_prometheus(self, prometheus_req, prometheus_output='./'):
         contains_ps = False
         contains_pp = False
         for req in prometheus_req:
             if 'PROMETHEUS_SOFTWARE' in req:
                 contains_ps = True
                 continue
-            if 'PROMPYTHON' in req:
+            if 'PROMETHEUS_PYTHON' in req:
                 contains_pp = True
                 continue
             else:
-                prometheus_req += ['export PROMPYTHON={}'.format(sys.executable)]
+                prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
                 contains_pp = True
                 continue
         if not contains_pp:
-            prometheus_req += ['export PROMPYTHON={}'.format(sys.executable)]
+            prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
             contains_pp = True
 
         if not contains_ps or not contains_pp:
             exit('When requesting prometheus profiling, prometheus_req must include "export PROMETHEUS_SOFTWARE=".')
         self.prometheus = True
         self.prometheus_file = impresources.files(data) / "prometheus_commands.txt"
         self.prometheus_initEndSplit = -1
@@ -755,15 +757,15 @@
         return
 
     def init_prometheus(self, profilefile):
         profilefile.write('# Prometheus initialisation declarations\n')
         for i in self.prometheus_req:
             profilefile.write(i)
             profilefile.write('\n')
-        profilefile.write('export PROMET_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
+        profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
         scrape_path = str(impresources.path(data, 'read_prometheus.py'))[:-19]
         profilefile.write('export PROFILE_SCRAPE={}\n'.format(scrape_path))
         profilefile.write('\n')
         with open(self.prometheus_file, 'r') as prometheus_file:
             for number, line in enumerate(prometheus_file):
                 if line == '# *=*\n':
                     self.prometheus_initEndSplit = number + 1
```

### Comparing `PyProfQueue-0.1.1/PyProfQueue/submission.py` & `PyProfQueue-0.1.2/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.1/ReadMe.md` & `PyProfQueue-0.1.2/ReadMe.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,95 @@
 # PyProfQueue
-The package PyProfQueue provides the Script class, which takes the path and name of
-the bash script to be submitted and profiled in order to read in the queue options
-and add any needed initialisations in order to profile using prometheus and likwid.
+The package PyProfQueue provides the Script class, which takes the path and name of the bash script to be submitted and 
+profiled in order to read in the queue options and add any needed initialisations in order to profile using prometheus 
+and likwid.
 
-The Script class has a few methods that can be called, these are:
+When initiating a *Script* object, the following arguments are available:
+```
+script = PyProfQueue.Script(queue_system: str,
+                            work_script: str,
+                            read_queue_system: str =None,
+                            queue_options: dict = None,
+                            likwid: bool = False,
+                            likwid_output: str = None,
+                            likwid_req: list = None,
+                            prometheus: bool = False,
+                            prometheus_output: str = None,
+                            prometheus_req: list = None
+                            )   
+```
+- queue_system: The intended target queue system
+- work_script: The bash script which contains the queue options and work to be done
+- read_queue_system (Optional: defaults to queue_system): The name of the queue system for which the script was written 
+if different from queue_system
+- queue_options(Optional): Any queue options to add or override when compared to the work_script 
+- likwid (Optional: defaults to False): Bool to determine if likwid should be used
+- likwid_output (Optional): Likwid output directory, if a specific one is to be used
+- likwid_req (Optional): Likwid requirements, details can be found in the section about **add_likwid**
+- prometheus (Optional: defaults to False): Bool to determine if prometheus should be used
+- prometheus_output (Optional): Prometheus output directory, if a specific one is to be used
+- prometheus_req (Optional): Prometheus requirements, details can be found in the section about **add_prometheus**
+
+The *Script* class has a few methods that are intended for external use, these are:
 
 - **add_likwid**(likwid_req: list, likwid_output: str ='./')
-  - Adds necessary initiation to use likwid to create a roof-line model
+  - Adds necessary initiation to use likwid to create a roof-line model and plot the work_script onto the model
+  - This can be used if a *Script* object was not initiated with likwid options, or if they are to be changed
   - likwid_req is a list that should contain the necessary lines for the system in use to be able to use liquid. 
 For example, loading the likwid module:
 ```
-likwid_req = ['module load oneAPI_comp', 'module load likwid']
+likwid_req = ['module load likwid']
 ```
 - **add_prometheus**(prometheus_req: list, prometheus_output: str ='./')
-  - Adds necessary initiation to use likwid to create a roof-line model
+  - Adds necessary initiation to use measure computing resource usage
+  - This can be used if a *Script* object was not initiated with prometheus options, or if they are to be changed
   - prometheus_req is a list that should contain the necessary lines for the system in use to be able to use
 prometheus.
-It is necessary to at least add the following two entries:
+It is necessary to at least add the following entry:
 ``` 
 prometheus_req = [
-    'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>',
-    'export PROMPYTHON=<Path to Python file for read_prometheus.py>'
+    'export PROMETHEUS_SOFTWARE=<Path to Prometheus software>'
 ]
 ```
+
 - **change_options**(queue_options: dict)
-  - Allows for options to be changed post initiation of a Script object, in case the options given in the 
+  - Allows for options to be changed post initiation of a *Script* object, in case the options given in the 
 initialisation are no longer desired.
 
-Beyond these three, it is also possible to call the method 'create_profilefile' if one wants to create the
-bash files. This method is called automatically by the submit option and is provided as an optional method
-to validate the content of the files to be submitted.
+Beyond these three, it is also possible to call the method 'create_profilefile' if one wants to create the bash files. 
+This method is called automatically by the submit option and is provided as an optional method to validate the content 
+of the files to be submitted.
 
 ## Requirements
 ### Python Packages
 
 For the sake of PyProfQueue, the required python version is at least 3.10, as this package utilises the match 
-functionality. In order to run *read_prometheus.py*, the path to a python implementation/environment needs to 
-be provided. This implementation needs to have the following packages:
+functionality. In order to run *read_prometheus.py*, the path to a python implementation/environment needs to be 
+provided. This implementation needs to have the following packages:
 - promql_http_api   
 - numpy             
 - pytz              
 - pandas            
 - datetime          
 
-This python implementation does not need to be the same as the one being used to submit the scripts, but does
-need to be present on the system on which the job is being submitted.
+This python implementation does not need to be the same as the one being used to submit the scripts, but does needs to 
+be present on the system on which the job is being submitted. By default, these packages are requested to be installed 
+with PyProfQueue.
 
 ### Non python requirements
 
-In addition to the python requirements listed above, PyProfQueue also needs to have the following software on 
-the system to which the job will be submitted:
+In addition to the python requirements listed above, PyProfQueue also needs to have the following software on the system 
+to which the job will be submitted:
 - [Prometheus](https://prometheus.io/)
 - [likwid](https://github.com/RRZE-HPC/likwid)
 
-For prometheus, it is enough to download the software as long as prometheus can be launched by the user without 
-sudo rights. For the sake of likwid, it needs to be installed or loaded in such a way that a user could run the 
-following command without sudo rights:
+For prometheus, it is enough to download the software as long as prometheus can be launched by the user without sudo 
+rights. For the sake of likwid, it needs to be installed or loaded in such a way that a user could run the following 
+command without sudo rights:
 ```
 likwid-perfctr -g MEM_DP -f <executable>
 ```
 
 ## Adding new Queue system compatibility
 
-In order to add new queue system compatibility refer to the block comments in the Script class in script.py. 
-Each of the four section that needs changes is marked with "Queue System specifics" followed by a {1}, {2}, 
-{3} or {4}.
+In order to add new queue system compatibility refer to the block comments in the *Script* class in script.py. Each of 
+the four section that needs changes is marked with "Queue System specifics" followed by a {1}, {2}, {3} or {4}.
```

### Comparing `PyProfQueue-0.1.1/setup.py` & `PyProfQueue-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

