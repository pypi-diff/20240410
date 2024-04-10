# Comparing `tmp/nti.testing-4.0.0.tar.gz` & `tmp/nti.testing-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nti.testing-4.0.0.tar", last modified: Tue Oct 24 17:54:05 2023, max compression
+gzip compressed data, was "nti.testing-4.1.0.tar", last modified: Wed Apr 10 16:05:03 2024, max compression
```

## Comparing `nti.testing-4.0.0.tar` & `nti.testing-4.1.0.tar`

### file list

```diff
@@ -1,71 +1,67 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.040714 nti.testing-4.0.0/
--rw-r--r--   0 jmadden    (501) staff       (20)      537 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.coveragerc
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.031853 nti.testing-4.0.0/.github/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.035290 nti.testing-4.0.0/.github/workflows/
--rw-r--r--   0 jmadden    (501) staff       (20)     1270 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.github/workflows/tests.yml
--rw-r--r--   0 jmadden    (501) staff       (20)       66 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.gitignore
--rw-r--r--   0 jmadden    (501) staff       (20)      330 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.isort.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)       27 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.nti_cover_package
--rw-r--r--   0 jmadden    (501) staff       (20)     9336 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.pylintrc
--rw-r--r--   0 jmadden    (501) staff       (20)      715 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.readthedocs.yml
--rw-r--r--   0 jmadden    (501) staff       (20)      503 2023-10-24 17:54:04.000000 nti.testing-4.0.0/.travis.yml
--rw-r--r--   0 jmadden    (501) staff       (20)     3282 2023-10-24 17:54:04.000000 nti.testing-4.0.0/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       73 2023-10-24 17:54:04.000000 nti.testing-4.0.0/COPYRIGHT.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-10-24 17:54:04.000000 nti.testing-4.0.0/INSTALL
--rw-r--r--   0 jmadden    (501) staff       (20)      529 2023-10-24 17:54:04.000000 nti.testing-4.0.0/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)      417 2023-10-24 17:54:04.000000 nti.testing-4.0.0/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)    15008 2023-10-24 17:54:05.040591 nti.testing-4.0.0/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     9734 2023-10-24 17:54:04.000000 nti.testing-4.0.0/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-10-24 17:54:04.000000 nti.testing-4.0.0/TODO
--rw-r--r--   0 jmadden    (501) staff       (20)        8 2023-10-24 17:54:04.000000 nti.testing-4.0.0/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.036293 nti.testing-4.0.0/docs/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.036402 nti.testing-4.0.0/docs/_static/
--rw-r--r--   0 jmadden    (501) staff       (20)     3329 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/_static/custom.css
--rw-r--r--   0 jmadden    (501) staff       (20)      430 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       90 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/base.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       28 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/changelog.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     7219 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)      227 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      249 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/layers.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      106 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/matchers.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       90 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/time.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       90 2023-10-24 17:54:04.000000 nti.testing-4.0.0/docs/zodb.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      293 2023-10-24 17:54:04.000000 nti.testing-4.0.0/nose2.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)      128 2023-10-24 17:54:05.041008 nti.testing-4.0.0/setup.cfg
--rwxr-xr-x   0 jmadden    (501) staff       (20)     2483 2023-10-24 17:54:04.000000 nti.testing-4.0.0/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.032393 nti.testing-4.0.0/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.036506 nti.testing-4.0.0/src/nti/
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/__init__.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.037933 nti.testing-4.0.0/src/nti/testing/
--rw-r--r--   0 jmadden    (501) staff       (20)     3441 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)    20328 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/base.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.038352 nti.testing-4.0.0/src/nti/testing/layers/
--rw-r--r--   0 jmadden    (501) staff       (20)     1318 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2315 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/cleanup.py
--rw-r--r--   0 jmadden    (501) staff       (20)    22900 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/postgres.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.038537 nti.testing-4.0.0/src/nti/testing/layers/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)      258 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/tests/test_postgres.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3771 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/layers/zope.py
--rw-r--r--   0 jmadden    (501) staff       (20)    10921 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/matchers.py
--rw-r--r--   0 jmadden    (501) staff       (20)      483 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/mock.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.039483 nti.testing-4.0.0/src/nti/testing/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3908 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_base.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4297 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_component_cleanup_broken.txt
--rw-r--r--   0 jmadden    (501) staff       (20)     1316 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_layers.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1328 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_main.py
--rw-r--r--   0 jmadden    (501) staff       (20)     8226 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_matchers.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4666 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_time.py
--rw-r--r--   0 jmadden    (501) staff       (20)     9500 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/tests/test_zodb.py
--rw-r--r--   0 jmadden    (501) staff       (20)     5274 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/time.py
--rw-r--r--   0 jmadden    (501) staff       (20)     8174 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti/testing/zodb.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2023-10-24 17:54:05.037251 nti.testing-4.0.0/src/nti.testing.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)    15008 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     1383 2023-10-24 17:54:05.000000 nti.testing-4.0.0/src/nti.testing.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/namespace_packages.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      393 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2023-10-24 17:54:04.000000 nti.testing-4.0.0/src/nti.testing.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)      691 2023-10-24 17:54:04.000000 nti.testing-4.0.0/tox.ini
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.666953 nti.testing-4.1.0/
+-rw-r--r--   0 jmadden    (501) staff       (20)      537 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.coveragerc
+-rw-r--r--   0 jmadden    (501) staff       (20)      330 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.isort.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)       27 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.nti_cover_package
+-rw-r--r--   0 jmadden    (501) staff       (20)     9411 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      715 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.readthedocs.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      503 2024-04-10 16:05:03.000000 nti.testing-4.1.0/.travis.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)     3485 2024-04-10 16:05:03.000000 nti.testing-4.1.0/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       73 2024-04-10 16:05:03.000000 nti.testing-4.1.0/COPYRIGHT.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-10 16:05:03.000000 nti.testing-4.1.0/INSTALL
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2024-04-10 16:05:03.000000 nti.testing-4.1.0/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)      417 2024-04-10 16:05:03.000000 nti.testing-4.1.0/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)    15124 2024-04-10 16:05:03.666751 nti.testing-4.1.0/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     9734 2024-04-10 16:05:03.000000 nti.testing-4.1.0/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-10 16:05:03.000000 nti.testing-4.1.0/TODO
+-rw-r--r--   0 jmadden    (501) staff       (20)        8 2024-04-10 16:05:03.000000 nti.testing-4.1.0/doc-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.662134 nti.testing-4.1.0/docs/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.662249 nti.testing-4.1.0/docs/_static/
+-rw-r--r--   0 jmadden    (501) staff       (20)     3329 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/_static/custom.css
+-rw-r--r--   0 jmadden    (501) staff       (20)      430 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       90 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/base.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       28 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/changelog.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     7219 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      227 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      249 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/layers.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      106 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/matchers.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       90 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/time.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       90 2024-04-10 16:05:03.000000 nti.testing-4.1.0/docs/zodb.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      293 2024-04-10 16:05:03.000000 nti.testing-4.1.0/nose2.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)      128 2024-04-10 16:05:03.667153 nti.testing-4.1.0/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     2437 2024-04-10 16:05:03.000000 nti.testing-4.1.0/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.658451 nti.testing-4.1.0/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.662370 nti.testing-4.1.0/src/nti/
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/__init__.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.664063 nti.testing-4.1.0/src/nti/testing/
+-rw-r--r--   0 jmadden    (501) staff       (20)     3410 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    20897 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/base.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.664655 nti.testing-4.1.0/src/nti/testing/layers/
+-rw-r--r--   0 jmadden    (501) staff       (20)     1318 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     2315 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/cleanup.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    23137 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/postgres.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.664842 nti.testing-4.1.0/src/nti/testing/layers/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      258 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/tests/test_postgres.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3744 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/layers/zope.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    10935 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/matchers.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      483 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/mock.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.665762 nti.testing-4.1.0/src/nti/testing/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4748 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_base.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4297 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_component_cleanup_broken.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)     1349 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_layers.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1328 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_main.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     8237 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_matchers.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     4666 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_time.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     9491 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/tests/test_zodb.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     5275 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/time.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     8214 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti/testing/zodb.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-10 16:05:03.666034 nti.testing-4.1.0/src/nti.testing.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)    15124 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     1344 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/namespace_packages.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      405 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-10 16:05:03.000000 nti.testing-4.1.0/src/nti.testing.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)      691 2024-04-10 16:05:03.000000 nti.testing-4.1.0/tox.ini
```

### Comparing `nti.testing-4.0.0/.coveragerc` & `nti.testing-4.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/.pylintrc` & `nti.testing-4.1.0/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [MASTER]
-load-plugins=
+load-plugins=pylint.extensions.bad_builtin,
    pylint.extensions.broad_try_clause,
-   pylint.extensions.bad_builtin,
    pylint.extensions.check_elif,
    pylint.extensions.code_style,
-   pylint.extensions.comparison_placement,
-   pylint.extensions.confusing_elif,
-   pylint.extensions.consider_refactoring_into_while_condition,
    pylint.extensions.dict_init_mutate,
-   pylint.extensions.docparams,
    pylint.extensions.docstyle,
    pylint.extensions.dunder,
-   pylint.extensions.eq_without_hash,
+   pylint.extensions.comparison_placement,
+   pylint.extensions.confusing_elif,
    pylint.extensions.for_any_all,
+   pylint.extensions.consider_refactoring_into_while_condition,
    pylint.extensions.mccabe,
+   pylint.extensions.eq_without_hash,
+   pylint.extensions.redefined_variable_type,
    pylint.extensions.overlapping_exceptions,
+   pylint.extensions.docparams,
    pylint.extensions.private_import,
-   pylint.extensions.redefined_variable_type,
-   pylint.extensions.set_membership,
    pylint.extensions.typing,
 
+#    pylint.extensions.set_membership,
+# wants you to turn ``foo in (1, 2)`` into ``foo in {1, 2}``;
+# but for small tuples, the former is actually more
+# performant.
+
 # magic_value wants you to not use arbitrary strings and numbers
 # inline in the code. But it's overzealous and has way too many false
 # positives. Trust people to do the most readable thing.
 #   pylint.extensions.magic_value
 
 # Empty comment would be good, except it detects blank lines within
 # a single comment block.
@@ -38,16 +41,16 @@
 # redefined_loop_name tends to catch us with things like
 # for name in (a, b, c): name = name + '_column' ...
 #    pylint.extensions.redefined_loop_name,
 
 # This wants you to turn ``x in (1, 2)`` into ``x in {1, 2}``.
 # They both result in the LOAD_CONST bytecode, one a tuple one a
 # frozenset. In theory a set lookup using hashing is faster than
-# a linear scan of a tuple; but if the tuple is small, it can
-# actually be faster to scan the tuple. This one is debatable.
+# a linear scan of a tuple; but if the tuple is small, it can often
+# actually be faster to scan the tuple.
 #   pylint.extensions.set_membership,
 
 # Fix zope.cachedescriptors.property.Lazy; the property-classes doesn't seem to
 # do anything.
 # https://stackoverflow.com/questions/51160955/pylint-how-to-specify-a-self-defined-property-decorator-with-property-classes
 # For releases prior to 2.14.2, this needs to be a one-line, quoted string. After that,
 # a multi-line string.
@@ -120,15 +123,14 @@
 #   if foo: ...
 #
 # Into ``if (foo := get_foo()):``
 # But there are a *lot* of those. Trust people to do the right, most
 # readable, thing
 #
 # docstring-first-line-empty: That's actually our standard, based on Django.
-# empty-comment: Two lines above this would trigger that. Yick.
 # XXX: unclear on the docstring warnings, missing-type-doc, missing-param-doc,
 # differing-param-doc, differing-type-doc (are the last two replacements for the first two?)
 #
 # They should be addressed, in general they are a good thing, but sometimes they are
 # unnecessary.
 disable=wrong-import-position,
     wrong-import-order,
@@ -150,14 +152,15 @@
     missing-type-doc,
     missing-param-doc,
     differing-param-doc,
     differing-type-doc,
     compare-to-zero,
     docstring-first-line-empty,
     too-many-try-statements,
+    redefined-variable-type,
 
 enable=consider-using-augmented-assign
 
 [FORMAT]
 max-line-length=100
 max-module-lines=1100
```

### Comparing `nti.testing-4.0.0/.readthedocs.yml` & `nti.testing-4.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/CHANGES.rst` & `nti.testing-4.1.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+4.1.0 (2024-04-10)
+==================
+
+- Add support for, and require, testgres 1.10. This is needed because
+  they changed the signature for ``get_pg_version``.
+- Drop support for Python 3.8 and 3.9.
+
+
 4.0.0 (2023-10-24)
 ==================
 
 - Add support for Python 3.10, 3.11 and 3.12.
 - Drop support for Python 2 and Python 3.6 and 3.7.
 - Add a layer for working with a ``testgres`` Postgres instance.
 - Add methods to the test base classes to support ``unittest.mock`` patches.
```

### Comparing `nti.testing-4.0.0/LICENSE` & `nti.testing-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/PKG-INFO` & `nti.testing-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: nti.testing
-Version: 4.0.0
+Version: 4.1.0
 Summary: Support for testing code
 Home-page: https://github.com/OpenNTI/nti.testing
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
 Project-URL: Documentation, https://ntitesting.readthedocs.io/en/latest/
 Keywords: nose2 testing zope3 ZTK hamcrest
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Zope3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: ZODB>=5.6.0
 Requires-Dist: zope.interface>=5.4.0
 Requires-Dist: pyhamcrest
 Requires-Dist: six
 Requires-Dist: setuptools
 Requires-Dist: transaction
@@ -36,21 +34,21 @@
 Requires-Dist: zope.exceptions
 Requires-Dist: zope.schema
 Requires-Dist: zope.testing
 Provides-Extra: test
 Requires-Dist: Acquisition; extra == "test"
 Requires-Dist: zope.site; extra == "test"
 Requires-Dist: zope.testrunner; extra == "test"
-Requires-Dist: testgres; extra == "test"
+Requires-Dist: testgres>=1.10; extra == "test"
 Requires-Dist: psycopg2-binary; platform_python_implementation != "PyPy" and extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: testgres
-Requires-Dist: testgres; extra == "testgres"
+Requires-Dist: testgres>=1.10; extra == "testgres"
 Requires-Dist: psycopg2-binary; platform_python_implementation != "PyPy" and extra == "testgres"
 
 =============
  nti.testing
 =============
 
 .. image:: https://img.shields.io/pypi/v/nti.testing.svg
@@ -299,14 +297,22 @@
 ZODB in `nti.testing.zodb`. See the API documentation for details.
 
 
 =========
  Changes
 =========
 
+4.1.0 (2024-04-10)
+==================
+
+- Add support for, and require, testgres 1.10. This is needed because
+  they changed the signature for ``get_pg_version``.
+- Drop support for Python 3.8 and 3.9.
+
+
 4.0.0 (2023-10-24)
 ==================
 
 - Add support for Python 3.10, 3.11 and 3.12.
 - Drop support for Python 2 and Python 3.6 and 3.7.
 - Add a layer for working with a ``testgres`` Postgres instance.
 - Add methods to the test base classes to support ``unittest.mock`` patches.
```

### Comparing `nti.testing-4.0.0/README.rst` & `nti.testing-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/docs/_static/custom.css` & `nti.testing-4.1.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/docs/conf.py` & `nti.testing-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/setup.py` & `nti.testing-4.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright 2017 NextThought
+# Copyright 2022-2024 Jason Madden
 # Released under the terms of the LICENSE file.
 import codecs
 from setuptools import setup, find_packages
 
 
-version = '4.0.0'
+version = '4.1.0'
 
 entry_points = {
 }
 
 TESTS_REQUIRE = [
     'Acquisition',
     'zope.site',
     'zope.testrunner',
-    'testgres',
+    'testgres >= 1.10',
     'psycopg2-binary; python_implementation != "PyPy"',
 ]
 
 def _read(fname):
     with codecs.open(fname, encoding='utf-8') as f:
         return f.read()
 
@@ -36,16 +37,14 @@
     },
     classifiers=[
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Testing',
         'Framework :: Zope3',
@@ -74,13 +73,13 @@
     extras_require={
         'test': TESTS_REQUIRE,
         'docs': [
             'Sphinx',
             'furo',
         ],
         'testgres': [
-            'testgres',
+            'testgres >= 1.10',
             'psycopg2-binary; python_implementation != "PyPy"',
         ],
     },
-    python_requires=">=3.8",
+    python_requires=">=3.10",
 )
```

### Comparing `nti.testing-4.0.0/src/nti/testing/__init__.py` & `nti.testing-4.1.0/src/nti/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 from .matchers import is_true
 from .matchers import is_false
 from .matchers import provides
 from .matchers import implements
 from .matchers import verifiably_provides
 from .matchers import validly_provides
-from .matchers import provides
 from .matchers import validated_by
 from .matchers import not_validated_by
 from .matchers import aq_inContextOf
 
 from .time import time_monotonically_increases
```

### Comparing `nti.testing-4.0.0/src/nti/testing/base.py` & `nti.testing-4.1.0/src/nti/testing/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -396,15 +396,16 @@
 
     .. note:: The ZCML configuration is executed for each test.
     """
 
     def _doSetUpSuper(self):
         super().setUp()
 
-    setUp = AbstractConfiguringObject._doSetUp
+    def setUp(self):
+        AbstractConfiguringObject._doSetUp(self)
 
     #: Configure additional packages. This should only be done in the ``setUp`` method
     #: of a subclass. Note that this is called by ``setUp``.
     configure_packages = AbstractConfiguringObject._do_configure_packages
 
     def configure_string(self, zcml_string):
         """
@@ -415,15 +416,31 @@
         """
         self.configuration_context = xmlconfig.string(zcml_string, self.configuration_context)
         return self.configuration_context
 
     def _doTearDownSuper(self):
         super().tearDown()
 
-    tearDown = AbstractConfiguringObject._doTearDown
+    def tearDown(self):
+        self._doTearDownConfiguration()
+
+    def _doTearDownConfiguration(self):
+        """
+        Hook for subclasses to override.
+
+        This implementation calls :meth:`AbstractConfiguringObject._doTearDown`
+        with the default parameters. If you need to call it with a different
+        set of parameters, override this method to do so.
+
+        This method takes no arguments because the arguments passed to
+        ``_doTearDown`` are almost always static at the callsite.
+        """
+        AbstractConfiguringObject._doTearDown(
+            self,
+        )
 
 class SharedConfiguringTestBase(AbstractConfiguringObject,
                                 AbstractSharedTestBase):
     """
     Test case that can be subclassed when ZCML configuration is desired.
 
     Configuration is established by the class attributes documented on
```

### Comparing `nti.testing-4.0.0/src/nti/testing/layers/__init__.py` & `nti.testing-4.1.0/src/nti/testing/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/src/nti/testing/layers/cleanup.py` & `nti.testing-4.1.0/src/nti/testing/layers/cleanup.py`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/src/nti/testing/layers/postgres.py` & `nti.testing-4.1.0/src/nti/testing/layers/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,27 +74,31 @@
             SAVE_DATABASE_FILENAME = val
 
 
 if 'NTI_LOAD_DB_FILE' in os.environ:
     LOAD_DATABASE_ON_SETUP = os.environ['NTI_LOAD_DB_FILE']
 
 
-def patched_get_pg_version():
+def patched_get_pg_version(*args, **kwargs):
+    # We patch  this in testgres.node, so its ok to import
+    # the original. In version 1.10, they changed the signature
+    # of this function, so be sure to accept whatever it does and
+    # pass it on.
     from testgres.utils import get_pg_version
     from testgres.node import PgVer
     from packaging.version import InvalidVersion
 
     # Some installs of postgres return
     # strings that the version parser doesn't like;
     # notably the Python images get a debian build that says
     # "15.3-0+deb12u1" which get_pg_version() chops down to
     # "15.3-0+". If it can't be parsed, then return a fake.
 
     try:
-        version = get_pg_version()
+        version = get_pg_version(*args, **kwargs)
         PgVer(version)
     except InvalidVersion:
         print('testgres: Got invalid postgres version', version)
         # The actual version string looks like "postgres (PostgreSQL) 15.4",
         # and get_pg_version() processes that down to this
         version = "15.4"
         print('testgres: Substituting version', version)
```

### Comparing `nti.testing-4.0.0/src/nti/testing/layers/zope.py` & `nti.testing-4.1.0/src/nti/testing/layers/zope.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # -*- coding: utf-8 -*-
 """
 Test layers for working with Zope libraries.
 
 """
 
 import gc
-import sys
-import unittest
 import logging
 
 
 from zope import component
 from zope.component import eventtesting
 from zope.component.hooks import setHooks
```

### Comparing `nti.testing-4.0.0/src/nti/testing/matchers.py` & `nti.testing-4.1.0/src/nti/testing/matchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,17 @@
             return self
     return _orig_append_description_of(self, value)
 
 BaseDescription.append_description_of = _append_description_of_map
 
 
 class TypeCheckedDict(dict):
-    "A dictionary that ensures keys and values are of the required type when set"
+    """
+    A dictionary that ensures keys and values are of the required type when set
+    """
 
     def __init__(self, key_class=object, val_class=object, notify=None):
         dict.__init__(self)
         self.key_class = key_class
         self.val_class = val_class
         self.notify = notify
```

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_base.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         import gc
         class MyTest(base.AbstractSharedTestBase):
             HANDLE_GC = True
             def test_thing(self):
                 raise AssertionError("Not called")
 
         MyTest.setUpClass()
+        # pylint:disable-next=simplifiable-if-expression
         assert_that(gc.isenabled(), is_(False if not base._is_pypy else True))
         MyTest.tearDownClass()
         assert_that(gc.isenabled(), is_(True))
 
         MyTest('test_thing').setUp()
         MyTest('test_thing').tearDown()
 
@@ -126,7 +127,34 @@
 
         MyTest('test_thing').tearDown()
 
     def test_module_setup(self):
         base.module_setup()
         base.module_setup(set_up_packages=('zope.component',))
         base.module_teardown()
+
+    def test_calling_super_linting(self):
+        # Deriving a class from our bases and calling their setup
+        # methods should NOT produce linter warnings.
+        # So this section should not have pylint disable commands.
+        class X(base.AbstractTestBase):
+            def setUp(self):
+                super().setUp()
+                self.thing = 1
+
+            def tearDown(self):
+                super().tearDown()
+                self.thing = 2
+
+        class Y(base.ConfiguringTestBase):
+            def setUp(self):
+                super().setUp()
+                self.thing = 1
+
+            def tearDown(self):
+                super().tearDown()
+                self.thing = 2
+
+        X().setUp()
+        X().tearDown()
+        Y().setUp()
+        Y().tearDown()
```

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_component_cleanup_broken.txt` & `nti.testing-4.1.0/src/nti/testing/tests/test_component_cleanup_broken.txt`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_layers.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def test_find_test(self):
 
         def func():
             assert_that(layers.find_test(), is_(self))
 
         func()
 
-        def via_test(test):
+        def via_test(test): # pylint:disable=unused-argument
             func()
 
         via_test(self)
 
     def _check_methods(self, layer, extra_methods=()):
         default_methods = ('setUp', 'tearDown', 'testSetUp', 'testTearDown')
         for meth in default_methods + extra_methods:
```

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_main.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_matchers.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         from zope import interface
 
         class IThing(interface.Interface):
             thing = interface.Attribute("thing")
 
             def method(): # pylint:disable=no-method-argument
-                "method"
+                """Does nothing."""
 
         @interface.implementer(IThing)
         class Thing(object):
             thing = 1
 
             def method(self):
                 raise AssertionError("Not called")
```

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_time.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `nti.testing-4.0.0/src/nti/testing/tests/test_zodb.py` & `nti.testing-4.1.0/src/nti/testing/tests/test_zodb.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 class MockDBTrans(zodb.mock_db_trans):
 
     def __init__(self, db=None):
         if db is None:
             db = MockDB()
-        super(MockDBTrans, self).__init__(db)
+        super().__init__(db)
         self.exc_file = NativeStringIO()
 
 class TestMockDBTrans(unittest.TestCase):
 
     def setUp(self):
         self._was_explicit = transaction.manager.explicit
         transaction.manager.explicit = False
@@ -81,15 +81,15 @@
             with MockDBTrans():
                 transaction.manager.explicit = False
 
     def test_error_if_mode_changed_and_error_in_body(self):
         with self.assertRaises(zodb._TransactionManagerModeChanged) as exc:
             with MockDBTrans():
                 transaction.manager.explicit = False
-                raise Exception("BodyError")
+                raise Exception("BodyError") # pylint:disable=broad-exception-raised
         # The backing exception is included
         self.assertIn('BodyError', str(exc.exception))
 
     def test_error_if_tx_ended(self):
         with self.assertRaises(zodb._TransactionChanged):
             with MockDBTrans():
                 transaction.commit()
@@ -215,15 +215,16 @@
         self.assertIn('Module nti.testing.zodb', msg)
 
     def test_error_in_on_opened(self):
         class OpenEx(Exception):
             pass
 
         class MyFalse(object):
-            __nonzero__ = __bool__ = lambda _self: False
+            def __bool__(self):
+                return False
 
         transaction.manager.explicit = MyFalse()
         class MyMock(MockDBTrans):
             seen_tx = None
             aborted = False
             def on_connection_opened(self, conn):
                 # pylint:disable=no-member
@@ -272,34 +273,34 @@
         reg_db = gsm.queryUtility(IDatabase)
         self.assertIsNone(reg_db)
 
         self.layer.setUp()
 
 
 class IExtra(interface.Interface): # pylint:disable=inherit-non-class
-    "An extra interface"
+    """An extra interface."""
 
 class IExtra2(interface.Interface): # pylint:disable=inherit-non-class
-    "Another extra interface"
+    """Another extra interface."""
 
 class Object(object):
 
     def __init__(self, *args):
         pass
 
 class TestResetDbCaches(unittest.TestCase):
     layer = zodb.ZODBLayer
 
     def setUp(self):
-        super(TestResetDbCaches, self).setUp()
+        super().setUp()
         gc.disable()
 
     def tearDown(self):
         gc.enable()
-        super(TestResetDbCaches, self).tearDown()
+        super().tearDown()
 
     def test_persistent_site_closed(self):
         from zope.site.site import LocalSiteManager
         from ZODB import DB
         from ZODB.DemoStorage import DemoStorage
 
         interface.classImplements(LocalSiteManager, IExtra)
```

### Comparing `nti.testing-4.0.0/src/nti/testing/time.py` & `nti.testing-4.1.0/src/nti/testing/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def install_fakes(self):
         time.time = self.fake_time
         time.gmtime = self.fake_gmtime
 
     __enter__ = install_fakes
 
-    def close(self, *args):
+    def close(self, *_args):
         time.time = _real_time
         time.gmtime = _real_gmtime
 
     __exit__ = close
 
     def __call__(self, func):
         @functools.wraps(func)
```

### Comparing `nti.testing-4.0.0/src/nti/testing/zodb.py` & `nti.testing-4.1.0/src/nti/testing/zodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         print(msg, file=f)
         print_exception(t, v, tb, file=f, with_filenames=False)
 
     def _close_connection(self, conn, ignore_errors):
         catch = Exception if ignore_errors else ()
         try:
             conn.close()
-        except catch:
+        except catch: # pylint:disable=broad-exception-caught
             self._report_exception("Unexpected error closing connection; ignored.", *sys.exc_info())
 
     def __exit__(self, t, v, tb):
         # Returning a True value from __exit__ suppresses any
         # exception raised in the body.
         body_raised = t is not None
         abort_only = body_raised # Should we commit our transaction, or only abort it?
```

### Comparing `nti.testing-4.0.0/src/nti.testing.egg-info/PKG-INFO` & `nti.testing-4.1.0/src/nti.testing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: nti.testing
-Version: 4.0.0
+Version: 4.1.0
 Summary: Support for testing code
 Home-page: https://github.com/OpenNTI/nti.testing
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
 Project-URL: Documentation, https://ntitesting.readthedocs.io/en/latest/
 Keywords: nose2 testing zope3 ZTK hamcrest
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Zope3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: ZODB>=5.6.0
 Requires-Dist: zope.interface>=5.4.0
 Requires-Dist: pyhamcrest
 Requires-Dist: six
 Requires-Dist: setuptools
 Requires-Dist: transaction
@@ -36,21 +34,21 @@
 Requires-Dist: zope.exceptions
 Requires-Dist: zope.schema
 Requires-Dist: zope.testing
 Provides-Extra: test
 Requires-Dist: Acquisition; extra == "test"
 Requires-Dist: zope.site; extra == "test"
 Requires-Dist: zope.testrunner; extra == "test"
-Requires-Dist: testgres; extra == "test"
+Requires-Dist: testgres>=1.10; extra == "test"
 Requires-Dist: psycopg2-binary; platform_python_implementation != "PyPy" and extra == "test"
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: testgres
-Requires-Dist: testgres; extra == "testgres"
+Requires-Dist: testgres>=1.10; extra == "testgres"
 Requires-Dist: psycopg2-binary; platform_python_implementation != "PyPy" and extra == "testgres"
 
 =============
  nti.testing
 =============
 
 .. image:: https://img.shields.io/pypi/v/nti.testing.svg
@@ -299,14 +297,22 @@
 ZODB in `nti.testing.zodb`. See the API documentation for details.
 
 
 =========
  Changes
 =========
 
+4.1.0 (2024-04-10)
+==================
+
+- Add support for, and require, testgres 1.10. This is needed because
+  they changed the signature for ``get_pg_version``.
+- Drop support for Python 3.8 and 3.9.
+
+
 4.0.0 (2023-10-24)
 ==================
 
 - Add support for Python 3.10, 3.11 and 3.12.
 - Drop support for Python 2 and Python 3.6 and 3.7.
 - Add a layer for working with a ``testgres`` Postgres instance.
 - Add methods to the test base classes to support ``unittest.mock`` patches.
```

### Comparing `nti.testing-4.0.0/src/nti.testing.egg-info/SOURCES.txt` & `nti.testing-4.1.0/src/nti.testing.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .coveragerc
-.gitignore
 .isort.cfg
 .nti_cover_package
 .pylintrc
 .readthedocs.yml
 .travis.yml
 CHANGES.rst
 COPYRIGHT.txt
@@ -13,15 +12,14 @@
 README.rst
 TODO
 doc-requirements.txt
 nose2.cfg
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/tests.yml
 docs/api.rst
 docs/base.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/layers.rst
 docs/matchers.rst
```

### Comparing `nti.testing-4.0.0/tox.ini` & `nti.testing-4.1.0/tox.ini`

 * *Files identical despite different names*

