# Comparing `tmp/smart_parallelize-2.0.3.tar.gz` & `tmp/smart_parallelize-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.3.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.4.tar", max compression
```

## Comparing `smart_parallelize-2.0.3.tar` & `smart_parallelize-2.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.3/README.md
--rw-r--r--   0        0        0      317 2024-04-05 18:20:58.138795 smart_parallelize-2.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.3/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-05 18:20:48.853427 smart_parallelize-2.0.3/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.4/README.md
+-rw-r--r--   0        0        0      317 2024-04-09 22:33:58.860124 smart_parallelize-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.4/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     4313 2024-04-05 18:40:15.452279 smart_parallelize-2.0.4/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.4/PKG-INFO
```

### Comparing `smart_parallelize-2.0.3/README.md` & `smart_parallelize-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.3/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.4/smart_parallelize/parallelize.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,25 @@
 def smart_parallelize(func): 
     '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
 
     def wrap(**kwargs): 
         def f2(**kwargs):
             par_args = list(kwargs.keys())[:n_args2parallelize]
             data_par_args = [kwargs[i] for i in par_args]
+
+            fnc = np.vectorize(func)
+            print(fnc(**kwargs))
             results = []
             for i, _ in enumerate(data_par_args[0]):
                 kwargs_0 = kwargs.copy()
                 for j, _ in enumerate(data_par_args):
                     kwargs_0[par_args[j]] = data_par_args[j][i]
                 r = func(**kwargs_0)
                 results.append(r)
+            print(results)
             return results
         @ray.remote(memory=MEM_PER_WORKER)
         def get_results(**kwargs):
             try:
                 args_names = ray.get(args_names_put)
                 args_vals  = ray.get(args_vals_put)
                 kwargs2 = dict(zip(args_names, args_vals))
```

### Comparing `smart_parallelize-2.0.3/PKG-INFO` & `smart_parallelize-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```
