# Comparing `tmp/erdantic-1.0.0.post2.tar.gz` & `tmp/erdantic-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "erdantic-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `erdantic-1.0.0.post2.tar` & `erdantic-1.0.0rc1.tar`

### file list

```diff
@@ -1,110 +1,23 @@
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/CONTRIBUTING.md
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/HISTORY.md
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/Makefile
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/noxfile.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/.github/codecov.yml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/.github/workflows/docs-main.yml
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/.github/workflows/release.yml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/generate_images.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/generate_pydantic_with_default_column_diagram.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/hooks.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/mkdocs.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/changelog.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/cli.md
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/customizing.md
--rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/extending.md
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/forward-references.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/convenience.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/core.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/exceptions.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/typing_utils.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/examples/attrs.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/examples/dataclasses.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/examples/pydantic.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/examples/pydantic_v1.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/plugins/attrs.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/plugins/dataclasses.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/plugins/index.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/api-reference/plugins/pydantic.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/edge-many-unspecified.png
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/edge-many-zero.png
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/edge-one-one.png
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/edge-one-zero.png
--rw-r--r--   0        0        0    93950 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/erdantic_diagram.png
--rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/erdantic_diagram.svg
--rw-r--r--   0        0        0    46733 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/example_diagram.png
--rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/example_diagram.svg
--rw-r--r--   0        0        0    46156 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/assets/pydantic_with_default_column_diagram.png
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/docs/css/mkdocs-jupyter-extra.css
--rw-r--r--   0        0        0   295642 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/notebooks/attrs.ipynb
--rw-r--r--   0        0        0   295870 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/notebooks/dataclasses.ipynb
--rw-r--r--   0        0        0   292514 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/docs/notebooks/pydantic.ipynb
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/__main__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/_logging.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/_repr_utils.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/_version.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/convenience.py
--rw-r--r--   0        0        0    28058 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/core.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/py.typed
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/typing_utils.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/examples/__init__.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/examples/attrs.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/examples/dataclasses.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/examples/pydantic.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/examples/pydantic_v1.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/plugins/__init__.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/plugins/attrs.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/plugins/dataclasses.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/erdantic/plugins/pydantic.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/requirements/dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/requirements/docs.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/requirements/lint.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/requirements/tests.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/requirements/typecheck.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/conftest.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/pydantic_with_default_column.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_against_assets.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_attrs.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_cli.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_convenience.py
--rw-r--r--   0        0        0    14246 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_core.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_dataclasses.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_plugins.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_pydantic.py
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_pydantic_v1.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/test_typing_utils.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/typechecks.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/utils.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/attrs.dot
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/attrs.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/attrs.png
--rw-r--r--   0        0        0    13191 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/attrs.svg
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/dataclasses.dot
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/dataclasses.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/dataclasses.png
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/dataclasses.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic.dot
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic.png
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic.svg
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic_v1.dot
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic_v1.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic_v1.png
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/pydantic_v1.svg
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/test_core-test_subclass/pydantic_with_default_column.dot
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/test_core-test_subclass/pydantic_with_default_column.json
--rw-r--r--   0        0        0    46347 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/test_core-test_subclass/pydantic_with_default_column.png
--rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/assets/test_core-test_subclass/pydantic_with_default_column.svg
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/scripts/generate_pydantic_with_defaults_assets.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/tests/scripts/generate_static_assets.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/LICENSE
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/README.md
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/pyproject.toml
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 erdantic-1.0.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     4154 2024-03-31 00:41:27.886743 erdantic-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      426 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/__main__.py
+-rw-r--r--   0        0        0      112 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_logging.py
+-rw-r--r--   0        0        0     2656 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_repr_utils.py
+-rw-r--r--   0        0        0       80 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/_version.py
+-rw-r--r--   0        0        0     7502 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/cli.py
+-rw-r--r--   0        0        0     8420 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/convenience.py
+-rw-r--r--   0        0        0    28058 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/core.py
+-rw-r--r--   0        0        0      189 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2302 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/attrs.py
+-rw-r--r--   0        0        0     2330 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2251 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     2307 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py
+-rw-r--r--   0        0        0     5000 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/exceptions.py
+-rw-r--r--   0        0        0     3446 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/__init__.py
+-rw-r--r--   0        0        0     2184 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/attrs.py
+-rw-r--r--   0        0        0     3847 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/dataclasses.py
+-rw-r--r--   0        0        0     4797 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/plugins/pydantic.py
+-rw-r--r--   0        0        0        0 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/py.typed
+-rw-r--r--   0        0        0     3526 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/erdantic/typing_utils.py
+-rw-r--r--   0        0        0     2123 2024-03-31 00:41:27.894743 erdantic-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 erdantic-1.0.0rc1/PKG-INFO
```

### Comparing `erdantic-1.0.0.post2/docs/docs/customizing.md` & `erdantic-1.0.0rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,110 @@
-# Customizing diagrams
+Metadata-Version: 2.1
+Name: erdantic
+Version: 1.0.0rc1
+Summary: Entity relationship diagrams for Python data model classes like Pydantic.
+Keywords: erd,entity relationship diagram,dataclasses,pydantic,attrs
+Author: Jay Qi
+Author-email: DrivenData <info@drivendata.org>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
+Requires-Dist: pydantic >= 2
+Requires-Dist: pydantic-core
+Requires-Dist: pygraphviz
+Requires-Dist: sortedcontainers-pydantic
+Requires-Dist: typenames
+Requires-Dist: typer
+Requires-Dist: attrs ; extra == "attrs"
+Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
+Project-URL: Changelog, https://erdantic.drivendata.org/stable/changelog/
+Project-URL: Documentation, https://erdantic.drivendata.org/
+Project-URL: Repository, https://github.com/drivendataorg/erdantic
+Provides-Extra: attrs
+
+# erdantic: Entity Relationship Diagrams
+
+[![Docs Status](https://img.shields.io/badge/docs-stable-informational)](https://erdantic.drivendata.org/)
+[![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
+[![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
+[![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
+[![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
+
+> [!NOTE]
+> erdantic v1.0 is coming soon and involves big backend changes. See the [changelog](./HISTORY.md) for more information.
+
+**erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
+
+- [Pydantic V2](https://docs.pydantic.dev/latest/)
+- [Pydantic V1 legacy](https://docs.pydantic.dev/latest/migration/#continue-using-pydantic-v1-features)
+- [attrs](https://www.attrs.org/en/stable/)
+- [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
+
+You can use erdantic either as a convenient CLI or as a Python library. Great for adding a simple and clean data model reference to your documentation.
+
+<object type="image/svg+xml" data="./docs/docs/assets/example_diagram.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="./docs/docs/assets/example_diagram.svg"></object>
+
+## Installation
+
+erdantic's graph modeling depends on [pygraphviz](https://pygraphviz.github.io/documentation/stable/index.html) and [Graphviz](https://graphviz.org/), an open-source C library. If you are on Linux or macOS, the easiest way to install everything together is to use conda and conda-forge:
+
+```bash
+conda install erdantic -c conda-forge
+```
+
+If not using conda, Graphviz must be installed first (before you can install pygraphviz). For recommended options and installation troubleshooting, see the [pygraphviz docs](https://pygraphviz.github.io/documentation/stable/install.html). Then to install erdantic and its Python dependencies from PyPI:
+
+```bash
+pip install erdantic
+```
+
+### Development version
+
+You can get the development version from GitHub with:
+
+```bash
+pip install git+https://github.com/drivendataorg/erdantic.git#egg=erdantic
+```
+
+## Quick usage
+
+First, make sure that the data model classes that you want to include in your diagram are importable. This means the code with your models should either be available on your [`sys.path`](https://docs.python.org/3/library/sys_path_init.html) or installed into the same virtual environment as erdantic.
+
+The fastest way to produce a diagram like the above example is to use the erdantic CLI. Simply specify the full dotted import path to your model and an output file path. The rendered format is interpreted from the filename extension.
+
+```bash
+erdantic erdantic.examples.pydantic.Party -o diagram.png
+```
+
+You can also import the erdantic Python library. This lets you inspect the diagram data and potentially modify it. You will have greater ability to customize the diagram in Python.
+
+```python
+import erdantic as erd
+from erdantic.examples.pydantic import Party
+
+# Easy one-liner
+erd.draw(Party, out="diagram.png")
+
+# Or create a diagram object that you can inspect and do stuff with
+diagram = erd.create(Party)
+list(diagram.models.keys())
+#> [ 'erdantic.examples.pydantic.Adventurer',
+#>   'erdantic.examples.pydantic.Party',
+#>   'erdantic.examples.pydantic.Quest',
+#>   'erdantic.examples.pydantic.QuestGiver']
+diagram.draw("diagram.png")
+```
 
-!!! note
+Check out the "Usage Examples" section of our [docs](https://erdantic.drivendata.org/) to see more.
 
-    Major changes were made to the backend in v1.0 to support the customization capabilities described on this page.
-
-## Customizing graph appearance
-
-erdantic uses the [Graphviz](https://graphviz.org/) program for laying out and rendering the diagram via the [PyGraphviz](https://pygraphviz.github.io/documentation/stable/index.html) package. When calling the [`draw`][erdantic.convenience.draw] function, you have the ability to pass in overrides for Graphviz graph, node, and edge attributes with the following keyword arguments:
-
-- `graph_attr: dict[str, Any]` — key-value pairs of graph attributes. See ["Graph Attributes"](https://graphviz.org/docs/graph/) in the Graphviz docs for valid options.
-- `node_attr: dict[str, Any]` — key-value pairs of node attributes to set on all nodes. See ["Node Attributes"](https://graphviz.org/docs/nodes/) in the Graphviz docs for valid options.
-- `edge_attr: dict[str, Any]` — key-value pairs of edge attributes to set on all edges. See ["Edge Attributes"](https://graphviz.org/docs/edges/) in the Graphviz docs for valid options.
-
-These will be merged with erdantic's default values (see [`DEFAULT_GRAPH_ATTR`][erdantic.core.DEFAULT_GRAPH_ATTR], [`DEFAULT_GRAPH_ATTR`][erdantic.core.DEFAULT_NODE_ATTR], and [`DEFAULT_GRAPH_ATTR`][erdantic.core.DEFAULT_EDGE_ATTR]).
-
-Some common attributes you might want to change:
-
-- `graph_attr["nodesep"]: float` — controls vertical spacing between models in diagram.
-- `graph_attr["ranksep"]: float` — controls horizontal spacing between models in diagram.
-- `node_attr["fontsize"]: float` — controls font size of text in model tables.
-
-
-## Customizing diagram content
-
-Behind the scenes, all of the information that erdantic extracts from data model classes is stored as data on Pydantic models. Because everything is represented as just data, you can do any of the following:
-
-- Edit any of the fields directly to change information. 
-- Serialize the model to JSON and save to disk.
-- Deserialize JSON data back into instances of erdantic's models. 
-
-### Data model
-
-The data model for erdantic has the following classes:
-
-- [`EntityRelationshipDiagram`][erdantic.core.EntityRelationshipDiagram] — overall container for everything in the diagram.
-- [`ModelInfo`][erdantic.core.ModelInfo] — stores the information of one model. Each instance gets rendered as one node in the diagram.
-- [`FieldInfo`][erdantic.core.FieldInfo] — stores the information of one field on a model. Each instance gets rendered as one row in the table of a node in the diagram.
-- [`Edge`][erdantic.core.Edge] — stores the information about the relationship between a model field and another model. 
-
-Additionally, there is a utility model [`FullyQualifiedName`][erdantic.core.FullyQualifiedName] that stores the ["fully qualified name"](https://stackoverflow.com/a/17403972), a precise reference to a model class as a Python object. This allows us to reimport that object if needed. 
-
-An entity relationship diagram for the these models is shown below.
-
-<object type="image/svg+xml" data="../assets/erdantic_diagram.svg" width="100%" typemustmatch><img alt="Example diagram created by erdantic" src="../assets/erdantic_diagram.svg"></object>
-
-erdantic fills in these fields at the time that a model is added to a diagram and the respective instance is created. After that, the values in these fields are all just static data. You can directly edit any of these fields to override the values that erdantic extracted. 
-
-The `SortedDict` class on `EntityRelationshipDiagram` is from [sortedcontainers-pydantic](https://github.com/drivendataorg/sortedcontainers-pydantic) and allows erdantic to store models and edges in a stable ordering no matter the order that they were added to the diagram. 
-
-### Customizing edges
-
-erdantic uses [crow's foot notation](https://www.gleek.io/blog/crows-foot-notation) to represent the cardinality and modality of the relationships between models. Cardinality refers to the maximum number of instances of the target that can be related, with possible values of "one" or "many". Modality refers to the minimum number of instances of the target, i.e., whether it is optional, with values of "zero" or "one". 
-
-Here are the four possible cases that erdantic will extract by default:
-
-| Example Type Annotation  | Cardinality | Modality    | Notation |
-|--------------------------|-------------|-------------|----------|
-| `Target`                 | one         | one         | ![Crow's foot notation showing tee-tee](assets/edge-one-one.png) |
-| `Optional[Target]`       | one         | zero        | ![Crow's foot notation showing odot-tee](assets/edge-one-zero.png) |
-| `List[Target]`           | many        | unspecified | ![Crow's foot notation showing crow](assets/edge-many-unspecified.png) |
-| `Optional[List[Target]]` | many        | zero        | ![Crow's foot notation showing odot-crow](assets/edge-many-zero.png) |
-
-You will notice that, for example, that we only have a (many, unspecified) case and no (many, one) case. While erdantic treats `List[Target]` as having ambiguous modality, if you have knowledge about your data model, you can manually override the modality value. The cardinality and modality are set on the `target_cardinality` and `target_modality` fields on an [`Edge`][erdantic.core.Edge] using the [`Cardinality`][erdantic.core.Cardinality] and [`Modality`][erdantic.core.Modality] enums. These enums each have three levels:
-
-- `Cardinality.UNSPECIFIED`, `Cardinality.ONE`, `Cardinality.MANY`
-- `Modality.UNSPECIFIED`, `Modality.ZERO`, `Modality.ONE`
-
-When setting manually, you can use any possible combination to indicate a relationship of your choice. 
-
-`Edge` instances also have fields `source_cardinality` and `source_modality` that you can use to indicate the cardinality and modality of the _source_ model. Edges created by erdantic will always set these to `Cardinality.UNSPECIFIED` and `Modality.UNSPECIFIED`, but you can use your own knowledge to set them to other values.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `erdantic-1.0.0.post2/erdantic/_repr_utils.py` & `erdantic-1.0.0rc1/erdantic/_repr_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/cli.py` & `erdantic-1.0.0rc1/erdantic/cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/convenience.py` & `erdantic-1.0.0rc1/erdantic/convenience.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/core.py` & `erdantic-1.0.0rc1/erdantic/core.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/exceptions.py` & `erdantic-1.0.0rc1/erdantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/typing_utils.py` & `erdantic-1.0.0rc1/erdantic/typing_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/examples/attrs.py` & `erdantic-1.0.0rc1/erdantic/examples/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/examples/dataclasses.py` & `erdantic-1.0.0rc1/erdantic/examples/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/examples/pydantic.py` & `erdantic-1.0.0rc1/erdantic/examples/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/examples/pydantic_v1.py` & `erdantic-1.0.0rc1/erdantic/examples/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/plugins/__init__.py` & `erdantic-1.0.0rc1/erdantic/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/plugins/attrs.py` & `erdantic-1.0.0rc1/erdantic/plugins/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/plugins/dataclasses.py` & `erdantic-1.0.0rc1/erdantic/plugins/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/erdantic/plugins/pydantic.py` & `erdantic-1.0.0rc1/erdantic/plugins/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.0.post2/README.md` & `erdantic-1.0.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI](https://img.shields.io/pypi/v/erdantic.svg)](https://pypi.org/project/erdantic/)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/erdantic.svg)](https://anaconda.org/conda-forge/erdantic)
 [![conda-forge feedstock](https://img.shields.io/badge/conda--forge-feedstock-yellowgreen)](https://github.com/conda-forge/erdantic-feedstock)
 [![tests](https://github.com/drivendataorg/erdantic/workflows/tests/badge.svg?branch=main)](https://github.com/drivendataorg/erdantic/actions?query=workflow%3Atests+branch%3Amain)
 [![codecov](https://codecov.io/gh/drivendataorg/erdantic/branch/main/graph/badge.svg)](https://codecov.io/gh/drivendataorg/erdantic)
 
 > [!NOTE]
-> erdantic v1.0 has been released! See the [changelog](./HISTORY.md) for more information.
+> erdantic v1.0 is coming soon and involves big backend changes. See the [changelog](./HISTORY.md) for more information.
 
 **erdantic** is a simple tool for drawing [entity relationship diagrams (ERDs)](https://en.wikipedia.org/wiki/Data_modeling#Entity%E2%80%93relationship_diagrams) for Python data model classes. Diagrams are rendered using the venerable [Graphviz](https://graphviz.org/) library. Supported data modeling frameworks are:
 
 - [Pydantic V2](https://docs.pydantic.dev/latest/)
 - [Pydantic V1 legacy](https://docs.pydantic.dev/latest/migration/#continue-using-pydantic-v1-features)
 - [attrs](https://www.attrs.org/en/stable/)
 - [dataclasses](https://docs.python.org/3/library/dataclasses.html) from the Python standard library
```

### Comparing `erdantic-1.0.0.post2/pyproject.toml` & `erdantic-1.0.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "erdantic"
-version = "1.0.0.post2"
+version = "1.0.0rc1"
 description = "Entity relationship diagrams for Python data model classes like Pydantic."
 readme = "README.md"
 authors = [{ name = "DrivenData", email = "info@drivendata.org" }, { name = "Jay Qi" }]
 license = { text = "MIT License" }
 keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic", "attrs"]
 classifiers = [
   "Intended Audience :: Developers",
@@ -28,15 +28,14 @@
 dependencies = [
   "pydantic >= 2",
   "pydantic-core",
   "pygraphviz",
   "sortedcontainers-pydantic",
   "typenames",
   "typer",
-  "typing_extensions>4 ; python_version < '3.12'",
 ]
 
 [project.optional-dependencies]
 attrs = ["attrs"]
 
 [project.scripts]
 erdantic = "erdantic.cli:app"
```

