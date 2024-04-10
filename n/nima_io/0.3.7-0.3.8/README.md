# Comparing `tmp/nima_io-0.3.7.tar.gz` & `tmp/nima_io-0.3.8.tar.gz`

## Comparing `nima_io-0.3.7.tar` & `nima_io-0.3.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.7/.gitmodules
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 nima_io-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.7/.readthedocs.yml
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 nima_io-0.3.7/CHANGELOG.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.7/cz_customize_info.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/dependabot.yml
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/Makefile
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/click.rst
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/conf.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/make.bat
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/api/api.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/api/nima_io.rst
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/contributing.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/description.rst
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/development.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/ii.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/ii.uml.rst
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/main_module_docstring.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/references.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.7/examples/mydatafile.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/py.typed
--rw-r--r--   0        0        0    29255 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/read.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/conftest.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.md5
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.sh
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.txt
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/test_cli.py
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/test_read.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.7/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.7/LICENSE.txt
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.7/README.md
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 nima_io-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 nima_io-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.8/.gitmodules
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 nima_io-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.8/.readthedocs.yml
+-rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 nima_io-0.3.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.8/cz_customize_info.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/Makefile
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/click.rst
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/conf.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/make.bat
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/api/api.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/api/nima_io.rst
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/contributing.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/description.rst
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/development.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/ii.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/ii.uml.rst
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/main_module_docstring.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/references.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.8/examples/mydatafile.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/py.typed
+-rw-r--r--   0        0        0    29255 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/read.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/conftest.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.md5
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.sh
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.txt
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/test_cli.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/test_read.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.8/LICENSE.txt
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.8/README.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 nima_io-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 nima_io-0.3.8/PKG-INFO
```

### Comparing `nima_io-0.3.7/.pre-commit-config.yaml` & `nima_io-0.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/.readthedocs.yml` & `nima_io-0.3.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/CHANGELOG.md` & `nima_io-0.3.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.3.8 (2024-04-10)
+
+### Fix
+
+- license
+
 ## v0.3.7 (2024-04-10)
 
 ### Build
 
 - **style**: Adopt ruff format instead of black
 - **docs**: Update to the official upload-artifact action
 - **deps-dev**: update matplotlib requirement from <=3.8.3 to <=3.8.4 (#117)
```

### Comparing `nima_io-0.3.7/cz_customize_info.txt` & `nima_io-0.3.8/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/.github/workflows/ci.yml` & `nima_io-0.3.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/.github/workflows/docs.yml` & `nima_io-0.3.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/Makefile` & `nima_io-0.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/conf.py` & `nima_io-0.3.8/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "NImA-io"
-release = "0.3.7"
+release = "0.3.8"
 author = "Daniele Arosio"
 copyright = f"2023, {author}"  # noqa: A001
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
```

### Comparing `nima_io-0.3.7/docs/index.rst` & `nima_io-0.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/make.bat` & `nima_io-0.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/references/contributing.rst` & `nima_io-0.3.8/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/references/development.rst` & `nima_io-0.3.8/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/references/ii.uml.rst` & `nima_io-0.3.8/docs/references/ii.uml.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/docs/references/main_module_docstring.rst` & `nima_io-0.3.8/docs/references/main_module_docstring.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/examples/mydatafile.txt` & `nima_io-0.3.8/examples/mydatafile.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/src/nima_io/__main__.py` & `nima_io-0.3.8/src/nima_io/__main__.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/src/nima_io/read.py` & `nima_io-0.3.8/src/nima_io/read.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/tests/data.filenames.md5` & `nima_io-0.3.8/tests/data.filenames.md5`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/tests/data.filenames.sh` & `nima_io-0.3.8/tests/data.filenames.sh`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/tests/test_cli.py` & `nima_io-0.3.8/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # tests path
 tpath = Path(__file__).parent
 datafolder = tpath / "data"
 
 
 def test_version() -> None:
     """Report correct version."""
-    expected_version = "0.3.7"
+    expected_version = "0.3.8"
     runner = CliRunner()
     result = runner.invoke(imgdiff, ["--version"])
     assert result.output.startswith(expected_version)
 
 
 @pytest.fixture(
     params=[
```

### Comparing `nima_io-0.3.7/tests/test_read.py` & `nima_io-0.3.8/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/.gitignore` & `nima_io-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/LICENSE.txt` & `nima_io-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.7/README.md` & `nima_io-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.7"
+- Version: "0.3.8"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

### Comparing `nima_io-0.3.7/pyproject.toml` & `nima_io-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 keywords = [
   "Bioimage",
   "Image Analysis",
   "Metadata",
   "Open Microscopy",
   "Tiled Images"
 ]
-license = {file = "LICENSE.txt"}
+license = "BSD-3-Clause"
 name = "nima_io"
 readme = "README.md"
 requires-python = ">=3.10, <3.13"
-version = "0.3.7"
+version = "0.3.8"
 
 [project.optional-dependencies]
 dev = [
   "commitizen <= 3.21.3",
   "ipykernel",
   "jupyter",
   # "jupyterlab",
@@ -117,15 +117,15 @@
 ignore-words-list = 'ciao'
 quiet-level = 3
 skip = 'examples/general_reading_and_development.ipynb,aics_et_al.ipynb'
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.3.7"
+version = "0.3.8"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version",
   "tests/test_cli.py:expected_version"
 ]
```

### Comparing `nima_io-0.3.7/PKG-INFO` & `nima_io-0.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,18 @@
 Metadata-Version: 2.3
 Name: nima_io
-Version: 0.3.7
+Version: 0.3.8
 Summary: A project to read microscopy files.
 Project-URL: Bug Tracker, https://github.com/darosio/nima_io/issues
 Project-URL: Changelog, https://github.com/darosio/nima_io/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://nima-io.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/nima_io/releases
 Project-URL: Homepage, https://github.com/darosio/nima_io
 Author-email: Daniele Arosio <darosio@duck.com>
-License: Copyright (c) 2023, Daniele Arosio
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of NImA-io nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Keywords: Bioimage,Image Analysis,Metadata,Open Microscopy,Tiled Images
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -99,15 +73,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.7"
+- Version: "0.3.8"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

