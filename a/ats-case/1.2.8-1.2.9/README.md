# Comparing `tmp/ats_case-1.2.8.tar.gz` & `tmp/ats_case-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-1.2.8.tar", last modified: Mon Feb  5 03:24:30 2024, max compression
+gzip compressed data, was "ats_case-1.2.9.tar", last modified: Mon Feb  5 05:45:14 2024, max compression
```

## Comparing `ats_case-1.2.8.tar` & `ats_case-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.952944 ats_case-1.2.8/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-1.2.8/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1172 2024-02-05 03:24:30.949952 ats_case-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-10-23 10:03:10.000000 ats_case-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.162944 ats_case-1.2.8/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-1.2.8/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.521946 ats_case-1.2.8/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-1.2.8/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0     6789 2024-02-02 05:39:12.000000 ats_case-1.2.8/ats_case/case/asb.py
--rw-rw-rw-   0        0        0       91 2023-12-07 03:11:31.000000 ats_case-1.2.8/ats_case/case/atm.py
--rw-rw-rw-   0        0        0     7884 2024-02-02 03:08:32.000000 ats_case-1.2.8/ats_case/case/base.py
--rw-rw-rw-   0        0        0     1082 2024-01-16 02:44:14.000000 ats_case-1.2.8/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12003 2024-02-02 05:55:42.000000 ats_case-1.2.8/ats_case/case/context.py
--rw-rw-rw-   0        0        0    10033 2024-02-02 05:53:37.000000 ats_case-1.2.8/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     6031 2024-01-16 02:27:13.000000 ats_case-1.2.8/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.625946 ats_case-1.2.8/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-1.2.8/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      355 2023-12-08 02:19:03.000000 ats_case-1.2.8/ats_case/common/enum.py
--rw-rw-rw-   0        0        0     1490 2024-02-02 03:04:35.000000 ats_case-1.2.8/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.805945 ats_case-1.2.8/ats_case/entity/
--rw-rw-rw-   0        0        0        0 2024-01-16 02:16:52.000000 ats_case-1.2.8/ats_case/entity/__init__.py
--rw-rw-rw-   0        0        0     4765 2024-01-16 02:32:11.000000 ats_case-1.2.8/ats_case/entity/ats.py
--rw-rw-rw-   0        0        0     8688 2024-02-02 05:55:10.000000 ats_case-1.2.8/ats_case/entity/bench.py
--rw-rw-rw-   0        0        0     1388 2024-01-16 02:33:07.000000 ats_case-1.2.8/ats_case/entity/client.py
--rw-rw-rw-   0        0        0     2439 2024-01-16 05:27:20.000000 ats_case-1.2.8/ats_case/entity/encrypt.py
--rw-rw-rw-   0        0        0    10852 2024-01-22 01:13:32.000000 ats_case-1.2.8/ats_case/entity/meter.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.871944 ats_case-1.2.8/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-1.2.8/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-12-08 06:54:54.000000 ats_case-1.2.8/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     5950 2024-02-05 03:24:02.000000 ats_case-1.2.8/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.907944 ats_case-1.2.8/ats_case/security/
--rw-rw-rw-   0        0        0        0 2024-01-10 01:22:44.000000 ats_case-1.2.8/ats_case/security/__init__.py
--rw-rw-rw-   0        0        0     3207 2024-01-17 07:40:45.000000 ats_case-1.2.8/ats_case/security/link.py
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.939944 ats_case-1.2.8/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-1.2.8/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2397 2023-09-08 04:31:54.000000 ats_case-1.2.8/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2024-02-05 03:24:30.269945 ats_case-1.2.8/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1172 2024-02-05 03:24:29.000000 ats_case-1.2.8/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2024-02-05 03:24:29.000000 ats_case-1.2.8/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-05 03:24:29.000000 ats_case-1.2.8/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-02-05 03:24:29.000000 ats_case-1.2.8/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-05 03:24:29.000000 ats_case-1.2.8/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-05 03:24:30.953974 ats_case-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      945 2024-02-05 03:24:24.000000 ats_case-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.916424 ats_case-1.2.9/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1172 2024-02-05 05:45:14.912425 ats_case-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-10-23 10:03:10.000000 ats_case-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:13.806423 ats_case-1.2.9/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-1.2.9/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.159421 ats_case-1.2.9/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-1.2.9/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0     6789 2024-02-02 05:39:12.000000 ats_case-1.2.9/ats_case/case/asb.py
+-rw-rw-rw-   0        0        0       91 2023-12-07 03:11:31.000000 ats_case-1.2.9/ats_case/case/atm.py
+-rw-rw-rw-   0        0        0     7884 2024-02-02 03:08:32.000000 ats_case-1.2.9/ats_case/case/base.py
+-rw-rw-rw-   0        0        0     1082 2024-01-16 02:44:14.000000 ats_case-1.2.9/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12003 2024-02-02 05:55:42.000000 ats_case-1.2.9/ats_case/case/context.py
+-rw-rw-rw-   0        0        0    10033 2024-02-02 05:53:37.000000 ats_case-1.2.9/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     6031 2024-01-16 02:27:13.000000 ats_case-1.2.9/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.242424 ats_case-1.2.9/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-1.2.9/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      355 2023-12-08 02:19:03.000000 ats_case-1.2.9/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0     1490 2024-02-02 03:04:35.000000 ats_case-1.2.9/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.480428 ats_case-1.2.9/ats_case/entity/
+-rw-rw-rw-   0        0        0        0 2024-01-16 02:16:52.000000 ats_case-1.2.9/ats_case/entity/__init__.py
+-rw-rw-rw-   0        0        0     4765 2024-01-16 02:32:11.000000 ats_case-1.2.9/ats_case/entity/ats.py
+-rw-rw-rw-   0        0        0     8698 2024-02-05 05:44:36.000000 ats_case-1.2.9/ats_case/entity/bench.py
+-rw-rw-rw-   0        0        0     1388 2024-01-16 02:33:07.000000 ats_case-1.2.9/ats_case/entity/client.py
+-rw-rw-rw-   0        0        0     2439 2024-01-16 05:27:20.000000 ats_case-1.2.9/ats_case/entity/encrypt.py
+-rw-rw-rw-   0        0        0    10852 2024-01-22 01:13:32.000000 ats_case-1.2.9/ats_case/entity/meter.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.739423 ats_case-1.2.9/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-1.2.9/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-12-08 06:54:54.000000 ats_case-1.2.9/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     5950 2024-02-05 03:24:02.000000 ats_case-1.2.9/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.850426 ats_case-1.2.9/ats_case/security/
+-rw-rw-rw-   0        0        0        0 2024-01-10 01:22:44.000000 ats_case-1.2.9/ats_case/security/__init__.py
+-rw-rw-rw-   0        0        0     3207 2024-01-17 07:40:45.000000 ats_case-1.2.9/ats_case/security/link.py
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:14.900422 ats_case-1.2.9/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-1.2.9/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2397 2023-09-08 04:31:54.000000 ats_case-1.2.9/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2024-02-05 05:45:13.929422 ats_case-1.2.9/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1172 2024-02-05 05:45:13.000000 ats_case-1.2.9/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2024-02-05 05:45:13.000000 ats_case-1.2.9/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-05 05:45:13.000000 ats_case-1.2.9/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-02-05 05:45:13.000000 ats_case-1.2.9/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-02-05 05:45:13.000000 ats_case-1.2.9/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-05 05:45:14.916424 ats_case-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-02-05 05:44:45.000000 ats_case-1.2.9/setup.py
```

### Comparing `ats_case-1.2.8/PKG-INFO` & `ats_case-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 1.2.8
+Version: 1.2.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-1.2.8/README.md` & `ats_case-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/asb.py` & `ats_case-1.2.9/ats_case/case/asb.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/base.py` & `ats_case-1.2.9/ats_case/case/base.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/command.py` & `ats_case-1.2.9/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/context.py` & `ats_case-1.2.9/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/executor.py` & `ats_case-1.2.9/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/case/translator.py` & `ats_case-1.2.9/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/common/error.py` & `ats_case-1.2.9/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/entity/ats.py` & `ats_case-1.2.9/ats_case/entity/ats.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/entity/bench.py` & `ats_case-1.2.9/ats_case/entity/bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 if self._is_meter_pos_operation:
                     pass_quantity = asb.Application.get(context.test_sn, 'pass_quantity')
                     if pass_quantity == 'NULL':
                         pass_quantity = 0
                     pass_quantity = int(pass_quantity) + 1
                     asb.Application.set(context.test_sn, 'pass_quantity', pass_quantity)
 
-                    if pass_quantity >= asb.Application.get(context.test_sn, "meter:quantity"):
+                    if pass_quantity >= int(asb.Application.get(context.test_sn, "meter:quantity")):
                         asb.Application.set(context.test_sn, 'pass_quantity', 0)
                         self.sleep(context)
                 else:
                     self.sleep(context)
 
     def _exec_main(self, context: Context):
         self.encode(context)
@@ -172,15 +172,15 @@
                         finished_quantity += 1
                         asb.Application.set(context.test_sn, 'finished_quantity', finished_quantity)
                     else:
                         one_loop_finished_quantity += 1
                         asb.Application.set(context.test_sn, 'one_loop_finished_quantity', one_loop_finished_quantity)
 
                 # 多表测试时, 判断是否是最后一只表, 是否睡眠
-                quantity = asb.Application.get(context.test_sn, "meter:quantity")
+                quantity = int(asb.Application.get(context.test_sn, "meter:quantity"))
                 if one_loop_finished_quantity >= quantity - finished_quantity:
                     # 一轮循环最后一只表
                     asb.Application.set(context.test_sn, 'one_loop_finished_quantity', 0)
                     if finished_quantity < quantity:
                         # 最后一轮最后一只表不睡眠, 其他轮次最后一只表都睡眠
                         if isinstance(self._repeat_sleep, int) and self._repeat_sleep > 0:
                             base.sleep(self._repeat_sleep)
```

### Comparing `ats_case-1.2.8/ats_case/entity/client.py` & `ats_case-1.2.9/ats_case/entity/client.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/entity/encrypt.py` & `ats_case-1.2.9/ats_case/entity/encrypt.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/entity/meter.py` & `ats_case-1.2.9/ats_case/entity/meter.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/manage/core.py` & `ats_case-1.2.9/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/manage/start.py` & `ats_case-1.2.9/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/security/link.py` & `ats_case-1.2.9/ats_case/security/link.py`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case/template/testcase_v1.tmp` & `ats_case-1.2.9/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/ats_case.egg-info/PKG-INFO` & `ats_case-1.2.9/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 1.2.8
+Version: 1.2.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-1.2.8/ats_case.egg-info/SOURCES.txt` & `ats_case-1.2.9/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-1.2.8/setup.py` & `ats_case-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="1.2.8",
+    version="1.2.9",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

