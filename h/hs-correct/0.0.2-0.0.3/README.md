# Comparing `tmp/hs_correct-0.0.2.tar.gz` & `tmp/hs_correct-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hs_correct-0.0.2.tar", last modified: Tue Apr  9 07:45:47 2024, max compression
+gzip compressed data, was "hs_correct-0.0.3.tar", last modified: Tue Apr  9 08:33:47 2024, max compression
```

## Comparing `hs_correct-0.0.2.tar` & `hs_correct-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.311773 hs_correct-0.0.2/
--rw-rw-rw-   0        0        0      213 2024-04-09 07:45:37.000000 hs_correct-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      272 2024-04-09 07:45:47.311773 hs_correct-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.292271 hs_correct-0.0.2/correct/
--rw-rw-rw-   0        0        0     3669 2024-04-09 02:53:54.000000 hs_correct-0.0.2/correct/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.293296 hs_correct-0.0.2/correct/exception/
--rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.2/correct/exception/correct_exception.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.296275 hs_correct-0.0.2/correct/funcs/
--rw-rw-rw-   0        0        0    15852 2024-04-08 06:52:42.000000 hs_correct-0.0.2/correct/funcs/alignment.py
--rw-rw-rw-   0        0        0     2536 2024-04-09 02:49:43.000000 hs_correct-0.0.2/correct/funcs/correction.py
--rw-rw-rw-   0        0        0     6329 2024-04-09 02:45:54.000000 hs_correct-0.0.2/correct/funcs/data_handle.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.297313 hs_correct-0.0.2/correct/logger/
--rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.2/correct/logger/logger.py
--rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.2/correct/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.299274 hs_correct-0.0.2/correct/response/
--rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.2/correct/response/response.py
--rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.2/correct/response/response_code.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.303817 hs_correct-0.0.2/correct/tools/
--rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.2/correct/tools/constants.py
--rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.2/correct/tools/min_edit_distance.py
--rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.2/correct/tools/point_handle.py
--rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.2/correct/tools/rectangle_handle.py
--rw-rw-rw-   0        0        0     5275 2024-04-09 02:47:59.000000 hs_correct-0.0.2/correct/tools/str_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:45:47.310774 hs_correct-0.0.2/hs_correct.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-09 07:45:47.000000 hs_correct-0.0.2/hs_correct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-04-09 07:45:47.000000 hs_correct-0.0.2/hs_correct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:45:47.000000 hs_correct-0.0.2/hs_correct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-09 07:45:47.000000 hs_correct-0.0.2/hs_correct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 07:45:47.000000 hs_correct-0.0.2/hs_correct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-04-09 06:21:01.000000 hs_correct-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 07:45:47.312772 hs_correct-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-04-09 07:33:42.000000 hs_correct-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/
+-rw-rw-rw-   0        0        0      213 2024-04-09 07:56:33.000000 hs_correct-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      272 2024-04-09 08:33:47.014705 hs_correct-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-04-01 06:28:15.000000 hs_correct-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:46.998344 hs_correct-0.0.3/correct/
+-rw-rw-rw-   0        0        0     3668 2024-04-09 07:54:40.000000 hs_correct-0.0.3/correct/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:46.998344 hs_correct-0.0.3/correct/exception/
+-rw-rw-rw-   0        0        0      610 2024-04-02 06:36:33.000000 hs_correct-0.0.3/correct/exception/correct_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/correct/funcs/
+-rw-rw-rw-   0        0        0    15852 2024-04-08 06:52:42.000000 hs_correct-0.0.3/correct/funcs/alignment.py
+-rw-rw-rw-   0        0        0     2536 2024-04-09 02:49:43.000000 hs_correct-0.0.3/correct/funcs/correction.py
+-rw-rw-rw-   0        0        0     6329 2024-04-09 02:45:54.000000 hs_correct-0.0.3/correct/funcs/data_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/correct/logger/
+-rw-rw-rw-   0        0        0     1791 2024-03-19 09:58:45.000000 hs_correct-0.0.3/correct/logger/logger.py
+-rw-rw-rw-   0        0        0       24 2024-04-01 08:38:32.000000 hs_correct-0.0.3/correct/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/correct/response/
+-rw-rw-rw-   0        0        0     1210 2024-04-02 06:36:33.000000 hs_correct-0.0.3/correct/response/response.py
+-rw-rw-rw-   0        0        0      186 2024-03-29 02:44:54.000000 hs_correct-0.0.3/correct/response/response_code.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/correct/tools/
+-rw-rw-rw-   0        0        0      461 2024-03-29 02:14:14.000000 hs_correct-0.0.3/correct/tools/constants.py
+-rw-rw-rw-   0        0        0     1632 2024-04-08 06:46:25.000000 hs_correct-0.0.3/correct/tools/min_edit_distance.py
+-rw-rw-rw-   0        0        0     1625 2024-03-27 06:56:01.000000 hs_correct-0.0.3/correct/tools/point_handle.py
+-rw-rw-rw-   0        0        0     2655 2024-03-27 06:56:01.000000 hs_correct-0.0.3/correct/tools/rectangle_handle.py
+-rw-rw-rw-   0        0        0     5275 2024-04-09 02:47:59.000000 hs_correct-0.0.3/correct/tools/str_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:33:47.014705 hs_correct-0.0.3/hs_correct.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-09 08:33:46.000000 hs_correct-0.0.3/hs_correct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-04-09 08:33:46.000000 hs_correct-0.0.3/hs_correct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 08:33:46.000000 hs_correct-0.0.3/hs_correct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-09 08:33:46.000000 hs_correct-0.0.3/hs_correct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 08:33:46.000000 hs_correct-0.0.3/hs_correct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-04-09 06:21:01.000000 hs_correct-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 08:33:47.014705 hs_correct-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-09 08:33:39.000000 hs_correct-0.0.3/setup.py
```

### Comparing `hs_correct-0.0.2/correct/__init__.py` & `hs_correct-0.0.3/correct/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def correct_with_res_code(param: dict):
     try:
 
         # 记录开始时间
         start_time = time.perf_counter()
 
-        res = tmp_correct(param)
+        res = do_correct(param)
 
         # 记录结束时间
         end_time = time.perf_counter()
         # 计算时长
         duration = end_time - start_time
         logger.info(f"[correct_with_res_code]本次调用耗时{duration}秒")
```

### Comparing `hs_correct-0.0.2/correct/exception/correct_exception.py` & `hs_correct-0.0.3/correct/exception/correct_exception.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/funcs/alignment.py` & `hs_correct-0.0.3/correct/funcs/alignment.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/funcs/correction.py` & `hs_correct-0.0.3/correct/funcs/correction.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/funcs/data_handle.py` & `hs_correct-0.0.3/correct/funcs/data_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/logger/logger.py` & `hs_correct-0.0.3/correct/logger/logger.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/response/response.py` & `hs_correct-0.0.3/correct/response/response.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/tools/min_edit_distance.py` & `hs_correct-0.0.3/correct/tools/min_edit_distance.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/tools/point_handle.py` & `hs_correct-0.0.3/correct/tools/point_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/tools/rectangle_handle.py` & `hs_correct-0.0.3/correct/tools/rectangle_handle.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/correct/tools/str_tools.py` & `hs_correct-0.0.3/correct/tools/str_tools.py`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/hs_correct.egg-info/SOURCES.txt` & `hs_correct-0.0.3/hs_correct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hs_correct-0.0.2/setup.py` & `hs_correct-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def parse_requirements(filename):
     line_iter = (line.strip() for line in open(filename))
     return [line for line in line_iter if line and not line.startswith("#")]
 
 
 setup(
     name='hs_correct',
-    version='0.0.2',
+    version='0.0.3',
     description='hs-correct-module',
     classifiers=[],
     keywords='hs-correct-module',
     author='zgl',
     author_email='',
     url='',
     license='MIT',
```

