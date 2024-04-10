# Comparing `tmp/imio.history-1.33.tar.gz` & `tmp/imio.history-1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.history-1.33.tar", last modified: Mon Dec 11 09:41:47 2023, max compression
+gzip compressed data, was "dist/imio.history-1.34.tar", last modified: Wed Apr 10 07:06:36 2024, max compression
```

## Comparing `imio.history-1.33.tar` & `imio.history-1.34.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18027 2023-12-11 09:41:47.000000 imio.history-1.33/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14957 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2304 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio.history.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1111 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4962 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/es/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/es/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      623 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/es/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1129 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      594 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1250 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      260 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      217 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/default/viewlets.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2411 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      717 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/testing-adapter.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1628 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/interfaces.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3108 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/mk_sync_locales.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6524 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      180 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/safe_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2927 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_revisionhistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12241 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_workflowhistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1325 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_versionpreview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1266 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3130 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_documentbylineviewlet.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11337 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_contenthistory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      188 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/static/imiohistory.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7784 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1645 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6233 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/content_history.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      152 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/event_preview.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3408 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/document_byline.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      112 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/header.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/templates/version_preview.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-12-11 09:41:47.000000 imio.history-1.33/src/imio/history/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       50 2023-12-11 09:41:47.000000 imio.history-1.33/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1515 2023-12-11 09:41:47.000000 imio.history-1.33/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14957 2023-12-11 09:41:47.000000 imio.history-1.33/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2023-12-11 09:41:47.000000 imio.history-1.33/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8962 2023-12-11 09:41:47.000000 imio.history-1.33/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2023-12-11 09:41:47.000000 imio.history-1.33/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2023-12-11 09:41:47.000000 imio.history-1.33/versions.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2438 2023-12-11 09:41:47.000000 imio.history-1.33/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       94 2023-12-11 09:41:47.000000 imio.history-1.33/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-12-11 09:41:47.000000 imio.history-1.33/.isort.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-12-11 09:41:47.000000 imio.history-1.33/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2023-12-11 09:41:47.000000 imio.history-1.33/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2023-12-11 09:41:47.000000 imio.history-1.33/ci.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18027 2024-04-10 07:06:36.000000 imio.history-1.34/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15302 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2304 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio.history.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1111 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5059 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      623 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/es/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/es/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1129 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      594 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      523 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1250 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      260 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      217 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/default/viewlets.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      457 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2411 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      717 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/testing-adapter.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1628 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/interfaces.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3108 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/mk_sync_locales.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6551 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      180 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/safe_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      817 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2927 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_revisionhistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12241 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_workflowhistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1325 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_versionpreview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1266 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3130 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_documentbylineviewlet.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11430 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_contenthistory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      584 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      188 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      252 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/static/imiohistory.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7932 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1645 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6243 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/content_history.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      152 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/event_preview.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3408 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/document_byline.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      112 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/header.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       96 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/templates/version_preview.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:06:36.000000 imio.history-1.34/src/imio/history/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       50 2024-04-10 07:06:36.000000 imio.history-1.34/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1515 2024-04-10 07:06:36.000000 imio.history-1.34/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15302 2024-04-10 07:06:36.000000 imio.history-1.34/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2024-04-10 07:06:36.000000 imio.history-1.34/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9235 2024-04-10 07:06:36.000000 imio.history-1.34/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2024-04-10 07:06:36.000000 imio.history-1.34/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      595 2024-04-10 07:06:36.000000 imio.history-1.34/versions.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2438 2024-04-10 07:06:36.000000 imio.history-1.34/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       94 2024-04-10 07:06:36.000000 imio.history-1.34/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-04-10 07:06:36.000000 imio.history-1.34/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-04-10 07:06:36.000000 imio.history-1.34/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-04-10 07:06:36.000000 imio.history-1.34/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      164 2024-04-10 07:06:36.000000 imio.history-1.34/ci.cfg
```

### Comparing `imio.history-1.33/LICENSE.rst` & `imio.history-1.34/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio.history.egg-info/PKG-INFO` & `imio.history-1.34/src/imio.history.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.history
-Version: 1.33
+Version: 1.34
 Summary: Imio history
 Home-page: http://pypi.python.org/pypi/imio.history
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: .. image:: https://github.com/IMIO/imio.history/actions/workflows/main.yml/badge.svg?branch=master
             :target: https://github.com/IMIO/imio.history/actions/workflows/main.yml
@@ -67,14 +67,23 @@
         
         Contributors
         ============
         
         Changelog
         =========
         
+        1.34 (2024-04-10)
+        -----------------
+        
+        - Adapted `utils.getPreviousEvent` to add parameter `history_name='workflow'`.
+          [gbastien]
+        - Fixed display of `HISTORY_COMMENT_NOT_VIEWABLE` in `@@contenthistory` view
+          that was displayed as text, showing the HTML code.
+          [gbastien]
+        
         1.33 (2023-12-11)
         -----------------
         
         - Added `utils.add_event_to_wf_history` to insert an event
           to the `workflow_history` of an element.
           [gbastien]
```

### Comparing `imio.history-1.33/src/imio.history.egg-info/SOURCES.txt` & `imio.history-1.34/src/imio.history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/configure.zcml` & `imio.history-1.34/src/imio/history/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/adapters.py` & `imio.history-1.34/src/imio/history/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             # Make sure original event is not modified
             event = event.copy()
             if self.history_type:
                 event['type'] = self.history_type
 
             if checkMayViewEvent and not self.mayViewEvent(event):
                 continue
+            event['comments_viewable'] = True
             if checkMayViewComment and not self.mayViewComment(event):
+                event['comments_viewable'] = False
                 event['comments'] = self.comment_not_viewable_value
             res.append(event)
         return res
 
     def mayViewComment(self, event):
         """See docstring in interfaces.py."""
         return True
```

### Comparing `imio.history-1.33/src/imio/history/locales/manual.pot` & `imio.history-1.34/src/imio/history/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/es/LC_MESSAGES/plone.po` & `imio.history-1.34/src/imio/history/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/es/LC_MESSAGES/imio.history.po` & `imio.history-1.34/src/imio/history/locales/es/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/imio.history.pot` & `imio.history-1.34/src/imio/history/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/en/LC_MESSAGES/plone.po` & `imio.history-1.34/src/imio/history/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/en/LC_MESSAGES/imio.history.po` & `imio.history-1.34/src/imio/history/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/plone.pot` & `imio.history-1.34/src/imio/history/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/fr/LC_MESSAGES/plone.po` & `imio.history-1.34/src/imio/history/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po` & `imio.history-1.34/src/imio/history/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/testing.py` & `imio.history-1.34/src/imio/history/testing.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/testing-adapter.zcml` & `imio.history-1.34/src/imio/history/testing-adapter.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/interfaces.py` & `imio.history-1.34/src/imio/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/mk_sync_locales.sh` & `imio.history-1.34/src/imio/history/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/utils.py` & `imio.history-1.34/src/imio/history/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
                 event = None
         if checkMayViewComment and event is not None:
             if not adapter.mayViewComment(event):
                 event['comments'] = adapter.comment_not_viewable_value
     return event
 
 
-def getPreviousEvent(obj, event, checkMayViewEvent=False, checkMayViewComment=False):
+def getPreviousEvent(obj, event, history_name='workflow', checkMayViewEvent=False, checkMayViewComment=False):
     '''Returns the previous event found in the history for the given p_event
        on p_obj if p_event is found.  p_checkMayView is passed to IImioHistory.getHistory
        and will enable/disable event's comments viewability check.'''
 
-    adapter = getAdapter(obj, IImioHistory, 'workflow')
+    adapter = getAdapter(obj, IImioHistory, history_name)
     # for performance, checkMayViewEvent and checkMayViewComment only on found event
     history = adapter.getHistory(
         checkMayViewEvent=False, checkMayViewComment=False)
     res = None
     if event in history and history.index(event) > 0:
         res = history[history.index(event) - 1]
```

### Comparing `imio.history-1.33/src/imio/history/config.py` & `imio.history-1.34/src/imio/history/config.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/testing.zcml` & `imio.history-1.34/src/imio/history/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_revisionhistory.py` & `imio.history-1.34/src/imio/history/tests/test_revisionhistory.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_utils.py` & `imio.history-1.34/src/imio/history/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_workflowhistory.py` & `imio.history-1.34/src/imio/history/tests/test_workflowhistory.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_versionpreview.py` & `imio.history-1.34/src/imio/history/tests/test_versionpreview.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/adapters.py` & `imio.history-1.34/src/imio/history/tests/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_documentbylineviewlet.py` & `imio.history-1.34/src/imio/history/tests/test_documentbylineviewlet.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/tests/test_contenthistory.py` & `imio.history-1.34/src/imio/history/tests/test_contenthistory.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,16 @@
         zcml.load_config('testing-adapter.zcml', imio_history)
         self.request.set('hide_wf_history_comment', True)
         history = view.getHistory()
         lastEvent = history[0]
         self.assertEqual(lastEvent['action'], 'publish')
         # now comment is no more viewable
         self.assertEqual(lastEvent['comments'], HISTORY_COMMENT_NOT_VIEWABLE)
+        # correctly rendered
+        self.assertTrue(HISTORY_COMMENT_NOT_VIEWABLE in view())
 
         # getHistory can be called with checkMayViewComment set to False,
         # in this case, mayViewComment check is not done
         history = view.getHistory(checkMayViewComment=False)
         lastEvent = history[0]
         self.assertEqual(lastEvent['action'], 'publish')
         # comment is viewable as mayViewComment was not done
```

### Comparing `imio.history-1.33/src/imio/history/tests/test_setup.py` & `imio.history-1.34/src/imio/history/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/browser/views.py` & `imio.history-1.34/src/imio/history/browser/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,17 @@
         mapping.update(self._extra_render_comments_mapping())
         # try to translate comments before it is turned into text/html
         translated = translate(
             safe_unicode(event['comments']),
             mapping=mapping,
             domain='imio.history',
             context=self.request)
+        # bypass transform when comments not viewable as we have HTML
+        if event['comments_viewable'] is False:
+            return translated
         transformsTool = api.portal.get_tool('portal_transforms')
         data = transformsTool.convertTo(
             'text/x-html-safe', translated, mimetype=mimetype)
         return data.getData()
 
     @memoize
     def _getCurrentContextWorkflow(self):
```

### Comparing `imio.history-1.33/src/imio/history/browser/configure.zcml` & `imio.history-1.34/src/imio/history/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/src/imio/history/browser/templates/content_history.pt` & `imio.history-1.34/src/imio/history/browser/templates/content_history.pt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div id="content" define-macro="history" i18n:domain="plone"
-     tal:condition="view/show_history"
+     tal:condition="python: view.show_history()"
      tal:define="events python: view.getHistory();
                  showColors python: view.showColors();
                  showRevisionInfos python: view.showRevisionInfos();
                  ploneView python: context.restrictedTraverse('@@plone');
                  member python: view.member">
   <tal:block replace="structure python: view.renderCustomJS()"></tal:block>
   <tal:header replace="structure context/@@header" />
```

### Comparing `imio.history-1.33/src/imio/history/browser/templates/document_byline.pt` & `imio.history-1.34/src/imio/history/browser/templates/document_byline.pt`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/setup.py` & `imio.history-1.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'Contributors\n'
     '============\n' + '\n' +
     open('CHANGES.rst').read() + '\n')
 
 
 setup(
     name='imio.history',
-    version='1.33',
+    version='1.34',
     description="Imio history",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.history-1.33/PKG-INFO` & `imio.history-1.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.history
-Version: 1.33
+Version: 1.34
 Summary: Imio history
 Home-page: http://pypi.python.org/pypi/imio.history
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: .. image:: https://github.com/IMIO/imio.history/actions/workflows/main.yml/badge.svg?branch=master
             :target: https://github.com/IMIO/imio.history/actions/workflows/main.yml
@@ -67,14 +67,23 @@
         
         Contributors
         ============
         
         Changelog
         =========
         
+        1.34 (2024-04-10)
+        -----------------
+        
+        - Adapted `utils.getPreviousEvent` to add parameter `history_name='workflow'`.
+          [gbastien]
+        - Fixed display of `HISTORY_COMMENT_NOT_VIEWABLE` in `@@contenthistory` view
+          that was displayed as text, showing the HTML code.
+          [gbastien]
+        
         1.33 (2023-12-11)
         -----------------
         
         - Added `utils.add_event_to_wf_history` to insert an event
           to the `workflow_history` of an element.
           [gbastien]
```

### Comparing `imio.history-1.33/CHANGES.rst` & `imio.history-1.34/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+1.34 (2024-04-10)
+-----------------
+
+- Adapted `utils.getPreviousEvent` to add parameter `history_name='workflow'`.
+  [gbastien]
+- Fixed display of `HISTORY_COMMENT_NOT_VIEWABLE` in `@@contenthistory` view
+  that was displayed as text, showing the HTML code.
+  [gbastien]
+
 1.33 (2023-12-11)
 -----------------
 
 - Added `utils.add_event_to_wf_history` to insert an event
   to the `workflow_history` of an element.
   [gbastien]
```

### Comparing `imio.history-1.33/versions.cfg` & `imio.history-1.34/versions.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 collective.profiler = 0.3
 ecreall.helpers.testing = 1.7
 ipdb = 0.8
 ipython = 3.2.2
 pathtools = 0.1.2
 watchdog = 0.7.1
 pep517 = 0.8.2
+backports.functools-lru-cache = 1.5
+six = 1.16.0
 
 plone.api =
 imio.prettylink =
 future = 0.18.2
 zope.configuration = 3.8.1
 zc.lockfile = 1.2.1
```

### Comparing `imio.history-1.33/README.rst` & `imio.history-1.34/README.rst`

 * *Files identical despite different names*

### Comparing `imio.history-1.33/buildout.cfg` & `imio.history-1.34/buildout.cfg`

 * *Files identical despite different names*

