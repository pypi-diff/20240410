# Comparing `tmp/qci-client-3.1.0.tar.gz` & `tmp/qci-client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qci-client-3.1.0.tar", last modified: Wed Apr  3 20:05:50 2024, max compression
+gzip compressed data, was "qci-client-3.2.0.tar", last modified: Wed Apr 10 20:57:28 2024, max compression
```

## Comparing `qci-client-3.1.0.tar` & `qci-client-3.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.506949 qci-client-3.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-03 20:02:27.000000 qci-client-3.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5375 2024-04-03 20:02:27.000000 qci-client-3.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-03 20:02:27.000000 qci-client-3.1.0/.mega-linter.yml
--rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-03 20:02:27.000000 qci-client-3.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-03 20:02:27.000000 qci-client-3.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-03 20:05:50.506949 qci-client-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-03 20:02:27.000000 qci-client-3.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-03 20:02:27.000000 qci-client-3.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/qci_client/
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5234 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/enum.py
--rw-rw-rw-   0 root         (0) root         (0)    26746 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)    13005 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/types.py
--rw-rw-rw-   0 root         (0) root         (0)    16140 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/qci_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 20:05:50.506949 qci-client-3.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12057 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_data_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    29749 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_qci_client.py
--rw-rw-rw-   0 root         (0) root         (0)     7826 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_remote_jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-10 20:54:33.000000 qci-client-3.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-10 20:54:33.000000 qci-client-3.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-10 20:54:33.000000 qci-client-3.2.0/.mega-linter.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-10 20:54:33.000000 qci-client-3.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-10 20:54:33.000000 qci-client-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-10 20:57:28.920869 qci-client-3.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-10 20:54:33.000000 qci-client-3.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-10 20:54:33.000000 qci-client-3.2.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.916869 qci-client-3.2.0/qci_client/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    27324 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    13726 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/types.py
+-rw-rw-rw-   0 root         (0) root         (0)    16845 2024-04-10 20:54:33.000000 qci-client-3.2.0/qci_client/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/qci_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-10 20:57:28.000000 qci-client-3.2.0/qci_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 20:57:28.920869 qci-client-3.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 20:57:28.920869 qci-client-3.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9336 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    32556 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-10 20:54:33.000000 qci-client-3.2.0/tests/test_remote_jobs.py
```

### Comparing `qci-client-3.1.0/.gitlab-ci.yml` & `qci-client-3.2.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     - sphinx-build -b html source build/html
     - sphinx-build -b xml source build/xml
     - cd build/html
     - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *
     - cd ../xml
     - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *.xml
   artifacts:
-    name: $CI_PROJECT_NAME-docs-$CI_COMMIT_BRANCH-$CI_COMMIT_SHORT_SHA
+    name: ${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}
     when: always
     paths:
       - docs/dist
     expire_in: 1 week
 
 docs-tag:
   stage: build
@@ -103,19 +103,19 @@
     - mkdir dist
     - mkdir dist/html
     - mkdir dist/xml
     - make clean
     - sphinx-build -b html source build/html
     - sphinx-build -b xml source build/xml
     - cd build/html
-    - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *
+    - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}.zip *
     - cd ../xml
-    - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *.xml
+    - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}.zip *.xml
   artifacts:
-    name: $CI_PROJECT_NAME-docs-$CI_COMMIT_BRANCH-$CI_COMMIT_SHORT_SHA
+    name: ${CI_PROJECT_NAME}-docs-${CI_COMMIT_TAG}
     when: always
     paths:
       - docs/dist
     expire_in: never
 
 code-check-semgrep:
   stage: test
```

### Comparing `qci-client-3.1.0/.mega-linter.yml` & `qci-client-3.2.0/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/LICENSE` & `qci-client-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/PKG-INFO` & `qci-client-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.1.0
+Version: 3.2.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `qci-client-3.1.0/README.md` & `qci-client-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/pyproject.toml` & `qci-client-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/qci_client/base.py` & `qci-client-3.2.0/qci_client/base.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/qci_client/data_converter.py` & `qci-client-3.2.0/qci_client/data_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -76,50 +76,46 @@
     Args:
         file: file dictionary whose data of type numpy.ndarray, scipy.sparse.spmatrix, or networkx.Graph is to be converted
         debug: Optional, if set to True, enables debug output (default = False for no debug output)
 
     Returns:
         file dictionary with JSON-serializable data
     """
-    # TODO: could add support for matrices stored as lists
-    start = time.perf_counter()
+    start_time_s = time.perf_counter()
 
-    supported_file_types = [
-        "graph",
-        "qubo",
-        "hamiltonian",
-        "objective",
-        "constraints",
-    ]
+    supported_file_types = [type.value for type in enum.JOB_INPUTS_FILE_TYPES]
+    supported_file_types.sort()
+    supported_file_types = tuple(supported_file_types)
+    matrix_file_types = [type.value for type in enum.JOB_INPUTS_MATRIX_FILE_TYPES]
+    matrix_file_types.sort()
+    matrix_file_types = tuple(matrix_file_types)
 
     file_type = enum.get_file_type(file=file).value
 
     if file_type not in supported_file_types:
         raise AssertionError(
-            f"Unsupported file type input, specify one of {supported_file_types}"
+            f"data conversion not supported for file type '{file_type}', supported "
+            f"types are {supported_file_types}"
         )
 
     data = file['file_config'][file_type]['data']
-    file_config = {}
 
     if file_type == "graph":
-        
         if not isinstance(data, nx.Graph):
-            raise AssertionError("file_type 'graph' data must be type networkx.Graph")
+            raise AssertionError("file_type 'graph' data must be a networkx.Graph")
 
-        data = {
+        file_config = {
             **nx.node_link_data(data),
             "num_edges": data.number_of_edges(),
             "num_nodes": data.number_of_nodes(),
         }
-    else:
+    elif file_type in matrix_file_types:
         if isinstance(data, nx.Graph):
             raise AssertionError(
-                "file_types ['objective', 'qubo', 'constraints', 'hamiltonian'] do not"
-                "support networkx.Graph data"
+                f"file_type '{file_type}' data cannot be a networkx.Graph"
             )
 
         data_ls = []
 
         if sp.isspmatrix_dok(data):
             for idx, val in zip(data.keys(), data.values()):
                 # dok type has trouble subsequently serializing to json without type
@@ -130,31 +126,31 @@
 
             for i, j, val in zip(
                 data.row.tolist(), data.col.tolist(), data.data.tolist()
             ):
                 data_ls.append({"i": i, "j": j, "val": val})
         else:
             raise ValueError(
-                "file_types = ['qubo', 'objective', 'constraints', 'hamiltonian'] only "
-                "support types numpy.ndarray and scipy.sparse.spmatrix, got "
-                f"{type(data)}"
+                f"file_type '{file_type}' only supports types numpy.ndarray and "
+                f"scipy.sparse.spmatrix, got {type(data)}"
             )
 
+        file_config = {"data": data_ls}
         rows, cols = data.get_shape()
-        data = {"data": data_ls}
 
         if file_type == "constraints":
             # Constraints matrix is [A | -b]
             file_config.update({"num_constraints": rows, "num_variables": cols-1})
         else:
             # This works for hamiltonians, qubos, and objectives.
             file_config["num_variables"] = rows
-
-    file_config.update(data)
+    else:
+        # Polynomial file types do not require translation.
+        file_config = file["file_config"][file_type]
 
     if debug:
-        print(f"Time to convert data to json: {time.perf_counter()-start} s.")
+        print(f"Time to convert data to json: {time.perf_counter()-start_time_s} s.")
 
     return {
         "file_name": file.get("file_name", f"{file_type}.json"),
         "file_config": {file_type: file_config}
     }
```

### Comparing `qci-client-3.1.0/qci_client/enum.py` & `qci-client-3.2.0/qci_client/enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     # Enums should match corresponding literals in types module.
     # Job input files.
     CONSTRAINTS = "constraints"
     GRAPH = "graph"
     HAMILTONIAN = "hamiltonian"
     OBJECTIVE = "objective"
+    POLYNOMIAL = "polynomial"
     QUBO = "qubo"
     # Job results files.
     GP_RESULTS = "graph_partitioning_results"
     IHO_RESULTS = "ising_hamiltonian_optimization_results"
     NQHO_CONTINUOUS_RESULTS = (
         "normalized_qudit_hamiltonian_optimization_continuous_results"
     )
@@ -28,15 +29,16 @@
     QUBO_RESULTS = "quadratic_unconstrained_binary_optimization_results"
 
 
 FILE_TYPES = frozenset(type.value for type in FileType)
 JOB_INPUTS_FILE_TYPES = frozenset(
     type for type in FileType if "results" not in type.value
 )
-JOB_INPUTS_MATRIX_FILE_TYPES = JOB_INPUTS_FILE_TYPES - frozenset([FileType.GRAPH])
+JOB_INPUTS_MATRIX_FILE_TYPES = JOB_INPUTS_FILE_TYPES - frozenset([FileType.GRAPH, FileType.POLYNOMIAL])
+JOB_INPUTS_NON_GRAPH_FILE_TYPES = JOB_INPUTS_FILE_TYPES - frozenset([FileType.GRAPH])
 JOB_RESULTS_FILE_TYPES = frozenset(type for type in FileType if "results" in type.value)
 
 
 def get_file_type(file: dict) -> FileType:
     """Get file type from a file."""
     file_config_keys = list(file["file_config"].keys())
```

### Comparing `qci-client-3.1.0/qci_client/qci_client.py` & `qci-client-3.2.0/qci_client/qci_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,14 +343,15 @@
         job_type: str,
         job_params: dict,
         qubo_file_id: Optional[str] = None,
         graph_file_id: Optional[str] = None,
         hamiltonian_file_id: Optional[str] = None,
         objective_file_id: Optional[str] = None,
         constraints_file_id: Optional[str] = None,
+        polynomial_file_id: Optional[str] = None,
         job_name: Optional[str] = None,
         job_tags: Optional[list] = None,
     ) -> dict:
         """
         Constructs body for job submission requests
 
         Args:
@@ -438,37 +439,45 @@
 
                 if "sum_constraint" in job_params:
                     # Optional parameter.
                     device_config["sum_constraint"] = job_params["sum_constraint"]
             else:
                 raise ValueError(f"{job_type} not supported on {device_name}.")
 
-            if not hamiltonian_file_id:
+            if (not hamiltonian_file_id and not polynomial_file_id) or \
+                (hamiltonian_file_id and polynomial_file_id):
                 raise AssertionError(
-                    "hamiltonian_file_id must be specified for "
-                    "job_type='sample-hamiltonian'"
+                    "exactly one of hamiltonian_file_id or polynomial_file_id must be "
+                    "specified for job_type='sample-hamiltonian'"
                 )
 
-            problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+            if hamiltonian_file_id:
+                problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+            else:
+                problem_config["polynomial_file_id"] = polynomial_file_id
         elif job_type == 'sample-hamiltonian-ising':
             if device_name in ('dirac-2', 'dirac-3'):
                 raise ValueError(
                     f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
                     "job_type sample-hamiltonian for dirac-2 and dirac-3."
                 )
 
             problem_name = 'ising_hamiltonian_optimization'
             
-            if not hamiltonian_file_id:
+            if (not hamiltonian_file_id and not polynomial_file_id) or \
+                (hamiltonian_file_id and polynomial_file_id):
                 raise AssertionError(
-                    "hamiltonian_file_id must be specified for "
-                    "job_type='sample-hamiltonian-ising'"
+                    "exactly one of hamiltonian_file_id or polynomial_file_id must be "
+                    "specified for job_type='sample-hamiltonian-ising'"
                 )
 
-            problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+            if hamiltonian_file_id:
+                problem_config["hamiltonian_file_id"] = hamiltonian_file_id
+            else:
+                problem_config["polynomial_file_id"] = polynomial_file_id
         elif job_type == "sample-constraint":
             if device_name in ('dirac-2', 'dirac-3'):
                 raise ValueError(
                     f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
                     "job_type sample-hamiltonian for dirac-2 and dirac-3."
                 )
```

### Comparing `qci-client-3.1.0/qci_client/types.py` & `qci-client-3.2.0/qci_client/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from typing import Dict, List, Literal, Protocol, TypedDict, Union
 
 # Literals should match corresponding values in enum.FileType.
 Hamiltonian = Literal["hamiltonian"]
 Qubo = Literal["qubo"]
 Objective = Literal["objective"]
+Polynomial = Literal["polynomial"]
 Constraints = Literal["constraints"]
 Graph = Literal["graph"]
 GpResults = Literal["graph_partitioning_results"]
 IhoResults = Literal["ising_hamiltonian_optimization_results"]
 NqhoContinuousResults = Literal[
     "normalized_qudit_hamiltonian_optimization_continuous_results"
 ]
@@ -92,14 +93,28 @@
 
 class ObjectiveMetadataConfig(TypedDict):
     """Objective file metadata configuration."""
 
     objective: ObjectiveMetadata
 
 
+class PolynomialMetadata(TypedDict):
+    """Polynomial file metadata."""
+
+    min_degree: int
+    max_degree: int
+    num_variables: int
+
+
+class PolynomialMetadataConfig(TypedDict):
+    """Polynomial file metadata configuration."""
+
+    polynomial: PolynomialMetadata
+
+
 class QuboMetadata(TypedDict):
     """QUBO file metadata."""
 
     num_variables: int
 
 
 class QuboMetadataConfig(TypedDict):
@@ -209,14 +224,15 @@
     """Request body for POSTing any input file metadata."""
 
     file_config: Union[
         ConstraintsMetadataConfig,
         GraphMetadataConfig,
         HamiltonianMetadataConfig,
         ObjectiveMetadataConfig,
+        PolynomialMetadataConfig,
         QuboMetadataConfig,
     ]
 
 
 class ResultsMetadataPostRequestBody(MetadataOptionalPostRequestBody):
     """Request body for POSTing any results file metadata."""
 
@@ -242,26 +258,26 @@
 
 class MetadataPostResponseBody(TypedDict):
     """File metadata POST response body."""
 
     file_id: str
 
 
-class DataDict(TypedDict):
-    """Dictionary elements of data array."""
+class MatrixElement(TypedDict):
+    """Matrix element dictionary."""
 
     i: int
     j: int
     val: float
 
 
 class ConstraintsPart(TypedDict):
     """Constraints file part."""
 
-    data: List[DataDict]
+    data: List[MatrixElement]
 
 
 class ConstraintsPartConfig(TypedDict):
     """Constraints file part configuration."""
 
     constraints: ConstraintsPart
 
@@ -297,39 +313,58 @@
 
     graph: GraphPart
 
 
 class HamiltonianPart(TypedDict):
     """Hamiltonian file part."""
 
-    data: List[DataDict]
+    data: List[MatrixElement]
 
 
 class HamiltonianPartConfig(TypedDict):
     """Hamiltonian file part configuration."""
 
     hamiltonian: HamiltonianPart
 
 
 class ObjectivePart(TypedDict):
     """Objective file part."""
 
-    data: List[DataDict]
+    data: List[MatrixElement]
 
 
 class ObjectivePartConfig(TypedDict):
     """Objective file part configuration."""
 
     objective: ObjectivePart
 
 
+class PolynomialElement(TypedDict):
+    """Polynomial element dictionary."""
+
+    idx: List[int]
+    val: float
+
+
+class PolynomialPart(TypedDict):
+    """Polynomial file part."""
+
+    data: List[PolynomialElement]
+
+
+class PolynomialPartConfig(TypedDict):
+    """Polynomial file part configuration."""
+
+    polynomial: PolynomialPart
+
+
 class QuboPart(TypedDict):
     """QUBO file part."""
 
-    data: List[DataDict]
+    data: List[MatrixElement]
 
 
 class QuboPartConfig(TypedDict):
     """QUBO file part configuration."""
 
     qubo: QuboPart
 
@@ -451,14 +486,15 @@
     """The request body for PATCHing all input and results file parts."""
 
     file_config: Union[
         ConstraintsPartConfig,
         GraphPartConfig,
         HamiltonianPartConfig,
         ObjectivePartConfig,
+        PolynomialPartConfig,
         QuboPartConfig,
         GpResultsPartConfig,
         IhoResultsPartConfig,
         NqhoContinuousResultsPartConfig,
         NqhoIntegerResultsPartConfig,
         NqhoResultsPartConfig,
         QlcboResultsPartConfig,
```

### Comparing `qci-client-3.1.0/qci_client/utilities.py` & `qci-client-3.2.0/qci_client/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,26 @@
             file_config=types.ObjectiveMetadataConfig(
                 objective=types.ObjectiveMetadata(
                     num_variables=file_config["num_variables"],
                 )
             ),
         )
 
+    if file_type == enum.FileType.POLYNOMIAL:
+        return types.InputMetadataPostRequestBody(
+            **optional_fields,
+            file_config=types.PolynomialMetadataConfig(
+                polynomial=types.PolynomialMetadata(
+                    min_degree=file_config["min_degree"],
+                    max_degree=file_config["max_degree"],
+                    num_variables=file_config["num_variables"],
+                )
+            ),
+        )
+
     if file_type == enum.FileType.QUBO:
         return types.InputMetadataPostRequestBody(
             **optional_fields,
             file_config=types.QuboMetadataConfig(
                 qubo=types.QuboMetadata(
                     num_variables=file_config["num_variables"],
                 )
@@ -190,14 +202,21 @@
     if file_type == enum.FileType.OBJECTIVE:
         return types.PartPatchRequestBody(
             file_config=types.ObjectivePartConfig(
                 objective=types.ObjectivePart(data=file_config["data"])
             ),
         )
 
+    if file_type == enum.FileType.POLYNOMIAL:
+        return types.PartPatchRequestBody(
+            file_config=types.PolynomialPartConfig(
+                polynomial=types.PolynomialPart(data=file_config["data"])
+            ),
+        )
+
     if file_type == enum.FileType.QUBO:
         return types.PartPatchRequestBody(
             file_config=types.QuboPartConfig(
                 qubo=types.QuboPart(data=file_config["data"])
             ),
         )
 
@@ -309,15 +328,15 @@
         # keeps uploaded chunks below this value. After some testing, we decided to
         # limit this to chunks of 10000 elements for performance reasons.
         data_chunk_size_max = 10000
 
     file_type = enum.get_file_type(file=file)
     file_config = file["file_config"][file_type.value]
 
-    if file_type in enum.JOB_INPUTS_MATRIX_FILE_TYPES:
+    if file_type in enum.JOB_INPUTS_NON_GRAPH_FILE_TYPES:
         return _data_generator(
             file_type=file_type,
             file_config=file_config,
             step_length=data_chunk_size_max,
         )
 
     if file_type == enum.FileType.GRAPH:
```

### Comparing `qci-client-3.1.0/qci_client.egg-info/PKG-INFO` & `qci-client-3.2.0/qci_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.1.0
+Version: 3.2.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
 Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `qci-client-3.1.0/qci_client.egg-info/SOURCES.txt` & `qci-client-3.2.0/qci_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qci-client-3.1.0/tests/test_qci_client.py` & `qci-client-3.2.0/tests/test_qci_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,25 +102,85 @@
                             [2.0, 0.0, 1.0]
                         ]
                     )
                 }
             }
         }
 
+        cls.polynomial_dict_hamiltonian_input = {
+            "file_name": "polynomial-hamiltonian.json",
+            "file_config": {
+                "polynomial": {
+                    "min_degree": 1,
+                    "max_degree": 2,
+                    "num_variables": 2,
+                    "data": [
+                        {
+                            "idx": [0, 1],
+                            "val": 1.0
+                        },
+                        {
+                            "idx": [1, 1],
+                            "val": -2.0
+                        },
+                        {
+                            "idx": [1, 2],
+                            "val": 1.0
+                        },
+                        {
+                            "idx": [2, 2],
+                            "val": -1.0
+                        }
+
+                    ]
+                }
+            }
+        }
+
+        cls.polynomial_dict_input = {
+            "file_name": "polynomial.json",
+            "file_config": {
+                "polynomial": {
+                    "min_degree": 2,
+                    "max_degree": 4,
+                    "num_variables": 2,
+                    "data": [
+                        {
+                            "idx": [0, 0, 1, 1],
+                            "val": 1.0
+                        },
+                        {
+                            "idx": [0, 1, 1, 1],
+                            "val": -2.0
+                        },
+                        {
+                            "idx": [1, 1, 1, 1],
+                            "val": 1.0
+                        }
+                    ]
+                }
+            }
+        }
+
         cls.graph_file_id = cls.q1.upload_file(file=cls.graph_dict_input)["file_id"]
         cls.qubo_file_id = cls.q1.upload_file(file=cls.qubo_dict_input)["file_id"]
         cls.objective_file_id = cls.q1.upload_file(file=cls.objective_dict_input)[
             "file_id"
         ]
         cls.constraints_file_id = cls.q1.upload_file(file=cls.constraint_dict_input)[
             "file_id"
         ]
         cls.hamiltonian_file_id = cls.q1.upload_file(file=cls.hamiltonian_dict_input)[
             "file_id"
         ]
+        cls.polynomial_hamiltonian_file_id = cls.q1.upload_file(
+            file=cls.polynomial_dict_hamiltonian_input
+        )["file_id"]
+        cls.polynomial_min_degree_2_max_degree_4_file_id = cls.q1.upload_file(
+            file=cls.polynomial_dict_input)["file_id"]
 
         cls.all_statuses = [
             JobStatus.QUEUED,
             JobStatus.SUBMITTED,
             JobStatus.RUNNING,
             JobStatus.COMPLETED,
             JobStatus.ERRORED,
@@ -171,145 +231,173 @@
                 },
                 "device_config": {
                     "dirac-1": {}
                 }
             }
         }
 
-        cls.hamiltonian_job_body_solution_precision_omitted = {
+        cls.hamiltonian_job_body_ising_dirac1 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-1",
                 "problem_config": {
-                    "normalized_qudit_hamiltonian_optimization": {
+                    "ising_hamiltonian_optimization": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
+                    },
+                },
+                "device_config": {
+                    "dirac-1": {
+                        "num_samples": 2,
                     }
+                }
+            }
+        }
+
+        cls.polynomial_job_body_ising_dirac1 = {
+            "job_submission": {
+                "job_name": "dirac-1",
+                "problem_config": {
+                    "ising_hamiltonian_optimization": {
+                        "polynomial_file_id": cls.polynomial_hamiltonian_file_id
+                    },
                 },
                 "device_config": {
-                    "dirac-3": {
-                        "relaxation_parameter": 1,
-                        "sum_constraint": 2.4,
+                    "dirac-1": {
                     }
                 }
             }
         }
 
-        cls.hamiltonian_job_body_solution_precision_continuous = {
+        cls.hamiltonian_job_body_continous_dirac2 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-2",
                 "problem_config": {
-                    "normalized_qudit_hamiltonian_optimization": {
+                    "normalized_qudit_hamiltonian_optimization_continuous": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     }
                 },
                 "device_config": {
-                    "dirac-3": {
-                        "relaxation_parameter": 1,
-                        "sum_constraint": 2.4,
-                        "solution_precision": 0.1,
+                    "dirac-2": {}
+                }
+            }
+        }
+
+        cls.hamiltonian_job_body_integer_dirac2 = {
+            "job_submission": {
+                "job_name": "dirac-2",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization_integer": {
+                        "hamiltonian_file_id": cls.hamiltonian_file_id
+                    },
+                },
+                "device_config": {
+                    "dirac-2": {}
+                }
+            }
+        }
+
+        cls.polynomial_job_body_hamiltonian_continuous_dirac2 = {
+            "job_submission": {
+                "job_name": "dirac-2",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization_continuous": {
+                        "polynomial_file_id": cls.polynomial_hamiltonian_file_id
+                    },
+                },
+                "device_config": {
+                    "dirac-2": {}
+                }
+            }
+        }
+
+        cls.polynomial_job_body_hamiltonian_integer_dirac2 = {
+            "job_submission": {
+                "job_name": "dirac-2",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization_integer": {
+                        "polynomial_file_id": cls.polynomial_hamiltonian_file_id
+                    },
+                },
+                "device_config": {
+                    "dirac-2": {
+                        "num_samples": 2,
                     }
                 }
             }
         }
 
-        cls.hamiltonian_job_body_solution_precision_integer = {
+        cls.hamiltonian_job_body_undistilled_dirac3 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-3",
                 "problem_config": {
                     "normalized_qudit_hamiltonian_optimization": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     }
                 },
                 "device_config": {
                     "dirac-3": {
                         "relaxation_parameter": 1,
-                        "solution_precision": 1,
+                        "sum_constraint": 2.4,
                     }
                 }
             }
         }
 
-        cls.hamiltonian_job_body_continous = {
+        cls.hamiltonian_job_body_distilled_continuous_dirac3 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-3",
                 "problem_config": {
-                    "normalized_qudit_hamiltonian_optimization_continuous": {
+                    "normalized_qudit_hamiltonian_optimization": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     }
                 },
                 "device_config": {
-                    "dirac-2": {}
+                    "dirac-3": {
+                        "relaxation_parameter": 1,
+                        "sum_constraint": 2.4,
+                        "solution_precision": 0.1,
+                    }
                 }
             }
         }
 
-        cls.hamiltonian_job_body_integer = {
+        cls.hamiltonian_job_body_distilled_integer_dirac3 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-3",
                 "problem_config": {
-                    "normalized_qudit_hamiltonian_optimization_integer": {
+                    "normalized_qudit_hamiltonian_optimization": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
-                    },
+                    }
                 },
                 "device_config": {
-                    "dirac-2": {}
+                    "dirac-3": {
+                        "relaxation_parameter": 1,
+                        "solution_precision": 1,
+                    }
                 }
             }
         }
 
-        cls.hamiltonian_job_body_ising = {
+        cls.polynomial_min_degree_2_max_degree_4_job_body_distilled_continuous_dirac3 = {
             "job_submission": {
-                "job_name": "job_0",
+                "job_name": "dirac-3",
                 "problem_config": {
-                    "ising_hamiltonian_optimization": {
-                        "hamiltonian_file_id": cls.hamiltonian_file_id
+                    "normalized_qudit_hamiltonian_optimization": {
+                        "polynomial_file_id": cls.polynomial_min_degree_2_max_degree_4_file_id
                     },
                 },
                 "device_config": {
-                    "dirac-1": {
-                        "num_samples": 2,
+                    "dirac-3": {
+                        "relaxation_parameter": 2,
+                        "sum_constraint": 2.4,
+                        "solution_precision": 0.1,
                     }
                 }
             }
         }
 
-    def run_end_end(
-        self, job_type: str, job_body: dict, results_key: Optional[list] = None
-    ):
-        """
-        Utility function for testing end to end pipeline.
-        :param job_type: one of _supported_job_types
-        :param job_body: a validate job request
-        Testing each in series:
-            - submit_job
-            - get_job_status
-            - get_job_response
-            - get_file
-        """
-        job_id = self.q1.submit_job(job_body=job_body, job_type=job_type)
-
-        self.assertIn("job_id", job_id)
-        self.assertIsInstance(job_id["job_id"], str)
-
-        status = self.q1.get_job_status(job_id=job_id["job_id"])
-        self.assertIn("status", status)
-        self.assertIn(status["status"], self.all_statuses)
-
-        while status["status"] not in self.final_status:
-            status = self.q1.get_job_status(job_id=job_id["job_id"])
-
-        self.assertEqual(JobStatus.COMPLETED, status["status"])
-        response = self.q1.get_job_response(job_id=job_id["job_id"], job_type=job_type)
-
-        # test job info has appropriate keys
-        # self.assertEqual(self.job_info, set(response.keys()))  # FIXME
-
-        result = self.q1.download_file(file_id=response["job_result"]["file_id"])
-        result = list(result)
-        # self.assertTrue(all(i in result[0] for i in result_keys))  # FIXME
-
     def test_upload_file_error(self):
         """Test uploading improperly formatted file."""
         with self.assertRaises(KeyError):
             error_input = {
                 "file_type": "graph",
                 "file_name": "qubo.json",
                 "data": [
@@ -477,24 +565,24 @@
         hamiltonian_body = self.q1.build_job_body(
             job_type="sample-hamiltonian",
             job_params={
                 "sampler_type": "dirac-3",
                 "sum_constraint": 200,
                 "solution_precision": 1,
             },
-            hamiltonian_file_id="hamiltonian_fid"
+            polynomial_file_id="polynomial_fid"
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "problem_config": {
                         "normalized_qudit_hamiltonian_optimization": {
-                            "hamiltonian_file_id": "hamiltonian_fid",
+                            "polynomial_file_id": "polynomial_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "sum_constraint": 200,
                             "solution_precision": 1,
                         }
@@ -505,24 +593,24 @@
 
         hamiltonian_body = self.q1.build_job_body(
             job_type="sample-hamiltonian",
             job_params={
                 "sampler_type": "dirac-3",
                 "sum_constraint": 2.4
             },
-            hamiltonian_file_id="hamiltonian_fid"
+            polynomial_file_id="polynomial_fid"
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "problem_config": {
                         "normalized_qudit_hamiltonian_optimization": {
-                            "hamiltonian_file_id": "hamiltonian_fid",
+                            "polynomial_file_id": "polynomial_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "sum_constraint": 2.4,
                         }
                     }
```

### Comparing `qci-client-3.1.0/tests/test_remote_jobs.py` & `qci-client-3.2.0/tests/test_remote_jobs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Test suite for jobs run on a remote backend."""
 
 from copy import deepcopy
-from datetime import datetime, timedelta
 from typing import Optional
 import unittest
 
 import numpy as np
 import scipy.sparse as sp
 
 from qci_client import JobStatus
@@ -13,41 +12,38 @@
 from tests.test_qci_client import TestQciClientFiles
 
 
 class TestQciClientRemoteJobs(TestQciClientFiles):
     """Collection of tests for remote jobs."""
 
     def run_end_end(
-        self, job_type: str, job_body: dict, results_key: Optional[list] = None
+        self, job_type: str, job_body: dict, result_keys: Optional[list] = None
     ):
         """
         Utility function for testing end to end pipeline.
         :param job_type: one of _supported_job_types
         :param job_body: a validate job request
         Testing each in series:
             - submit_job
             - get_job_status
             - get_job_response
             - get_file
         """
 
-        result_keys = self.result_keys if results_key is None else results_key
+        result_keys = self.result_keys if result_keys is None else result_keys
 
         job_id = self.q1.submit_job(job_body=job_body, job_type=job_type)
 
         self.assertIn("job_id", job_id)
         self.assertIsInstance(job_id["job_id"], str)
 
-        status = self.q1.get_job_status(job_id=job_id["job_id"])
-        self.assertIn("status", status)
-        self.assertIn(status["status"], self.all_statuses)
+        status = {"status": ""}
 
         while status["status"] not in self.final_status:
             status = self.q1.get_job_status(job_id=job_id["job_id"])
-            self.assertIn("status", status)
             self.assertIn(status["status"], self.all_statuses)
 
         self.assertEqual(JobStatus.COMPLETED, status["status"])
         response = self.q1.get_job_response(job_id=job_id["job_id"], job_type=job_type)
 
         # test job info has appropriate keys
         # self.assertEqual(self.job_info, set(response.keys()))  # FIXME
@@ -104,67 +100,121 @@
 
     def test_process_constraint(self):
         """Test that sample-constraint job process can be checked."""
         self.process_job_check(
             job_type="sample-constraint", job_body=self.constraint_job_body
         )
 
-    # def test_graph_partitioning(self):
-    #     """Test graph-partitioning job."""
-    #     self.run_end_end(job_type="graph-partitioning", job_body=self.graph_job_body)
+    def test_process_hamiltonian_ising_dirac1(self):
+        """Test that sample-hamiltonian-ising process job on dirac-1 can be checked."""
+        self.process_job_check(
+            job_type="sample-hamiltonian-ising",
+            job_body=self.hamiltonian_job_body_ising_dirac1,
+        )
+
+    def test_process_hamiltonian_dirac2(self):
+        """Test that integer sample-hamiltonian process job on dirac-2 can be checked."""
+        self.process_job_check(
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_integer_dirac2,
+        )
+
+    def test_process_hamiltonian_dirac3(self):
+        """
+        Test that undistilled sample-hamiltonian process on dirac-3 job can be checked.
+        """
+        self.process_job_check(
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_undistilled_dirac3,
+        )
+
+    def test_graph_partitioning(self):
+        """Test graph-partitioning job."""
+        self.run_end_end(job_type="graph-partitioning", job_body=self.graph_job_body)
 
     def test_sample_qubo(self):
         """Test sample-qubo job."""
         self.run_end_end(job_type="sample-qubo", job_body=self.qubo_job_body)
 
     def test_sample_constraint(self):
         """Test sample-constraint job."""
-        self.run_end_end(job_type="sample-constraint", job_body=self.constraint_job_body)
+        self.run_end_end(
+            job_type="sample-constraint",
+            job_body=self.constraint_job_body,
+        )
 
-    def test_process_hamiltonian_continous(self):
-        """Test that continuous sample-hamiltonian job process can be checked."""
-        self.process_job_check(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_continous
+    def test_sample_hamiltonian_ising_polynomial_dirac1(self):
+        """Test sample-hamiltonian-ising job using polynomial on dirac-1."""
+        self.run_end_end(
+            job_type="sample-hamiltonian-ising",
+            job_body=self.polynomial_job_body_ising_dirac1
         )
 
-    def test_sample_hamiltonian_continuous(self):
-        """Test continuous sample-hamiltonian job."""
+    def test_sample_hamiltonian_ising_hamiltonian_dirac1(self):
+        """Test sample-hamiltonian-ising job using hamiltonian matrix on dirac-1."""
         self.run_end_end(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_continous
+            job_type="sample-hamiltonian-ising",
+            job_body=self.hamiltonian_job_body_ising_dirac1
         )
 
-    def test_sample_hamiltonian_integer(self):
-        """Test integer sample-hamiltonian job."""
+    def test_sample_hamiltonian_polynomial_continuous_dirac2(self):
+        """Test sample-hamiltonian continuous job using polynomial on dirac-2."""
         self.run_end_end(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_integer
+            job_type="sample-hamiltonian",
+            job_body=self.polynomial_job_body_hamiltonian_continuous_dirac2
         )
 
-    def test_sample_hamiltonian_solution_precision_omitted(self):
-        """Test continuous sample-hamiltonian job."""
+    def test_sample_hamiltonian_polynomial_integer_dirac2(self):
+        """Test sample-hamiltonian integer job using polynomial on dirac-2."""
         self.run_end_end(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_solution_precision_omitted
+            job_type="sample-hamiltonian",
+            job_body=self.polynomial_job_body_hamiltonian_integer_dirac2
         )
 
-    def test_sample_hamiltonian_solution_precision_continuous(self):
-        """Test continuous sample-hamiltonian job."""
+    def test_sample_hamiltonian_continuous_dirac2(self):
+        """Test continuous sample-hamiltonian job on dirac-2."""
         self.run_end_end(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_solution_precision_continuous
+            job_type="sample-hamiltonian",job_body=self.hamiltonian_job_body_continous_dirac2
         )
 
-    def test_sample_hamiltonian_solution_precision_integer(self):
-        """Test integer sample-hamiltonian job."""
+    def test_sample_hamiltonian_integer_dirac2(self):
+        """Test integer sample-hamiltonian job on dirac-2."""
         self.run_end_end(
-            job_type="sample-hamiltonian", job_body=self.hamiltonian_job_body_solution_precision_integer
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_integer_dirac2
         )
 
-    def test_sample_hamiltonian_ising(self):
-        """Test sample-hamiltonian-ising job."""
+    def test_sample_hamiltonian_polynomial_distilled_continuous_dirac3(self):
+        """
+        Test distilled-to-continuous sample-hamiltonian job using polynomial on dirac-3.
+        """
         self.run_end_end(
-            job_type="sample-hamiltonian-ising",
-            job_body=self.hamiltonian_job_body_ising
+            job_type="sample-hamiltonian",
+            job_body=self.polynomial_min_degree_2_max_degree_4_job_body_distilled_continuous_dirac3,
+        )
+
+    def test_sample_hamiltonian_undistilled_dirac3(self):
+        """Test undistilled sample-hamiltonian job on dirac-3."""
+        self.run_end_end(
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_undistilled_dirac3,
+        )
+
+    def test_sample_hamiltonian_distilled_continuous_dirac3(self):
+        """Test distilled-to-continuous sample-hamiltonian job on dirac-3."""
+        self.run_end_end(
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_distilled_continuous_dirac3,
+        )
+
+    def test_sample_hamiltonian_distilled_integer_dirac3(self):
+        """Test distilled-to-integer sample-hamiltonian job on dirac-3."""
+        self.run_end_end(
+            job_type="sample-hamiltonian",
+            job_body=self.hamiltonian_job_body_distilled_integer_dirac3,
         )
 
 
 @qci_client.base.BaseApi.refresh_token
 def refresh_token_wrapped_function(*_, **__) -> None:
     """Mock function wrapped with token checking/fetching."""
```

