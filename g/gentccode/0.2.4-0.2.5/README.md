# Comparing `tmp/gentccode-0.2.4.tar.gz` & `tmp/gentccode-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.4.tar", max compression
+gzip compressed data, was "gentccode-0.2.5.tar", max compression
```

## Comparing `gentccode-0.2.4.tar` & `gentccode-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.4/LICENSE
--rw-r--r--   0        0        0     1066 2024-04-10 03:12:23.157802 gentccode-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.4/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.4/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.4/gentccode/check_version.py
--rw-r--r--   0        0        0     3107 2024-04-10 06:27:33.017555 gentccode-0.2.4/gentccode/cli.py
--rw-r--r--   0        0        0    20333 2024-04-10 03:04:41.206073 gentccode-0.2.4/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.4/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.4/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.4/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.4/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.4/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.4/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0      612 2024-04-10 06:28:21.204007 gentccode-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 gentccode-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.5/gentccode/__init__.py
+-rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.5/gentccode/cartesian_for_case.py
+-rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.5/gentccode/check_version.py
+-rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.5/gentccode/cli.py
+-rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.5/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.5/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.5/gentccode/generate_case_code.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.5/gentccode/merge_api.py
+-rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.5/gentccode/produce_search_case.py
+-rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.5/gentccode/produce_test_case.py
+-rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.5/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0      612 2024-04-10 07:53:59.621191 gentccode-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.5/PKG-INFO
```

### Comparing `gentccode-0.2.4/LICENSE` & `gentccode-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/README.md` & `gentccode-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ```bash
 gtc cp -n a. curl.txt
 ```
 
 3. 执行下面命令,会生成对应的压测脚本
 
 ```bash
-gtc jmeter curl.txt --json-assert code=0
+gtc jmeter curl.txt --jsonassert code=0 --rate 10 --time 5
 gtc locust curl.txt
 ```
 
 ## 已知问题
 
 - 若postman文件中有变量,则不会生成相对应的代码块.
 - url中必须有http或https协议头
```

### Comparing `gentccode-0.2.4/gentccode/cartesian_for_case.py` & `gentccode-0.2.5/gentccode/cartesian_for_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/check_version.py` & `gentccode-0.2.5/gentccode/check_version.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/cli.py` & `gentccode-0.2.5/gentccode/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,18 +64,30 @@
 @click.command(help="generate jmeter script by curl file")
 @click.option(
     "-ja",
     "--jsonassert",
     required=True,
     help="json node, like: 'code','data.code','a.b.c'",
 )
+@click.option(
+    "-r",
+    "--rate",
+    required=True,
+    help="qps/s, like: 1, 10",
+)
+@click.option(
+    "-t",
+    "--time",
+    required=True,
+    help="total stress time: 1min, like: 1, 10",
+)
 @click.argument("filename", type=click.Path(exists=True))
-def jmeter(filename, jsonassert): # cli方法中的参数必须为小写
+def jmeter(filename, jsonassert, rate, time):  # cli方法中的参数必须为小写
     convert_payloads_of_curl_to_jmx_file(
-        curl_file_path=filename, json_path_assert=jsonassert
+        curl_file_path=filename, json_path_assert=jsonassert, rate=rate, total_time=time
     )
 
 
 @click.command(help="auto generate swagger2 document's test code")
 @click.argument("filename", type=click.Path(exists=True))
 def swagger_at(filename):
     ptc.produce_merged_case_for_swagger_and_curl(curl_file_path=filename)
```

### Comparing `gentccode-0.2.4/gentccode/convert_to_jmx.py` & `gentccode-0.2.5/gentccode/convert_to_jmx.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,35 @@
     stringProp.text = "60"
     stringProp = etree.SubElement(theadGroup, "stringProp")
     stringProp.set("name", "ThreadGroup.delay")
     stringProp.text = ""
     return etree.SubElement(parent_xml, "hashTree")
 
 
+def open_model_thread_group(parent_xml, rate, total_time):
+    # 创建 OpenModelThreadGroup 元素
+    open_model_thread_group = etree.SubElement(parent_xml, "OpenModelThreadGroup")
+    open_model_thread_group.set("guiclass", "OpenModelThreadGroupGui")
+    open_model_thread_group.set("testclass", "OpenModelThreadGroup")
+    open_model_thread_group.set("testname", "Open Model Thread Group")
+
+    # 创建 elementProp 元素
+    element_prop = etree.SubElement(open_model_thread_group, "elementProp")
+    element_prop.set("name", "ThreadGroup.main_controller")
+    element_prop.set("elementType", "OpenModelThreadGroupController")
+
+    # 创建 stringProp 元素
+    string_prop = etree.SubElement(
+        open_model_thread_group, "stringProp", name="OpenModelThreadGroup.schedule"
+    )
+    # TODO 模型固定,后续需要传入动态模型
+    string_prop.text = f"rate(0/s) random_arrivals(10 s) rate({rate}/s) random_arrivals({total_time} min) rate({rate}/s)"
+    return etree.SubElement(parent_xml, "hashTree")
+
+
 def arguments(parent_xml):
     """
 
     :param parent_xml:
     :return: etree object
     """
     Arguments = etree.SubElement(parent_xml, "ThreadGroup")
@@ -448,19 +469,20 @@
     :param datas:
     :return:
     """
     for key, value in datas.items():
         obj_xml.set(key, value)
 
 
-def write_to_jmx(payloads: list, json_path_assert: str):
+def write_to_jmx(payloads: list, json_path_assert: str, rate: str, total_time: str):
     jmeterTestPlan = etree.Element("jmeterTestPlan")
     hashTree = jmeter_test_plan(jmeterTestPlan)
     testPlan = test_plan(hashTree, "autotest")
-    threadGroup = thread_group(testPlan)
+    # threadGroup = thread_group(testPlan)
+    threadGroup = open_model_thread_group(testPlan, rate, total_time)
     controller(threadGroup, payloads, json_path_assert)
     view_result_tree(threadGroup)
     etree.tostring(jmeterTestPlan, pretty_print=True)
     tree = etree.ElementTree(jmeterTestPlan)
     now_date = time.strftime("%Y%m%d%H%M%S", time.localtime(time.time()))
     tree.write(
         f"jmeter-{now_date}.jmx",
@@ -500,19 +522,26 @@
 def _reduce_url_path(path):
     if path[0] != "/":
         return "/" + path
     else:
         return path
 
 
-def convert_payloads_of_curl_to_jmx_file(curl_file_path, json_path_assert):
+def convert_payloads_of_curl_to_jmx_file(
+    curl_file_path, json_path_assert, rate, total_time
+):
     gaf = GenerateApiFile()
     http_payloads = gaf.convert_curl_data_to_model(curl_file_path)
     jmx_payloads = convert_payloads_to_jmx_model(http_payloads=http_payloads)
-    write_to_jmx(payloads=jmx_payloads, json_path_assert=json_path_assert)
+    write_to_jmx(
+        payloads=jmx_payloads,
+        json_path_assert=json_path_assert,
+        rate=rate,
+        total_time=total_time,
+    )
 
 
 def convert_payloads_to_jmx_model(http_payloads: list[ReqData]) -> list:
     i = 1
     jmx_payloads = []
     for http_payload in http_payloads:
         http_payload = parse_req_data_model(http_payload)
```

### Comparing `gentccode-0.2.4/gentccode/convert_to_locust.py` & `gentccode-0.2.5/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/generate_case_code.py` & `gentccode-0.2.5/gentccode/generate_case_code.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/merge_api.py` & `gentccode-0.2.5/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/produce_search_case.py` & `gentccode-0.2.5/gentccode/produce_search_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/produce_test_case.py` & `gentccode-0.2.5/gentccode/produce_test_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/gentccode/read_swagger_rule.py` & `gentccode-0.2.5/gentccode/read_swagger_rule.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.4/pyproject.toml` & `gentccode-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.4"
+version = "0.2.5"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `gentccode-0.2.4/PKG-INFO` & `gentccode-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.4
+Version: 0.2.5
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -56,15 +56,15 @@
 ```bash
 gtc cp -n a. curl.txt
 ```
 
 3. 执行下面命令,会生成对应的压测脚本
 
 ```bash
-gtc jmeter curl.txt --json-assert code=0
+gtc jmeter curl.txt --jsonassert code=0 --rate 10 --time 5
 gtc locust curl.txt
 ```
 
 ## 已知问题
 
 - 若postman文件中有变量,则不会生成相对应的代码块.
 - url中必须有http或https协议头
```

