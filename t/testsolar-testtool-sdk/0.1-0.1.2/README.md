# Comparing `tmp/testsolar-testtool-sdk-0.1.tar.gz` & `tmp/testsolar-testtool-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.1.tar", last modified: Tue Apr  9 08:36:49 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.1.2.tar", last modified: Tue Apr  9 13:14:55 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.1.tar` & `testsolar-testtool-sdk-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.147272 testsolar-testtool-sdk-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.147272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 08:36:49.000000 testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:36:49.151272 testsolar-testtool-sdk-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-09 08:36:20.000000 testsolar-testtool-sdk-0.1/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.928002 testsolar-testtool-sdk-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 13:14:55.000000 testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:14:55.932002 testsolar-testtool-sdk-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-09 13:14:21.000000 testsolar-testtool-sdk-0.1.2/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1/LICENSE` & `testsolar-testtool-sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from typing import List, Optional
+from datetime import datetime
 
 from pydantic import BaseModel, Field
 
 from .test import TestCase
 
 
 class ResultType(str, Enum):
@@ -50,33 +51,52 @@
     url: str = Field(alias="Url")
     type: AttachmentType = Field(alias="AttachmentType")
 
 
 class TestCaseLog(BaseModel):
     __test__ = False
 
-    time: str = Field(alias="Time")
+    time: datetime = Field(alias="Time")
     level: LogLevel = Field(alias="Level")
     content: str = Field(alias="Content")
     attachments: List[Attachment] = Field(alias="Attachments")
     assert_error: TestCaseAssertError = Field(alias="AssertError")
     runtime_error: Optional[TestCaseRuntimeError] = Field(None, alias="RuntimeError")
 
+    class Config:
+        json_encoders = {
+            datetime: lambda dt: _format_datetime(dt),
+        }
+
 
 class TestCaseStep(BaseModel):
     __test__ = False
 
-    start_time: str = Field(alias="StartTime")
-    end_time: Optional[str] = Field(alias="EndTime")
+    start_time: datetime = Field(alias="StartTime")
+    end_time: Optional[datetime] = Field(alias="EndTime")
     title: str = Field(alias="Title")
     logs: List[TestCaseLog] = Field(alias="Logs")
 
+    class Config:
+        json_encoders = {
+            datetime: lambda dt: _format_datetime(dt),
+        }
+
+
+def _format_datetime(t: datetime) -> str:
+    return t.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
+
 
 class TestResult(BaseModel):
     __test__ = False
 
     test: TestCase = Field(alias="Test")
-    start_time: str = Field(alias="StartTime")
-    end_time: Optional[str] = Field(alias="EndTime")
+    start_time: datetime = Field(alias="StartTime")
+    end_time: Optional[datetime] = Field(alias="EndTime")
     result_type: ResultType = Field(alias="ResultType")
     message: str = Field(alias="Message")
     steps: List[TestCaseStep] = Field(alias="Steps")
+
+    class Config:
+        json_encoders = {
+            datetime: lambda dt: _format_datetime(dt),
+        }
```

### Comparing `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.1.2/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1/tests/test_report.py` & `testsolar-testtool-sdk-0.1.2/tests/test_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import concurrent.futures
 import io
+import json
 import logging
 import random
 from datetime import datetime, timedelta
-from typing import BinaryIO
 from functools import partial
+from typing import BinaryIO
 
 from src.testsolar_testtool_sdk.model.load import LoadResult, LoadError
 from src.testsolar_testtool_sdk.model.test import TestCase
 from src.testsolar_testtool_sdk.model.testresult import ResultType, LogLevel
 from src.testsolar_testtool_sdk.model.testresult import (
     TestResult,
     TestCaseStep,
@@ -18,18 +19,14 @@
 from src.testsolar_testtool_sdk.pipe_reader import read_load_result, read_test_result
 from src.testsolar_testtool_sdk.reporter import Reporter, ReportType
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
-def _format_datetime(t: datetime) -> str:
-    return t.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
-
-
 def generate_demo_load_result() -> LoadResult:
     r: LoadResult = LoadResult(Tests=[], LoadErrors=[])
 
     for x in range(40):
         r.tests.append(
             TestCase(
                 Name=f"mumu/mu.py/test_case_name_{x}_p1", Attributes={"tag": "P1"}
@@ -58,29 +55,29 @@
     return r
 
 
 def generate_test_result(index: int) -> TestResult:
     start: datetime = datetime.utcnow() - timedelta(seconds=40)
     _tr = TestResult(
         Test=TestCase(Name=f"mumu/mu.py/test_case_name_{index}_p1", Attributes={}),
-        StartTime=_format_datetime(start),
-        EndTime=_format_datetime(datetime.utcnow()),
+        StartTime=start,
+        EndTime=datetime.utcnow(),
         ResultType=ResultType.SUCCEED,
         Message="ファイルが見つかりません。ファイルパスを確認して、もう一度試してください。",
         Steps=[generate_testcase_step(f"{index}_{x}") for x in range(10)],
     )
 
     return _tr
 
 
 def generate_testcase_log(index: str) -> TestCaseLog:
     start: datetime = datetime.utcnow() - timedelta(seconds=15)
 
     return TestCaseLog(
-        Time=_format_datetime(start),
+        Time=start,
         Level=LogLevel.INFO,
         Attachments=[
             # Attachment(
             #     Name=f"access.log_{index}",
             #     Url=str(Path(__file__).parent.resolve().joinpath("test_access.log")),
             #     AttachmentType=AttachmentType.FILE,
             # ),
@@ -91,16 +88,16 @@
         Content=f"采集器：coll-imrv6szb当前状态为0，预期状态为1，状态不一致（0:处理中,1:正常） -> {get_random_unicode(20)}",
     )
 
 
 def generate_testcase_step(index: str) -> TestCaseStep:
     start: datetime = datetime.utcnow() - timedelta(seconds=10)
     return TestCaseStep(
-        StartTime=_format_datetime(start),
-        EndTime=_format_datetime(datetime.utcnow()),
+        StartTime=start,
+        EndTime=datetime.utcnow(),
         Title=get_random_unicode(100),
         Logs=[generate_testcase_log(f"{index}_{x}") for x in range(100)],
     )
 
 
 def get_random_unicode(length) -> str:
     get_char = chr
@@ -152,14 +149,27 @@
     reporter = Reporter(reporter_type=ReportType.Pipeline, pipe_io=pipe_io)
     test_results = []
     run_case_result = generate_test_result(0)
     test_results.append(run_case_result)
     reporter.report_run_case_result(run_case_result)
 
 
+def test_datetime_formatted():
+    run_case_result = generate_test_result(0)
+    data = run_case_result.model_dump_json(by_alias=True, indent=2)
+    tr = json.loads(data)
+    assert tr['StartTime'].endswith("Z")
+    assert tr['EndTime'].endswith("Z")
+
+    assert tr['Steps'][0]['StartTime'].endswith("Z")
+    assert tr['Steps'][0]['EndTime'].endswith("Z")
+
+    assert tr['Steps'][0]['Logs'][0]['Time'].endswith("Z")
+
+
 def test_report_run_case_result():
     # 创建一个Reporter实例
     pipe_io = io.BytesIO()
 
     send_action = partial(send_test_result, pipe_io)
 
     # 创建五个LoadResult实例并发调用report_run_case_result方法
```

