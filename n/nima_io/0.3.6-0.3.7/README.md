# Comparing `tmp/nima_io-0.3.6.tar.gz` & `tmp/nima_io-0.3.7.tar.gz`

## Comparing `nima_io-0.3.6.tar` & `nima_io-0.3.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.6/.gitmodules
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nima_io-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.6/.readthedocs.yml
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 nima_io-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.6/cz_customize_info.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.6/.github/dependabot.yml
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 nima_io-0.3.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.6/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 nima_io-0.3.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/Makefile
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/click.rst
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/conf.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/make.bat
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/api/api.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/api/nima_io.rst
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/contributing.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/description.rst
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/development.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/ii.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/ii.uml.rst
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/main_module_docstring.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/references/references.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.6/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.6/examples/mydatafile.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.6/src/nima_io/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.6/src/nima_io/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.6/src/nima_io/py.typed
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 nima_io-0.3.6/src/nima_io/read.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/conftest.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/data.filenames.md5
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/data.filenames.sh
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/data.filenames.txt
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/test_cli.py
--rw-r--r--   0        0        0    16246 2020-02-02 00:00:00.000000 nima_io-0.3.6/tests/test_read.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.6/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.6/README.md
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 nima_io-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 nima_io-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.7/.gitmodules
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 nima_io-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.7/.readthedocs.yml
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 nima_io-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.7/cz_customize_info.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 nima_io-0.3.7/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/Makefile
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/click.rst
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/conf.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/make.bat
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/api/api.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/api/nima_io.rst
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/contributing.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/description.rst
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/development.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/ii.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/ii.uml.rst
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/main_module_docstring.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/references/references.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.7/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.7/examples/mydatafile.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/py.typed
+-rw-r--r--   0        0        0    29255 2020-02-02 00:00:00.000000 nima_io-0.3.7/src/nima_io/read.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/conftest.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.md5
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.sh
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/data.filenames.txt
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/test_cli.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 nima_io-0.3.7/tests/test_read.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.7/README.md
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 nima_io-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 nima_io-0.3.7/PKG-INFO
```

### Comparing `nima_io-0.3.6/.pre-commit-config.yaml` & `nima_io-0.3.7/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-shebang-scripts-are-executable
       - id: check-merge-conflict
@@ -22,39 +22,30 @@
       - id: name-tests-test
         args: [--pytest-test-first]
       - id: requirements-txt-fixer
       - id: detect-private-key
       - id: trailing-whitespace
 
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.12.0
+    rev: v2.13.0
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.4
+    rev: v0.3.5
     hooks:
       - id: ruff
-
-  - repo: https://github.com/psf/black
-    rev: 24.3.0
-    hooks:
-      - id: black-jupyter
-      - id: black
-        require_serial: true
-
-  - repo: https://github.com/asottile/blacken-docs
-    rev: 1.16.0
-    hooks:
-      - id: blacken-docs
-        additional_dependencies: [black]
-        exclude: docs/tutorials/usage.*.rst
+        types_or: [python, pyi, jupyter]
+        args: [--fix]
+      # Run the formatter.
+      - id: ruff-format
+        types_or: [python, pyi, jupyter]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         files: \.(yaml|yml|md|html|css|scss|js|json)$
         types_or: [yaml, markdown, html, css, scss, javascript, json]
@@ -91,12 +82,12 @@
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.10.0.1
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.20.0
+    rev: v3.21.3
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `nima_io-0.3.6/.readthedocs.yml` & `nima_io-0.3.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/CHANGELOG.md` & `nima_io-0.3.7/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.3.7 (2024-04-10)
+
+### Build
+
+- **style**: Adopt ruff format instead of black
+- **docs**: Update to the official upload-artifact action
+- **deps-dev**: update matplotlib requirement from <=3.8.3 to <=3.8.4 (#117)
+- **deps**: bump codecov/codecov-action from 4.1.1 to 4.2.0 (#116)
+- **deps-dev**: update lxml requirement from <=5.2.0 to <=5.2.1 (#115)
+- **deps-dev**: update ruff requirement from <=0.3.4 to <=0.3.5 (#114)
+- **deps**: bump actions/configure-pages from 4 to 5 (#112)
+- **deps-dev**: update commitizen requirement from <=3.20.0 to <=3.21.3 (#111)
+- **deps-dev**: update lxml requirement from <=5.1.0 to <=5.2.0 (#110)
+
+### chore
+
+- update pre-commit hooks (#118)
+- update pre-commit hooks (#113)
+
 ## v0.3.6 (2024-03-28)
 
 ### Fix
 
 - **ci**: Add codecov token
 
 ## v0.3.5 (2024-03-28)
```

### Comparing `nima_io-0.3.6/cz_customize_info.txt` & `nima_io-0.3.7/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/.github/workflows/ci.yml` & `nima_io-0.3.7/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
       - name: Run coverage
         if: matrix.tests == 'pytest'
         run: hatch run tests.py${{ matrix.python }}:cov
 
       - name: Upload coverage report
         if: matrix.tests == 'pytest'
-        uses: codecov/codecov-action@v4.1.1
+        uses: codecov/codecov-action@v4.2.0
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
 
       - name: Run mypy
         if: matrix.tests == 'mypy'
         run: hatch run tests.py${{ matrix.python }}:type
```

### Comparing `nima_io-0.3.6/.github/workflows/docs.yml` & `nima_io-0.3.7/.github/workflows/docs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 # Allow one concurrent deployment
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
-  STABLE_PYTHON_VERSION: "3.11"
-permissions:
-  contents: write
+  STABLE_PYTHON_VERSION: "3.12"
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout Repository
         uses: actions/checkout@v4
@@ -76,16 +74,17 @@
         run: |
           python -m pip install --constraint=.github/workflows/constraints.txt pip hatch
 
       - name: Run hatch
         run: hatch run docs
 
       - name: Upload artifact
-        uses: actions/upload-pages-artifact@v2
+        uses: actions/upload-pages-artifact@v3
         with:
+          name: github-pages
           path: "./docs/_build"
 
   deploy:
     runs-on: ubuntu-latest
     if: ${{ github.ref == 'refs/heads/main' }}
     needs: build
     environment:
@@ -94,17 +93,14 @@
     # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
     permissions:
       contents: read
       pages: write
       id-token: write
     steps:
       - name: Download artifact
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: github-pages
 
-      - name: Setup Pages
-        uses: actions/configure-pages@v4
-
       - name: Deploy to GitHub Pages
         id: deployment
-        uses: actions/deploy-pages@v3
+        uses: actions/deploy-pages@v4
```

### Comparing `nima_io-0.3.6/docs/Makefile` & `nima_io-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/conf.py` & `nima_io-0.3.7/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "NImA-io"
-release = "0.3.6"
+release = "0.3.7"
 author = "Daniele Arosio"
 copyright = f"2023, {author}"  # noqa: A001
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
```

### Comparing `nima_io-0.3.6/docs/index.rst` & `nima_io-0.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/make.bat` & `nima_io-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/references/contributing.rst` & `nima_io-0.3.7/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/references/development.rst` & `nima_io-0.3.7/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/references/ii.uml.rst` & `nima_io-0.3.7/docs/references/ii.uml.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/docs/references/main_module_docstring.rst` & `nima_io-0.3.7/docs/references/main_module_docstring.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/examples/mydatafile.txt` & `nima_io-0.3.7/examples/mydatafile.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/src/nima_io/__main__.py` & `nima_io-0.3.7/src/nima_io/__main__.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/src/nima_io/read.py` & `nima_io-0.3.7/src/nima_io/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     log_manager = scyjava.jimport("org.apache.log4j.LogManager")
     file_appender = scyjava.jimport("org.apache.log4j.FileAppender")
     pattern_layout = scyjava.jimport("org.apache.log4j.PatternLayout")
     log_manager.resetConfiguration()
     # Create a FileAppender set to overwrite existing log file
     appender = file_appender(
         pattern_layout("%-4r [%t] %-5p %c %x - %m%n"), log_fp, False  # noqa: FBT003
-    )
+    )  # fmt: skip
     log_manager.getRootLogger().addAppender(appender)
     # Get java runtime version
     runtime = scyjava.jimport("java.lang.Runtime")
     runtime_memory = np.round(runtime.getRuntime().maxMemory() / 2**30, 2)
     system = scyjava.jimport("java.lang.System")
     java_version = system.getProperty("java.version")
     print(f"Bioformats-{version} on java-{java_version} ({runtime_memory} GB)")
@@ -403,21 +403,21 @@
     Raises
     ------
     FileNotFoundError
         If the specified file is not found.
 
     Examples
     --------
-    >>> md, wr = read('tests/data/multi-channel-time-series.ome.tif')
+    >>> md, wr = read("tests/data/multi-channel-time-series.ome.tif")
     >>> md.core.file_format
     'OME-TIFF'
     >>> md.core.size_c, md.core.size_t, md.core.size_x, md.core.bits
     ([3], [7], [439], [8])
     >>> a = wr.read(c=2, t=6, series=0, z=0, rescale=False)
-    >>> a[20,200]
+    >>> a[20, 200]
     -1
     >>> md, wr = read("tests/data/LC26GFP_1.tf8")
     >>> wr.rdr.getSizeX(), md.core.size_x
     (1600, [1600])
     >>> wr.rdr.getMetadataStore()
     <java object 'loci.formats.ome.OMEPyramidStore'>
```

### Comparing `nima_io-0.3.6/tests/data.filenames.md5` & `nima_io-0.3.7/tests/data.filenames.md5`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/tests/data.filenames.sh` & `nima_io-0.3.7/tests/data.filenames.sh`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/tests/test_cli.py` & `nima_io-0.3.7/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # tests path
 tpath = Path(__file__).parent
 datafolder = tpath / "data"
 
 
 def test_version() -> None:
     """Report correct version."""
-    expected_version = "0.3.6"
+    expected_version = "0.3.7"
     runner = CliRunner()
     result = runner.invoke(imgdiff, ["--version"])
     assert result.output.startswith(expected_version)
 
 
 @pytest.fixture(
     params=[
```

### Comparing `nima_io-0.3.6/tests/test_read.py` & `nima_io-0.3.7/tests/test_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     with pytest.raises(FileNotFoundError) as excinfo:
         ir.read(str(tpath / "pippo.tif"))
     expected_error_message = f'File not found: {tpath / "pippo.tif"}'
     assert expected_error_message in str(excinfo.value)
 
 
 def test_metadata_data(
-    tdata_all: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper]
+    tdata_all: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper],
 ) -> None:
     """Test metadata and data consistency."""
     test_d, md, wrapper = tdata_all
     # Check core_md
     assert md.core.size_s == test_d.SizeS
     assert md.core.size_x == test_d.SizeX
     assert md.core.size_y == test_d.SizeY
@@ -183,15 +183,15 @@
         for ls in test_d.data:
             series, x, y, channel, time, z, value = ls[:7]
             a = wrapper.read(c=channel, t=time, series=series, z=z, rescale=False)
             assert a[y, x] == value  # Mind the order: Y then X
 
 
 def test_tile_stitch(
-    tdata_img_tile: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper]
+    tdata_img_tile: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper],
 ) -> None:
     """Test tile stitching for a specific image with tiles."""
     td, md3, wrapper = tdata_img_tile
     md = md3.core
     stitched_plane = ir.stitch(md, wrapper)
     # Y then X
     assert stitched_plane[861, 1224] == 7779
@@ -199,15 +199,15 @@
     stitched_plane = ir.stitch(md, wrapper, t=2, c=3)
     assert stitched_plane[1236, 1488] == 6294
     stitched_plane = ir.stitch(md, wrapper, t=1, c=2)
     assert stitched_plane[564, 1044] == 8560
 
 
 def test_void_tile_stitch(
-    tdata_img_void_tile: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper]
+    tdata_img_void_tile: tuple[TDataItem, ir.Metadata, ir.ImageReaderWrapper],
 ) -> None:
     """Test void tile stitching for a specific image with void tiles."""
     td, md3, wrapper = tdata_img_void_tile
     md = md3.core
     stitched_plane = ir.stitch(md, wrapper, t=0, c=0)
     assert stitched_plane[1179, 882] == 6395
     stitched_plane = ir.stitch(md, wrapper, t=0, c=1)
```

### Comparing `nima_io-0.3.6/.gitignore` & `nima_io-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/LICENSE.txt` & `nima_io-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.6/README.md` & `nima_io-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.6"
+- Version: "0.3.7"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

### Comparing `nima_io-0.3.6/pyproject.toml` & `nima_io-0.3.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering",
   "Development Status :: 3 - Alpha"
 ]
 dependencies = [
   'click <= 8.1.7',
   'jpype1 <= 1.5.0',
-  'lxml <= 5.1.0',
+  'lxml <= 5.2.1',
   'numpy <= 1.26.4',
   'pims <= 0.6.1',
   "setuptools",
   "scyjava <= 1.9.1",
   "bioio-bioformats <= 1.0.0",
   "bfio <= 2.3.6",
   "aicsimageio <= 4.14.0",
@@ -37,33 +37,32 @@
 keywords = [
   "Bioimage",
   "Image Analysis",
   "Metadata",
   "Open Microscopy",
   "Tiled Images"
 ]
-license = "BSD-3-Clause"
-license-files = {paths = ["LICENSE.txt"]}
+license = {file = "LICENSE.txt"}
 name = "nima_io"
 readme = "README.md"
 requires-python = ">=3.10, <3.13"
-version = "0.3.6"
+version = "0.3.7"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen <= 3.20.0",
+  "commitizen <= 3.21.3",
   "ipykernel",
   "jupyter",
   # "jupyterlab",
-  "ruff <= 0.3.4",
+  "ruff <= 0.3.5",
   "pre-commit <= 3.7.0",
   "pylsp-mypy",
-  "python-lsp-ruff",
+  "ruff-lsp",
   "scikit-image <= 0.22.0",
-  "matplotlib <= 3.8.3"
+  "matplotlib <= 3.8.4"
 ]
 docs = [
   "autodocsumm <= 0.2.12",
   "nbsphinx <= 0.9.3",
   "pydata-sphinx-theme <= 0.15.2",
   "Sphinx <= 7.2.6",
   "sphinx-click <= 5.1.0",
@@ -118,15 +117,15 @@
 ignore-words-list = 'ciao'
 quiet-level = 3
 skip = 'examples/general_reading_and_development.ipynb,aics_et_al.ipynb'
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.3.6"
+version = "0.3.7"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version",
   "tests/test_cli.py:expected_version"
 ]
 
@@ -278,16 +277,22 @@
 minversion = "6.0"
 testpaths = [
   "tests"
 ]
 
 [tool.ruff]
 force-exclude = true
-ignore = ["ANN101", "ANN102"]
 line-length = 88
+target-version = "py312"
+
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint]
+ignore = ["ANN101", "ANN102", "ISC001"]
 select = [
   "A",  # builtins
   "ANN",  # typing annotation
   "ARG",  # unused arguments
   "B",  # bugbear
   "C",
   "C4",  # comprehensions
@@ -314,25 +319,22 @@
   "S",  # bandit XXX
   "SIM",  # simplify
   "TID",  # tidy-imports
   "UP",  # pyupgrade
   "YTT",  # 2020
   "W"  # pycodestyle
 ]
+isort.combine-as-imports = true
+isort.force-single-line = false
+isort.known-first-party = ["nima_io"]
+isort.split-on-trailing-comma = true
+mccabe.max-complexity = 12
 
-[tool.ruff.isort]
-combine-as-imports = true
-force-single-line = false
-known-first-party = ["nima_io"]
-split-on-trailing-comma = true
-
-[tool.ruff.mccabe]
-max-complexity = 12
-
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
+"*.ipynb" = ["ERA", "N816", "S314"]
 "tests/*" = ["PLR2004", "S101"]
 "tests/test_cli.py" = [
   "S603"  # Need to call a process as CliRunner and javabridge does not play well together
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
```

### Comparing `nima_io-0.3.6/PKG-INFO` & `nima_io-0.3.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,44 @@
 Metadata-Version: 2.3
 Name: nima_io
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to read microscopy files.
 Project-URL: Bug Tracker, https://github.com/darosio/nima_io/issues
 Project-URL: Changelog, https://github.com/darosio/nima_io/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://nima-io.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/nima_io/releases
 Project-URL: Homepage, https://github.com/darosio/nima_io
 Author-email: Daniele Arosio <darosio@duck.com>
-License-Expression: BSD-3-Clause
+License: Copyright (c) 2023, Daniele Arosio
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of NImA-io nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
 Keywords: Bioimage,Image Analysis,Metadata,Open Microscopy,Tiled Images
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -24,30 +50,30 @@
 Requires-Python: <3.13,>=3.10
 Requires-Dist: aicsimageio<=4.14.0
 Requires-Dist: bfio<=2.3.6
 Requires-Dist: bioio-bioformats<=1.0.0
 Requires-Dist: click<=8.1.7
 Requires-Dist: dask-image<=2023.8.1
 Requires-Dist: jpype1<=1.5.0
-Requires-Dist: lxml<=5.1.0
+Requires-Dist: lxml<=5.2.1
 Requires-Dist: numpy<=1.26.4
 Requires-Dist: pims<=0.6.1
 Requires-Dist: pyometiff<=1.0.0
 Requires-Dist: readlif<=0.6.5
 Requires-Dist: scyjava<=1.9.1
 Requires-Dist: setuptools
 Provides-Extra: dev
-Requires-Dist: commitizen<=3.20.0; extra == 'dev'
+Requires-Dist: commitizen<=3.21.3; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
-Requires-Dist: matplotlib<=3.8.3; extra == 'dev'
+Requires-Dist: matplotlib<=3.8.4; extra == 'dev'
 Requires-Dist: pre-commit<=3.7.0; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
-Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff<=0.3.4; extra == 'dev'
+Requires-Dist: ruff-lsp; extra == 'dev'
+Requires-Dist: ruff<=0.3.5; extra == 'dev'
 Requires-Dist: scikit-image<=0.22.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm<=0.2.12; extra == 'docs'
 Requires-Dist: nbsphinx<=0.9.3; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme<=0.15.2; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints<=2.0.0; extra == 'docs'
 Requires-Dist: sphinx-click<=5.1.0; extra == 'docs'
@@ -73,15 +99,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.6"
+- Version: "0.3.7"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

