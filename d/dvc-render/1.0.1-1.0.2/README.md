# Comparing `tmp/dvc-render-1.0.1.tar.gz` & `tmp/dvc-render-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-render-1.0.1.tar", last modified: Tue Jan 23 02:13:56 2024, max compression
+gzip compressed data, was "dvc-render-1.0.2.tar", last modified: Wed Apr 10 14:28:50 2024, max compression
```

## Comparing `dvc-render-1.0.1.tar` & `dvc-render-1.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.300300 dvc-render-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.292300 dvc-render-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.292300 dvc-render-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-01-23 02:13:38.000000 dvc-render-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-01-23 02:13:38.000000 dvc-render-1.0.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-01-23 02:13:38.000000 dvc-render-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-01-23 02:13:38.000000 dvc-render-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-23 02:13:56.300300 dvc-render-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-01-23 02:13:38.000000 dvc-render-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.292300 dvc-render-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.292300 dvc-render-1.0.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-01-23 02:13:38.000000 dvc-render-1.0.1/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-23 02:13:38.000000 dvc-render-1.0.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-23 02:13:38.000000 dvc-render-1.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-23 02:13:38.000000 dvc-render-1.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-23 02:13:38.000000 dvc-render-1.0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-01-23 02:13:38.000000 dvc-render-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 02:13:56.300300 dvc-render-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.292300 dvc-render-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.296300 dvc-render-1.0.1/src/dvc_render/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/vega.py
--rw-r--r--   0 runner    (1001) docker     (127)    25976 2024-01-23 02:13:38.000000 dvc-render-1.0.1/src/dvc_render/vega_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.296300 dvc-render-1.0.1/src/dvc_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-23 02:13:56.000000 dvc-render-1.0.1/src/dvc_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-23 02:13:56.000000 dvc-render-1.0.1/src/dvc_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 02:13:56.000000 dvc-render-1.0.1/src/dvc_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-23 02:13:56.000000 dvc-render-1.0.1/src/dvc_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-23 02:13:56.000000 dvc-render-1.0.1/src/dvc_render.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:56.296300 dvc-render-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    43609 2024-01-23 02:13:38.000000 dvc-render-1.0.1/tests/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.908561 dvc-render-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.900561 dvc-render-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.900561 dvc-render-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-10 14:28:33.000000 dvc-render-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-10 14:28:33.000000 dvc-render-1.0.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-10 14:28:33.000000 dvc-render-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-10 14:28:33.000000 dvc-render-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-10 14:28:50.908561 dvc-render-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-10 14:28:33.000000 dvc-render-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.900561 dvc-render-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.900561 dvc-render-1.0.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-10 14:28:33.000000 dvc-render-1.0.2/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 14:28:33.000000 dvc-render-1.0.2/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 14:28:33.000000 dvc-render-1.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-10 14:28:33.000000 dvc-render-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-10 14:28:33.000000 dvc-render-1.0.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-10 14:28:33.000000 dvc-render-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:28:50.908561 dvc-render-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.896561 dvc-render-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.904561 dvc-render-1.0.2/src/dvc_render/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15649 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/vega.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-04-10 14:28:33.000000 dvc-render-1.0.2/src/dvc_render/vega_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.904561 dvc-render-1.0.2/src/dvc_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-10 14:28:50.000000 dvc-render-1.0.2/src/dvc_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-10 14:28:50.000000 dvc-render-1.0.2/src/dvc_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:28:50.000000 dvc-render-1.0.2/src/dvc_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 14:28:50.000000 dvc-render-1.0.2/src/dvc_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 14:28:50.000000 dvc-render-1.0.2/src/dvc_render.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:50.904561 dvc-render-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43599 2024-04-10 14:28:33.000000 dvc-render-1.0.2/tests/test_vega.py
```

### Comparing `dvc-render-1.0.1/.cruft.json` & `dvc-render-1.0.2/.cruft.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'e4ec95f4cfd03d4af0a8604d462ee11d07d63b42'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "15ee26df315020399731c6291d61bef81a3fc5d3",
+    "commit": "e4ec95f4cfd03d4af0a8604d462ee11d07d63b42",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Iterative",
             "copyright_year": "2022",
             "development_status": "Development Status :: 4 - Beta",
             "docs": "True",
```

### Comparing `dvc-render-1.0.1/.github/workflows/docs.yml` & `dvc-render-1.0.2/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     steps:
       - name: Check out the repository
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Configure git
         run: |
           git config user.name 'github-actions[bot]'
           git config user.email 'github-actions[bot]@users.noreply.github.com'
```

### Comparing `dvc-render-1.0.1/.github/workflows/release.yml` & `dvc-render-1.0.2/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,29 @@
   release:
     environment: pypi
     permissions:
       contents: read
       id-token: write
     runs-on: ubuntu-latest
     steps:
-    - name: Check out the repository
-      uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
+      - name: Check out the repository
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
 
-    - name: Set up Python 3.10
-      uses: actions/setup-python@v3
-      with:
-        python-version: '3.10'
+      - name: Set up Python 3.10
+        uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
 
-    - name: Upgrade pip and nox
-      run: |
-        pip install --upgrade pip nox
-        pip --version
-        nox --version
+      - name: Upgrade pip and nox
+        run: |
+          pip install --upgrade pip nox
+          pip --version
+          nox --version
 
-    - name: Build package
-      run: nox -s build
+      - name: Build package
+        run: nox -s build
 
-    - name: Upload package
-      if: github.event_name == 'release'
-      uses: pypa/gh-action-pypi-publish@release/v1
+      - name: Upload package
+        if: github.event_name == 'release'
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `dvc-render-1.0.1/.github/workflows/tests.yml` & `dvc-render-1.0.2/.github/workflows/tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -17,42 +17,42 @@
   tests:
     timeout-minutes: 20
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-latest, macos-latest]
-        pyv: ['3.8', '3.9', '3.10', '3.11']
+        pyv: ['3.9', '3.10', '3.11', '3.12']
         include:
-        - {os: ubuntu-latest, pyv: 'pypy3.8'}
+          - {os: ubuntu-latest, pyv: 'pypy3.9'}
 
     steps:
-    - name: Check out the repository
-      uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
-
-    - name: Set up Python ${{ matrix.pyv }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.pyv }}
-
-    - name: Upgrade pip and nox
-      run: |
-        python -m pip install --upgrade pip nox
-        pip --version
-        nox --version
-
-    - name: Lint code and check dependencies
-      run: nox -s lint safety
-
-    - name: Run tests
-      run: nox -s tests-${{ matrix.nox_pyv || matrix.pyv }} -- --cov-report=xml
+      - name: Check out the repository
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+
+      - name: Set up Python ${{ matrix.pyv }}
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.pyv }}
+
+      - name: Upgrade pip and nox
+        run: |
+          python -m pip install --upgrade pip nox
+          pip --version
+          nox --version
+
+      - name: Lint code and check dependencies
+        run: nox -s lint safety
+
+      - name: Run tests
+        run: nox -s tests-${{ matrix.nox_pyv || matrix.pyv }} -- --cov-report=xml
 
-    - name: Upload coverage report
-      uses: codecov/codecov-action@v3.1.4
+      - name: Upload coverage report
+        uses: codecov/codecov-action@v4
 
-    - name: Build package
-      run: nox -s build
+      - name: Build package
+        run: nox -s build
 
-    - name: Build docs
-      run: nox -s docs
+      - name: Build docs
+        run: nox -s docs
```

### Comparing `dvc-render-1.0.1/.gitignore` & `dvc-render-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/.pre-commit-config.yaml` & `dvc-render-1.0.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-json
       - id: check-merge-conflict
         args: ['--assume-in-merge']
       - id: check-toml
       - id: check-yaml
-      - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.1.7'
+    rev: 'v0.3.5'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
+  - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+    rev: v2.13.0
+    hooks:
+      - id: pretty-format-toml
+        args: [--autofix, --no-sort]
+      - id: pretty-format-yaml
+        args: [--autofix, --indent, '2', '--offset', '2', --preserve-quotes]
```

### Comparing `dvc-render-1.0.1/CODE_OF_CONDUCT.rst` & `dvc-render-1.0.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/CONTRIBUTING.rst` & `dvc-render-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/LICENSE` & `dvc-render-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/PKG-INFO` & `dvc-render-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dvc Render
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvc-render/issues
 Project-URL: Source, https://github.com/iterative/dvc-render
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: table
 Requires-Dist: tabulate>=0.8.7; extra == "table"
 Requires-Dist: flatten_dict<1,>=0.4.1; extra == "table"
 Provides-Extra: markdown
 Requires-Dist: dvc-render[table]; extra == "markdown"
 Requires-Dist: matplotlib; extra == "markdown"
 Provides-Extra: docs
-Requires-Dist: mkdocs==1.5.2; extra == "docs"
-Requires-Dist: mkdocs-gen-files==0.5.0; extra == "docs"
-Requires-Dist: mkdocs-material==9.3.1; extra == "docs"
-Requires-Dist: mkdocs-section-index==0.3.6; extra == "docs"
-Requires-Dist: mkdocstrings-python==1.6.3; extra == "docs"
+Requires-Dist: mkdocs<2,>=1.5.2; extra == "docs"
+Requires-Dist: mkdocs-gen-files<1,>=0.5.0; extra == "docs"
+Requires-Dist: mkdocs-material<10,>=9.3.1; extra == "docs"
+Requires-Dist: mkdocs-section-index<1,>=0.3.6; extra == "docs"
+Requires-Dist: mkdocstrings-python<2,>=1.6.3; extra == "docs"
 Provides-Extra: tests
-Requires-Dist: dvc-render[table]; extra == "tests"
-Requires-Dist: dvc-render[markdown]; extra == "tests"
-Requires-Dist: pytest==7.2.0; extra == "tests"
-Requires-Dist: pytest-sugar==0.9.7; extra == "tests"
-Requires-Dist: pytest-cov==3.0.0; extra == "tests"
-Requires-Dist: pytest-mock==3.8.2; extra == "tests"
-Requires-Dist: mypy==1.2.0; extra == "tests"
+Requires-Dist: dvc-render[markdown,table]; extra == "tests"
+Requires-Dist: pytest<9,>=7; extra == "tests"
+Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
+Requires-Dist: pytest-sugar; extra == "tests"
+Requires-Dist: pytest-mock; extra == "tests"
 Provides-Extra: dev
-Requires-Dist: dvc-render[table]; extra == "dev"
-Requires-Dist: dvc-render[markdown]; extra == "dev"
-Requires-Dist: dvc-render[tests]; extra == "dev"
-Requires-Dist: dvc-render[docs]; extra == "dev"
+Requires-Dist: dvc-render[docs,tests]; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 
 dvc-render
 ==========
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
```

### Comparing `dvc-render-1.0.1/README.rst` & `dvc-render-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/docs/assets/logo.svg` & `dvc-render-1.0.2/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/docs/gen_ref_pages.py` & `dvc-render-1.0.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/noxfile.py` & `dvc-render-1.0.2/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Automation using nox."""
+
 import glob
 import os
 
 import nox
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.sessions = "lint", "tests"
@@ -11,15 +12,15 @@
 
 @nox.session
 def docs(session: nox.Session) -> None:
     session.install(".[docs]")
     session.run("mkdocs", "build")
 
 
-@nox.session(python=["3.8", "3.9", "3.10", "3.11", "pypy3.8", "pypy3.9"])
+@nox.session(python=["3.9", "3.10", "3.11", "3.12", "pypy3.9"])
 def tests(session: nox.Session) -> None:
     session.install(".[tests]")
     session.run(
         "pytest",
         "--cov",
         "--cov-config=pyproject.toml",
         *session.posargs,
```

### Comparing `dvc-render-1.0.1/pyproject.toml` & `dvc-render-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 [build-system]
 requires = ["setuptools>=48", "setuptools_scm[toml]>=6.3.1"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-
 [project]
 name = "dvc-render"
 description = "Dvc Render"
 readme = "README.rst"
 license = {text = "Apache-2.0"}
-authors = [{ name = "Iterative", email = "support@dvc.org" }]
+authors = [{name = "Iterative", email = "support@dvc.org"}]
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Development Status :: 4 - Beta",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Development Status :: 4 - Beta"
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dynamic = ["version"]
 dependencies = []
 
 [project.urls]
 Issues = "https://github.com/iterative/dvc-render/issues"
 Source = "https://github.com/iterative/dvc-render"
 
 [project.optional-dependencies]
 table = [
-    "tabulate>=0.8.7",
-    "flatten_dict<1,>=0.4.1",
+  "tabulate>=0.8.7",
+  "flatten_dict<1,>=0.4.1"
 ]
 markdown = [
-    "dvc-render[table]",
-    "matplotlib",
+  "dvc-render[table]",
+  "matplotlib"
 ]
 docs = [
-    "mkdocs==1.5.2",
-    "mkdocs-gen-files==0.5.0",
-    "mkdocs-material==9.3.1",
-    "mkdocs-section-index==0.3.6",
-    "mkdocstrings-python==1.6.3",
+  "mkdocs>=1.5.2,<2",
+  "mkdocs-gen-files>=0.5.0,<1",
+  "mkdocs-material>=9.3.1,<10",
+  "mkdocs-section-index>=0.3.6,<1",
+  "mkdocstrings-python>=1.6.3,<2"
 ]
 tests = [
-    "dvc-render[table]",
-    "dvc-render[markdown]",
-    "pytest==7.2.0",
-    "pytest-sugar==0.9.7",
-    "pytest-cov==3.0.0",
-    "pytest-mock==3.8.2",
-    "mypy==1.2.0",
+  "dvc-render[table,markdown]",
+  "pytest>=7,<9",
+  "pytest-cov>=4.1.0",
+  "pytest-sugar",
+  "pytest-mock"
 ]
 dev = [
-    "dvc-render[table]",
-    "dvc-render[markdown]",
-    "dvc-render[tests]",
-    "dvc-render[docs]",
+  "dvc-render[tests,docs]",
+  "mypy==1.9.0"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
 
+[tool.setuptools_scm]
+
 [tool.pytest.ini_options]
 addopts = "-ra"
 
 [tool.coverage.run]
 branch = true
 source = ["dvc_render", "tests"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
-    "pragma: no cover",
-    "if __name__ == .__main__.:",
-    "if typing.TYPE_CHECKING:",
-    "if TYPE_CHECKING:",
-    "raise NotImplementedError",
-    "raise AssertionError",
-    "@overload",
+  "pragma: no cover",
+  "if __name__ == .__main__.:",
+  "if typing.TYPE_CHECKING:",
+  "if TYPE_CHECKING:",
+  "raise NotImplementedError",
+  "raise AssertionError",
+  "@overload"
 ]
 
 [tool.mypy]
 # Error output
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
@@ -105,36 +101,75 @@
 ]
 ignore_missing_imports = true
 
 [tool.codespell]
 ignore-words-list = "fpr"
 
 [tool.ruff]
+output-format = "full"
+show-fixes = true
+
+[tool.ruff.lint]
 ignore = [
-    "S101", # assert
-    "PLR2004", # magic-value-comparison
-    "PLW2901", # redefined-loop-name
-    "ISC001", # single-line-implicit-string-concatenation
-    "SIM105", # suppressible-exception
-    "SIM108", # if-else-block-instead-of-if-exp
-    "D203", # one blank line before class
-    "D213", # multi-line-summary-second-line
-    "RUF012", # mutable class attributes
-    "PT007", # value types in pytest.mark.parametrize
+  "S101",  # assert
+  "PLR2004",  # magic-value-comparison
+  "PLW2901",  # redefined-loop-name
+  "ISC001",  # single-line-implicit-string-concatenation
+  "SIM105",  # suppressible-exception
+  "SIM108",  # if-else-block-instead-of-if-exp
+  "D203",  # one blank line before class
+  "D213",  # multi-line-summary-second-line
+  "RUF012",  # mutable class attributes
+  "PT007"  # value types in pytest.mark.parametrize
 ]
 select = [
-    "F", "E", "W", "C90", "I", "N", "UP", "YTT", "ASYNC", "S", "BLE", "B", "A", "C4", "T10",
-    "EXE", "ISC", "ICN", "G", "INP", "PIE", "T20", "PYI", "PT", "Q", "RSE", "RET",
-    "SLOT", "SIM", "TID", "TCH", "ARG", "PGH", "PLC", "PLE", "PLR", "PLW", "TRY",
-    "FLY", "PERF101", "RUF",
+  "F",
+  "E",
+  "W",
+  "C90",
+  "I",
+  "N",
+  "UP",
+  "YTT",
+  "ASYNC",
+  "S",
+  "BLE",
+  "B",
+  "A",
+  "C4",
+  "T10",
+  "EXE",
+  "ISC",
+  "ICN",
+  "G",
+  "INP",
+  "PIE",
+  "T20",
+  "PYI",
+  "PT",
+  "Q",
+  "RSE",
+  "RET",
+  "SLOT",
+  "SIM",
+  "TID",
+  "TCH",
+  "ARG",
+  "PGH",
+  "PLC",
+  "PLE",
+  "PLR",
+  "PLW",
+  "TRY",
+  "FLY",
+  "PERF101",
+  "RUF"
 ]
-show-source = true
-show-fixes = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "noxfile.py" = ["D", "PTH"]
 "tests/**" = ["S", "ARG001", "ARG002", "ANN"]
 "docs/**" = ["INP"]
 
 [tool.ruff.lint.flake8-type-checking]
 strict = true
```

### Comparing `dvc-render-1.0.1/src/dvc_render/base.py` & `dvc-render-1.0.2/src/dvc_render/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
+from collections.abc import Iterable
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, List, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 if TYPE_CHECKING:
     from os import PathLike
 
 StrPath = Union[str, "PathLike[str]"]
 
 
@@ -17,15 +18,15 @@
     </div>
     """
 
     EXTENSIONS: Iterable[str] = {}
 
     def __init__(
         self,
-        datapoints: Optional[List] = None,
+        datapoints: Optional[list] = None,
         name: Optional[str] = None,
         **properties,
     ):
         self.datapoints = datapoints or []
         self.name = name or ""
         self.properties = properties
```

### Comparing `dvc-render-1.0.1/src/dvc_render/html.py` & `dvc-render-1.0.2/src/dvc_render/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 from dvc_render.image import ImageRenderer
 
 from .exceptions import DvcRenderError
 
 if TYPE_CHECKING:
     from .base import Renderer, StrPath
@@ -46,15 +46,15 @@
         refresh_seconds: Optional[int] = None,
     ):
         template = template or PAGE_HTML
         if self.PLOTS_PLACEHOLDER_FORMAT_STR not in template:
             raise MissingPlaceholderError(self.PLOTS_PLACEHOLDER_FORMAT_STR)
 
         self.template = template
-        self.elements: List[str] = []
+        self.elements: list[str] = []
         self.scripts: str = ""
         self.refresh_tag = ""
         if refresh_seconds is not None:
             self.refresh_tag = self.REFRESH_TAG.format(refresh_seconds)
 
     def with_scripts(self, scripts: str) -> "HTML":
         "Extend scripts element."
@@ -95,15 +95,15 @@
         os.path.dirname(path),
         image_number,
         basename,
     )
 
 
 def render_html(
-    renderers: List["Renderer"],
+    renderers: list["Renderer"],
     output_file: "StrPath",
     html_template: Optional["StrPath"] = None,
     refresh_seconds: Optional[int] = None,
 ) -> "StrPath":
     "Use `renderers` to fill an HTML template and write to `output_file`."
     output_path = Path(output_file)
     output_path.parent.mkdir(exist_ok=True)
```

### Comparing `dvc-render-1.0.1/src/dvc_render/image.py` & `dvc-render-1.0.2/src/dvc_render/image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/src/dvc_render/markdown.py` & `dvc-render-1.0.2/src/dvc_render/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 from .exceptions import MissingPlaceholderError
 
 if TYPE_CHECKING:
     from .base import Renderer, StrPath
 
 
@@ -23,15 +23,15 @@
         template = template or PAGE_MARKDOWN
         if self.RENDERERS_PLACEHOLDER_FORMAT_STR not in template:
             raise MissingPlaceholderError(
                 self.RENDERERS_PLACEHOLDER_FORMAT_STR, "Markdown"
             )
 
         self.template = template
-        self.elements: List[str] = []
+        self.elements: list[str] = []
 
     def with_element(self, md: str) -> "Markdown":
         "Adds custom markdown element."
         self.elements.append(md)
         return self
 
     def embed(self) -> str:
@@ -41,15 +41,15 @@
         }
         for placeholder, value in kwargs.items():
             self.template = self.template.replace("{" + placeholder + "}", value)
         return self.template
 
 
 def render_markdown(
-    renderers: List["Renderer"],
+    renderers: list["Renderer"],
     output_file: Optional["StrPath"] = None,
     template_path: Optional["StrPath"] = None,
 ) -> "StrPath":
     "User renderers to fill an Markdown template and write to path."
     output_path = None
     if output_file:
         output_path = Path(output_file)
```

### Comparing `dvc-render-1.0.1/src/dvc_render/plotly.py` & `dvc-render-1.0.2/src/dvc_render/plotly.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from .base import Renderer
 from .utils import list_dict_to_dict_list
 
 
 class ParallelCoordinatesRenderer(Renderer):
     """
@@ -44,15 +44,15 @@
 
     def partial_html(self, **kwargs) -> str:  # noqa: ARG002
         return json.dumps(self._get_plotly_data())
 
     def _get_plotly_data(self):
         tabular_dict = list_dict_to_dict_list(self.datapoints)
 
-        trace: Dict[str, Any] = {"type": "parcoords", "dimensions": []}
+        trace: dict[str, Any] = {"type": "parcoords", "dimensions": []}
         for label, values in tabular_dict.items():
             values = list(map(str, values))
             is_categorical = False
             try:
                 float_values = [
                     float(x) if x != self.fill_value else None for x in values
                 ]
```

### Comparing `dvc-render-1.0.1/src/dvc_render/table.py` & `dvc-render-1.0.2/src/dvc_render/table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/src/dvc_render/vega.py` & `dvc-render-1.0.2/src/dvc_render/vega.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import io
 import json
 from collections import defaultdict
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Optional, Union
 from warnings import warn
 
 from .base import Renderer
 from .utils import list_dict_to_dict_list
 from .vega_templates import BadTemplateError, LinearTemplate, Template, get_template
 
 FIELD_SEPARATOR = "::"
@@ -41,15 +41,15 @@
     "plot_width",
     "row",
     "shape",
     "stroke_dash",
     "tooltip",
     "zoom_and_pan",
 ]
-OPTIONAL_ANCHOR_RANGES: Dict[str, Union[List[str], List[List[int]]]] = {
+OPTIONAL_ANCHOR_RANGES: dict[str, Union[list[str], list[list[int]]]] = {
     "stroke_dash": [[1, 0], [8, 8], [8, 4], [4, 4], [4, 2], [2, 1], [1, 1]],
     "color": [
         "#945dd6",
         "#13adc7",
         "#f46837",
         "#48bb78",
         "#4299e1",
@@ -78,28 +78,28 @@
     <script src="https://cdn.jsdelivr.net/npm/vega@5.20.2"></script>
     <script src="https://cdn.jsdelivr.net/npm/vega-lite@5.2.0"></script>
     <script src="https://cdn.jsdelivr.net/npm/vega-embed@6.18.2"></script>
     """
 
     EXTENSIONS = {".yml", ".yaml", ".json", ".csv", ".tsv"}
 
-    def __init__(self, datapoints: List, name: str, **properties):
+    def __init__(self, datapoints: list, name: str, **properties):
         super().__init__(datapoints, name, **properties)
         self.template = get_template(
             self.properties.get("template", None),
             self.properties.get("template_dir", None),
         )
 
-        self._split_content: Dict[str, str] = {}
+        self._split_content: dict[str, str] = {}
 
     def get_filled_template(  # noqa: C901
         self,
-        split_anchors: Optional[List[str]] = None,
+        split_anchors: Optional[list[str]] = None,
         strict: bool = True,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Returns a functional vega specification"""
         self.template.reset()
         if not self.datapoints:
             return {}
 
         if split_anchors is None:
             split_anchors = []
@@ -220,15 +220,15 @@
         revs = []
         for datapoint in self.datapoints:
             rev = datapoint.get("rev")
             if rev and rev not in revs:
                 revs.append(rev)
         return revs
 
-    def _process_optional_anchors(self, split_anchors: List[str]):
+    def _process_optional_anchors(self, split_anchors: list[str]):
         optional_anchors = [
             anchor for anchor in OPTIONAL_ANCHORS if self.template.has_anchor(anchor)
         ]
         if not optional_anchors:
             return None
 
         self._fill_color(split_anchors, optional_anchors)
@@ -241,59 +241,59 @@
             self._process_single_source_plot(split_anchors, optional_anchors)
             return []
 
         return self._process_multi_source_plot(
             split_anchors, optional_anchors, y_definitions
         )
 
-    def _fill_color(self, split_anchors: List[str], optional_anchors: List[str]):
+    def _fill_color(self, split_anchors: list[str], optional_anchors: list[str]):
         all_revs = self.get_revs()
         self._fill_optional_anchor_mapping(
             split_anchors,
             optional_anchors,
             REV,
             "color",
             all_revs,
         )
 
-    def _fill_set_encoding(self, split_anchors: List[str], optional_anchors: List[str]):
+    def _fill_set_encoding(self, split_anchors: list[str], optional_anchors: list[str]):
         for name, encoding in [
             ("zoom_and_pan", {"name": "grid", "select": "interval", "bind": "scales"}),
             ("plot_height", 300),
             ("plot_width", 300),
         ]:
             self._fill_optional_anchor(split_anchors, optional_anchors, name, encoding)
 
     def _process_single_source_plot(
-        self, split_anchors: List[str], optional_anchors: List[str]
+        self, split_anchors: list[str], optional_anchors: list[str]
     ):
         self._fill_group_by(split_anchors, optional_anchors, [REV])
         self._fill_optional_anchor(
             split_anchors, optional_anchors, "pivot_field", "datum.rev"
         )
         self._fill_tooltip(split_anchors, optional_anchors)
         for anchor in optional_anchors:
             self.template.fill_anchor(anchor, {})
 
     def _process_multi_source_plot(
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
-        y_definitions: List[Dict[str, str]],
+        split_anchors: list[str],
+        optional_anchors: list[str],
+        y_definitions: list[dict[str, str]],
     ):
         varied_keys, domain = self._collect_variations(y_definitions)
 
         self._fill_optional_multi_source_anchors(
             split_anchors, optional_anchors, varied_keys, domain
         )
         return varied_keys
 
     def _collect_variations(
-        self, y_definitions: List[Dict[str, str]]
-    ) -> Tuple[List[str], List[str]]:
+        self, y_definitions: list[dict[str, str]]
+    ) -> tuple[list[str], list[str]]:
         varied_values = defaultdict(set)
         for defn in y_definitions:
             for key in FILENAME_FIELD:
                 varied_values[key].add(defn.get(key, None))
             varied_values[CONCAT_FIELDS].add(
                 FIELD_SEPARATOR.join([defn.get(FILENAME, ""), defn.get(FIELD, "")])
             )
@@ -309,18 +309,18 @@
 
         domain = self._get_domain(varied_keys, varied_values)
 
         return varied_keys, domain
 
     def _fill_optional_multi_source_anchors(
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
-        varied_keys: List[str],
-        domain: List[str],
+        split_anchors: list[str],
+        optional_anchors: list[str],
+        varied_keys: list[str],
+        domain: list[str],
     ):
         if not optional_anchors:
             return
 
         concat_field = FIELD_SEPARATOR.join(varied_keys)
         self._fill_group_by(split_anchors, optional_anchors, [REV, concat_field])
 
@@ -348,17 +348,17 @@
         for anchor in ["stroke_dash", "shape"]:
             self._fill_optional_anchor_mapping(
                 split_anchors, optional_anchors, concat_field, anchor, domain
             )
 
     def _fill_group_by(
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
-        group_by: List[str],
+        split_anchors: list[str],
+        optional_anchors: list[str],
+        group_by: list[str],
     ):
         self._fill_optional_anchor(
             split_anchors, optional_anchors, "group_by", group_by
         )
         self._fill_optional_anchor(
             split_anchors,
             optional_anchors,
@@ -370,17 +370,17 @@
             optional_anchors,
             "group_by_y",
             [*group_by, self.properties.get("y")],
         )
 
     def _fill_tooltip(
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
-        additional_fields: Optional[List[str]] = None,
+        split_anchors: list[str],
+        optional_anchors: list[str],
+        additional_fields: Optional[list[str]] = None,
     ):
         if not additional_fields:
             additional_fields = []
         self._fill_optional_anchor(
             split_anchors,
             optional_anchors,
             "tooltip",
@@ -390,47 +390,47 @@
                 {"field": self.properties.get("y")},
                 *[{"field": field} for field in additional_fields],
             ],
         )
 
     def _fill_optional_anchor(
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
+        split_anchors: list[str],
+        optional_anchors: list[str],
         name: str,
         value: Any,
     ):
         if name not in optional_anchors:
             return
 
         optional_anchors.remove(name)
 
         if name in split_anchors:
             self._set_split_content(name, value)
             return
 
         self.template.fill_anchor(name, value)
 
-    def _get_domain(self, varied_keys: List[str], varied_values: Dict[str, set]):
+    def _get_domain(self, varied_keys: list[str], varied_values: dict[str, set]):
         if len(varied_keys) == 2:
             domain = list(varied_values[CONCAT_FIELDS])
         else:
             filename_or_field = varied_keys[0]
             domain = list(varied_values[filename_or_field])
 
         domain.sort()
         return domain
 
     def _fill_optional_anchor_mapping(  # noqa: PLR0913
         self,
-        split_anchors: List[str],
-        optional_anchors: List[str],
+        split_anchors: list[str],
+        optional_anchors: list[str],
         field: str,
         name: str,
-        domain: List[str],
+        domain: list[str],
     ):  # pylint: disable=too-many-arguments
         if name not in optional_anchors:
             return
 
         optional_anchors.remove(name)
 
         encoding = self._get_optional_anchor_mapping(field, name, domain)
@@ -441,17 +441,17 @@
 
         self.template.fill_anchor(name, encoding)
 
     def _get_optional_anchor_mapping(
         self,
         field: str,
         name: str,
-        domain: List[str],
+        domain: list[str],
     ):
-        full_range_values: List[Any] = OPTIONAL_ANCHOR_RANGES.get(name, [])
+        full_range_values: list[Any] = OPTIONAL_ANCHOR_RANGES.get(name, [])
         anchor_range_values = full_range_values.copy()
 
         anchor_range = []
         for _ in range(len(domain)):
             if not anchor_range_values:
                 anchor_range_values = full_range_values.copy()
             range_value = anchor_range_values.pop(0)
@@ -466,15 +466,15 @@
 
         return {
             "field": field,
             "scale": {"domain": domain, "range": anchor_range},
             **legend,
         }
 
-    def _update_datapoints(self, varied_keys: Optional[List[str]] = None):
+    def _update_datapoints(self, varied_keys: Optional[list[str]] = None):
         if varied_keys is None:
             return
 
         if len(varied_keys) == 2:
             to_concatenate = varied_keys
             to_remove = varied_keys
         else:
```

### Comparing `dvc-render-1.0.1/src/dvc_render/vega_templates.py` & `dvc-render-1.0.2/src/dvc_render/vega_templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=missing-function-docstring
 import json
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from .exceptions import DvcRenderError
 
 if TYPE_CHECKING:
     from .base import StrPath
 
 
@@ -76,29 +76,29 @@
     return False
 
 
 class Template:
     EXTENSION = ".json"
     ANCHOR = "<DVC_METRIC_{}>"
 
-    DEFAULT_CONTENT: Dict[str, Any] = {}
+    DEFAULT_CONTENT: dict[str, Any] = {}
     DEFAULT_NAME: str = ""
 
     def __init__(
-        self, content: Optional[Dict[str, Any]] = None, name: Optional[str] = None
+        self, content: Optional[dict[str, Any]] = None, name: Optional[str] = None
     ):
         if (
             content
             and not isinstance(content, dict)
             or self.DEFAULT_CONTENT
             and not isinstance(self.DEFAULT_CONTENT, dict)
         ):
             raise BadTemplateError
         self._original_content = content or self.DEFAULT_CONTENT
-        self.content: Dict[str, Any] = self._original_content
+        self.content: dict[str, Any] = self._original_content
         self.name = name or self.DEFAULT_NAME
         self.filename = Path(self.name).with_suffix(self.EXTENSION)
 
     @classmethod
     def anchor(cls, name):
         "Get ANCHOR formatted with name."
         return cls.ANCHOR.format(name.upper())
@@ -131,15 +131,15 @@
 
 class BarHorizontalSortedTemplate(Template):
     DEFAULT_NAME = "bar_horizontal_sorted"
 
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "mark": {"type": "bar"},
         "params": [Template.anchor("zoom_and_pan")],
         "encoding": {
             "x": {
                 "field": Template.anchor("x"),
@@ -162,15 +162,15 @@
 
 class BarHorizontalTemplate(Template):
     DEFAULT_NAME = "bar_horizontal"
 
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "mark": {"type": "bar"},
         "params": [Template.anchor("zoom_and_pan")],
         "encoding": {
             "x": {
                 "field": Template.anchor("x"),
@@ -191,15 +191,15 @@
 
 
 class ConfusionTemplate(Template):
     DEFAULT_NAME = "confusion"
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "facet": {
             "column": {"field": "rev", "sort": []},
             "row": Template.anchor("row"),
         },
         "params": [
             {
                 "name": "showValues",
@@ -317,15 +317,15 @@
 
 
 class NormalizedConfusionTemplate(Template):
     DEFAULT_NAME = "confusion_normalized"
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "facet": {
             "column": {"field": "rev", "sort": []},
             "row": Template.anchor("row"),
         },
         "spec": {
             "transform": [
                 {
@@ -435,15 +435,15 @@
 
 class ScatterTemplate(Template):
     DEFAULT_NAME = "scatter"
 
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "mark": {"type": "point", "tooltip": {"content": "data"}},
         "params": [Template.anchor("zoom_and_pan")],
         "encoding": {
             "x": {
                 "field": Template.anchor("x"),
@@ -464,15 +464,15 @@
 
 class ScatterJitterTemplate(Template):
     DEFAULT_NAME = "scatter_jitter"
 
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "transform": [
             {"calculate": "random()", "as": "randomX"},
             {"calculate": "random()", "as": "randomY"},
         ],
         "mark": {"type": "point", "tooltip": {"content": "data"}},
@@ -495,15 +495,15 @@
 
 
 class SmoothLinearTemplate(Template):
     DEFAULT_NAME = "smooth"
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "params": [
             {
                 "name": "smooth",
                 "value": 0.001,
                 "bind": {
@@ -633,15 +633,15 @@
 
 class SimpleLinearTemplate(Template):
     DEFAULT_NAME = "simple"
 
     DEFAULT_CONTENT = {
         "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
         "data": {"values": Template.anchor("data")},
-        "title": Template.anchor("title"),
+        "title": {"text": Template.anchor("title"), "anchor": "middle"},
         "params": [Template.anchor("zoom_and_pan")],
         "width": Template.anchor("plot_width"),
         "height": Template.anchor("plot_height"),
         "mark": {
             "type": "line",
             "tooltip": {"content": "data"},
         },
@@ -728,15 +728,15 @@
     for template_cls in TEMPLATES:
         if template == template_cls.DEFAULT_NAME:
             return template_cls()
 
     raise TemplateNotFoundError(template)
 
 
-def dump_templates(output: "StrPath", targets: Optional[List] = None) -> None:
+def dump_templates(output: "StrPath", targets: Optional[list] = None) -> None:
     "Write TEMPLATES in `.json` format to `output`."
     output = Path(output)
     output.mkdir(exist_ok=True)
 
     if targets:
         templates = [
             template for template in TEMPLATES if template.DEFAULT_NAME in targets
```

### Comparing `dvc-render-1.0.1/src/dvc_render.egg-info/PKG-INFO` & `dvc-render-1.0.2/src/dvc_render.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dvc Render
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvc-render/issues
 Project-URL: Source, https://github.com/iterative/dvc-render
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: table
 Requires-Dist: tabulate>=0.8.7; extra == "table"
 Requires-Dist: flatten_dict<1,>=0.4.1; extra == "table"
 Provides-Extra: markdown
 Requires-Dist: dvc-render[table]; extra == "markdown"
 Requires-Dist: matplotlib; extra == "markdown"
 Provides-Extra: docs
-Requires-Dist: mkdocs==1.5.2; extra == "docs"
-Requires-Dist: mkdocs-gen-files==0.5.0; extra == "docs"
-Requires-Dist: mkdocs-material==9.3.1; extra == "docs"
-Requires-Dist: mkdocs-section-index==0.3.6; extra == "docs"
-Requires-Dist: mkdocstrings-python==1.6.3; extra == "docs"
+Requires-Dist: mkdocs<2,>=1.5.2; extra == "docs"
+Requires-Dist: mkdocs-gen-files<1,>=0.5.0; extra == "docs"
+Requires-Dist: mkdocs-material<10,>=9.3.1; extra == "docs"
+Requires-Dist: mkdocs-section-index<1,>=0.3.6; extra == "docs"
+Requires-Dist: mkdocstrings-python<2,>=1.6.3; extra == "docs"
 Provides-Extra: tests
-Requires-Dist: dvc-render[table]; extra == "tests"
-Requires-Dist: dvc-render[markdown]; extra == "tests"
-Requires-Dist: pytest==7.2.0; extra == "tests"
-Requires-Dist: pytest-sugar==0.9.7; extra == "tests"
-Requires-Dist: pytest-cov==3.0.0; extra == "tests"
-Requires-Dist: pytest-mock==3.8.2; extra == "tests"
-Requires-Dist: mypy==1.2.0; extra == "tests"
+Requires-Dist: dvc-render[markdown,table]; extra == "tests"
+Requires-Dist: pytest<9,>=7; extra == "tests"
+Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
+Requires-Dist: pytest-sugar; extra == "tests"
+Requires-Dist: pytest-mock; extra == "tests"
 Provides-Extra: dev
-Requires-Dist: dvc-render[table]; extra == "dev"
-Requires-Dist: dvc-render[markdown]; extra == "dev"
-Requires-Dist: dvc-render[tests]; extra == "dev"
-Requires-Dist: dvc-render[docs]; extra == "dev"
+Requires-Dist: dvc-render[docs,tests]; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 
 dvc-render
 ==========
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
```

### Comparing `dvc-render-1.0.1/src/dvc_render.egg-info/SOURCES.txt` & `dvc-render-1.0.2/src/dvc_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_html.py` & `dvc-render-1.0.2/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_image.py` & `dvc-render-1.0.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_markdown.py` & `dvc-render-1.0.2/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_parallel_coordinates.py` & `dvc-render-1.0.2/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_table.py` & `dvc-render-1.0.2/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_templates.py` & `dvc-render-1.0.2/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-1.0.1/tests/test_vega.py` & `dvc-render-1.0.2/tests/test_vega.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import Any, Dict, List
+from typing import Any
 
 import pytest
 from dvc_render.vega import OPTIONAL_ANCHOR_RANGES, BadTemplateError, VegaRenderer
 from dvc_render.vega_templates import NoFieldInDataError, Template
 
 # pylint: disable=missing-function-docstring, C1803, C0302
 
@@ -1389,24 +1389,24 @@
     for anchor in split_anchors:
         assert anchor in content_str
     for key, value in split["anchor_definitions"].items():
         assert value == expected_split[key]
 
 
 def _get_expected_datapoints(
-    datapoints: List[Dict[str, Any]], expected_dp_keys: List[str]
+    datapoints: list[dict[str, Any]], expected_dp_keys: list[str]
 ):
-    expected_datapoints: List[Dict[str, Any]] = []
+    expected_datapoints: list[dict[str, Any]] = []
     for datapoint in datapoints:
         expected_datapoint = {}
         for key in expected_dp_keys:
             if key == "filename::field":
-                expected_datapoint[
-                    key
-                ] = f"{datapoint['filename']}::{datapoint['field']}"
+                expected_datapoint[key] = (
+                    f"{datapoint['filename']}::{datapoint['field']}"
+                )
             else:
                 value = datapoint.get(key)
                 if value is None:
                     continue
                 expected_datapoint[key] = value
         expected_datapoints.append(expected_datapoint)
```

