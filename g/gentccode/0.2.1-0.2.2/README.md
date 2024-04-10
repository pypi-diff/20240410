# Comparing `tmp/gentccode-0.2.1.tar.gz` & `tmp/gentccode-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.1.tar", max compression
+gzip compressed data, was "gentccode-0.2.2.tar", max compression
```

## Comparing `gentccode-0.2.1.tar` & `gentccode-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.1/LICENSE
--rw-r--r--   0        0        0      906 2023-10-23 06:36:33.788844 gentccode-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.1/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.1/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.1/gentccode/check_version.py
--rw-r--r--   0        0        0     2890 2023-10-24 06:56:36.400121 gentccode-0.2.1/gentccode/cli.py
--rw-r--r--   0        0        0    17722 2024-01-05 11:04:47.064584 gentccode-0.2.1/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.1/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.1/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.1/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.1/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.1/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.1/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0      613 2024-01-16 11:15:59.334461 gentccode-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 gentccode-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1066 2024-04-10 03:12:23.157802 gentccode-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.2/gentccode/__init__.py
+-rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.2/gentccode/cartesian_for_case.py
+-rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.2/gentccode/check_version.py
+-rw-r--r--   0        0        0     3014 2024-04-10 03:10:47.777166 gentccode-0.2.2/gentccode/cli.py
+-rw-r--r--   0        0        0    20333 2024-04-10 03:04:41.206073 gentccode-0.2.2/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.2/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.2/gentccode/generate_case_code.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.2/gentccode/merge_api.py
+-rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.2/gentccode/produce_search_case.py
+-rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.2/gentccode/produce_test_case.py
+-rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.2/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0      612 2024-04-10 03:17:34.058423 gentccode-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 gentccode-0.2.2/PKG-INFO
```

### Comparing `gentccode-0.2.1/LICENSE` & `gentccode-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/README.md` & `gentccode-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 ## 简介
+
 gtc(generate test case) 是一个把http请求转换为测试代码的cli工具
 
 ## 功能
 
 - [x] 支持解析curl命令
 - [x] 支持解析postman文件
 - [x] 支持解析swagger2文件
 - [x] 支持生成笛卡尔积测试脚本
 - [x] 支持解析curl文件并生成Jmeter性能脚本
 - [x] 支持解析curl文件并生成Locust性能脚本
 - [ ] 支持解析postman文件并生成Jmeter性能脚本
 - [ ] 一键生成Jmeter性能压测方案脚本
+
 ## 安装
 
 ```bash
 pip3 install gentccode
+gtc version
 ```
+
 ## 使用
-执行下面命令,会在当前目录生成api文件(`api.yaml`)和测试代码的脚本文件(`test_case.py`)
+
+1. 执行下面命令,会在当前目录生成api文件(`api.yaml`)和测试代码的脚本文件(`test_case.py`)
+
 ```bash
 gtc curl curl.txt
 gtc postman postman.json
 gtc swagger2 swagger.json
--------------------------
-gtc jmeter curl.txt
-gtc locust curl.txt
--------------------------
+```
+
+2. 根据参数生成笛卡尔积的用例脚本
+
+```bash
 gtc cp -n a. curl.txt
 ```
+
+3. 执行下面命令,会生成对应的压测脚本
+
+```bash
+gtc jmeter curl.txt --json-assert code=0
+gtc locust curl.txt
+```
+
 ## 已知问题
 
-- 若postman文件中有变量,则不会生成相对应的代码块.
+- 若postman文件中有变量,则不会生成相对应的代码块.
+- url中必须有http或https协议头
```

### Comparing `gentccode-0.2.1/gentccode/cartesian_for_case.py` & `gentccode-0.2.2/gentccode/cartesian_for_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/check_version.py` & `gentccode-0.2.2/gentccode/check_version.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/cli.py` & `gentccode-0.2.2/gentccode/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 @click.argument("filename", type=click.Path(exists=True))
 def locust(filename):
     product_locust_code(curl_file_path=filename)
 
 
 @click.command(help="generate jmeter script by curl file")
 @click.argument("filename", type=click.Path(exists=True))
+@click.option(
+    "-ja",
+    "--json-assert",
+    required=True,
+    help="json node, like: 'code','data.code','a.b.c'",
+)
 def jmeter(filename):
     convert_payloads_of_curl_to_jmx_file(curl_file_path=filename)
 
 
 @click.command(help="auto generate swagger2 document's test code")
 @click.argument("filename", type=click.Path(exists=True))
 def swagger_at(filename):
```

### Comparing `gentccode-0.2.1/gentccode/convert_to_jmx.py` & `gentccode-0.2.2/gentccode/convert_to_jmx.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,32 +75,32 @@
             "elementType": "LoopController",
             "guiclass": "LoopControlPanel",
             "testclass": "LoopController",
             "testname": "Loop Controller",
             "enabled": "true",
         },
     )
-    boolProp = etree.SubElement(elementProp, "boolProp")
-    boolProp.set("name", "LoopController.continue_forever")
-    boolProp.text = "false"
+    # boolProp = etree.SubElement(elementProp, "boolProp")
+    # boolProp.set("name", "LoopController.continue_forever")
+    # boolProp.text = "false"
     stringProp = etree.SubElement(elementProp, "stringProp")
     stringProp.set("name", "LoopController.loops")
-    stringProp.text = "1"
+    stringProp.text = "-1"
     stringProp = etree.SubElement(theadGroup, "stringProp")
     stringProp.set("name", "ThreadGroup.num_threads")
     stringProp.text = "1"
     stringProp = etree.SubElement(theadGroup, "stringProp")
     stringProp.set("name", "ThreadGroup.ramp_time")
     stringProp.text = "1"
     boolProp = etree.SubElement(theadGroup, "boolProp")
     boolProp.set("name", "ThreadGroup.scheduler")
-    boolProp.text = "false"
+    boolProp.text = "true"
     stringProp = etree.SubElement(theadGroup, "stringProp")
     stringProp.set("name", "ThreadGroup.duration")
-    stringProp.text = ""
+    stringProp.text = "60"
     stringProp = etree.SubElement(theadGroup, "stringProp")
     stringProp.set("name", "ThreadGroup.delay")
     stringProp.text = ""
     return etree.SubElement(parent_xml, "hashTree")
 
 
 def arguments(parent_xml):
@@ -171,30 +171,32 @@
     boolProp.text = "false"
     intProp = etree.SubElement(responseAssertion, "intProp")
     intProp.set("name", "Assertion.test_type")
     intProp.text = "16"
     return etree.SubElement(parent_xml, "hashTree")
 
 
-def json_path_assertion(parent_xml):
+def json_path_assertion(parent_xml, json_path_assert):
+    json_path = json_path_assert.split("=")[0]
+    json_value = json_path_assert.split("=")[1]
     jsonAssertion = etree.SubElement(parent_xml, "JSONPathAssertion")
     set_kv_to_xml(
         jsonAssertion,
         {
             "guiclass": "JSONPathAssertionGui",
             "testclass": "JSONPathAssertion",
             "testname": "JSON Assertion",
         },
     )
     stringProp = etree.SubElement(jsonAssertion, "stringProp")
     stringProp.set("name", "JSON_PATH")
-    stringProp.text = "$.error"
+    stringProp.text = f"$.{json_path}"
     stringProp = etree.SubElement(jsonAssertion, "stringProp")
     stringProp.set("name", "EXPECTED_VALUE")
-    stringProp.text = "0"
+    stringProp.text = f"{json_value}"
     boolProp = etree.SubElement(jsonAssertion, "boolProp")
     boolProp.set("name", "JSONVALIDATION")
     boolProp.text = "false"
     boolProp = etree.SubElement(jsonAssertion, "boolProp")
     boolProp.set("name", "EXPECT_NULL")
     boolProp.text = "false"
     boolProp = etree.SubElement(jsonAssertion, "boolProp")
@@ -350,15 +352,15 @@
 
     # comments
     stringProp = etree.SubElement(HTTPSamplerProxy, "stringProp")
     stringProp.set("name", "TestPlan.comments")
     stringProp.text = payload.get("sampler_comments")
 
 
-def controller(parent_xml, payloads: list):
+def controller(parent_xml, payloads: list, json_path_assert: str):
     for payload in payloads:
         GenericController = etree.SubElement(parent_xml, "GenericController")
         GenericController.set("guiclass", "LogicControllerGui")
         GenericController.set("testclass", "GenericController")
         GenericController.set("testname", payload.get("controller_name"))
         GenericController.set("enabled", "true")
         stringProp = etree.SubElement(GenericController, "stringProp")
@@ -366,34 +368,101 @@
         stringProp.text = payload.get("description")
         shashTree = etree.SubElement(parent_xml, "hashTree")
         header_manager(shashTree, headers=payload["header"])
         # http sampler
         http_sampler_proxy(shashTree, payload)
         # http response assert, hasTree 必须要当前树下,不能做为参数传下去
         responseAssertionTree = etree.SubElement(shashTree, "hashTree")
-        json_path_assertion(responseAssertionTree)
+        json_path_assertion(responseAssertionTree, json_path_assert)
+
+
+def view_result_tree(parent_xml):
+    result_collector = etree.SubElement(parent_xml, "ResultCollector")
+    set_kv_to_xml(
+        result_collector,
+        {
+            "guiclass": "ViewResultsFullVisualizer",
+            "testclass": "ResultCollector",
+            "testname": "View Results Tree",
+        },
+    )
+    # 创建 ResultCollector 的子元素
+    bool_prop = etree.SubElement(
+        result_collector, "boolProp", name="ResultCollector.error_logging"
+    )
+    bool_prop.text = "false"
+
+    obj_prop = etree.SubElement(result_collector, "objProp")
+    etree.SubElement(obj_prop, "name", value="saveConfig")
+    save_config_value = etree.SubElement(
+        obj_prop, "value", {"class": "SampleSaveConfiguration"}
+    )
+
+    # 创建 SampleSaveConfiguration 的子元素
+    elements_to_save = [
+        "time",
+        "latency",
+        "timestamp",
+        "success",
+        "label",
+        "code",
+        "message",
+        "threadName",
+        "dataType",
+        "assertions",
+        "subresults",
+        "bytes",
+        "sentBytes",
+        "url",
+        "threadCounts",
+        "idleTime",
+        "connectTime",
+    ]
+    for element in elements_to_save:
+        sub_element = etree.SubElement(save_config_value, element)
+        sub_element.text = "true"
+
+    etree.SubElement(save_config_value, "encoding").text = "false"
+    etree.SubElement(save_config_value, "responseData").text = "false"
+    etree.SubElement(save_config_value, "samplerData").text = "false"
+    etree.SubElement(save_config_value, "xml").text = "false"
+    etree.SubElement(save_config_value, "fieldNames").text = "true"
+    etree.SubElement(save_config_value, "responseHeaders").text = "false"
+    etree.SubElement(save_config_value, "requestHeaders").text = "false"
+    etree.SubElement(save_config_value, "responseDataOnError").text = "false"
+
+    etree.SubElement(save_config_value, "saveAssertionResultsFailureMessage").text = (
+        "true"
+    )
+    etree.SubElement(save_config_value, "assertionsResultsToSave").text = "0"
+
+    # 创建 stringProp 元素
+    string_prop = etree.SubElement(result_collector, "stringProp", name="filename")
+    string_prop.text = ""
+    return etree.SubElement(parent_xml, "hashTree")
 
 
 def set_kv_to_xml(obj_xml, datas):
     """
 
     :param obj_xml:
     :param datas:
     :return:
     """
     for key, value in datas.items():
         obj_xml.set(key, value)
 
 
-def write_to_jmx(payloads: list):
+def write_to_jmx(payloads: list, json_path_assert: str):
     jmeterTestPlan = etree.Element("jmeterTestPlan")
     hashTree = jmeter_test_plan(jmeterTestPlan)
     testPlan = test_plan(hashTree, "autotest")
     threadGroup = thread_group(testPlan)
-    controller(threadGroup, payloads)
+    controller(threadGroup, payloads, json_path_assert)
+    view_result_tree(threadGroup)
     etree.tostring(jmeterTestPlan, pretty_print=True)
     tree = etree.ElementTree(jmeterTestPlan)
     now_date = time.strftime("%Y%m%d%H%M%S", time.localtime(time.time()))
     tree.write(
         f"jmeter-{now_date}.jmx",
         pretty_print=True,
         xml_declaration=True,
@@ -431,19 +500,19 @@
 def _reduce_url_path(path):
     if path[0] != "/":
         return "/" + path
     else:
         return path
 
 
-def convert_payloads_of_curl_to_jmx_file(curl_file_path):
+def convert_payloads_of_curl_to_jmx_file(curl_file_path, json_path_assert):
     gaf = GenerateApiFile()
     http_payloads = gaf.convert_curl_data_to_model(curl_file_path)
     jmx_payloads = convert_payloads_to_jmx_model(http_payloads=http_payloads)
-    write_to_jmx(payloads=jmx_payloads)
+    write_to_jmx(payloads=jmx_payloads, json_path_assert=json_path_assert)
 
 
 def convert_payloads_to_jmx_model(http_payloads: list[ReqData]) -> list:
     i = 1
     jmx_payloads = []
     for http_payload in http_payloads:
         http_payload = parse_req_data_model(http_payload)
@@ -485,9 +554,11 @@
         "params": "",
         "http_type": "https",
         "params_type": "parameters",
         "sampler_comments": "test-comments",
         "controller_name": "test-controller",
     }
     yaml_file_path = "./script/generated_result/api_template.yaml"
-    curl_file = "/Users/lei.susl/Desktop/test1/tmp"
-    convert_payloads_of_curl_to_jmx_file(curl_file_path=curl_file)
+    curl_file = "/Users/lei.susl/Desktop/test1/risk-control/iac.txt"
+    convert_payloads_of_curl_to_jmx_file(
+        curl_file_path=curl_file, json_path_assert="success=true"
+    )
```

### Comparing `gentccode-0.2.1/gentccode/convert_to_locust.py` & `gentccode-0.2.2/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/generate_case_code.py` & `gentccode-0.2.2/gentccode/generate_case_code.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/merge_api.py` & `gentccode-0.2.2/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/produce_search_case.py` & `gentccode-0.2.2/gentccode/produce_search_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/produce_test_case.py` & `gentccode-0.2.2/gentccode/produce_test_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/gentccode/read_swagger_rule.py` & `gentccode-0.2.2/gentccode/read_swagger_rule.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.1/pyproject.toml` & `gentccode-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.1"
+version = "0.2.2"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 pyyaml = "^6.0"
 http-content-parser = "^0.0.14"
 click = "^8.1.7"
 lxml = "^4.9.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
```

### Comparing `gentccode-0.2.1/PKG-INFO` & `gentccode-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.1
+Version: 0.2.2
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: http-content-parser (>=0.0.14,<0.0.15)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## 简介
+
 gtc(generate test case) 是一个把http请求转换为测试代码的cli工具
 
 ## 功能
 
 - [x] 支持解析curl命令
 - [x] 支持解析postman文件
 - [x] 支持解析swagger2文件
 - [x] 支持生成笛卡尔积测试脚本
 - [x] 支持解析curl文件并生成Jmeter性能脚本
 - [x] 支持解析curl文件并生成Locust性能脚本
 - [ ] 支持解析postman文件并生成Jmeter性能脚本
 - [ ] 一键生成Jmeter性能压测方案脚本
+
 ## 安装
 
 ```bash
 pip3 install gentccode
+gtc version
 ```
+
 ## 使用
-执行下面命令,会在当前目录生成api文件(`api.yaml`)和测试代码的脚本文件(`test_case.py`)
+
+1. 执行下面命令,会在当前目录生成api文件(`api.yaml`)和测试代码的脚本文件(`test_case.py`)
+
 ```bash
 gtc curl curl.txt
 gtc postman postman.json
 gtc swagger2 swagger.json
--------------------------
-gtc jmeter curl.txt
-gtc locust curl.txt
--------------------------
+```
+
+2. 根据参数生成笛卡尔积的用例脚本
+
+```bash
 gtc cp -n a. curl.txt
 ```
+
+3. 执行下面命令,会生成对应的压测脚本
+
+```bash
+gtc jmeter curl.txt --json-assert code=0
+gtc locust curl.txt
+```
+
 ## 已知问题
 
 - 若postman文件中有变量,则不会生成相对应的代码块.
+- url中必须有http或https协议头
+
```

