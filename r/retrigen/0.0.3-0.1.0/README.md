# Comparing `tmp/retrigen-0.0.3.tar.gz` & `tmp/retrigen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrigen-0.0.3.tar", last modified: Wed Apr 10 12:44:37 2024, max compression
+gzip compressed data, was "retrigen-0.1.0.tar", last modified: Wed Apr 10 13:08:52 2024, max compression
```

## Comparing `retrigen-0.0.3.tar` & `retrigen-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.548811 retrigen-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-10 12:44:33.000000 retrigen-0.0.3/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      659 2024-04-10 12:44:33.000000 retrigen-0.0.3/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.540811 retrigen-0.0.3/.github/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      505 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/lint.yml
--rw-r--r--   0 root         (0) root         (0)     1957 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1165 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     1836 2024-04-10 12:44:33.000000 retrigen-0.0.3/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-10 12:44:33.000000 retrigen-0.0.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-10 12:44:33.000000 retrigen-0.0.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2024-04-10 12:44:33.000000 retrigen-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2251 2024-04-10 12:44:33.000000 retrigen-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-10 12:44:33.000000 retrigen-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-10 12:44:37.548811 retrigen-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3031 2024-04-10 12:44:33.000000 retrigen-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   124305 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/_static/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/docs/api/
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/api/docs_example.md
--rw-r--r--   0 root         (0) root         (0)     1538 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/faq.md
--rw-r--r--   0 root         (0) root         (0)     1799 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-10 12:44:33.000000 retrigen-0.0.3/docs/tutorials/usage.ipynb
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-10 12:44:33.000000 retrigen-0.0.3/makefile
--rw-r--r--   0 root         (0) root         (0)     1510 2024-04-10 12:44:33.000000 retrigen-0.0.3/mkdocs.yml
--rw-r--r--   0 root         (0) root         (0)     2863 2024-04-10 12:44:34.000000 retrigen-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 12:44:37.548811 retrigen-0.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.540811 retrigen-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/src/retrigen/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:44:33.000000 retrigen-0.0.3/src/retrigen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-04-10 12:44:33.000000 retrigen-0.0.3/src/retrigen/docs_example.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 12:44:33.000000 retrigen-0.0.3/src/retrigen/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.548811 retrigen-0.0.3/src/retrigen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-10 12:44:37.000000 retrigen-0.0.3/src/retrigen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2024-04-10 12:44:37.000000 retrigen-0.0.3/src/retrigen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:44:37.000000 retrigen-0.0.3/src/retrigen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      238 2024-04-10 12:44:37.000000 retrigen-0.0.3/src/retrigen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 12:44:37.000000 retrigen-0.0.3/src/retrigen.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:44:37.544811 retrigen-0.0.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 12:44:33.000000 retrigen-0.0.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-10 12:44:33.000000 retrigen-0.0.3/tests/first_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.919617 retrigen-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-10 13:08:48.000000 retrigen-0.1.0/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      659 2024-04-10 13:08:48.000000 retrigen-0.1.0/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.911617 retrigen-0.1.0/.github/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.911617 retrigen-0.1.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      505 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)     1836 2024-04-10 13:08:48.000000 retrigen-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-10 13:08:48.000000 retrigen-0.1.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-10 13:08:48.000000 retrigen-0.1.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-04-10 13:08:48.000000 retrigen-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-10 13:08:48.000000 retrigen-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-10 13:08:48.000000 retrigen-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5955 2024-04-10 13:08:52.919617 retrigen-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3031 2024-04-10 13:08:48.000000 retrigen-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.911617 retrigen-0.1.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   124305 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/_static/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/api/docs_example.md
+-rw-r--r--   0 root         (0) root         (0)     1538 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/faq.md
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    18504 2024-04-10 13:08:48.000000 retrigen-0.1.0/docs/tutorials/usage.ipynb
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-10 13:08:48.000000 retrigen-0.1.0/makefile
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-10 13:08:48.000000 retrigen-0.1.0/mkdocs.yml
+-rw-r--r--   0 root         (0) root         (0)     2988 2024-04-10 13:08:49.000000 retrigen-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 13:08:52.919617 retrigen-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.907617 retrigen-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/src/retrigen/
+-rw-r--r--   0 root         (0) root         (0)    22200 2024-04-10 13:08:48.000000 retrigen-0.1.0/src/retrigen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/src/retrigen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5955 2024-04-10 13:08:52.000000 retrigen-0.1.0/src/retrigen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      721 2024-04-10 13:08:52.000000 retrigen-0.1.0/src/retrigen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:08:52.000000 retrigen-0.1.0/src/retrigen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-10 13:08:52.000000 retrigen-0.1.0/src/retrigen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 13:08:52.000000 retrigen-0.1.0/src/retrigen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:08:52.915617 retrigen-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:08:48.000000 retrigen-0.1.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-04-10 13:08:48.000000 retrigen-0.1.0/tests/test_text_filter.py
```

### Comparing `retrigen-0.0.3/.cruft.json` & `retrigen-0.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/.github/workflows/documentation.yml` & `retrigen-0.1.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/.github/workflows/release.yml` & `retrigen-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/.github/workflows/stalebot.yml` & `retrigen-0.1.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/.github/workflows/tests.yml` & `retrigen-0.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/CHANGELOG.md` & `retrigen-0.1.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.0.3 (2024-04-10)
+
+### Ci
+
+* ci: fix docs publishing ([`09da5c4`](https://github.com/KennethEnevoldsen/retrigen/commit/09da5c4765ab185ab80ecd241a8ad6e99d741cbe))
+
+### Fix
+
+* fix: testing publishing ci ([`7f72fad`](https://github.com/KennethEnevoldsen/retrigen/commit/7f72fad010abb30f836ceb2db74507f77b871c93))
+
+### Unknown
+
+* Merge branch &#39;main&#39; of https://github.com/KennethEnevoldsen/regen ([`151e34b`](https://github.com/KennethEnevoldsen/retrigen/commit/151e34b70c15ee04fb5c99943170b4b334c8f465))
+
+
 ## v0.0.2 (2024-04-10)
 
 ### Fix
 
 * fix: rename package ([`37a8811`](https://github.com/KennethEnevoldsen/retrigen/commit/37a8811ccf6e3a896a0f7bff502d3047a7621ad9))
 
 * fix: Updated package name ([`e3d9a82`](https://github.com/KennethEnevoldsen/retrigen/commit/e3d9a82625370353787bc9f50c9f91568b0a2eb7))
```

### Comparing `retrigen-0.0.3/CODE_OF_CONDUCT.md` & `retrigen-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/CONTRIBUTING.md` & `retrigen-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/LICENSE` & `retrigen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/PKG-INFO` & `retrigen-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: retrigen
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package for automatically generating datasets for training or evaluating retrieval models
+Author: Jesper Alkestrup
 Author-email: Kenneth Enevoldsen <Kenneth.enevoldsen@cas.au.dk>
 License: MIT License
         
         Copyright © 2024 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,14 +35,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai
+Requires-Dist: tqdm
+Requires-Dist: langchain
+Requires-Dist: textdescriptives
+Requires-Dist: spacy>3.6.0
+Requires-Dist: chromadb
 Provides-Extra: dev
 Requires-Dist: cruft>=2.0.0; extra == "dev"
 Requires-Dist: pyright>=1.1.338; extra == "dev"
 Requires-Dist: ruff>=0.3.0; extra == "dev"
 Requires-Dist: pyproject-parser[cli,readme]>=0.9.1; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: pytest>=7.1.3; extra == "tests"
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: retrigen Version: 0.0.3 Summary: A package for
+Metadata-Version: 2.1 Name: retrigen Version: 0.1.0 Summary: A package for
 automatically generating datasets for training or evaluating retrieval models
-Author-email: Kenneth Enevoldsen
+Author: Jesper Alkestrup Author-email: Kenneth Enevoldsen
 cas.au.dk> License: MIT License Copyright Â© 2024 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -20,15 +20,17 @@
 KennethEnevoldsen/retrigen Project-URL: documentation, https://
 KennethEnevoldsen.github.io/retrigen/ Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python ::
 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Provides-Extra: dev Requires-Dist: cruft>=2.0.0; extra == "dev"
+LICENSE Requires-Dist: openai Requires-Dist: tqdm Requires-Dist: langchain
+Requires-Dist: textdescriptives Requires-Dist: spacy>3.6.0 Requires-Dist:
+chromadb Provides-Extra: dev Requires-Dist: cruft>=2.0.0; extra == "dev"
 Requires-Dist: pyright>=1.1.338; extra == "dev" Requires-Dist: ruff>=0.3.0;
 extra == "dev" Requires-Dist: pyproject-parser[cli,readme]>=0.9.1; extra ==
 "dev" Provides-Extra: tests Requires-Dist: pytest>=7.1.3; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests" Requires-Dist: pytest-xdist;
 extra == "tests" Provides-Extra: docs Requires-Dist: mkdocs-jupyter==0.24.2;
 extra == "docs" Requires-Dist: mkdocs-material==9.1.21; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "docs" Requires-Dist:
```

### Comparing `retrigen-0.0.3/README.md` & `retrigen-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/docs/_static/favicon.ico` & `retrigen-0.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/docs/_static/icon.png` & `retrigen-0.1.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/docs/faq.md` & `retrigen-0.1.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/docs/index.md` & `retrigen-0.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/makefile` & `retrigen-0.1.0/makefile`

 * *Files identical despite different names*

### Comparing `retrigen-0.0.3/mkdocs.yml` & `retrigen-0.1.0/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -32,28 +32,29 @@
 markdown_extensions:
   - pymdownx.superfences
   - pymdownx.tabbed:
       alternate_style: true
   - toc:
       permalink: true
 
-copyright: Copyright &copy; 2024 Kenneth Enevoldsen
+copyright: Copyright &copy; 2024 Jesper Alkestrup
 
 nav:
   - Package:
       - Overview: index.md
       - Installation: installation.md
       - Tutorials:
           - tutorials/usage.ipynb
       - FAQ: faq.md
   - API References:
       - api/docs_example.md
 
 plugins:
-  - mkdocs-jupyter
+  - mkdocs-jupyter:
+      execute: False
   - search
   - mkdocstrings:
       handlers:
         python:
           paths: [src]
           type: python
           root_package: retrigen
```

### Comparing `retrigen-0.0.3/pyproject.toml` & `retrigen-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "retrigen"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
+  { name = "Jesper Alkestrup" },
   { name = "Kenneth Enevoldsen", email = "Kenneth.enevoldsen@cas.au.dk" },
 ]
 description = "A package for automatically generating datasets for training or evaluating retrieval models"
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.9"
-dependencies = []
+dependencies = [
+  "openai",
+  "tqdm",
+  "langchain",
+  "textdescriptives",
+  "spacy>3.6.0",
+  "chromadb",
+
+]
 [project.license]
 file = "LICENSE"
 name = "MIT"
 [project.optional-dependencies]
 dev = [
   "cruft>=2.0.0",
   "pyright>=1.1.338",
```

### Comparing `retrigen-0.0.3/src/retrigen.egg-info/PKG-INFO` & `retrigen-0.1.0/src/retrigen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: retrigen
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package for automatically generating datasets for training or evaluating retrieval models
+Author: Jesper Alkestrup
 Author-email: Kenneth Enevoldsen <Kenneth.enevoldsen@cas.au.dk>
 License: MIT License
         
         Copyright © 2024 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -34,14 +35,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai
+Requires-Dist: tqdm
+Requires-Dist: langchain
+Requires-Dist: textdescriptives
+Requires-Dist: spacy>3.6.0
+Requires-Dist: chromadb
 Provides-Extra: dev
 Requires-Dist: cruft>=2.0.0; extra == "dev"
 Requires-Dist: pyright>=1.1.338; extra == "dev"
 Requires-Dist: ruff>=0.3.0; extra == "dev"
 Requires-Dist: pyproject-parser[cli,readme]>=0.9.1; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: pytest>=7.1.3; extra == "tests"
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: retrigen Version: 0.0.3 Summary: A package for
+Metadata-Version: 2.1 Name: retrigen Version: 0.1.0 Summary: A package for
 automatically generating datasets for training or evaluating retrieval models
-Author-email: Kenneth Enevoldsen
+Author: Jesper Alkestrup Author-email: Kenneth Enevoldsen
 cas.au.dk> License: MIT License Copyright Â© 2024 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
@@ -20,15 +20,17 @@
 KennethEnevoldsen/retrigen Project-URL: documentation, https://
 KennethEnevoldsen.github.io/retrigen/ Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python ::
 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Provides-Extra: dev Requires-Dist: cruft>=2.0.0; extra == "dev"
+LICENSE Requires-Dist: openai Requires-Dist: tqdm Requires-Dist: langchain
+Requires-Dist: textdescriptives Requires-Dist: spacy>3.6.0 Requires-Dist:
+chromadb Provides-Extra: dev Requires-Dist: cruft>=2.0.0; extra == "dev"
 Requires-Dist: pyright>=1.1.338; extra == "dev" Requires-Dist: ruff>=0.3.0;
 extra == "dev" Requires-Dist: pyproject-parser[cli,readme]>=0.9.1; extra ==
 "dev" Provides-Extra: tests Requires-Dist: pytest>=7.1.3; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests" Requires-Dist: pytest-xdist;
 extra == "tests" Provides-Extra: docs Requires-Dist: mkdocs-jupyter==0.24.2;
 extra == "docs" Requires-Dist: mkdocs-material==9.1.21; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "docs" Requires-Dist:
```

### Comparing `retrigen-0.0.3/src/retrigen.egg-info/SOURCES.txt` & `retrigen-0.1.0/src/retrigen.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,26 +10,23 @@
 mkdocs.yml
 pyproject.toml
 .github/pull_request_template.md
 .github/workflows/documentation.yml
 .github/workflows/lint.yml
 .github/workflows/release.yml
 .github/workflows/stalebot.yml
-.github/workflows/static_type_checks.yml
 .github/workflows/tests.yml
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/_static/favicon.ico
 docs/_static/icon.png
 docs/api/docs_example.md
 docs/tutorials/usage.ipynb
 src/retrigen/__init__.py
-src/retrigen/docs_example.py
-src/retrigen/py.typed
 src/retrigen.egg-info/PKG-INFO
 src/retrigen.egg-info/SOURCES.txt
 src/retrigen.egg-info/dependency_links.txt
 src/retrigen.egg-info/requires.txt
 src/retrigen.egg-info/top_level.txt
 tests/__init__.py
-tests/first_test.py
+tests/test_text_filter.py
```

