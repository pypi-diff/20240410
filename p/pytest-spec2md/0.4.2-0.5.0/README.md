# Comparing `tmp/pytest_spec2md-0.4.2-py3-none-any.whl.zip` & `tmp/pytest_spec2md-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21567 bytes, number of entries: 9
+Zip file size: 21816 bytes, number of entries: 9
 -rw-r--r--  2.0 unx    18092 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 pytest_spec2md/__init__.py
--rw-r--r--  2.0 unx     3292 b- defN 80-Jan-01 00:00 pytest_spec2md/plugin.py
--rw-r--r--  2.0 unx    12934 b- defN 80-Jan-01 00:00 pytest_spec2md/spec_creator.py
--rw-r--r--  2.0 unx    18092 b- defN 80-Jan-01 00:00 pytest_spec2md-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3918 b- defN 80-Jan-01 00:00 pytest_spec2md-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pytest_spec2md-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 pytest_spec2md-0.4.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      740 b- defN 16-Jan-01 00:00 pytest_spec2md-0.4.2.dist-info/RECORD
-9 files, 57231 bytes uncompressed, 20293 bytes compressed:  64.5%
+-rw-r--r--  2.0 unx     3882 b- defN 80-Jan-01 00:00 pytest_spec2md/plugin.py
+-rw-r--r--  2.0 unx    13392 b- defN 80-Jan-01 00:00 pytest_spec2md/spec_creator.py
+-rw-r--r--  2.0 unx    18092 b- defN 80-Jan-01 00:00 pytest_spec2md-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3918 b- defN 80-Jan-01 00:00 pytest_spec2md-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pytest_spec2md-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 pytest_spec2md-0.5.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      740 b- defN 16-Jan-01 00:00 pytest_spec2md-0.5.0.dist-info/RECORD
+9 files, 58279 bytes uncompressed, 20542 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pytest_spec2md/plugin.py
 Comment: 
 
 Filename: pytest_spec2md/spec_creator.py
 Comment: 
 
-Filename: pytest_spec2md-0.4.2.dist-info/LICENSE
+Filename: pytest_spec2md-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytest_spec2md-0.4.2.dist-info/METADATA
+Filename: pytest_spec2md-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pytest_spec2md-0.4.2.dist-info/WHEEL
+Filename: pytest_spec2md-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_spec2md-0.4.2.dist-info/entry_points.txt
+Filename: pytest_spec2md-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_spec2md-0.4.2.dist-info/RECORD
+Filename: pytest_spec2md-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_spec2md/plugin.py

```diff
@@ -101,11 +101,26 @@
 @pytest.hookimpl(trylast=True)
 def pytest_runtest_logreport(report):
     if report.when == 'call':
         pytest_spec2md.spec_creator.SpecWriter.create_specification_documents(
             config=_act_config, report=report)
 
 
-def pytest_terminal_summary(terminalreporter, exitstatus, config):
+def pytest_terminal_summary(terminalreporter: _pytest.terminal.TerminalReporter, exitstatus, config):
     writer = pytest_spec2md.spec_creator.SpecWriter.get_writer(pytest_spec2md.spec_creator.SpecWithTestsWriter, None)
 
     writer.write_final_report()
+
+    terminalreporter.write(("\n"
+                            "================================== Doc Stats ==================================\n"
+                            f"Number of Keywords: {len(writer.keys)}\n"
+                            f"Used Keywords: {writer.used_keywords}\n"
+                            "\n"
+                            ), flush=True)
+
+    if writer.warnings:
+        terminalreporter.write("Warnings:\n  * ")
+        terminalreporter.write('\n  * '.join(writer.warnings))
+        terminalreporter.write("\n", flush=True)
+
+
+
```

## pytest_spec2md/spec_creator.py

```diff
@@ -1,14 +1,15 @@
 import datetime
 import importlib
 import inspect
 import os
 import sys
 import typing
 import warnings
+from copy import copy
 
 import _pytest.nodes
 import _pytest.reports
 import pytest
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
@@ -250,14 +251,28 @@
 
         self._target_file = config.getini('spec_target_file')
 
         self._version = config.option.spec2md_version
         self._test_run_id = f'TestRun {datetime.datetime.now():%Y-%m-%d %H:%M}'
 
         self._results: dict[str, _pytest.reports.TestReport] = {}
+        self._used_keywords: int = 0
+        self._warnings: list[str] = []
+
+    @property
+    def keys(self) -> list[str]:
+        return list(self._results.keys())
+
+    @property
+    def used_keywords(self) -> int:
+        return self._used_keywords
+
+    @property
+    def warnings(self):
+        return copy(self._warnings)
 
     def write_node_to_file(self, report: _pytest.reports.TestReport):
         self._results[report.nodeid] = report
 
     def add_test(self, key: str, test: _pytest.nodes.Node):
         if key not in self._grouped_tests:
             self._grouped_tests[key] = []
@@ -271,14 +286,17 @@
         content = self._get_content()
 
         with open(self._target_file, 'w') as target:
             for line in content:
                 target.write(line)
 
     def _get_content(self):
+        self._used_keywords = 0
+        self._warnings .clear()
+
         if not self._source_file or not os.path.exists(self._source_file):
             return
 
         used_identifier = []
 
         with open(self._source_file) as source:
             for line in source.readlines():
@@ -287,38 +305,39 @@
         self._check_for_usage(used_identifier)
 
     def _process_line(self, line, used_identifier):
         yield line
 
         line = line.strip()
         if line.startswith('<!-- TestRef:') and line.endswith('-->'):
+            self._used_keywords += 1
             identifier = line[13:-3].strip()
             used_identifier.append(identifier)
             for entry in self._format_tests(identifier):
                 yield entry
 
     def _check_for_usage(self, used_identifier):
         for key in self._grouped_tests:
             if key not in used_identifier:
-                warnings.warn(Warning(f'Identifier {key} was not used in the spec document {self._source_file}.'))
+                self._warnings.append(f'Identifier "{key}" was not used in the spec document "{self._source_file}".')
 
     def _format_tests(self, identifier: str):
         if identifier not in self._grouped_tests:
-            warnings.warn(Warning(f'Identifier {identifier} in file {self._source_file}'
-                                    f' is not used in any test.'))
+            self._warnings.append(f'Identifier "{identifier}" in file "{self._source_file}"'
+                                  f' is not used in any test.')
             yield f'> **No Proves found for Reference *{identifier}*** \n'
             return
 
         items = self._grouped_tests[identifier]
 
-        yield f'> **Proved by Tests for Reference *{identifier}*** \n'
-        yield '>\n'
-        yield (f'> The following tests proved this feature in the test run *{self._test_run_id}* '
-               f'on version {self._version}.\n')
-        yield '>\n'
+        yield (f'> **Proved by Tests for Reference *{identifier}*** \n'
+               '>\n'
+               f'> The following tests proved this feature in the test run *{self._test_run_id}* '
+               f'on version {self._version}.\n'
+               '>\n')
 
         yield '>>| # |   | Name | Type | Explanation | Path |  \n'
         yield '>>| --- | --- | --- | --- | --- | --- | \n'
         for index, item in enumerate(items):
             report = self._results[item.nodeid]
             yield (f">>| {index + 1} | "
                    f"{':heavy_check_mark:' if report.passed else ':x:'} | "
```

## Comparing `pytest_spec2md-0.4.2.dist-info/LICENSE` & `pytest_spec2md-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytest_spec2md-0.4.2.dist-info/METADATA` & `pytest_spec2md-0.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-spec2md
-Version: 0.4.2
+Version: 0.5.0
 Summary: Library pytest-spec2md is a pytest plugin to create a markdown specification while running pytest.
 Home-page: https://dev.azure.com/h7d/Quality/
 License: GPL-2.0-or-later
 Keywords: pytest,test,unittest,specification,markdown
 Author: mh7d
 Maintainer: mh7d
 Requires-Python: >3.9,<4
```

