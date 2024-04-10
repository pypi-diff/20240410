# Comparing `tmp/chamferdist-1.0.1.tar.gz` & `tmp/chamferdist-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamferdist-1.0.1.tar", last modified: Wed Oct 11 19:22:41 2023, max compression
+gzip compressed data, was "chamferdist-1.0.3.tar", last modified: Wed Apr 10 03:41:34 2024, max compression
```

## Comparing `chamferdist-1.0.1.tar` & `chamferdist-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 soroush    (501) staff       (20)        0 2023-10-11 19:22:41.258819 chamferdist-1.0.1/
--rw-r--r--   0 soroush    (501) staff       (20)     2208 2023-10-11 19:20:29.000000 chamferdist-1.0.1/LICENSE
--rw-r--r--   0 soroush    (501) staff       (20)      347 2023-10-11 19:22:41.258534 chamferdist-1.0.1/PKG-INFO
--rw-r--r--   0 soroush    (501) staff       (20)     3083 2023-10-11 19:20:29.000000 chamferdist-1.0.1/README.md
-drwxr-xr-x   0 soroush    (501) staff       (20)        0 2023-10-11 19:22:41.257301 chamferdist-1.0.1/chamferdist/
--rw-r--r--   0 soroush    (501) staff       (20)       37 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/__init__.py
--rw-r--r--   0 soroush    (501) staff       (20)    14080 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/chamfer.py
--rw-r--r--   0 soroush    (501) staff       (20)      376 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/cutils.h
--rw-r--r--   0 soroush    (501) staff       (20)    10219 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/dispatch.cuh
--rw-r--r--   0 soroush    (501) staff       (20)      289 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/ext.cpp
--rw-r--r--   0 soroush    (501) staff       (20)     5188 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/index_utils.cuh
--rw-r--r--   0 soroush    (501) staff       (20)    20851 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/knn.cu
--rw-r--r--   0 soroush    (501) staff       (20)     4957 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/knn.h
--rw-r--r--   0 soroush    (501) staff       (20)     3546 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/knn_cpu.cpp
--rw-r--r--   0 soroush    (501) staff       (20)     4574 2023-10-11 19:20:29.000000 chamferdist-1.0.1/chamferdist/mink.cuh
--rw-r--r--   0 soroush    (501) staff       (20)       22 2023-10-11 19:21:58.000000 chamferdist-1.0.1/chamferdist/version.py
-drwxr-xr-x   0 soroush    (501) staff       (20)        0 2023-10-11 19:22:41.257969 chamferdist-1.0.1/chamferdist.egg-info/
--rw-r--r--   0 soroush    (501) staff       (20)      347 2023-10-11 19:22:41.000000 chamferdist-1.0.1/chamferdist.egg-info/PKG-INFO
--rw-r--r--   0 soroush    (501) staff       (20)      446 2023-10-11 19:22:41.000000 chamferdist-1.0.1/chamferdist.egg-info/SOURCES.txt
--rw-r--r--   0 soroush    (501) staff       (20)        1 2023-10-11 19:22:41.000000 chamferdist-1.0.1/chamferdist.egg-info/dependency_links.txt
--rw-r--r--   0 soroush    (501) staff       (20)       26 2023-10-11 19:22:41.000000 chamferdist-1.0.1/chamferdist.egg-info/requires.txt
--rw-r--r--   0 soroush    (501) staff       (20)       12 2023-10-11 19:22:41.000000 chamferdist-1.0.1/chamferdist.egg-info/top_level.txt
--rw-r--r--   0 soroush    (501) staff       (20)       38 2023-10-11 19:22:41.258873 chamferdist-1.0.1/setup.cfg
--rw-r--r--   0 soroush    (501) staff       (20)     2713 2023-10-11 19:20:29.000000 chamferdist-1.0.1/setup.py
+drwxr-xr-x   0 soroush    (501) staff       (20)        0 2024-04-10 03:41:34.330140 chamferdist-1.0.3/
+-rw-r--r--   0 soroush    (501) staff       (20)     2208 2023-10-11 19:20:29.000000 chamferdist-1.0.3/LICENSE
+-rw-r--r--   0 soroush    (501) staff       (20)      347 2024-04-10 03:41:34.329896 chamferdist-1.0.3/PKG-INFO
+-rw-r--r--   0 soroush    (501) staff       (20)     3083 2023-10-11 19:20:29.000000 chamferdist-1.0.3/README.md
+drwxr-xr-x   0 soroush    (501) staff       (20)        0 2024-04-10 03:41:34.328752 chamferdist-1.0.3/chamferdist/
+-rw-r--r--   0 soroush    (501) staff       (20)       37 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/__init__.py
+-rw-r--r--   0 soroush    (501) staff       (20)    14080 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/chamfer.py
+-rw-r--r--   0 soroush    (501) staff       (20)      376 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/cutils.h
+-rw-r--r--   0 soroush    (501) staff       (20)    10219 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/dispatch.cuh
+-rw-r--r--   0 soroush    (501) staff       (20)      289 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/ext.cpp
+-rw-r--r--   0 soroush    (501) staff       (20)     5188 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/index_utils.cuh
+-rw-r--r--   0 soroush    (501) staff       (20)    20851 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/knn.cu
+-rw-r--r--   0 soroush    (501) staff       (20)     4957 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/knn.h
+-rw-r--r--   0 soroush    (501) staff       (20)     3546 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/knn_cpu.cpp
+-rw-r--r--   0 soroush    (501) staff       (20)     4574 2023-10-11 19:20:29.000000 chamferdist-1.0.3/chamferdist/mink.cuh
+-rw-r--r--   0 soroush    (501) staff       (20)       22 2024-04-10 03:40:56.000000 chamferdist-1.0.3/chamferdist/version.py
+drwxr-xr-x   0 soroush    (501) staff       (20)        0 2024-04-10 03:41:34.329401 chamferdist-1.0.3/chamferdist.egg-info/
+-rw-r--r--   0 soroush    (501) staff       (20)      347 2024-04-10 03:41:34.000000 chamferdist-1.0.3/chamferdist.egg-info/PKG-INFO
+-rw-r--r--   0 soroush    (501) staff       (20)      446 2024-04-10 03:41:34.000000 chamferdist-1.0.3/chamferdist.egg-info/SOURCES.txt
+-rw-r--r--   0 soroush    (501) staff       (20)        1 2024-04-10 03:41:34.000000 chamferdist-1.0.3/chamferdist.egg-info/dependency_links.txt
+-rw-r--r--   0 soroush    (501) staff       (20)       26 2024-04-10 03:41:34.000000 chamferdist-1.0.3/chamferdist.egg-info/requires.txt
+-rw-r--r--   0 soroush    (501) staff       (20)       12 2024-04-10 03:41:34.000000 chamferdist-1.0.3/chamferdist.egg-info/top_level.txt
+-rw-r--r--   0 soroush    (501) staff       (20)       38 2024-04-10 03:41:34.330187 chamferdist-1.0.3/setup.cfg
+-rw-r--r--   0 soroush    (501) staff       (20)     2713 2024-04-10 03:22:31.000000 chamferdist-1.0.3/setup.py
```

### Comparing `chamferdist-1.0.1/LICENSE` & `chamferdist-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/README.md` & `chamferdist-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/chamfer.py` & `chamferdist-1.0.3/chamferdist/chamfer.py`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/dispatch.cuh` & `chamferdist-1.0.3/chamferdist/dispatch.cuh`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/index_utils.cuh` & `chamferdist-1.0.3/chamferdist/index_utils.cuh`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/knn.cu` & `chamferdist-1.0.3/chamferdist/knn.cu`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/knn.h` & `chamferdist-1.0.3/chamferdist/knn.h`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/knn_cpu.cpp` & `chamferdist-1.0.3/chamferdist/knn_cpu.cpp`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/chamferdist/mink.cuh` & `chamferdist-1.0.3/chamferdist/mink.cuh`

 * *Files identical despite different names*

### Comparing `chamferdist-1.0.1/setup.py` & `chamferdist-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     main_source = os.path.join("chamferdist", "ext.cpp")
     sources = [os.path.join("chamferdist", "knn_cpu.cpp")]
     source_cuda = [os.path.join("chamferdist", "knn.cu")]
     sources = [main_source] + sources
 
     extension = CppExtension
 
-    extra_compile_args = {"cxx": ["-std=c++14"]}
+    extra_compile_args = {"cxx": ["-std=c++17"]}
     define_macros = []
 
     force_cuda = os.getenv("FORCE_CUDA", "0") == "1"
     if (torch.cuda.is_available() and CUDA_HOME is not None) or force_cuda:
         extension = CUDAExtension
         sources += source_cuda
         define_macros += [("WITH_CUDA", None)]
```

