# Comparing `tmp/group_decomposition-0.6.0.tar.gz` & `tmp/group_decomposition-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_decomposition-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "group_decomposition-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `group_decomposition-0.6.0.tar` & `group_decomposition-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-01-19 16:35:39.016878 group_decomposition-0.6.0/LICENSE
--rw-r--r--   0        0        0     3830 2024-01-19 16:35:39.016878 group_decomposition-0.6.0/README.md
--rw-r--r--   0        0        0     6148 2024-01-19 16:35:39.020878 group_decomposition-0.6.0/group_decomposition/.DS_Store
--rw-r--r--   0        0        0      118 2024-01-19 16:35:39.020878 group_decomposition-0.6.0/group_decomposition/__init__.py
--rw-r--r--   0        0        0     6159 2024-01-19 16:35:39.024878 group_decomposition-0.6.0/group_decomposition/fg_query.py
--rw-r--r--   0        0        0    48053 2024-01-19 16:35:39.024878 group_decomposition-0.6.0/group_decomposition/fragfunctions.py
--rw-r--r--   0        0        0    34055 2024-01-19 16:35:39.024878 group_decomposition-0.6.0/group_decomposition/utils.py
--rw-r--r--   0        0        0     2830 2024-01-19 16:35:39.024878 group_decomposition-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 group_decomposition-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-10 19:07:36.299457 group_decomposition-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4457 2024-04-10 19:07:36.299457 group_decomposition-0.6.1/README.md
+-rw-r--r--   0        0        0     6148 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/group_decomposition/.DS_Store
+-rw-r--r--   0        0        0      118 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/group_decomposition/__init__.py
+-rw-r--r--   0        0        0     6159 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/group_decomposition/fg_query.py
+-rw-r--r--   0        0        0    48088 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/group_decomposition/fragfunctions.py
+-rw-r--r--   0        0        0    34055 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/group_decomposition/utils.py
+-rw-r--r--   0        0        0     2944 2024-04-10 19:07:36.303457 group_decomposition-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 group_decomposition-0.6.1/PKG-INFO
```

### Comparing `group_decomposition-0.6.0/LICENSE` & `group_decomposition-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `group_decomposition-0.6.0/README.md` & `group_decomposition-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![ci](https://github.com/kmlefran/group_decomposition/actions/workflows/ci.yml/badge.svg)](https://github.com/kmlefran/group_decomposition/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/group_decomposition/badge/?version=latest)](https://group_decomposition.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/kmlefran/group_decomposition/badge.svg?branch=main)](https://coveralls.io/github/kmlefran/group_decomposition?branch=main)
+[![PyPI version](https://badge.fury.io/py/group-decomposition.svg)](https://badge.fury.io/py/group-decomposition)
 # Identifying fragments in molecule SMILES codes
 
 Python functions to identify fragments in a molecule(or set of molecules) based on their SMILES codes, or .mol(and/or cml files). The fragments are chemically meaningful. Fragments identified include rings, linkers, side chains of molecules, and the functional groups(as defined by Ertl - heteroatoms and double bonds), and alkyl groups that compose them. There are two main functionalities currently, at the single molecule level, and at the batch level. At the single molecular level, the molecule is broken up into the fragments, and each fragment retains connectivity. At the batch level, for multiple molecules, connectivity is removed, and the unique fragments are identified, and their occurences counted. For example, this would identify that there are N methyl groups in the set of molecules.
 
 
 The code is implemented primarily through RDKit, using a mix of the rdScaffoldNetwork module, and SMARTS pattern matching. rdScaffoldNetwork is used to identify the ring systems due to its flexibility in bond breaking rules, and that rdScaffoldNetwork will not break fused rings. The molecule is fragmented using the rdkit FragmentOnBonds functionality, which provides the option to label the dummy atoms produced with labels that can indicate connectivity. SMARTS matching is used to break the molecule further into functional groups and alkyl groups  by breaking single bonds between non-ring sp3 carbons and ring atoms or heteroatoms.
```

### Comparing `group_decomposition-0.6.0/group_decomposition/.DS_Store` & `group_decomposition-0.6.1/group_decomposition/.DS_Store`

 * *Files identical despite different names*

### Comparing `group_decomposition-0.6.0/group_decomposition/fg_query.py` & `group_decomposition-0.6.1/group_decomposition/fg_query.py`

 * *Files identical despite different names*

### Comparing `group_decomposition-0.6.0/group_decomposition/fragfunctions.py` & `group_decomposition-0.6.1/group_decomposition/fragfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,14 +478,16 @@
         parent_list = frag_frame["Parent"]
         parent_inc = True
     else:
         parent_inc = False
     if "atom_types" in col_names:
         type_list = frag_frame["atom_types"]
         type_inc = True
+    else:
+        type_inc = False
     if "count" in col_names:
         count_list = frag_frame["count"]
         count_inc = True
     else:
         count_inc = False
     # print(type_list)
     no_connect_smile = []
```

### Comparing `group_decomposition-0.6.0/group_decomposition/utils.py` & `group_decomposition-0.6.1/group_decomposition/utils.py`

 * *Files identical despite different names*

### Comparing `group_decomposition-0.6.0/pyproject.toml` & `group_decomposition-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 description = "A plugin for extracting data from .sum files and manipuating them"
 authors = [{name = "Kevin Lefrancois-Gagnon", email = "kgagnon@lakeheadu.ca"}, {name = "Robert Mawhinney", email = "mawhinn@lakeheadu.ca"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python",
     'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
     "Framework :: AiiDA"
 ]
@@ -31,28 +32,31 @@
 
 [project.urls]
 Source = "https://github.com/kmlefran/group_decomposition"
 [project.optional-dependencies]
 testing = [
     "pgtest~=1.3.1",
     "wheel~=0.31",
-    "coverage[toml]",
+    "coverage",
     "pytest~=6.0",
     "pytest-cov",
-    "rdkit"
+    "pytest-regressions~=2.3",
+    "rdkit",
+    "coveralls"
 ]
 pre-commit = [
     "pre-commit~=2.2",
     "pylint~=2.15.10",
     "rdkit"
 ]
 docs = [
     "sphinx",
     "sphinxcontrib-contentui",
     "sphinxcontrib-details-directive",
+    "sphinx-rtd-theme",
     "furo",
     "markupsafe<2.1",
     "pandas",
     "numpy",
     "rdkit"
 ]
 
@@ -72,18 +76,18 @@
 [tool.pytest.ini_options]
 # Configuration for [pytest](https://docs.pytest.org)
 python_files = "test_*.py"
 filterwarnings = [
     "ignore::DeprecationWarning:yaml:",
 ]
 
-[tool.coverage.run]
+#[tool.coverage.run]
 # Configuration of [coverage.py](https://coverage.readthedocs.io)
 # reporting which lines of your plugin are covered by tests
-source=["group_decomposition"]
+#source=["group_decomposition"]
 
 [tool.isort]
 # Configuration of [isort](https://isort.readthedocs.io)
 line_length = 120
 force_sort_within_sections = true
 sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'FIRSTPARTY', 'LOCALFOLDER']
```

### Comparing `group_decomposition-0.6.0/PKG-INFO` & `group_decomposition-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 Metadata-Version: 2.1
 Name: group_decomposition
-Version: 0.6.0
+Version: 0.6.1
 Summary: A plugin for extracting data from .sum files and manipuating them
 Keywords: qtaim,functional groups
 Author-email: Kevin Lefrancois-Gagnon <kgagnon@lakeheadu.ca>, Robert Mawhinney <mawhinn@lakeheadu.ca>
 Requires-Python: >=3.10
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
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rdkit
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: markupsafe<2.1 ; extra == "docs"
 Requires-Dist: pandas ; extra == "docs"
 Requires-Dist: numpy ; extra == "docs"
 Requires-Dist: rdkit ; extra == "docs"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.15.10 ; extra == "pre-commit"
 Requires-Dist: rdkit ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3.1 ; extra == "testing"
 Requires-Dist: wheel~=0.31 ; extra == "testing"
-Requires-Dist: coverage[toml] ; extra == "testing"
+Requires-Dist: coverage ; extra == "testing"
 Requires-Dist: pytest~=6.0 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
+Requires-Dist: pytest-regressions~=2.3 ; extra == "testing"
 Requires-Dist: rdkit ; extra == "testing"
+Requires-Dist: coveralls ; extra == "testing"
 Project-URL: Source, https://github.com/kmlefran/group_decomposition
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: testing
 
+[![ci](https://github.com/kmlefran/group_decomposition/actions/workflows/ci.yml/badge.svg)](https://github.com/kmlefran/group_decomposition/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/group_decomposition/badge/?version=latest)](https://group_decomposition.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/kmlefran/group_decomposition/badge.svg?branch=main)](https://coveralls.io/github/kmlefran/group_decomposition?branch=main)
+[![PyPI version](https://badge.fury.io/py/group-decomposition.svg)](https://badge.fury.io/py/group-decomposition)
 # Identifying fragments in molecule SMILES codes
 
 Python functions to identify fragments in a molecule(or set of molecules) based on their SMILES codes, or .mol(and/or cml files). The fragments are chemically meaningful. Fragments identified include rings, linkers, side chains of molecules, and the functional groups(as defined by Ertl - heteroatoms and double bonds), and alkyl groups that compose them. There are two main functionalities currently, at the single molecule level, and at the batch level. At the single molecular level, the molecule is broken up into the fragments, and each fragment retains connectivity. At the batch level, for multiple molecules, connectivity is removed, and the unique fragments are identified, and their occurences counted. For example, this would identify that there are N methyl groups in the set of molecules.
 
 
 The code is implemented primarily through RDKit, using a mix of the rdScaffoldNetwork module, and SMARTS pattern matching. rdScaffoldNetwork is used to identify the ring systems due to its flexibility in bond breaking rules, and that rdScaffoldNetwork will not break fused rings. The molecule is fragmented using the rdkit FragmentOnBonds functionality, which provides the option to label the dummy atoms produced with labels that can indicate connectivity. SMARTS matching is used to break the molecule further into functional groups and alkyl groups  by breaking single bonds between non-ring sp3 carbons and ring atoms or heteroatoms.
```

