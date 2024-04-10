# Comparing `tmp/oteltest-0.3.0.tar.gz` & `tmp/oteltest-0.4.0.tar.gz`

## Comparing `oteltest-0.3.0.tar` & `oteltest-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.3.0/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 oteltest-0.3.0/example_scripts/simple_loop.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/__init__.py
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/common.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/main.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/sink.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.3.0/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.3.0/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.4.0/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1584 2020-02-02 00:00:00.000000 oteltest-0.4.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/common.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/sink.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.4.0/src/oteltest/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.4.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.4.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.4.0/PKG-INFO
```

### Comparing `oteltest-0.3.0/example_scripts/simple_loop.py` & `oteltest-0.4.0/example_scripts/simple_loop.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,40 +9,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
-from typing import Mapping, Sequence
+from typing import Mapping, Optional, Sequence
 
 from opentelemetry import trace
 from oteltest.common import OtelTest, Telemetry
 
 SERVICE_NAME = "integration-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
-            print(f"{i+1}/{NUM_ADDS}")
+            print(f"simple_loop.py: {i+1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
 class MyTest(OtelTest):
     def requirements(self) -> Sequence[str]:
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
     def environment_variables(self) -> Mapping[str, str]:
         return {"OTEL_SERVICE_NAME": SERVICE_NAME}
 
     def wrapper_script(self) -> str:
         return "opentelemetry-instrument"
 
     def run_client(self) -> None:
-        for j in range(10):
-            time.sleep(1)
-            print(f"i: {j}")
+        print("run_client()")
+
+    def max_wait(self) -> Optional[float]:
+        return 60
 
     def validate(self, telemetry: Telemetry) -> None:
         assert telemetry.num_spans() == NUM_ADDS
```

### Comparing `oteltest-0.3.0/src/oteltest/__init__.py` & `oteltest-0.4.0/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/src/oteltest/common.py` & `oteltest-0.4.0/src/oteltest/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,9 +128,13 @@
         pass
 
     @abc.abstractmethod
     def run_client(self) -> None:
         pass
 
     @abc.abstractmethod
+    def max_wait(self) -> Optional[float]:
+        return None
+
+    @abc.abstractmethod
     def validate(self, telemetry: Telemetry) -> None:
         pass
```

### Comparing `oteltest-0.3.0/src/oteltest/main.py` & `oteltest-0.4.0/src/oteltest/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,59 +86,64 @@
 def setup_script_environment(script, script_dir, tempdir, wheel_file):
     handler = AccumulatingHandler()
     sink = GrpcSink(handler)
     sink.start()
 
     module_name = script[:-3]
     test_class = load_test_class_for_script(module_name)
-    test_instance: OtelTest = test_class()
+    oteltest_instance: OtelTest = test_class()
 
     v = Venv(str(Path(tempdir) / module_name))
     v.create()
 
     pip_path = v.path_to_executable("pip")
 
     oteltest_dep = wheel_file or "oteltest"
     run_subprocess([pip_path, "install", oteltest_dep])
 
-    for req in test_instance.requirements():
+    for req in oteltest_instance.requirements():
         print(f"- Will install requirement: '{req}'")
         run_subprocess([pip_path, "install", req])
 
-    run_python_script(script, script_dir, test_instance, v)
+    run_python_script(script, script_dir, oteltest_instance, v)
 
     v.rm()
 
     with open(str(Path(script_dir) / f"{module_name}.json"), "w") as file:
         file.write(handler.telemetry_to_json())
 
-    test_instance.validate(handler.telemetry)
+    oteltest_instance.validate(handler.telemetry)
     print(f"- {script} PASSED")
 
 
-def run_python_script(script, script_dir, test_instance: OtelTest, v):
+def run_python_script(script, script_dir, oteltest_instance: OtelTest, v):
     python_script_cmd = [
         v.path_to_executable("python"),
         str(Path(script_dir) / script),
     ]
-    script = test_instance.wrapper_script()
+    script = oteltest_instance.wrapper_script()
     if script is not None:
         python_script_cmd.insert(0, v.path_to_executable(script))
 
     process = subprocess.Popen(
         python_script_cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
-        env=test_instance.environment_variables(),
+        env=oteltest_instance.environment_variables(),
     )
 
-    test_instance.run_client()
+    oteltest_instance.run_client()
 
     # wait for the process to terminate
-    stdout, stderr = process.communicate()
+    timeout = oteltest_instance.max_wait()
+    if timeout is None:
+        print("- Will wait indefinitely for script to finish (max_wait() returned None)")
+    else:
+        print(f"- Will wait up to {timeout} seconds for script to finish")
+    stdout, stderr = process.communicate(timeout=timeout)
 
     print_result(process.returncode, stderr, stdout)
 
 
 def run_subprocess(args, env_vars=None):
     print(f"- Subprocess: {args}")
     print(f"- Environment: {env_vars}")
```

### Comparing `oteltest-0.3.0/src/oteltest/sink.py` & `oteltest-0.4.0/src/oteltest/sink.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/src/oteltest/version.py` & `oteltest-0.4.0/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "0.3.0"
```

### Comparing `oteltest-0.3.0/tests/__init__.py` & `oteltest-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/.gitignore` & `oteltest-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/LICENSE.txt` & `oteltest-0.4.0/src/oteltest/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "0.4.0"
```

### Comparing `oteltest-0.3.0/README.md` & `oteltest-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/pyproject.toml` & `oteltest-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.3.0/PKG-INFO` & `oteltest-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

