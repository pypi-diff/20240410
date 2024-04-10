# Comparing `tmp/imio.helpers-1.0.0rc1.tar.gz` & `tmp/imio.helpers-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.helpers-1.0.0rc1.tar", last modified: Thu Feb  8 14:24:58 2024, max compression
+gzip compressed data, was "dist/imio.helpers-1.0.0rc2.tar", last modified: Wed Apr 10 07:05:43 2024, max compression
```

## Comparing `imio.helpers-1.0.0rc1.tar` & `imio.helpers-1.0.0rc2.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/test-5.2.cfg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    50974 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3511 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      427 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   120876 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/appy_pod.html
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3182 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/test_helpers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3314 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/pdf.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1425 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/events.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6803 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/date.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/path.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4367 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4299 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      718 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/manual.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      777 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/update.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1692 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/imio.helpers.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1827 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      237 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3955 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/types/testingtype.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      135 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3381 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4583 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4257 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/workflow.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7567 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/security.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      703 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/interfaces.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2377 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      307 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1206 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/fancytree.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/fancytree.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      727 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10286 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/cache.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32835 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/xhtml.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      942 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/barcode.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3332 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/ram.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1768 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/appy_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1377 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6380 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1025 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/testing.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3378 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      861 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/imageNotFound.jpg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5628 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_workflow.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3187 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      298 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      156 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/barcode_python3_zint_60x60_156bytes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26968 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_content.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      890 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_barcode.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23067 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_cache.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/barcode_python2_zint_60x60_278bytes.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2972 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_fancytree.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10661 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_transmogrifier.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12452 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3710 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_date.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54032 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_xhtml.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      751 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/dot.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      647 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1547 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_converters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10665 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_email.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4527 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_security.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4852 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      498 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_path.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1918 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_appy_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    27621 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/content.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3721 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7386 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/transmogrifier.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5527 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/ramcache.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7485 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/static/helpers.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1006 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/static/listings.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2524 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1712 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1490 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/content.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      656 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/folder_listing.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3529 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/container.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1690 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/browser/folder_listing_table.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8575 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/emailer.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/converters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3252 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/helpers/patches.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      269 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/src/imio/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/gha.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       85 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/requirements-6.0.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/checkouts.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2366 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/test-4.3.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       32 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2389 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1379 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/test-6.0.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    50974 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       91 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/requirements-5.2.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    39028 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2286 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/base.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      835 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/sources.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      886 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      142 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/.isort.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3367 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-02-08 14:24:58.000000 imio.helpers-1.0.0rc1/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       65 2024-02-08 14:24:57.000000 imio.helpers-1.0.0rc1/requirements-4.3.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1224 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/test-5.2.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    52005 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3566 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      425 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   120876 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/appy_pod.html
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3182 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/test_helpers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3314 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/pdf.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1425 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/events.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6803 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/date.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/path.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8643 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/batching.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4730 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4299 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      718 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/manual.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      777 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1692 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/imio.helpers.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1827 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      237 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3955 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/types/testingtype.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/types.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      135 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3381 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4583 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4257 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/workflow.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7567 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/security.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      703 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/interfaces.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2377 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      307 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1206 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/fancytree.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      546 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/fancytree.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      727 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10286 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/cache.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    32835 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/xhtml.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      942 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/barcode.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3332 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/ram.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1768 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/appy_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1377 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6380 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1025 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/testing.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3378 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      861 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/imageNotFound.jpg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5628 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_workflow.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      464 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3187 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      298 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      156 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/barcode_python3_zint_60x60_156bytes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8400 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_batching.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26618 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_content.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      890 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_barcode.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23067 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_cache.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      278 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/barcode_python2_zint_60x60_278bytes.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2972 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_fancytree.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10661 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_transmogrifier.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12452 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3710 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_date.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54032 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_xhtml.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      751 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      873 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/dot.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      647 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1547 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_converters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10665 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_email.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4527 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_security.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4852 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      498 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_path.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1918 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_appy_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    27499 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/content.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3925 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8605 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/transmogrifier.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5527 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/ramcache.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7791 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/static/helpers.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1006 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/static/listings.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3816 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2582 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1490 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/content.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      656 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/folder_listing.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3529 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/container.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1690 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/browser/folder_listing_table.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8628 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/emailer.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/converters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4704 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/helpers/patches.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      269 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/src/imio/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/gha.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       85 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/requirements-6.0.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2292 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/test-4.3.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       32 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2387 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1379 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/test-6.0.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    52005 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       91 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/requirements-5.2.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    39883 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2303 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/base.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      933 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/sources.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      886 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      142 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3367 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       65 2024-04-10 07:05:43.000000 imio.helpers-1.0.0rc2/requirements-4.3.txt
```

### Comparing `imio.helpers-1.0.0rc1/test-5.2.cfg` & `imio.helpers-1.0.0rc2/test-5.2.cfg`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/PKG-INFO` & `imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.helpers
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Various helper methods for development.
 Home-page: https://github.com/imio/imio.helpers
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
 Download-URL: https://pypi.org/project/imio.helpers
 Description: .. image:: https://github.com/IMIO/imio.helpers/actions/workflows/main.yml/badge.svg?branch=master
@@ -38,14 +38,36 @@
         
         Use cache.get_plone_groups_for_user(the_objects=True) instead portal_groups.getGroupsForPrincipal
         Avoid portal_groups.getGroupById but use source_groups.get
         
         Changelog
         =========
         
+        1.0.0rc2 (2024-04-10)
+        ---------------------
+        
+        - Added batching module.
+          [sgeulette]
+        - Fixed the way JS function `submitFormHelperOnsuccessDefault` manages
+          returned result when it is a file, now we have a correct `filename`.
+          [gbastien]
+        - Added transmogrifier Expression and Condition classes to log expression
+          compilation or interpretation errors.
+          [sgeulette]
+        - Removed `content.safe_encode` as already defined in `imio.pyutils`.
+          Import it from `imio.pyutils` in `imio.helpers.content` for temporary backward
+          compatibility, to be removed.
+          [gbastien]
+        - Overrided `@@folder_contents` to make it work with `DashboardCollection`.
+          [gbastien]
+        - Monkeypatched `plone.app.querystring.registryreader.getVocabularyValues`
+          to keep vocabulary order onloy for Plone4, behavior is correct in Plone5+.
+          Manage every `HAS_PLONE_X` values.
+          [gbastien]
+        
         1.0.0rc1 (2024-02-08)
         ---------------------
         
         - Made compliant with Plone 4, Plone 5, Plone 6
           [boulch, laulaz, sgeulette]
         - Require `pathlib2` in `setup.py`, backport `pathlib` for `py2.7`.
           [gbastien]
```

### Comparing `imio.helpers-1.0.0rc1/src/imio.helpers.egg-info/SOURCES.txt` & `imio.helpers-1.0.0rc2/src/imio.helpers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .coveragerc
 .isort.cfg
 CHANGES.rst
 MANIFEST.in
 Makefile
 README.rst
 base.cfg
-checkouts.cfg
 gha.cfg
 requirements-4.3.txt
 requirements-5.2.txt
 requirements-6.0.txt
 requirements.txt
 setup.py
 sources.cfg
@@ -28,14 +27,15 @@
 src/imio.helpers.egg-info/requires.txt
 src/imio.helpers.egg-info/top_level.txt
 src/imio/helpers/__init__.py
 src/imio/helpers/adapters.py
 src/imio/helpers/appy_pod.html
 src/imio/helpers/appy_pod.py
 src/imio/helpers/barcode.py
+src/imio/helpers/batching.py
 src/imio/helpers/cache.py
 src/imio/helpers/catalog.py
 src/imio/helpers/configure.zcml
 src/imio/helpers/content.py
 src/imio/helpers/converters.py
 src/imio/helpers/date.py
 src/imio/helpers/emailer.py
@@ -85,14 +85,15 @@
 src/imio/helpers/tests/__init__.py
 src/imio/helpers/tests/barcode_python2_zint_60x60_278bytes.png
 src/imio/helpers/tests/barcode_python3_zint_60x60_156bytes.png
 src/imio/helpers/tests/dot.gif
 src/imio/helpers/tests/indexes.py
 src/imio/helpers/tests/test_appy_pod.py
 src/imio/helpers/tests/test_barcode.py
+src/imio/helpers/tests/test_batching.py
 src/imio/helpers/tests/test_cache.py
 src/imio/helpers/tests/test_catalog.py
 src/imio/helpers/tests/test_content.py
 src/imio/helpers/tests/test_converters.py
 src/imio/helpers/tests/test_date.py
 src/imio/helpers/tests/test_email.py
 src/imio/helpers/tests/test_fancytree.py
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/appy_pod.html` & `imio.helpers-1.0.0rc2/src/imio/helpers/appy_pod.html`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/test_helpers.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/pdf.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/pdf.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/events.zcml` & `imio.helpers-1.0.0rc2/src/imio/helpers/events.zcml`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/date.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/date.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/configure.zcml` & `imio.helpers-1.0.0rc2/src/imio/helpers/configure.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,21 @@
     <monkey:patch
         description="Monkeypatch _listAllowedRolesAndUsers to add ram.cache on '_users_groups_value'"
         class="Products.CMFPlone.CatalogTool.CatalogTool"
         original="_listAllowedRolesAndUsers"
         replacement=".patches._listAllowedRolesAndUsers"
         preserveOriginal="true" />
 
+    <monkey:patch zcml:condition="not-have plone-5"
+        description="Monkeypatch getVocabularyValues from plone.app.querystring to keep vocabulary order"
+        class="plone.app.querystring.registryreader.QuerystringRegistryReader"
+        original="getVocabularyValues"
+        replacement=".patches.getVocabularyValues"
+        preserveOriginal="true" />
+
     <utility component=".vocabularies.SortedUsersFactory"
              name="imio.helpers.SortedUsers" />
 
     <utility component=".vocabularies.SimplySortedUsersFactory"
              name="imio.helpers.SimplySortedUsers" />
 
     <utility name="imio.helpers.YesNoForFacetedVocabulary"
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/adapters.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/locales/manual.pot` & `imio.helpers-1.0.0rc2/src/imio/helpers/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/locales/update.sh` & `imio.helpers-1.0.0rc2/src/imio/helpers/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/locales/imio.helpers.pot` & `imio.helpers-1.0.0rc2/src/imio/helpers/locales/imio.helpers.pot`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po` & `imio.helpers-1.0.0rc2/src/imio/helpers/locales/fr/LC_MESSAGES/imio.helpers.po`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/profiles/testing/types/testingtype.xml` & `imio.helpers-1.0.0rc2/src/imio/helpers/profiles/testing/types/testingtype.xml`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/testing.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/testing.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/setup.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/setup.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/workflow.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/workflow.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/security.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/security.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/interfaces.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/views.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/views.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/fancytree.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/fancytree.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/fancytree/fancytree.js` & `imio.helpers-1.0.0rc2/src/imio/helpers/fancytree/fancytree.js`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/utils.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/cache.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/xhtml.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/xhtml.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/barcode.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/barcode.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/ram.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/ram.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/appy_pod.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/appy_pod.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/events.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/events.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/catalog.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/catalog.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/testing.zcml` & `imio.helpers-1.0.0rc2/src/imio/helpers/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/vocabularies.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/imageNotFound.jpg` & `imio.helpers-1.0.0rc2/src/imio/helpers/imageNotFound.jpg`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_workflow.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_vocabularies.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_content.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from imio.helpers.content import get_vocab_values
 from imio.helpers.content import normalize_name
 from imio.helpers.content import object_ids
 from imio.helpers.content import object_values
 from imio.helpers.content import restore_link_integrity_checks
 from imio.helpers.content import richtextval
 from imio.helpers.content import safe_delattr
-from imio.helpers.content import safe_encode
 from imio.helpers.content import set_to_annotation
 from imio.helpers.content import sort_on_vocab_order
 from imio.helpers.content import uuidsToCatalogBrains
 from imio.helpers.content import uuidsToObjects
 from imio.helpers.content import uuidToCatalogBrain
 from imio.helpers.content import uuidToObject
 from imio.helpers.content import validate_fields
@@ -229,20 +228,14 @@
                              [WrongType(None, six.text_type, 'mandatory_textline')])
         # validate_fields may raise a ValueError if raise_on_errors=True
         self.assertRaises(ValueError, validate_fields, obj, raise_on_errors=True)
         # back to correct value
         obj.mandatory_textline = u'Some text'
         self.assertFalse(validate_fields(obj))
 
-    def test_safe_encode(self):
-        self.assertEqual(safe_encode('héhé'), 'héhé')
-        self.assertEqual(safe_encode(u'héhé'), 'héhé')
-        self.assertEqual(safe_encode(u'héhé', encoding='utf8'), 'héhé')
-        self.assertEqual(safe_encode('héhé', encoding='whatelse'), 'héhé')
-
     def test_add_and_remove_annotation(self):
         obj = api.content.create(container=self.portal.folder,
                                  id='tt',
                                  type='testingtype',
                                  enabled='Should be a boolean')
         fakeUid = obj.UID()
         api.content.delete(obj)
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_barcode.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_barcode.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_cache.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_fancytree.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_fancytree.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_transmogrifier.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_transmogrifier.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_catalog.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_date.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_xhtml.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_xhtml.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/utils.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/utils.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/dot.gif` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/dot.gif`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/vocabularies.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_converters.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_email.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_security.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_setup.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/tests/test_appy_pod.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/tests/test_appy_pod.py`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/content.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # -*- coding: utf-8 -*-
 
+from imio.helpers import HAS_PLONE_5_AND_MORE
 from imio.helpers.interfaces import IContainerOfUnindexedElementsMarker
 from imio.helpers.workflow import do_transitions
+from imio.pyutils.utils import safe_encode  # noqa, temporary import for backward compatibility as was also defined here
 from imio.pyutils.utils import sort_by_indexes
 from persistent.list import PersistentList
 from plone import api
 from plone.api.content import _parse_object_provides_query
 from plone.api.validation import mutually_exclusive_parameters
 from plone.app.textfield.value import RichTextValue
 from plone.behavior.interfaces import IBehavior
 from plone.i18n.normalizer.interfaces import IUserPreferredURLNormalizer
 from plone.namedfile.file import NamedBlobFile
 from plone.namedfile.file import NamedBlobImage
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.interfaces import IPropertiesTool
 from Products.CMFPlone.utils import base_hasattr
-from Products.CMFPlone.utils import getFSVersionTuple
 from Products.CMFPlone.utils import safe_unicode
 from zc.relation.interfaces import ICatalog
 from zope.annotation import IAnnotations
 from zope.component import getUtility
 from zope.component import queryUtility
 from zope.interface.interfaces import IMethod
 from zope.intid.interfaces import IIntIds
 from zope.schema._field import Bool
 from zope.schema.interfaces import IVocabularyFactory
 
 import logging
 import os
-import six
 
 
-HAS_PLONE5 = bool(getFSVersionTuple()[0] >= 5)
-if HAS_PLONE5:
+if HAS_PLONE_5_AND_MORE:
     from Products.CMFPlone.interfaces import IEditingSchema
 
 logger = logging.getLogger('imio.helpers.content')
 ADDED_TYPE_ERROR = 'A validation error occurred while instantiating "{0}" with id "{1}". {2}'
 
 
 def get_object(parent='', oid='', title='', ptype='', obj_path=''):
@@ -275,21 +274,14 @@
     if raise_on_errors and errors:
         error_msg = ADDED_TYPE_ERROR.format(
             obj.portal_type, obj.id, '\n'.join([repr(error) for error in errors]))
         raise ValueError(error_msg)
     return errors
 
 
-def safe_encode(value, encoding='utf-8'):
-    """
-        Converts a value to encoding, only when it is not already encoded.
-    """
-    return six.ensure_str(value, encoding=encoding)
-
-
 @mutually_exclusive_parameters('obj', 'uid')
 def add_to_annotation(annotation_key, value, obj=None, uid=None):
     """ Add annotation related to obj or uid """
     if not obj:
         obj = api.content.get(UID=uid)
         # api.content.get may return None
         if not obj:
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/__init__.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 import logging
 import os
 
 
 _ = MessageFactory('imio.helpers')
 logger = logging.getLogger('imio.helpers')
 
+HAS_PLONE_4 = api.env.plone_version().startswith('4')
+HAS_PLONE_5 = api.env.plone_version().startswith('5')
+HAS_PLONE_5_1 = api.env.plone_version() > '5.1'
+HAS_PLONE_5_2 = api.env.plone_version() > '5.2'
 HAS_PLONE_5_AND_MORE = int(api.env.plone_version()[0]) >= 5
 PLONE_MAJOR_VERSION = int(api.env.plone_version()[0])
 
 
 def GroupsTool__getGroupsForPrincipal_cachekey(method, self, principal):
     req = getRequest()
     if req is None:
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/transmogrifier.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/transmogrifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # -*- coding: utf-8 -*-
+
 from copy import deepcopy
 from datetime import datetime
-from imio.helpers.content import safe_encode
 from imio.pyutils.utils import letters_sequence
+from imio.pyutils.utils import safe_encode
 from Products.CMFPlone.utils import safe_unicode
 from six.moves import range
 from six.moves import zip
+from zope.tales.tales import CompilerError
 
+import logging
 import os
 import re
 
 
+logger = logging.getLogger('imio.helpers: transmogrifier')
+
+
 def clean_value(value, isep=u'\n', strip=u' ', patterns=(), osep=None):
     """Clean unicode multiline value
 
     :param value: input string
     :param isep: input separator
     :param strip: chars to strip on each "line"
     :param patterns: tuple line patterns list to remove ("line" evaluation) (tuple = search, replace)
@@ -227,7 +233,37 @@
         if max_val and dt > max_val:
             # raise ValueError(u"Given date '{}' > maximum value '{}' => set to None".format(val, max_val))
             raise ValueError
     except ValueError as ex:
         log_method(item, u"not a valid date '{}' in key '{}': {}".format(val, key, ex), **log_params)
         return None
     return dt
+
+
+try:
+    from collective.transmogrifier.utils import Expression as OrigExpression
+
+    class Expression(OrigExpression):
+        """Call the expression and log the expression"""
+
+        def __init__(self, expression, transmogrifier, name, options, **extras):
+            try:
+                super(Expression, self).__init__(expression, transmogrifier, name, options, **extras)
+            except CompilerError as e:
+                logger.error("Error in part '{}', expression: '{}': {}".format(name, expression, e))
+                raise e
+
+        def __call__(self, item, **extras):
+            try:
+                return super(Expression, self).__call__(item, **extras)
+            except Exception as e:
+                logger.error("Error in part '{}', expression: '{}': {}".format(self.name, self.expression.text, e))
+                raise e
+
+    class Condition(Expression):
+        """A transmogrifier condition expression with logging"""
+
+        def __call__(self, item, **extras):
+            return bool(super(Condition, self).__call__(item, **extras))
+
+except ImportError:
+    pass
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/ramcache.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/ramcache.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/static/helpers.js` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/static/helpers.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -202,22 +202,28 @@
 
 function submitFormHelperOnsuccessDefault(data, textStatus, request) {
     cancel_button = $('input#form-buttons-cancel');
     // download file if 'content-disposition' header found
     contentType = request.getResponseHeader('content-type');
     if (contentType && contentType.startsWith('application')) {
         data = new Uint8Array(data);
+        // to be able to download the blob and set a correct filename
+        // we need to add a fictious link (a), click on it then remove it...
         contentType = request.getResponseHeader('content-type');
+        fileName = request.getResponseHeader('Content-Disposition').split("filename=")[1];
         var blob = new Blob([data], {
             type: contentType
         });
-        var objectUrl = URL.createObjectURL(blob);
-        window.open(objectUrl);
+        var link = document.createElement('a');
+        link.href = URL.createObjectURL(blob);
+        link.download = fileName;
+        document.body.appendChild(link);
+        link.click();
+        link.remove();
         cancel_button.click();
-        URL.revokeObjectURL(objectUrl);
     } else {
         // close the overlay
         if (cancel_button) {
             cancel_button.click();
         }
         // reload faceted
         if (has_faceted()) {
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/static/listings.js` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/static/listings.js`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/configure.zcml` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/configure.zcml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
     i18n_domain="imio.helpers">
 
     <!-- Publish static files -->
     <browser:resourceDirectory
       name="imio.helpers"
       directory="static"
       />
@@ -40,8 +41,27 @@
         name="caching-controlpanel-ramcache"
         for="Products.CMFPlone.interfaces.IPloneSiteRoot"
         class=".views.IMIORAMCache"
         template="ramcache.pt"
         layer="imio.helpers.interfaces.IIMIOHelpersLayer"
         permission="cmf.ManagePortal" />
 
+    <!-- Override @@folder_contents to work with DashboardCollection -->
+    <!-- Folder contents -->
+    <configure package="plone.app.content" zcml:condition="not-have plone-5">
+        <browser:page
+            for="*"
+            class="imio.helpers.browser.views.IMIOFolderContentsView"
+            name="folder_contents"
+            template="browser/folder_contents.pt"
+            layer="imio.helpers.interfaces.IIMIOHelpersLayer"
+            permission="cmf.ListFolderContents" />
+        <browser:page
+            for="*"
+            class="imio.helpers.browser.views.IMIOFolderContentsBrowserView"
+            attribute="update_table"
+            name="foldercontents_get_table"
+            layer="imio.helpers.interfaces.IIMIOHelpersLayer"
+            permission="cmf.ListFolderContents" />
+    </configure>
+
 </configure>
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/content.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/content.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/folder_listing.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/folder_listing.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/container.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/container.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/browser/folder_listing_table.pt` & `imio.helpers-1.0.0rc2/src/imio/helpers/browser/folder_listing_table.pt`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/emailer.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/emailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from email import encoders
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import parseaddr
 from imio.helpers import _
-from imio.helpers.content import safe_encode
+from imio.pyutils.utils import safe_encode
 from plone import api
 from smtplib import SMTPException
 from unidecode import unidecode
 from zope import schema
 from zope.component import getMultiAdapter
 
 import csv
@@ -153,14 +153,15 @@
         kwargs['mbcc'] = mbcc
     if replyto is not None:
         kwargs['reply-to'] = replyto
     try:
         # secureSend is protected by permission 'Use mailhost'
         # secureSend is deprecated and patched in Products/CMFPlone/patches/securemailhost.py
         # send remove from headers bcc !!
+        # TODO replace securesend by send with headers
         mail_host.secureSend(eml, mto, mfrom, subject=subject, charset=charset, **kwargs)
     except (socket.error, SMTPException) as e:
         logger.error(u"Could not send email to '{}' with subject '{}': {}".format(mto, subject, e))
         return False, 'Could not send email : {}'.format(e)
     # sent successfully
     return True, ''
```

### Comparing `imio.helpers-1.0.0rc1/src/imio/helpers/patches.py` & `imio.helpers-1.0.0rc2/src/imio/helpers/patches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from imio.helpers import HAS_PLONE_4
 from imio.helpers.cache import get_cachekey_volatile
 from imio.helpers.cache import get_plone_groups_for_user
 from imio.helpers.cache import invalidate_cachekey_volatile_for
 from plone.api.exc import InvalidParameterError
 from plone.memoize import ram
 from Products.PlonePAS.plugins.role import GroupAwareRoleManager
 from Products.PluggableAuthService.plugins.ZODBRoleManager import ZODBRoleManager
@@ -82,7 +83,41 @@
     if groups:
         groups = ['user:%s' % x for x in groups]
         result = result + groups
     # Order the arguments from small to large sets
     result.insert(0, 'user:%s' % user.getId())
     result.append('Anonymous')
     return result
+
+
+if HAS_PLONE_4:
+    from operator import attrgetter
+    from plone.app.querystring.registryreader import logger
+    from zope.component import queryUtility
+    from zope.i18n import translate
+    from zope.i18nmessageid import Message
+    from zope.schema.interfaces import IVocabularyFactory
+
+    def getVocabularyValues(self, values):
+        """Get all vocabulary values if a vocabulary is defined"""
+
+        for field in values.get(self.prefix + '.field').values():
+            # XXX begin change by imio.helpers
+            # field['values'] = {}
+            from collections import OrderedDict
+            field['values'] = OrderedDict()
+            # XXX end change by imio.helpers
+            vocabulary = field.get('vocabulary', [])
+            if vocabulary:
+                utility = queryUtility(IVocabularyFactory, vocabulary)
+                if utility is not None:
+                    for item in sorted(utility(self.context),
+                                       key=attrgetter('title')):
+                        if isinstance(item.title, Message):
+                            title = translate(item.title, context=self.request)
+                        else:
+                            title = item.title
+
+                        field['values'][item.value] = {'title': title}
+                else:
+                    logger.info("%s is missing, ignored." % vocabulary)
+        return values
```

### Comparing `imio.helpers-1.0.0rc1/docs/LICENSE.rst` & `imio.helpers-1.0.0rc2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/docs/LICENSE.GPL` & `imio.helpers-1.0.0rc2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/test-4.3.cfg` & `imio.helpers-1.0.0rc2/test-4.3.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -115,10 +115,7 @@
 # Required by:
 # collective.fingerpointing==1.8.3
 file-read-backwards = 2.0.0
 
 # Required by:
 # Pillow==4.0.0
 olefile = 0.46
-
-# Added by buildout at 2023-11-28 16:14:08.561451
-imio.pyutils = 1.0.0a0
```

### Comparing `imio.helpers-1.0.0rc1/setup.py` & `imio.helpers-1.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 long_description = (
     open('README.rst').read() + '\n' + open('CHANGES.rst').read() + '\n')
 
 setup(
     name='imio.helpers',
-    version='1.0.0rc1',
+    version='1.0.0rc2',
     description="Various helper methods for development.",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -40,15 +40,15 @@
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'collective.fingerpointing',
         'collective.monkeypatcher',
         'future>=0.18.2',
-        'imio.pyutils>=1.0.0a0',
+        'imio.pyutils>=1.0.0',
         'natsort<7',
         "pathlib2;python_version<'3'",
         'plone.api>1.9.1',
         'plone.app.intid',
         'plone.app.relationfield',
         'plone.dexterity',
         'setuptools',
```

### Comparing `imio.helpers-1.0.0rc1/test-6.0.cfg` & `imio.helpers-1.0.0rc2/test-6.0.cfg`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/PKG-INFO` & `imio.helpers-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.helpers
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Various helper methods for development.
 Home-page: https://github.com/imio/imio.helpers
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL
 Download-URL: https://pypi.org/project/imio.helpers
 Description: .. image:: https://github.com/IMIO/imio.helpers/actions/workflows/main.yml/badge.svg?branch=master
@@ -38,14 +38,36 @@
         
         Use cache.get_plone_groups_for_user(the_objects=True) instead portal_groups.getGroupsForPrincipal
         Avoid portal_groups.getGroupById but use source_groups.get
         
         Changelog
         =========
         
+        1.0.0rc2 (2024-04-10)
+        ---------------------
+        
+        - Added batching module.
+          [sgeulette]
+        - Fixed the way JS function `submitFormHelperOnsuccessDefault` manages
+          returned result when it is a file, now we have a correct `filename`.
+          [gbastien]
+        - Added transmogrifier Expression and Condition classes to log expression
+          compilation or interpretation errors.
+          [sgeulette]
+        - Removed `content.safe_encode` as already defined in `imio.pyutils`.
+          Import it from `imio.pyutils` in `imio.helpers.content` for temporary backward
+          compatibility, to be removed.
+          [gbastien]
+        - Overrided `@@folder_contents` to make it work with `DashboardCollection`.
+          [gbastien]
+        - Monkeypatched `plone.app.querystring.registryreader.getVocabularyValues`
+          to keep vocabulary order onloy for Plone4, behavior is correct in Plone5+.
+          Manage every `HAS_PLONE_X` values.
+          [gbastien]
+        
         1.0.0rc1 (2024-02-08)
         ---------------------
         
         - Made compliant with Plone 4, Plone 5, Plone 6
           [boulch, laulaz, sgeulette]
         - Require `pathlib2` in `setup.py`, backport `pathlib` for `py2.7`.
           [gbastien]
```

### Comparing `imio.helpers-1.0.0rc1/CHANGES.rst` & `imio.helpers-1.0.0rc2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 Changelog
 =========
 
+1.0.0rc2 (2024-04-10)
+---------------------
+
+- Added batching module.
+  [sgeulette]
+- Fixed the way JS function `submitFormHelperOnsuccessDefault` manages
+  returned result when it is a file, now we have a correct `filename`.
+  [gbastien]
+- Added transmogrifier Expression and Condition classes to log expression
+  compilation or interpretation errors.
+  [sgeulette]
+- Removed `content.safe_encode` as already defined in `imio.pyutils`.
+  Import it from `imio.pyutils` in `imio.helpers.content` for temporary backward
+  compatibility, to be removed.
+  [gbastien]
+- Overrided `@@folder_contents` to make it work with `DashboardCollection`.
+  [gbastien]
+- Monkeypatched `plone.app.querystring.registryreader.getVocabularyValues`
+  to keep vocabulary order onloy for Plone4, behavior is correct in Plone5+.
+  Manage every `HAS_PLONE_X` values.
+  [gbastien]
+
 1.0.0rc1 (2024-02-08)
 ---------------------
 
 - Made compliant with Plone 4, Plone 5, Plone 6
   [boulch, laulaz, sgeulette]
 - Require `pathlib2` in `setup.py`, backport `pathlib` for `py2.7`.
   [gbastien]
```

### Comparing `imio.helpers-1.0.0rc1/base.cfg` & `imio.helpers-1.0.0rc2/base.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 #     os.environ['TZ'] = 'UTC'
 # defaults = ['-s', 'PACKAGE_NAME', '--auto-color', '--auto-progress']
 
 always-checkout = force
 auto-checkout +=
     appy
     collective.behavior.talcondition
+    imio.pyutils
 
 [testenv]
 decorate_acl_methods = true
 
 [omelette]
 recipe = collective.recipe.omelette
 eggs = ${test:eggs}
```

### Comparing `imio.helpers-1.0.0rc1/sources.cfg` & `imio.helpers-1.0.0rc2/sources.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 vincentfretin_push = git@github.com:vincentfretin
 cedricmessiant = https://github.com/cedricmessiant
 cedricmessiant_push = git@github.com:cedricmessiant
 
 [sources]
 appy = git ${remotes:imio}/appy.git pushurl=${remotes:imio_push}/appy.git
 collective.behavior.talcondition = git ${remotes:collective}/collective.behavior.talcondition.git pushurl=${remotes:collective_push}/collective.behavior.talcondition.git
+imio.pyutils = git ${remotes:imio}/imio.pyutils.git pushurl=${remotes:imio_push}/imio.pyutils.git
```

### Comparing `imio.helpers-1.0.0rc1/README.rst` & `imio.helpers-1.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `imio.helpers-1.0.0rc1/Makefile` & `imio.helpers-1.0.0rc2/Makefile`

 * *Files identical despite different names*

