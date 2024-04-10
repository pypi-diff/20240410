# Comparing `tmp/PyProfQueue-0.1.2.tar.gz` & `tmp/PyProfQueue-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.2.tar", last modified: Wed Apr 10 08:23:49 2024, max compression
+gzip compressed data, was "PyProfQueue-0.1.3.tar", last modified: Wed Apr 10 09:18:44 2024, max compression
```

## Comparing `PyProfQueue-0.1.2.tar` & `PyProfQueue-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.461137 PyProfQueue-0.1.2/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.2/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1435 2024-03-27 13:45:25.000000 PyProfQueue-0.1.2/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      809 2024-04-10 07:50:21.000000 PyProfQueue-0.1.2/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.2/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33688 2024-04-10 07:50:21.000000 PyProfQueue-0.1.2/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.2/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-10 08:23:49.000000 PyProfQueue-0.1.2/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4981 2024-04-10 08:22:46.000000 PyProfQueue-0.1.2/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-10 08:23:49.465137 PyProfQueue-0.1.2/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-10 07:51:41.000000 PyProfQueue-0.1.2/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.3/PyProfQueue/__init__.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/PyProfQueue/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1453 2024-04-10 09:16:59.000000 PyProfQueue-0.1.3/PyProfQueue/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      809 2024-04-10 07:50:21.000000 PyProfQueue-0.1.3/PyProfQueue/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4517 2024-04-09 09:21:10.000000 PyProfQueue-0.1.3/PyProfQueue/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    33688 2024-04-10 07:50:21.000000 PyProfQueue-0.1.3/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.3/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5681 2024-04-10 09:18:44.000000 PyProfQueue-0.1.3/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-10 09:18:44.000000 PyProfQueue-0.1.3/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-10 09:18:44.000000 PyProfQueue-0.1.3/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-10 09:18:44.000000 PyProfQueue-0.1.3/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-10 09:18:44.000000 PyProfQueue-0.1.3/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     4981 2024-04-10 08:22:46.000000 PyProfQueue-0.1.3/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-10 09:18:44.452994 PyProfQueue-0.1.3/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1196 2024-04-10 09:18:38.000000 PyProfQueue-0.1.3/setup.py
```

### Comparing `PyProfQueue-0.1.2/PKG-INFO` & `PyProfQueue-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.2/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.1.3/PyProfQueue/data/likwid_commands.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mkdir ${LIKWID_RUNNING_DIR}
 
 export LIK_OUTPUT=${LIKWID_RUNNING_DIR}/likwid_performance_out.txt
-export THREAD_COUNT=$(($(lscpu --all --parse=CPU,SOCKET,CORE | grep -v '^#' | tail -1 | grep -o -E '^.{2,3},' --max-count=1 | rev) + 1))
+export THREAD_COUNT=$(($(lscpu --all --parse=CPU,SOCKET,CORE | grep -v '^#' | tail -1 | grep -o -E '^.{2,3},' --max-count=1 | rev | cut -c 2- | rev) + 1))
 export STREAM_SIZE=$((10 * ${THREAD_COUNT}))kB
 echo 'Scalar MFlops/s' > ${LIK_OUTPUT}
 likwid-bench -t peakflops -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
 echo 'SSE MFlops/s' >> ${LIK_OUTPUT}
 likwid-bench -t peakflops_sse -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
 echo 'AVX MFlops/s' >> ${LIK_OUTPUT}
 likwid-bench -t peakflops_avx -W N:${STREAM_SIZE}:${THREAD_COUNT} | grep 'MFlops/s:' >> ${LIK_OUTPUT}
```

### Comparing `PyProfQueue-0.1.2/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.1.3/PyProfQueue/data/prometheus_commands.txt`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.2/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.1.3/PyProfQueue/data/read_prometheus.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.2/PyProfQueue/script.py` & `PyProfQueue-0.1.3/PyProfQueue/script.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.2/PyProfQueue/submission.py` & `PyProfQueue-0.1.3/PyProfQueue/submission.py`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.2/PyProfQueue.egg-info/PKG-INFO` & `PyProfQueue-0.1.3/PyProfQueue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyProfQueue
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to inject profiling initialisation into bash scripts, translate queue options and submit jobs
 Home-page: https://github.com/Marcus-Keil/PyProfQueue
 Author: Marcus Keil
 Author-email: marcusk050291@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `PyProfQueue-0.1.2/ReadMe.md` & `PyProfQueue-0.1.3/ReadMe.md`

 * *Files identical despite different names*

### Comparing `PyProfQueue-0.1.2/setup.py` & `PyProfQueue-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
     package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
```

