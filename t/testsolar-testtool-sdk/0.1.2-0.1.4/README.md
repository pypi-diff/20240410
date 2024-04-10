# Comparing `tmp/testsolar-testtool-sdk-0.1.2.tar.gz` & `tmp/testsolar-testtool-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.1.2.tar", last modified: Tue Apr  9 13:14:55 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.1.4.tar", last modified: Wed Apr 10 06:21:57 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.1.2.tar` & `testsolar-testtool-sdk-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.928002 testsolar-testtool-sdk-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.439765 testsolar-testtool-sdk-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.439765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1.2/LICENSE` & `testsolar-testtool-sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/reporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,68 @@
-import hashlib
+import dataclasses
+import json
+import logging
 import os
 import struct
-import logging
-from enum import Enum
 from typing import Optional, BinaryIO
 
 import portalocker
-from pydantic import BaseModel
 
+from .model.encoder import DateTimeEncoder
 from .model.load import LoadResult
 from .model.testresult import TestResult
 
 # 跟TestSolar uniSDK约定的管道上报魔数，避免乱序导致后续数据全部无法上报
 MAGIC_NUMBER = 0x1234ABCD
 
 # 跟TestSolar uniSDK约定的管道上报文件描述符号
 PIPE_WRITER = 3
 
 
-class ReportType(str, Enum):
-    Pipeline = 'pipeline'
-    File = 'file'
+class Reporter:
 
+    def __enter__(self):
+        return self
 
-class Reporter:
-    def __init__(self, reporter_type: ReportType, pipe_io: Optional[BinaryIO] = None, report_path: str = '') -> None:
+    def __init__(self, pipe_io: Optional[BinaryIO] = None) -> None:
         """
         初始化报告工具类
-        :param reporter_type: 报告类型，支持管道类型和文件类型
         :param pipe_io: 可选的管道，用于测试
-        :param report_path: 上报文件路径
         """
         self.lock_file = "/tmp/testsolar_reporter.lock"
-        self.reporter_type = reporter_type
-        if reporter_type == ReportType.Pipeline:
-            if pipe_io:
-                self.pipe_io = pipe_io
-            else:
-                self.pipe_io = os.fdopen(PIPE_WRITER, "wb")
-        elif reporter_type == ReportType.File:
-            if not report_path:
-                raise RuntimeError('report_path is required')
-            self.report_path = report_path
+
+        if pipe_io:
+            self.pipe_io = pipe_io
+        else:
+            self.pipe_io = os.fdopen(PIPE_WRITER, "wb")
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
     def report_load_result(self, load_result: LoadResult) -> None:
-        if self.reporter_type == ReportType.Pipeline:
-            with portalocker.Lock(self.lock_file, timeout=60):
-                self._send_json(load_result)
-        elif self.reporter_type == ReportType.File:
-            self._write_load_file(load_result)
+        with portalocker.Lock(self.lock_file, timeout=60):
+            self._send_json(dataclasses.asdict(load_result))
 
     def report_run_case_result(self, run_case_result: TestResult) -> None:
-        if self.reporter_type == ReportType.Pipeline:
-            with portalocker.Lock(self.lock_file, timeout=60):
-                self._send_json(run_case_result)
-        elif self.reporter_type == ReportType.File:
-            self._write_case_result(run_case_result)
+        with portalocker.Lock(self.lock_file, timeout=60):
+            self._send_json(dataclasses.asdict(run_case_result))
 
     def close(self) -> None:
         if self.pipe_io:
             self.pipe_io.close()
 
-    def _send_json(self, result: BaseModel) -> None:
-        data = result.model_dump_json(by_alias=True).encode("utf-8")
+    def _send_json(self, result: dict) -> None:
+        data = json.dumps(result, cls=DateTimeEncoder).encode('utf-8')
         length = len(data)
 
         # 将魔数写入管道
         self.pipe_io.write(struct.pack("<I", MAGIC_NUMBER))
 
         # 将 JSON 数据的长度写入管道
         self.pipe_io.write(struct.pack("<I", length))
 
         # 将 JSON 数据本身写入管道
         self.pipe_io.write(data)
 
         logging.debug(f"Sending {length} bytes to pipe {PIPE_WRITER}")
 
         self.pipe_io.flush()
-
-    def _write_load_file(self, load_result: LoadResult) -> None:
-        with open(os.path.join(self.report_path, 'result.json'), "wb") as f:
-            logging.debug(f"Writing load results to {self.report_path}")
-            f.write(load_result.model_dump_json(by_alias=True, indent=2).encode('utf-8'))
-
-    def _write_case_result(self, case_result: TestResult) -> None:
-        retry_id = case_result.test.attrs.get('retry', '0')
-        filename = hashlib.md5(f"{case_result.test.name}.{retry_id}".encode('utf-8')).hexdigest() + ".json"
-        with open(os.path.join(self.report_path, filename), "wb") as f:
-            logging.debug(f"Writing case results to {self.report_path}")
-            f.write(case_result.model_dump_json(by_alias=True, indent=2).encode('utf-8'))
```

### Comparing `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 src/testsolar_testtool_sdk/reporter.py
 src/testsolar_testtool_sdk.egg-info/PKG-INFO
 src/testsolar_testtool_sdk.egg-info/SOURCES.txt
 src/testsolar_testtool_sdk.egg-info/dependency_links.txt
 src/testsolar_testtool_sdk.egg-info/requires.txt
 src/testsolar_testtool_sdk.egg-info/top_level.txt
 src/testsolar_testtool_sdk/model/__init__.py
+src/testsolar_testtool_sdk/model/encoder.py
 src/testsolar_testtool_sdk/model/load.py
 src/testsolar_testtool_sdk/model/param.py
 src/testsolar_testtool_sdk/model/test.py
 src/testsolar_testtool_sdk/model/testresult.py
 tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1.2/tests/test_report.py` & `testsolar-testtool-sdk-0.1.4/tests/test_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import concurrent.futures
+import dataclasses
 import io
 import json
 import logging
 import random
 from datetime import datetime, timedelta
 from functools import partial
-from typing import BinaryIO
 
+from src.testsolar_testtool_sdk.model.encoder import DateTimeEncoder
 from src.testsolar_testtool_sdk.model.load import LoadResult, LoadError
 from src.testsolar_testtool_sdk.model.test import TestCase
 from src.testsolar_testtool_sdk.model.testresult import ResultType, LogLevel
 from src.testsolar_testtool_sdk.model.testresult import (
     TestResult,
     TestCaseStep,
     TestCaseAssertError,
     TestCaseLog,
 )
 from src.testsolar_testtool_sdk.pipe_reader import read_load_result, read_test_result
-from src.testsolar_testtool_sdk.reporter import Reporter, ReportType
+from src.testsolar_testtool_sdk.reporter import Reporter
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 def generate_demo_load_result() -> LoadResult:
     r: LoadResult = LoadResult(Tests=[], LoadErrors=[])
 
     for x in range(40):
-        r.tests.append(
+        r.Tests.append(
             TestCase(
                 Name=f"mumu/mu.py/test_case_name_{x}_p1", Attributes={"tag": "P1"}
             )
         )
 
     for x in range(20):
-        r.load_errors.append(
+        r.LoadErrors.append(
             LoadError(
                 name=f"load error {x}",
                 message=f"""
 文件读取失败。可能的原因包括：文件不存在、文件损坏、
 不正确的编码方式或其他未知错误。请检查文件路径和内容的正确性，
 确保文件具有正确的编码格式。如果问题仍然存在，可能需要尝试其他解决方法
 
@@ -126,66 +127,63 @@
     ]
     return "".join(random.choice(alphabet) for i in range(length))
 
 
 def test_report_load_result() -> None:
     # 创建一个Reporter实例
     pipe_io = io.BytesIO()
-    reporter = Reporter(reporter_type=ReportType.Pipeline, pipe_io=pipe_io)
+    with Reporter(pipe_io=pipe_io) as reporter:
+        # 创建一个LoadResult实例
+        load_result = generate_demo_load_result()
 
-    # 创建一个LoadResult实例
-    load_result = generate_demo_load_result()
+        # 调用report_load_result方法
+        reporter.report_load_result(load_result)
 
-    # 调用report_load_result方法
-    reporter.report_load_result(load_result)
+        # 检查管道中的魔数
+        pipe_io.seek(0)
 
-    # 检查管道中的魔数
-    pipe_io.seek(0)
+        loaded = read_load_result(pipe_io)
+        assert loaded == load_result
 
-    loaded = read_load_result(pipe_io)
-    assert loaded == load_result
 
-
-def send_test_result(pipe_io: BinaryIO):
-    reporter = Reporter(reporter_type=ReportType.Pipeline, pipe_io=pipe_io)
+def send_test_result(reporter: Reporter):
     test_results = []
     run_case_result = generate_test_result(0)
     test_results.append(run_case_result)
     reporter.report_run_case_result(run_case_result)
 
 
 def test_datetime_formatted():
     run_case_result = generate_test_result(0)
-    data = run_case_result.model_dump_json(by_alias=True, indent=2)
+    data = json.dumps(dataclasses.asdict(run_case_result), cls=DateTimeEncoder)
     tr = json.loads(data)
     assert tr['StartTime'].endswith("Z")
     assert tr['EndTime'].endswith("Z")
 
     assert tr['Steps'][0]['StartTime'].endswith("Z")
     assert tr['Steps'][0]['EndTime'].endswith("Z")
 
     assert tr['Steps'][0]['Logs'][0]['Time'].endswith("Z")
 
 
 def test_report_run_case_result():
     # 创建一个Reporter实例
     pipe_io = io.BytesIO()
-
-    send_action = partial(send_test_result, pipe_io)
-
-    # 创建五个LoadResult实例并发调用report_run_case_result方法
-    with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
-        for i in range(5):
-            executor.submit(send_action)
-
-    # 检查管道中的数据，确保每个用例的魔数和数据长度还有数据正确
-    pipe_io.seek(0)
-    r1: TestResult = read_test_result(pipe_io)
-    assert r1.result_type == ResultType.SUCCEED
-    r2 = read_test_result(pipe_io)
-    assert r2.result_type == ResultType.SUCCEED
-    r3 = read_test_result(pipe_io)
-    assert r3.result_type == ResultType.SUCCEED
-    r4 = read_test_result(pipe_io)
-    assert r4.result_type == ResultType.SUCCEED
-    r5 = read_test_result(pipe_io)
-    assert r5.result_type == ResultType.SUCCEED
+    with Reporter(pipe_io=pipe_io) as reporter:
+        # 创建五个LoadResult实例并发调用report_run_case_result方法
+        with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
+            send_action = partial(send_test_result, reporter)
+            for i in range(5):
+                executor.submit(send_action)
+
+        # 检查管道中的数据，确保每个用例的魔数和数据长度还有数据正确
+        pipe_io.seek(0)
+        r1: TestResult = read_test_result(pipe_io)
+        assert r1.ResultType == ResultType.SUCCEED
+        r2 = read_test_result(pipe_io)
+        assert r2.ResultType == ResultType.SUCCEED
+        r3 = read_test_result(pipe_io)
+        assert r3.ResultType == ResultType.SUCCEED
+        r4 = read_test_result(pipe_io)
+        assert r4.ResultType == ResultType.SUCCEED
+        r5 = read_test_result(pipe_io)
+        assert r5.ResultType == ResultType.SUCCEED
```

