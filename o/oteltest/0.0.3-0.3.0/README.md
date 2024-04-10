# Comparing `tmp/oteltest-0.0.3.tar.gz` & `tmp/oteltest-0.3.0.tar.gz`

## Comparing `oteltest-0.0.3.tar` & `oteltest-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.0.3/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 oteltest-0.0.3/example_scripts/simple_loop.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/__init__.py
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/common.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/main.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/sink.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.0.3/src/oteltest/version.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.0.3/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.0.3/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.3.0/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 oteltest-0.3.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/common.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/sink.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.3.0/src/oteltest/version.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.3.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.3.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.3.0/PKG-INFO
```

### Comparing `oteltest-0.0.3/example_scripts/simple_loop.json` & `oteltest-0.3.0/example_scripts/simple_loop.json`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/example_scripts/simple_loop.py` & `oteltest-0.3.0/example_scripts/simple_loop.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/src/oteltest/__init__.py` & `oteltest-0.3.0/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/src/oteltest/common.py` & `oteltest-0.3.0/src/oteltest/common.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/src/oteltest/main.py` & `oteltest-0.3.0/src/oteltest/main.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/src/oteltest/sink.py` & `oteltest-0.3.0/src/oteltest/sink.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/src/oteltest/version.py` & `oteltest-0.3.0/src/oteltest/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.3"
+__version__ = "0.3.0"
```

### Comparing `oteltest-0.0.3/tests/__init__.py` & `oteltest-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/.gitignore` & `oteltest-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/LICENSE.txt` & `oteltest-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/README.md` & `oteltest-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/pyproject.toml` & `oteltest-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.0.3/PKG-INFO` & `oteltest-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.0.3
+Version: 0.3.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

