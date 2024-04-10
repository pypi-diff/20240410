# Comparing `tmp/sphinx_autodoc_typehints-2.0.0.tar.gz` & `tmp/sphinx_autodoc_typehints-2.0.1.tar.gz`

## Comparing `sphinx_autodoc_typehints-2.0.0.tar` & `sphinx_autodoc_typehints-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.markdownlint.yaml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tox.ini
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/whitelist.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/release.yml
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/workflows/check.yml
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    36315 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/__init__.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/attributes_patch.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/parser.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/patches.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/py.typed
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/version.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0    22040 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/test_integration.py
--rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/test_sphinx_autodoc_typehints.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/test_version.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/conf.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_future_annotations.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_simple.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_simple_default_role.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_simple_no_use_rtype.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_without_complete_typehints.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/future_annotations.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/simple.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/simple_default_role.rst
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/simple_no_use_rtype.rst
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/without_complete_typehints.rst
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-integration/conf.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard/conf.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard/demo_typing_guard.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard/demo_typing_guard_dummy.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard/index.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard-tmp/conf.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard-tmp/demo_typing_guard.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard-tmp/index.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/LICENSE
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/README.md
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.markdownlint.yaml
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/ignore-words.txt
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tox.ini
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/whitelist.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/release.yml
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    36315 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/__init__.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/attributes_patch.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/parser.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/patches.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/version.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0    23807 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/test_integration.py
+-rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/test_sphinx_autodoc_typehints.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/test_version.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/conf.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_future_annotations.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_simple.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_simple_default_role.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_simple_no_use_rtype.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_without_complete_typehints.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/future_annotations.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/simple.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/simple_default_role.rst
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/simple_no_use_rtype.rst
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/without_complete_typehints.rst
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-integration/conf.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard/conf.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard/demo_typing_guard.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard/demo_typing_guard_dummy.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard/index.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard-tmp/conf.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard-tmp/demo_typing_guard.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard-tmp/index.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/LICENSE
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/README.md
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 sphinx_autodoc_typehints-2.0.1/PKG-INFO
```

### Comparing `sphinx_autodoc_typehints-2.0.0/.pre-commit-config.yaml` & `sphinx_autodoc_typehints-2.0.1/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.0"
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.1
     hooks:
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix]
-  - repo: https://github.com/psf/black
-    rev: 24.1.1
+      - id: check-github-workflows
+        args: [ "--verbose" ]
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.6
     hooks:
-      - id: black
+      - id: codespell
+        additional_dependencies: ["tomli>=2.0.1"]
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/tox-dev/pyproject-fmt
     rev: "1.7.0"
     hooks:
       - id: pyproject-fmt
-        additional_dependencies: ["tox>=4.11.4"]
+        additional_dependencies: ["tox>=4.13"]
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.3.5"
+    hooks:
+      - id: ruff-format
+      - id: ruff
+        args: ["--fix", "--unsafe-fixes", "--exit-non-zero-on-fix"]
   - repo: meta
     hooks:
       - id: check-hooks-apply
       - id: check-useless-excludes
```

### Comparing `sphinx_autodoc_typehints-2.0.0/CHANGELOG.md` & `sphinx_autodoc_typehints-2.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/tox.ini` & `sphinx_autodoc_typehints-2.0.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 env_list =
     fix
     py312
     py311
     py310
     py39
     py38
-    py37
     type
     coverage
     readme
 skip_missing_interpreters = true
 
 [testenv]
 description = run tests with {basepython}
@@ -35,41 +34,41 @@
       tests}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.5
+    pre-commit>=3.6.2
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:py312]
 extras =
     testing
     type-comment
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.7.1
-    types-docutils>=0.20.0.3
+    mypy==1.8
+    types-docutils>=0.20.0.20240304
 set_env =
     {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src
     mypy tests
 
 [testenv:coverage]
 description = combine coverage files and generate diff (against DIFF_AGAINST defaulting to origin/main)
 skip_install = true
 deps =
     covdefaults>=2.3
-    coverage>=7.3.2
-    diff-cover>=8.0.1
+    coverage>=7.4.3
+    diff-cover>=8.0.3
 extras =
 parallel_show_output = true
 pass_env =
     DIFF_AGAINST
 set_env =
     COVERAGE_FILE = {toxworkdir}/.coverage
 commands =
@@ -80,26 +79,26 @@
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}/coverage.xml
 depends =
     py312
     py311
     py310
     py39
     py38
-    py37
 
 [testenv:readme]
 description = check that the long description is valid (need for PyPI)
 skip_install = true
 deps =
-    build[virtualenv]>=1.0.3
-    twine>=4.0.2
+    build[virtualenv]>=1.1.1
+    twine>=5
 extras =
 commands =
     pyproject-build -o {envtmpdir} --wheel --sdist .
     twine check {envtmpdir}/*
 
 [testenv:dev]
 description = generate a DEV environment
 package = editable
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
+uv_seed = true
```

### Comparing `sphinx_autodoc_typehints-2.0.0/whitelist.txt` & `sphinx_autodoc_typehints-2.0.1/whitelist.txt`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/.github/workflows/check.yml` & `sphinx_autodoc_typehints-2.0.1/.github/workflows/check.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: check
 on:
   workflow_dispatch:
   push:
-    branches: "main"
+    branches: ["main"]
     tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
@@ -27,15 +27,15 @@
           - "3.8"
     steps:
       - name: Setup python for tox
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install tox
-        run: python -m pip install tox
+        run: python -m pip install tox-uv
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.py }}
@@ -76,15 +76,15 @@
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v5
         with:
           python-version: "3.12"
       - name: Install tox
-        run: python -m pip install tox
+        run: python -m pip install tox-uv
       - name: Setup coverage tool
         run: tox -e coverage --notest
       - name: Install package builder
         run: python -m pip install build
       - name: Build package
         run: pyproject-build --wheel .
       - name: Download coverage data
```

### Comparing `sphinx_autodoc_typehints-2.0.0/.github/workflows/release.yml` & `sphinx_autodoc_typehints-2.0.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         run: python -m pip install build
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Build package
         run: pyproject-build -s -w . -o dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/__init__.py` & `sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         return "builtins"
     if _get_types_type(annotation) is not None:
         return "types"
     is_new_type = sys.version_info >= (3, 10) and isinstance(annotation, NewType)
     if (
         is_new_type
         or isinstance(annotation, TypeVar)
-        or type(annotation).__name__ in ("ParamSpec", "ParamSpecArgs", "ParamSpecKwargs")
+        or type(annotation).__name__ in {"ParamSpec", "ParamSpecArgs", "ParamSpecKwargs"}
     ):
         return "typing"
     if hasattr(annotation, "__module__"):
         return annotation.__module__  # type: ignore[no-any-return]
     if hasattr(annotation, "__origin__"):
         return annotation.__origin__.__module__  # type: ignore[no-any-return]
     msg = f"Cannot determine the module of {annotation}"
@@ -103,15 +103,15 @@
     if _is_newtype(annotation):
         return "NewType"
 
     if getattr(annotation, "__qualname__", None):
         return annotation.__qualname__  # type: ignore[no-any-return]
     if getattr(annotation, "_name", None):  # Required for generic aliases on Python 3.7+
         return annotation._name  # type: ignore[no-any-return]  # noqa: SLF001
-    if module in ("typing", "typing_extensions") and isinstance(getattr(annotation, "name", None), str):
+    if module in {"typing", "typing_extensions"} and isinstance(getattr(annotation, "name", None), str):
         # Required for at least Pattern and Match
         return annotation.name  # type: ignore[no-any-return]
 
     origin = getattr(annotation, "__origin__", None)
     if origin:
         if getattr(origin, "__qualname__", None):  # Required for Protocol subclasses
             return origin.__qualname__  # type: ignore[no-any-return]
@@ -136,15 +136,15 @@
     except (KeyError, AttributeError):
         pass
     else:
         if annotation is original:
             return ()  # This is the original, not parametrized type
 
     # Special cases
-    if class_name in ("Pattern", "Match") and hasattr(annotation, "type_var"):  # Python < 3.7
+    if class_name in {"Pattern", "Match"} and hasattr(annotation, "type_var"):  # Python < 3.7
         return (annotation.type_var,)
     if class_name == "ClassVar" and hasattr(annotation, "__type__"):  # ClassVar on Python < 3.7
         return (annotation.__type__,)
     if class_name == "TypeVar" and hasattr(annotation, "__constraints__"):
         return annotation.__constraints__  # type: ignore[no-any-return]
     if class_name == "NewType" and hasattr(annotation, "__supertype__"):
         return (annotation.__supertype__,)
@@ -165,15 +165,15 @@
     if len(fmt) == 0:
         return "()"
     if len(fmt) == 1:
         return f"({fmt[0]}, )"
     return f"({', '.join(fmt)})"
 
 
-def format_annotation(annotation: Any, config: Config) -> str:  # noqa: C901, PLR0911, PLR0912, PLR0915
+def format_annotation(annotation: Any, config: Config) -> str:  # noqa: C901, PLR0911, PLR0912, PLR0915, PLR0914
     """
     Format the annotation.
 
     :param annotation:
     :param config:
     :return:
     """
@@ -234,27 +234,27 @@
         args_format = f"\\(``{annotation.__name__}``{', {}' if args else ''}"
         if params:
             args_format += "".join(f", {k}={v}" for k, v in params.items())
         args_format += ")"
         formatted_args = None if args else args_format
     elif full_name == "typing.Optional":
         args = tuple(x for x in args if x is not type(None))
-    elif full_name in ("typing.Union", "types.UnionType") and type(None) in args:
+    elif full_name in {"typing.Union", "types.UnionType"} and type(None) in args:
         if len(args) == 2:  # noqa: PLR2004
             full_name = "typing.Optional"
             role = "data"
             args = tuple(x for x in args if x is not type(None))
         else:
             simplify_optional_unions: bool = getattr(config, "simplify_optional_unions", True)
             if not simplify_optional_unions:
                 full_name = "typing.Optional"
                 role = "data"
                 args_format = f"\\[:py:data:`{prefix}typing.Union`\\[{{}}]]"
                 args = tuple(x for x in args if x is not type(None))
-    elif full_name in ("typing.Callable", "collections.abc.Callable") and args and args[0] is not ...:
+    elif full_name in {"typing.Callable", "collections.abc.Callable"} and args and args[0] is not ...:
         fmt = [format_annotation(arg, config) for arg in args]
         formatted_args = f"\\[\\[{', '.join(fmt[:-1])}], {fmt[-1]}]"
     elif full_name == "typing.Literal":
         formatted_args = f"\\[{', '.join(f'``{arg!r}``' for arg in args)}]"
     elif is_bars_union:
         return " | ".join([format_annotation(arg, config) for arg in args])
 
@@ -312,15 +312,15 @@
     aligned_suffix = [whitespace + remove_prefix(s, whitespace) for s in lines[idx + 1 :]]
 
     # Put it together again
     aligned_prefix.append(fn_def)
     return "\n".join(aligned_prefix + aligned_suffix)
 
 
-def process_signature(  # noqa: C901, PLR0913
+def process_signature(  # noqa: C901, PLR0913, PLR0917
     app: Sphinx,
     what: str,
     name: str,
     obj: Any,
     options: Options,  # noqa: ARG001
     signature: str,  # noqa: ARG001
     return_annotation: str,  # noqa: ARG001
@@ -537,15 +537,15 @@
     if comment_returns:
         rv["return"] = comment_returns
 
     args = load_args(obj_ast)
     comment_args = split_type_comment_args(comment_args_str)
     is_inline = len(comment_args) == 1 and comment_args[0] == "..."
     if not is_inline:
-        if args and args[0].arg in ("self", "cls") and len(comment_args) != len(args):
+        if args and args[0].arg in {"self", "cls"} and len(comment_args) != len(args):
             comment_args.insert(0, None)  # self/cls may be omitted in type comments, insert blank
 
         if len(args) != len(comment_args):
             _LOGGER.warning('Not enough type comments found on "%s"', name)
             return rv
 
     for at, arg in enumerate(args):
@@ -586,17 +586,17 @@
     comment = comment.strip().lstrip("(").rstrip(")")
     result: list[str | None] = []
     if not comment:
         return result
 
     brackets, start_arg_at, at = 0, 0, 0
     for at, char in enumerate(comment):
-        if char in ("[", "("):
+        if char in {"[", "("}:
             brackets += 1
-        elif char in ("]", ")"):
+        elif char in {"]", ")"}:
             brackets -= 1
         elif char == "," and brackets == 0:
             add(comment[start_arg_at:at])
             start_arg_at = at + 1
 
     add(comment[start_arg_at : at + 1])
     return result
@@ -612,15 +612,15 @@
             return f" (default: ``{formatted}``)"
         return f", default: ``{formatted}``"
     if app.config.typehints_defaults == "braces-after":
         return f" (default: ``{formatted}``)"
     return f"default: ``{formatted}``"
 
 
-def process_docstring(  # noqa: PLR0913
+def process_docstring(  # noqa: PLR0913, PLR0917, PLR0917
     app: Sphinx,
     what: str,
     name: str,
     obj: Any,
     options: Options | None,  # noqa: ARG001
     lines: list[str],
 ) -> None:
@@ -691,15 +691,15 @@
 
     if keyword not in {"param", "parameter", "arg", "argument"}:
         return False
 
     return any(doc_name == prefix + arg_name for prefix in ("", "\\*", "\\**", "\\*\\*"))
 
 
-def _inject_types_to_docstring(  # noqa: PLR0913
+def _inject_types_to_docstring(  # noqa: PLR0913, PLR0917
     type_hints: dict[str, Any],
     signature: inspect.Signature | None,
     original_obj: Any,
     app: Sphinx,
     what: str,
     name: str,
     lines: list[str],
@@ -775,14 +775,17 @@
 
     Descend through the first children until we locate one with a line number or return None if None of them have one.
 
     I'm not aware of any rst on which this returns None, to find out would require a more detailed analysis of the
     docutils rst parser source code. An example where the node doesn't have a line number but the first child does is
     all `definition_list` nodes. It seems like bullet_list and option_list get line numbers, but enum_list also doesn't.
     """
+    if node is None:
+        return None
+
     while node.line is None and node.children:
         node = node.children[0]
     return node.line
 
 
 def tag_name(node: Node) -> str:
     return node.tagname  # type:ignore[attr-defined,no-any-return]
@@ -822,25 +825,25 @@
         next_sibling = child.next_node(descend=False, siblings=True)
         line_no = node_line_no(next_sibling) if next_sibling else None
         at = line_no - 2 if line_no else len(lines)
         return InsertIndexInfo(insert_index=at, found_param=True)
 
     # 4. Insert before examples
     for child in doc.children:
-        if tag_name(child) in ["literal_block", "paragraph", "field_list"]:
+        if tag_name(child) in {"literal_block", "paragraph", "field_list"}:
             continue
         line_no = node_line_no(child)
         at = line_no - 2 if line_no else len(lines)
         return InsertIndexInfo(insert_index=at, found_directive=True)
 
     # 5. Otherwise, insert at end
     return InsertIndexInfo(insert_index=len(lines))
 
 
-def _inject_rtype(  # noqa: PLR0913
+def _inject_rtype(  # noqa: PLR0913, PLR0917
     type_hints: dict[str, Any],
     original_obj: Any,
     app: Sphinx,
     what: str,
     name: str,
     lines: list[str],
 ) -> None:
@@ -872,15 +875,15 @@
     if app.config.typehints_use_rtype or not r.found_return:
         line = f":rtype: {formatted_annotation}"
         lines.insert(insert_index, line)
         if r.found_directive:
             lines.insert(insert_index + 1, "")
     else:
         line = lines[insert_index]
-        lines[insert_index] = f":return: {formatted_annotation} --{line[line.find(' '):]}"
+        lines[insert_index] = f":return: {formatted_annotation} --{line[line.find(' ') :]}"
 
 
 def validate_config(app: Sphinx, env: BuildEnvironment, docnames: list[str]) -> None:  # noqa: ARG001
     valid = {None, "comma", "braces", "braces-after"}
     if app.config.typehints_defaults not in valid | {False}:
         msg = f"typehints_defaults needs to be one of {valid!r}, not {app.config.typehints_defaults!r}"
         raise ValueError(msg)
@@ -917,16 +920,15 @@
     """
     Add css tag around rendered type.
 
     The body should be escaped rst. This renders its body as rst and wraps the
     result in <span class="sphinx_autodoc_typehints-type"> </span>
     """
     unescaped = unescape(text)
-    # the typestubs for docutils don't have any info about Inliner
-    doc = parse(unescaped, inliner.document.settings)  # type: ignore[attr-defined]
+    doc = parse(unescaped, inliner.document.settings)
     n = nodes.inline(text)
     n["classes"].append("sphinx_autodoc_typehints-type")
     n += doc.children[0].children
     return [n], []
 
 
 def setup(app: Sphinx) -> dict[str, bool]:
@@ -946,16 +948,16 @@
     app.connect("autodoc-process-docstring", process_docstring)
     install_patches(app)
     return {"parallel_read_safe": True, "parallel_write_safe": True}
 
 
 __all__ = [
     "__version__",
+    "backfill_type_hints",
     "format_annotation",
     "get_annotation_args",
     "get_annotation_class_name",
     "get_annotation_module",
     "normalize_source_lines",
     "process_docstring",
     "process_signature",
-    "backfill_type_hints",
 ]
```

### Comparing `sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/attributes_patch.py` & `sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/attributes_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 orig_add_directive_header = AttributeDocumenter.add_directive_header
 orig_handle_signature = PyAttribute.handle_signature
 
 
 def _stringify_annotation(app: Sphinx, annotation: Any, mode: str = "") -> str:  # noqa: ARG001
     # Format the annotation with sphinx-autodoc-typehints and inject our magic prefix to tell our patched
     # PyAttribute.handle_signature to treat it as rst.
-    from . import format_annotation
+    from . import format_annotation  # noqa: PLC0415
 
     return TYPE_IS_RST_LABEL + format_annotation(annotation, app.config)
 
 
 def patch_attribute_documenter(app: Sphinx) -> None:
     """Instead of using stringify_typehint in `AttributeDocumenter.add_directive_header`, use `format_annotation`."""
```

### Comparing `sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/parser.py` & `sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,24 @@
 from sphinx.util.docutils import sphinx_domains
 
 if TYPE_CHECKING:
     import optparse
 
     from docutils import nodes
     from docutils.frontend import Values
+    from docutils.statemachine import StringList
+
+
+class _RstSnippetParser(RSTParser):
+    @staticmethod
+    def decorate(_content: StringList) -> None:
+        """Override to skip processing rst_epilog/rst_prolog for typing."""
 
 
 def parse(inputstr: str, settings: Values | optparse.Values) -> nodes.document:
     """Parse inputstr and return a docutils document."""
     doc = new_document("", settings=settings)
     with sphinx_domains(settings.env):
-        parser = RSTParser()
+        parser = _RstSnippetParser()
         parser.set_application(settings.env.app)
         parser.parse(inputstr, doc)
     return doc
```

### Comparing `sphinx_autodoc_typehints-2.0.0/src/sphinx_autodoc_typehints/patches.py` & `sphinx_autodoc_typehints-2.0.1/src/sphinx_autodoc_typehints/patches.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,39 +24,39 @@
     Normally, `FunctionDocumenter.format_signature` and `MethodDocumenter.format_signature` call
     `super().format_signature` which ends up going to `Documenter.format_signature`, and this last method emits the
     `autodoc-process-signature` event. However, if there are overloads, `FunctionDocumenter.format_signature` does
     something else and the event never occurs. Here we remove this alternative code path by brute force.
 
     See https://github.com/tox-dev/sphinx-autodoc-typehints/issues/296
     """
-    from sphinx.ext.autodoc import FunctionDocumenter, MethodDocumenter
+    from sphinx.ext.autodoc import FunctionDocumenter, MethodDocumenter  # noqa: PLC0415
 
     del FunctionDocumenter.format_signature
     del MethodDocumenter.format_signature
 
 
-def napoleon_numpy_docstring_return_type_processor(  # noqa: PLR0913
+def napoleon_numpy_docstring_return_type_processor(  # noqa: PLR0913, PLR0917
     app: Sphinx,
     what: str,
     name: str,  # noqa: ARG001
     obj: Any,  # noqa: ARG001
     options: Options | None,  # noqa: ARG001
     lines: list[str],
 ) -> None:
     """Insert a : under Returns: to tell napoleon not to look for a return type."""
-    if what not in ["function", "method"]:
+    if what not in {"function", "method"}:
         return
     if not getattr(app.config, "napoleon_numpy_docstring", False):
         return
 
     # Search for the returns header:
     # Returns:
     # --------
     for pos, line in enumerate(lines[:-2]):
-        if line.lower().strip(":") not in ["return", "returns"]:
+        if line.lower().strip(":") not in {"return", "returns"}:
             continue
         # Underline detection.
         chars = set(lines[pos + 1].strip())
         # Napoleon allows the underline to consist of a bunch of weirder things...
         if len(chars) != 1 or next(iter(chars)) not in "=-~_*+#":
             continue
         pos = pos + 2  # noqa: PLW2901
```

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/conftest.py` & `sphinx_autodoc_typehints-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/test_integration.py` & `sphinx_autodoc_typehints-2.0.1/tests/test_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     def __dunder_method(self, x: str) -> str:
         """
         Dunder method docstring.
 
         :param x: foo
         """
 
-    def __magic_custom_method__(self, x: str) -> str:
+    def __magic_custom_method__(self, x: str) -> str:  # noqa: PLW3201
         """
         Magic dunder method docstring.
 
         :param x: foo
         """
 
     @classmethod
-    def a_classmethod(cls, x: bool, y: int, z: Optional[str] = None) -> str:  # noqa: ANN102, UP007
+    def a_classmethod(cls, x: bool, y: int, z: Optional[str] = None) -> str:  # noqa: UP007
         """
         Classmethod docstring.
 
         :param x: foo
         :param y: bar
         :param z: baz
         """
@@ -411,27 +411,27 @@
     def __init__(
         self,
         x,  # type: int  # noqa: ANN001
     ) -> None:
         # type: (...) -> None
         pass
 
-    def foo(  # noqa: ANN201
+    def foo(  # noqa: ANN201, PLR6301
         self,
         x,  # type: str  # noqa: ANN001, ARG002
     ):
         # type: (...) -> int
         """
         Method docstring.
 
         :arg x: foo
         """
         return 42
 
-    def method_without_typehint(self, x):  # noqa: ANN001, ANN201, ARG002
+    def method_without_typehint(self, x):  # noqa: ANN001, ANN201, ARG002, PLR6301
         """
         Method docstring.
         """
         # test that multiline str can be correctly indented
         multiline_str = """
 test
 """
@@ -506,25 +506,25 @@
 
     :param x: foo
     """
 
     def __init__(self, x=None) -> None:  # type: (Optional[Callable[[int, bytes], int]]) -> None  # noqa: ANN001
         pass
 
-    def foo(self, x=1):  # type: (Callable[[int, bytes], int]) -> int  # noqa: ANN001, ANN201
+    def foo(self, x=1):  # type: (Callable[[int, bytes], int]) -> int  # noqa: ANN001, ANN201, PLR6301
         """
         Method docstring.
 
         :param x: foo
         """
         return x(1, b"")
 
     @classmethod
     def mk(  # noqa: ANN206
-        cls,  # noqa: ANN102
+        cls,
         x=None,  # noqa: ANN001
     ):  # type: (Optional[Callable[[int, bytes], int]]) -> ClassWithTypehintsNotInline
         """
         Method docstring.
 
         :param x: foo
         """
@@ -1090,15 +1090,15 @@
 
        Term
           A description
 
           maybe multiple lines
 
        Next Term
-          Somethign about it
+          Something about it
 
     """,
 )
 def docstring_with_definition_list_after_params(param: int) -> None:  # noqa: ARG001
     """Do something.
 
     Args:
@@ -1106,15 +1106,15 @@
 
     Term
         A description
 
         maybe multiple lines
 
     Next Term
-        Somethign about it
+        Something about it
     """
 
 
 @expected(
     """
     mod.docstring_with_enum_list_after_params(param)
 
@@ -1158,15 +1158,15 @@
 
        Term
           A description
 
           maybe multiple lines
 
        Next Term
-          Somethign about it
+          Something about it
 
        -[ Example ]-
     """,
 )
 def docstring_with_definition_list_after_params_no_blank_line(param: int) -> None:  # noqa: ARG001
     """Do something.
 
@@ -1175,15 +1175,15 @@
 
     Term
         A description
 
         maybe multiple lines
 
     Next Term
-        Somethign about it
+        Something about it
     .. rubric:: Example
     """
 
 
 @expected(
     """
     mod.has_typevar(param)
@@ -1264,31 +1264,118 @@
 
     Args:
         a: blah
     """
     return a
 
 
+prolog = """
+.. |test_node_start| replace:: {test_node_start}
+""".format(test_node_start="test_start")
+
+
+@expected(
+    """
+    mod.docstring_with_multiline_note_after_params_prolog_replace(param)
+
+       Do something.
+
+       Parameters:
+          **param** ("int") -- A parameter.
+
+       Return type:
+          "None"
+
+       Note:
+
+         Some notes. test_start More notes
+
+    """,
+    rst_prolog=prolog,
+)
+def docstring_with_multiline_note_after_params_prolog_replace(param: int) -> None:  # noqa: ARG001
+    """Do something.
+
+    Args:
+        param: A parameter.
+
+    Note:
+
+        Some notes. |test_node_start|
+        More notes
+    """
+
+
+epilog = """
+.. |test_node_end| replace:: {test_node_end}
+""".format(test_node_end="test_end")
+
+
+@expected(
+    """
+    mod.docstring_with_multiline_note_after_params_epilog_replace(param)
+
+       Do something.
+
+       Parameters:
+          **param** ("int") -- A parameter.
+
+       Return type:
+          "None"
+
+       Note:
+
+         Some notes. test_end More notes
+
+    """,
+    rst_epilog=epilog,
+)
+def docstring_with_multiline_note_after_params_epilog_replace(param: int) -> None:  # noqa: ARG001
+    """Do something.
+
+    Args:
+        param: A parameter.
+
+    Note:
+
+        Some notes. |test_node_end|
+        More notes
+    """
+
+
+# Config settings for each test run.
+# Config Name: Sphinx Options as Dict.
+configs = {
+    "default_conf": {},
+    "prolog_conf": {"rst_prolog": prolog},
+    "epilog_conf": {
+        "rst_epilog": epilog,
+    },
+    "bothlog_conf": {
+        "rst_prolog": prolog,
+        "rst_epilog": epilog,
+    },
+}
+
+
 @pytest.mark.parametrize("val", [x for x in globals().values() if hasattr(x, "EXPECTED")])
+@pytest.mark.parametrize("conf_run", ["default_conf", "prolog_conf", "epilog_conf", "bothlog_conf"])
 @pytest.mark.sphinx("text", testroot="integration")
 def test_integration(
-    app: SphinxTestApp,
-    status: StringIO,
-    warning: StringIO,
-    monkeypatch: pytest.MonkeyPatch,
-    val: Any,
+    app: SphinxTestApp, status: StringIO, warning: StringIO, monkeypatch: pytest.MonkeyPatch, val: Any, conf_run: str
 ) -> None:
     if isclass(val) and issubclass(val, BaseException):
         template = AUTO_EXCEPTION
     elif isclass(val):
         template = AUTO_CLASS
     else:
         template = AUTO_FUNCTION
 
     (Path(app.srcdir) / "index.rst").write_text(template.format(val.__name__))
+    app.config.__dict__.update(configs[conf_run])
     app.config.__dict__.update(val.OPTIONS)
     monkeypatch.setitem(sys.modules, "mod", sys.modules[__name__])
     app.build()
     assert "build succeeded" in status.getvalue()  # Build succeeded
 
     regexp = getattr(val, "WARNING", None)
     value = warning.getvalue().strip()
```

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/test_sphinx_autodoc_typehints.py` & `sphinx_autodoc_typehints-2.0.1/tests/test_sphinx_autodoc_typehints.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 from unittest.mock import create_autospec, patch
 
 import pytest
 import typing_extensions
 from sphinx.application import Sphinx
 from sphinx.config import Config
+
 from sphinx_autodoc_typehints import (
     _resolve_type_guarded_imports,
     backfill_type_hints,
     format_annotation,
     get_annotation_args,
     get_annotation_class_name,
     get_annotation_module,
@@ -602,15 +603,17 @@
 
     app.config.master_doc = "simple_default_role"  # type: ignore[attr-defined] # create flag
     app.config.default_role = "literal"  # type: ignore[attr-defined]
     app.build()
 
     assert "build succeeded" in status.getvalue()  # Build succeeded
 
-    contents_lines = (Path(app.srcdir) / "_build/pseudoxml/simple_default_role.pseudoxml").read_text().splitlines()
+    contents_lines = (
+        (Path(app.srcdir) / "_build/pseudoxml/simple_default_role.pseudoxml").read_text(encoding="utf-8").splitlines()
+    )
     list_item_idxs = [i for i, line in enumerate(contents_lines) if line.strip() == "<list_item>"]
     foo_param = dedent("\n".join(contents_lines[list_item_idxs[0] : list_item_idxs[1]]))
     expected_foo_param = """\
     <list_item>
         <paragraph>
             <literal_strong>
                 x
@@ -834,15 +837,15 @@
     set_python_path()
     app.build()
     assert "build succeeded" in status.getvalue()
     assert not warning.getvalue()
 
 
 def test_no_source_code_type_guard() -> None:
-    from csv import Error
+    from csv import Error  # noqa: PLC0415
 
     _resolve_type_guarded_imports([], Error)
 
 
 @pytest.mark.sphinx("text", testroot="dummy")
 @patch("sphinx.writers.text.MAXWIDTH", 2000)
 def test_sphinx_output_formatter_no_use_rtype(app: SphinxTestApp, status: StringIO) -> None:
```

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_simple_no_use_rtype.py` & `sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_simple_no_use_rtype.py`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/roots/test-dummy/dummy_module_without_complete_typehints.py` & `sphinx_autodoc_typehints-2.0.1/tests/roots/test-dummy/dummy_module_without_complete_typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard/demo_typing_guard.py` & `sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard/demo_typing_guard.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -55,13 +55,13 @@
             """
 
 
 def func(_x: Literal) -> None: ...
 
 
 __all__ = [
-    "a",
+    "AnotherClass",
+    "SomeClass",
     "ValueError",
+    "a",
     "cmp_to_key",
-    "SomeClass",
-    "AnotherClass",
 ]
```

### Comparing `sphinx_autodoc_typehints-2.0.0/tests/roots/test-resolve-typing-guard-tmp/demo_typing_guard.py` & `sphinx_autodoc_typehints-2.0.1/tests/roots/test-resolve-typing-guard-tmp/demo_typing_guard.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 class SomeClass:
     """This class does something."""
 
     date: datetime.date
     """Date to handle"""
 
     @classmethod
-    def from_str(cls, input_value: str) -> SomeClass:  # noqa: ANN102
+    def from_str(cls, input_value: str) -> SomeClass:
         """
-        Initialise from string
+        Initialize from string
 
         :param input_value: Input
         :return: result
         """
         return cls(input_value)
 
     @classmethod
-    def from_date(cls, input_value: datetime.date) -> SomeClass:  # noqa: ANN102
+    def from_date(cls, input_value: datetime.date) -> SomeClass:
         """
-        Initialise from date
+        Initialize from date
 
         :param input_value: Input
         :return: result
         """
         return cls(input_value)
 
     @classmethod
-    def from_time(cls, input_value: datetime.time) -> SomeClass:  # noqa: ANN102
+    def from_time(cls, input_value: datetime.time) -> SomeClass:
         """
-        Initialise from time
+        Initialize from time
 
         :param input_value: Input
         :return: result
         """
         return cls(input_value)
 
-    def calculate_thing(self, number: float) -> datetime.timedelta:
+    def calculate_thing(self, number: float) -> datetime.timedelta:  # noqa: PLR6301
         """
         Calculate a thing
 
         :param number: Input
         :return: result
         """
         return datetime.timedelta(number)
```

### Comparing `sphinx_autodoc_typehints-2.0.0/LICENSE` & `sphinx_autodoc_typehints-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_autodoc_typehints-2.0.0/README.md` & `sphinx_autodoc_typehints-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
 The following configuration options are accepted:
 
 - `typehints_fully_qualified` (default: `False`): if `True`, class names are always fully qualified (e.g.
   `module.for.Class`). If `False`, just the class name displays (e.g. `Class`)
 - `always_document_param_types` (default: `False`): If `False`, do not add type info for undocumented parameters. If
   `True`, add stub documentation for undocumented parameters to be able to add type info.
+- `always_use_bars_union ` (default: `False`): If `True`, display Union's using the | operator described in PEP 604.
+   (e.g `X` | `Y` or `int` | `None`). If `False`, Unions will display with the typing in brackets. (e.g. `Union[X, Y]`
+   or `Optional[int]`)
 - `typehints_document_rtype` (default: `True`): If `False`, never add an `:rtype:` directive. If `True`, add the
   `:rtype:` directive if no existing `:rtype:` is found.
 - `typehints_use_rtype` (default: `True`): Controls behavior when `typehints_document_rtype` is set to `True`. If
   `True`, document return type in the `:rtype:` directive. If `False`, document return type as part of the `:return:`
   directive, if present, otherwise fall back to using `:rtype:`. Use in conjunction with
   [napoleon_use_rtype](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#confval-napoleon_use_rtype)
   to avoid generation of duplicate or redundant return type information.
```

### Comparing `sphinx_autodoc_typehints-2.0.0/pyproject.toml` & `sphinx_autodoc_typehints-2.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.4",
-  "hatchling>=1.18",
+  "hatchling>=1.21.1",
 ]
 
 [project]
 name = "sphinx-autodoc-typehints"
 description = "Type hints (PEP 484) support for the Sphinx autodoc extension"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -37,73 +37,97 @@
 dynamic = [
   "version",
 ]
 dependencies = [
   "Sphinx>=7.1.2",
 ]
 optional-dependencies.docs = [
-  "furo>=2023.9.10",
+  "furo>=2024.1.29",
 ]
 optional-dependencies.numpy = [
   "nptyping>=2.5",
 ]
 optional-dependencies.testing = [
   "covdefaults>=2.3",
-  "coverage>=7.3.2",
-  "diff-cover>=8.0.1",
-  "pytest>=7.4.3",
+  "coverage>=7.4.2",
+  "diff-cover>=8.0.3",
+  "pytest>=8.0.1",
   "pytest-cov>=4.1",
   "sphobjinv>=2.3.1",
-  "typing-extensions>=4.8",
+  "typing-extensions>=4.9",
 ]
 urls.Changelog = "https://github.com/tox-dev/sphinx-autodoc-typehints/blob/main/CHANGELOG.md"
 urls.Homepage = "https://github.com/tox-dev/sphinx-autodoc-typehints"
 urls.Source = "https://github.com/tox-dev/sphinx-autodoc-typehints"
 urls.Tracker = "https://github.com/tox-dev/sphinx-autodoc-typehints/issues"
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/sphinx_autodoc_typehints/version.py"
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
-select = ["ALL"]
 line-length = 120
-target-version = "py37"
-isort = {known-first-party = ["tox", "tests"], required-imports = ["from __future__ import annotations"]}
-ignore = [
-  "ANN101",  # no typoe annotation for self
-  "ANN401",  # allow Any as type annotation
-  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
-  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
-  "S104",  # Possible binding to all interface
-]
-[tool.ruff.per-file-ignores]
+target-version = "py38"
+lint.select = ["ALL"]
+lint.isort = { known-first-party = [
+  "sphinx_autodoc_typehints",
+  "tests",
+], required-imports = [
+  "from __future__ import annotations",
+] }
+lint.ignore = [
+  "ANN101", # no type annotation for self
+  "ANN401", # allow Any as type annotation
+  "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",   # Possible binding to all interface
+  "COM812", # Conflict with formatter
+  "ISC001", # Conflict with formatter
+  "CPY",    # No copyright statements
+]
+lint.preview = true
+format.preview = true
+format.docstring-code-format = true
+format.docstring-code-line-length = 100
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
-  "S101",  # asserts allowed in tests...
-  "FBT",  # don"t care about booleans as positional arguments in tests
-  "INP001", # no implicit namespace
-  "D",  # don"t care about documentation in tests
-  "S603",  # `subprocess` call: check for execution of untrusted input
-  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
-]
+  "S101",    # asserts allowed in tests...
+  "FBT",     # don"t care about booleans as positional arguments in tests
+  "INP001",  # no implicit namespace
+  "D",       # don't care about documentation in tests
+  "S603",    # `subprocess` call: check for execution of untrusted input
+  "PLR2004", # Magic value used in comparison, consider replacing with a constant variable
+  "PLR0913", # any number of arguments in tests
+  "PLR0917", # any number of arguments in tests
+  "PLC2701", # private imports
+]
+
+[tool.codespell]
+builtin = "clear,usage,en-GB_to_en-US"
+ignore-words = "ignore-words.txt"
+write-changes = true
+count = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
   "src",
-  ".tox*/*/lib/python*/site-packages",
-  ".tox*/pypy*/site-packages",
-  ".tox*\\*\\Lib\\site-packages",
+  ".tox/*/lib/python*/site-packages",
+  ".tox/pypy*/site-packages",
+  ".tox\\*\\Lib\\site-packages",
+  ".tox/*/.venv/lib/python*/site-packages",
+  ".tox/pypy*/.venv/site-packages",
+  ".tox\\*\\.venv\\Lib\\site-packages",
   "*/src",
   "*\\src",
 ]
 report.fail_under = 85
 report.omit = []
 run.parallel = true
 run.plugins = ["covdefaults"]
```

### Comparing `sphinx_autodoc_typehints-2.0.0/PKG-INFO` & `sphinx_autodoc_typehints-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sphinx-autodoc-typehints
-Version: 2.0.0
+Version: 2.0.1
 Summary: Type hints (PEP 484) support for the Sphinx autodoc extension
 Project-URL: Changelog, https://github.com/tox-dev/sphinx-autodoc-typehints/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/tox-dev/sphinx-autodoc-typehints
 Project-URL: Source, https://github.com/tox-dev/sphinx-autodoc-typehints
 Project-URL: Tracker, https://github.com/tox-dev/sphinx-autodoc-typehints/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -22,25 +22,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.8
 Requires-Dist: sphinx>=7.1.2
 Provides-Extra: docs
-Requires-Dist: furo>=2023.9.10; extra == 'docs'
+Requires-Dist: furo>=2024.1.29; extra == 'docs'
 Provides-Extra: numpy
 Requires-Dist: nptyping>=2.5; extra == 'numpy'
 Provides-Extra: testing
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
-Requires-Dist: coverage>=7.3.2; extra == 'testing'
-Requires-Dist: diff-cover>=8.0.1; extra == 'testing'
+Requires-Dist: coverage>=7.4.2; extra == 'testing'
+Requires-Dist: diff-cover>=8.0.3; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
-Requires-Dist: pytest>=7.4.3; extra == 'testing'
+Requires-Dist: pytest>=8.0.1; extra == 'testing'
 Requires-Dist: sphobjinv>=2.3.1; extra == 'testing'
-Requires-Dist: typing-extensions>=4.8; extra == 'testing'
+Requires-Dist: typing-extensions>=4.9; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # sphinx-autodoc-typehints
 
 [![PyPI](https://img.shields.io/pypi/v/sphinx-autodoc-typehints?style=flat-square)](https://pypi.org/project/sphinx-autodoc-typehints/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/sphinx-autodoc-typehints.svg)](https://pypi.org/project/sphinx-autodoc-typehints/)
@@ -99,14 +99,17 @@
 
 The following configuration options are accepted:
 
 - `typehints_fully_qualified` (default: `False`): if `True`, class names are always fully qualified (e.g.
   `module.for.Class`). If `False`, just the class name displays (e.g. `Class`)
 - `always_document_param_types` (default: `False`): If `False`, do not add type info for undocumented parameters. If
   `True`, add stub documentation for undocumented parameters to be able to add type info.
+- `always_use_bars_union ` (default: `False`): If `True`, display Union's using the | operator described in PEP 604.
+   (e.g `X` | `Y` or `int` | `None`). If `False`, Unions will display with the typing in brackets. (e.g. `Union[X, Y]`
+   or `Optional[int]`)
 - `typehints_document_rtype` (default: `True`): If `False`, never add an `:rtype:` directive. If `True`, add the
   `:rtype:` directive if no existing `:rtype:` is found.
 - `typehints_use_rtype` (default: `True`): Controls behavior when `typehints_document_rtype` is set to `True`. If
   `True`, document return type in the `:rtype:` directive. If `False`, document return type as part of the `:return:`
   directive, if present, otherwise fall back to using `:rtype:`. Use in conjunction with
   [napoleon_use_rtype](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#confval-napoleon_use_rtype)
   to avoid generation of duplicate or redundant return type information.
```

