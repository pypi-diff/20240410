# Comparing `tmp/subproptools-0.4.0.tar.gz` & `tmp/subproptools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subproptools-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "subproptools-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `subproptools-0.4.0.tar` & `subproptools-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1099 2024-01-19 16:17:00.052770 subproptools-0.4.0/LICENSE
--rw-r--r--   0        0        0     2007 2024-01-19 16:17:00.052770 subproptools-0.4.0/README.md
--rw-r--r--   0        0        0     2743 2024-01-19 16:17:00.064770 subproptools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      548 2024-01-19 16:17:00.064770 subproptools-0.4.0/subproptools/__init__.py
--rw-r--r--   0        0        0     4519 2024-01-19 16:17:00.068770 subproptools-0.4.0/subproptools/deprecated.txt
--rw-r--r--   0        0        0    44124 2024-01-19 16:17:00.068770 subproptools-0.4.0/subproptools/qtaim_extract.py
--rw-r--r--   0        0        0    15792 2024-01-19 16:17:00.068770 subproptools-0.4.0/subproptools/reference_maps.py
--rw-r--r--   0        0        0    35048 2024-01-19 16:17:00.068770 subproptools-0.4.0/subproptools/sub_reor.py
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 subproptools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-10 19:06:06.566991 subproptools-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2579 2024-04-10 19:06:06.566991 subproptools-0.4.2/README.md
+-rw-r--r--   0        0        0     2875 2024-04-10 19:06:06.574991 subproptools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      548 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/__init__.py
+-rw-r--r--   0        0        0     4519 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/deprecated.txt
+-rw-r--r--   0        0        0    44124 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/qtaim_extract.py
+-rw-r--r--   0        0        0    15792 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/reference_maps.py
+-rw-r--r--   0        0        0    35254 2024-04-10 19:06:06.578991 subproptools-0.4.2/subproptools/sub_reor.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 subproptools-0.4.2/PKG-INFO
```

### Comparing `subproptools-0.4.0/LICENSE` & `subproptools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.0/README.md` & `subproptools-0.4.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+
+[![ci](https://github.com/kmlefran/subproptools/actions/workflows/ci.yml/badge.svg)](https://github.com/kmlefran/subproptools/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/subproptools/badge/?version=latest)](https://subproptools.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/kmlefran/subproptools/badge.svg?branch=main)](https://coveralls.io/github/kmlefran/subproptools?branch=main)
+[![PyPI version](https://badge.fury.io/py/subproptools.svg)](https://badge.fury.io/py/subproptools)
 # Molecule Reorientation and .sum file handling
 
 This package provides tools to extract data from .sum files (in the qtaimExtract module), and tools to reorient the molecule to defined coordinate systems (in the subreor module). The subreor module rotates to a defined coordinate system. First an atom is positioned at the origin. By convention, this is the atom of the group that is directly bonded to the rest of the molecule. The rest of the molecule is placed along the -x axis. The remaining axes are defined as follows:
 * if there is one lone pair(VSCC), that point lies on the +y
 * if there are two lone pairs, the average position of them lies on the +y
 * if there are no lone pairs, map the BCPs of the atom at the origin to a reference. Identify the closest match to the reference to determine a BCP to set as +y
```

### Comparing `subproptools-0.4.0/pyproject.toml` & `subproptools-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,50 +10,54 @@
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
 keywords = ["qtaim", "functional groups"]
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dependencies = [
     "numpy",
     "pandas"
 ]
 
 [project.urls]
 Source = "https://github.com/kmlefran/subproptools"
 [project.optional-dependencies]
 testing = [
     "pgtest~=1.3.1",
     "wheel~=0.31",
-    "coverage[toml]",
+    "coverage",
     "pytest~=6.0",
-    "pytest-cov"
+    "pytest-cov",
+    "pytest-regressions~=2.3",
+    "coveralls"
 ]
 pre-commit = [
     "pre-commit~=2.2",
     "pylint~=2.15.10"
 ]
 docs = [
     "sphinx",
     "sphinxcontrib-contentui",
     "sphinxcontrib-details-directive",
     "furo",
     "markupsafe<2.1",
     "pandas",
-    "numpy"
+    "numpy",
+    "sphinx-rtd-theme"
 ]
 
 [tool.flit.module]
 name = "subproptools"
 
 [tool.pylint.format]
 max-line-length = 125
@@ -68,22 +72,23 @@
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
-source=["subproptools"]
+#source=["subproptools"]
 
 [tool.isort]
 # Configuration of [isort](https://isort.readthedocs.io)
 line_length = 120
+profile = "black"
 force_sort_within_sections = true
 sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'FIRSTPARTY', 'LOCALFOLDER']
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py311
```

### Comparing `subproptools-0.4.0/subproptools/__init__.py` & `subproptools-0.4.2/subproptools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 .. _AIMAll:
     https://aim.tkgristmill.com/index.html
 
 .. _Mawhinney group:
     https://www.lakeheadu.ca/users/M/rmawhinn
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.2"
```

### Comparing `subproptools-0.4.0/subproptools/deprecated.txt` & `subproptools-0.4.2/subproptools/deprecated.txt`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.0/subproptools/qtaim_extract.py` & `subproptools-0.4.2/subproptools/qtaim_extract.py`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.0/subproptools/reference_maps.py` & `subproptools-0.4.2/subproptools/reference_maps.py`

 * *Files identical despite different names*

### Comparing `subproptools-0.4.0/subproptools/sub_reor.py` & `subproptools-0.4.2/subproptools/sub_reor.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,14 +673,16 @@
         posYPoint = []
     if len(posYPoint) > 0:
         xyz_w_y_pt = np.append(molecule_xyz["xyz"], [posYPoint], axis=0)
         # perform reorientation
         molecule_xaxis = _set_xaxis(_set_origin(xyz_w_y_pt, originAtom), negXAtom)
         final_y = molecule_xaxis[posYAtom - 1]
         final_orientation = _set_yaxis(molecule_xaxis[0:-1], final_y)
+    elif posYAtom:
+        posYPoint = molecule_xyz["xyz"][posYAtom - 1]
     else:
         molecule_xaxis = _set_xaxis(
             _set_origin(molecule_xyz["xyz"], originAtom), negXAtom
         )
         final_orientation = molecule_xaxis
     # Generate output
     final_orientation = final_orientation * 0.529177
@@ -741,17 +743,21 @@
     molecule_xyz = qt.get_xyz(data)
     # Labels format A1 etc
     negXAtomLabel = molecule_xyz["Atoms"][negXAtom - 1]
     attachedAtom = molecule_xyz["Atoms"][originAtom - 1]
     # perform reorientation
     if not posYAtom and len(molecule_xyz["Atoms"]) > 2:
         posYPoint = _get_posy_point(sumFileNoExt, atomDict, attachedAtom, negXAtomLabel)
+    elif posYAtom:
+        posYPoint = molecule_xyz["xyz"][posYAtom - 1]
     else:
         posYPoint = []
     if len(posYPoint) > 0:
+        print(molecule_xyz["xyz"])
+        print(posYPoint)
         xyz_w_y_pt = np.append(molecule_xyz["xyz"], [posYPoint], axis=0)
         # perform reorientation
         molecule_xaxis = _set_xaxis(_set_origin(xyz_w_y_pt, originAtom), negXAtom)
         final_y = molecule_xaxis[posYAtom - 1]
         final_orientation = _set_yaxis(molecule_xaxis[0:-1], final_y)
     else:
         molecule_xaxis = _set_xaxis(
@@ -852,15 +858,15 @@
 
     Args:
         csv_file - csv file containining these columns:
         Substituent, originAtom, negXAtom, posYAtom, charge, multiplicity,  label1, label2,...
         Substituent: string label for substituent
         originAtom: numerical index(starting form 1) of atom to use as origin
         negXAtom: numerical index(starting form 1) of atom to place on -x
-        posYAtom: usually 0, but if override desired, numerical index(starting form 1) of atom to place on +y
+        posYAtom: usually 0, but override if desired, numerical index(starting form 1) of atom to place on +y
         charge: charge of the molecule
         multiplicity: multiplicity of the molecule
         label1, label2... label depicting situation for molecule(substrate, method) e.g. "SubH", "B3LYP/cc-pvDZ" etc
         esm: electronic structure method (HF/MP2/DFT functional/etc)
         basis: string for basis to be used
         n_procs: number of processors for use on Cedar, default to 4
         mem: memory to use on Cedar, default to 3200MB
```

### Comparing `subproptools-0.4.0/PKG-INFO` & `subproptools-0.4.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: subproptools
-Version: 0.4.0
+Version: 0.4.2
 Summary: A plugin for extracting data from .sum files and manipuating them
 Keywords: qtaim,functional groups
 Author-email: Kevin Lefrancois-Gagnon <kgagnon@lakeheadu.ca>, Robert Mawhinney <mawhinn@lakeheadu.ca>
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
 Requires-Dist: numpy
@@ -19,26 +20,34 @@
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: markupsafe<2.1 ; extra == "docs"
 Requires-Dist: pandas ; extra == "docs"
 Requires-Dist: numpy ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.15.10 ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3.1 ; extra == "testing"
 Requires-Dist: wheel~=0.31 ; extra == "testing"
-Requires-Dist: coverage[toml] ; extra == "testing"
+Requires-Dist: coverage ; extra == "testing"
 Requires-Dist: pytest~=6.0 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
+Requires-Dist: pytest-regressions~=2.3 ; extra == "testing"
+Requires-Dist: coveralls ; extra == "testing"
 Project-URL: Source, https://github.com/kmlefran/subproptools
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: testing
 
+
+[![ci](https://github.com/kmlefran/subproptools/actions/workflows/ci.yml/badge.svg)](https://github.com/kmlefran/subproptools/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/subproptools/badge/?version=latest)](https://subproptools.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/kmlefran/subproptools/badge.svg?branch=main)](https://coveralls.io/github/kmlefran/subproptools?branch=main)
+[![PyPI version](https://badge.fury.io/py/subproptools.svg)](https://badge.fury.io/py/subproptools)
 # Molecule Reorientation and .sum file handling
 
 This package provides tools to extract data from .sum files (in the qtaimExtract module), and tools to reorient the molecule to defined coordinate systems (in the subreor module). The subreor module rotates to a defined coordinate system. First an atom is positioned at the origin. By convention, this is the atom of the group that is directly bonded to the rest of the molecule. The rest of the molecule is placed along the -x axis. The remaining axes are defined as follows:
 * if there is one lone pair(VSCC), that point lies on the +y
 * if there are two lone pairs, the average position of them lies on the +y
 * if there are no lone pairs, map the BCPs of the atom at the origin to a reference. Identify the closest match to the reference to determine a BCP to set as +y
```

