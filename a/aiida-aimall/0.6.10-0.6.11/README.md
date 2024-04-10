# Comparing `tmp/aiida_aimall-0.6.10.tar.gz` & `tmp/aiida_aimall-0.6.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_aimall-0.6.10.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_aimall-0.6.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_aimall-0.6.10.tar` & `aiida_aimall-0.6.11.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/LICENSE
--rw-r--r--   0        0        0     9730 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/README.md
--rw-r--r--   0        0        0       86 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/__init__.py
--rw-r--r--   0        0        0    13246 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/calculations.py
--rw-r--r--   0        0        0    16513 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/controllers.py
--rw-r--r--   0        0        0     3431 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/data/__init__.py
--rw-r--r--   0        0        0    15668 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/parsers.py
--rw-r--r--   0        0        0    21001 2024-02-27 19:40:20.550017 aiida_aimall-0.6.10/aiida_aimall/workchains.py
--rw-r--r--   0        0        0     4661 2024-02-27 19:40:20.554017 aiida_aimall-0.6.10/pyproject.toml
--rw-r--r--   0        0        0    12682 1970-01-01 00:00:00.000000 aiida_aimall-0.6.10/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/LICENSE
+-rw-r--r--   0        0        0     9730 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/README.md
+-rw-r--r--   0        0        0       86 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/__init__.py
+-rw-r--r--   0        0        0    15415 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/calculations.py
+-rw-r--r--   0        0        0    16513 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/controllers.py
+-rw-r--r--   0        0        0     3431 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/data/__init__.py
+-rw-r--r--   0        0        0    15668 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/parsers.py
+-rw-r--r--   0        0        0    21001 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/workchains.py
+-rw-r--r--   0        0        0     4707 2024-04-10 19:24:45.297841 aiida_aimall-0.6.11/pyproject.toml
+-rw-r--r--   0        0        0    12733 1970-01-01 00:00:00.000000 aiida_aimall-0.6.11/PKG-INFO
```

### Comparing `aiida_aimall-0.6.10/LICENSE` & `aiida_aimall-0.6.11/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/README.md` & `aiida_aimall-0.6.11/README.md`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/aiida_aimall/calculations.py` & `aiida_aimall-0.6.11/aiida_aimall/calculations.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,23 +154,64 @@
             self.OUTPUT_FILE.replace(".out", "_atomicfiles"),
         ]
 
         return calcinfo
 
 
 class GaussianWFXCalculation(CalcJob):
-    """AiiDA calculation plugin wrapping Gaussian
+    """AiiDA calculation plugin wrapping Gaussian. Adapted from aiida-gaussian
+        https://github.com/nanotech-empa/aiida-gaussian, Copyright (c) 2020 Kristjan Eimre.
+        Additions made to enable providing molecule input as orm.Str,
+        and wfx files are retrieved by default. We further define another input wfxgroup in which you can provide an
+        optional group to store the wfx file in and fragment_label as an optional extra to add on the output.
+
+    Args:
+        structure: StructureData for molecule to be run. Do not provide structure AND structure_str, but provide
+        at least one
+        structure_str: Str for molecule to be run. e.g. orm.Str(H 0.0 0.0 0.0\n H -1.0 0.0 0.0)
+        Do not provide structure AND structure_str, but provide at least one
+        wfxgroup: Str of a group to add the .wfx files to
+        parameters: required: Dict of Gaussian parameters, same as from aiida-gaussian. Note that the options provided should
+        generate a wfx file. See Example
+        settings: optional, additional input parameters
+        fragment_label: Str, optional: an extra to add to the wfx file node. Involved in the controllers,
+        which check extras
+        parent_calc_folder: RemoteData, optional: the folder of a completed gaussian calculation
+
+    Example:
+    ::
+
+        builder = GaussianCalculation.get_builder()
+        builder.structure_str = orm.Str("H 0.0 0.0 0.0 -1.0 0.0 0.0) # needs newline but docs doesn't like
+        builder.parameters = orm.Dict(dict={
+            'link0_parameters': {
+                '%chk':'aiida.chk',
+                "%mem": "3200MB", # Currently set to use 8000 MB in .sh files
+                "%nprocshared": 4,
+            },
+            'functional':'wb97xd',
+            'basis_set':'aug-cc-pvtz',
+            'charge': 0,
+            'multiplicity': 1,
+            'route_parameters': {'opt': None, 'Output':'WFX'},
+            "input_parameters": {"output.wfx": None},
+        })
+        builder.code = orm.load_code("g16@localhost")
+        builder.metadata.options.resources = {"num_machines": 1, "tot_num_mpiprocs": 4}
+        builder.metadata.options.max_memory_kb = int(6400 * 1.25) * 1024
+        builder.metadata.options.max_wallclock_seconds = 604800
+        submit(builder)
 
-    Adapted from aiida-gaussian https://github.com/nanotech-empa/aiida-gaussian, Copyright (c) 2020 Kristjan Eimre.
     """
 
     # Defaults
     INPUT_FILE = "aiida.inp"
     OUTPUT_FILE = "aiida.out"
     PARENT_FOLDER_NAME = "parent_calc"
+    # can override in metadata
     DEFAULT_PARSER = "aimall.gaussianwfx"
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         # Input parameters
@@ -205,15 +246,15 @@
             required=False,
             help="the folder of a completed gaussian calculation",
         )
 
         # Turn mpi off by default
         spec.input("metadata.options.withmpi", valid_type=bool, default=False)
 
-        spec.input(
+        spec.input(  # update parser here
             "metadata.options.parser_name",
             valid_type=str,
             default=cls.DEFAULT_PARSER,
             non_db=True,
         )
 
         # Outputs
```

### Comparing `aiida_aimall-0.6.10/aiida_aimall/controllers.py` & `aiida_aimall-0.6.11/aiida_aimall/controllers.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/aiida_aimall/data/__init__.py` & `aiida_aimall-0.6.11/aiida_aimall/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/aiida_aimall/parsers.py` & `aiida_aimall-0.6.11/aiida_aimall/parsers.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/aiida_aimall/workchains.py` & `aiida_aimall-0.6.11/aiida_aimall/workchains.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.10/pyproject.toml` & `aiida_aimall-0.6.11/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 description = "A plugin to interface AIMAll with AiiDA"
 authors = [{name = "Kevin Lefrancois-Gagnon", email = "kgagnon@lakeheadu.ca"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
     "Framework :: AiiDA"
 ]
 keywords = ["aiida", "plugin"]
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dependencies = [
     "aiida-core>=2.0,<3",
     "voluptuous",
     "aiida-submission-controller",
     "pydantic",
     "ase",
     "cclib",
```

### Comparing `aiida_aimall-0.6.10/PKG-INFO` & `aiida_aimall-0.6.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: aiida-aimall
-Version: 0.6.10
+Version: 0.6.11
 Summary: A plugin to interface AIMAll with AiiDA
 Keywords: aiida,plugin
 Author-email: Kevin Lefrancois-Gagnon <kgagnon@lakeheadu.ca>
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
 Requires-Dist: aiida-core>=2.0,<3
```

