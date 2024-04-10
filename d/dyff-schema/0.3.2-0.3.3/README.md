# Comparing `tmp/dyff-schema-0.3.2.tar.gz` & `tmp/dyff-schema-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-schema-0.3.2.tar", last modified: Tue Apr  9 18:09:22 2024, max compression
+gzip compressed data, was "dyff-schema-0.3.3.tar", last modified: Tue Apr  9 21:21:41 2024, max compression
```

## Comparing `dyff-schema-0.3.2.tar` & `dyff-schema-0.3.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.094730 dyff-schema-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 18:09:22.093730 dyff-schema-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.078730 dyff-schema-0.3.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.085730 dyff-schema-0.3.2/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.087730 dyff-schema-0.3.2/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.087730 dyff-schema-0.3.2/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.087730 dyff-schema-0.3.2/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.089730 dyff-schema-0.3.2/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.091730 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.091730 dyff-schema-0.3.2/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    55306 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     8014 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.093730 dyff-schema-0.3.2/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 18:09:22.000000 dyff-schema-0.3.2/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-09 18:09:22.000000 dyff-schema-0.3.2/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 18:09:22.000000 dyff-schema-0.3.2/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 18:09:22.000000 dyff-schema-0.3.2/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 18:09:22.000000 dyff-schema-0.3.2/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 18:09:22.094730 dyff-schema-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 18:09:22.093730 dyff-schema-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-09 18:09:16.000000 dyff-schema-0.3.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.692900 dyff-schema-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 21:21:41.691900 dyff-schema-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.678900 dyff-schema-0.3.3/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.684900 dyff-schema-0.3.3/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.685900 dyff-schema-0.3.3/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.685900 dyff-schema-0.3.3/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.685900 dyff-schema-0.3.3/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.688900 dyff-schema-0.3.3/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.689900 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.689900 dyff-schema-0.3.3/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    54650 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8014 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.691900 dyff-schema-0.3.3/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-09 21:21:41.000000 dyff-schema-0.3.3/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-09 21:21:41.000000 dyff-schema-0.3.3/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 21:21:41.000000 dyff-schema-0.3.3/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 21:21:41.000000 dyff-schema-0.3.3/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 21:21:41.000000 dyff-schema-0.3.3/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 21:21:41.692900 dyff-schema-0.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 21:21:41.691900 dyff-schema-0.3.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-09 21:21:36.000000 dyff-schema-0.3.3/tests/test_import.py
```

### Comparing `dyff-schema-0.3.2/.gitlab-ci.yml` & `dyff-schema-0.3.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/.pre-commit-config.yaml` & `dyff-schema-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/.secrets.baseline` & `dyff-schema-0.3.3/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/CODE_OF_CONDUCT.md` & `dyff-schema-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/LICENSE` & `dyff-schema-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/PKG-INFO` & `dyff-schema-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.2/README.md` & `dyff-schema-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/__init__.py` & `dyff-schema-0.3.3/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/copydoc.py` & `dyff-schema-0.3.3/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/ids.py` & `dyff-schema-0.3.3/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/quantity.py` & `dyff-schema-0.3.3/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/adapters.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/base.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/__init__.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/arrow.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/binary.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/dataset/text.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/io/vllm.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/platform.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,36 +195,19 @@
     """
 
     ALL = "*"
 
     @staticmethod
     def for_kind(kind: Entities) -> "Resources":
         try:
-            return __entities_to_resources[kind]
+            return Resources[kind.value]
         except KeyError:
             raise ValueError(f"No Resources for Entity kind: {kind}")
 
 
-__entities_to_resources: dict[Entities, Resources] = {
-    Entities.Analysis: Resources.Analysis,
-    Entities.Audit: Resources.Audit,
-    Entities.AuditProcedure: Resources.AuditProcedure,
-    Entities.Dataset: Resources.Dataset,
-    Entities.DataSource: Resources.DataSource,
-    Entities.Evaluation: Resources.Evaluation,
-    Entities.InferenceService: Resources.InferenceService,
-    Entities.InferenceSession: Resources.InferenceSession,
-    Entities.Method: Resources.Method,
-    Entities.Model: Resources.Model,
-    Entities.Module: Resources.Module,
-    Entities.Report: Resources.Report,
-    Entities.SafetyCase: Resources.SafetyCase,
-}
-
-
 class DyffModelWithID(DyffSchemaBaseModel):
     id: str = pydantic.Field(description="Unique identifier of the entity")
     account: str = pydantic.Field(description="Account that owns the entity")
 
 
 LabelKey: TypeAlias = pydantic.constr(  # type: ignore
     regex=_k8s_label_key_regex(), max_length=_k8s_label_key_maxlen()
```

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/requests.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/requests.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff/schema/v0/r1/test.py` & `dyff-schema-0.3.3/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/dyff_schema.egg-info/PKG-INFO` & `dyff-schema-0.3.3/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.2/dyff_schema.egg-info/SOURCES.txt` & `dyff-schema-0.3.3/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/pyproject.toml` & `dyff-schema-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.2/tests/test_import.py` & `dyff-schema-0.3.3/tests/test_import.py`

 * *Files identical despite different names*

