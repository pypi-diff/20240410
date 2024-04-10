# Comparing `tmp/Products.CPUtils-1.24.tar.gz` & `tmp/Products.CPUtils-1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.CPUtils-1.24.tar", last modified: Mon Feb 12 14:15:22 2024, max compression
+gzip compressed data, was "dist/Products.CPUtils-1.25.tar", last modified: Wed Apr 10 07:10:57 2024, max compression
```

## Comparing `Products.CPUtils-1.24.tar` & `Products.CPUtils-1.25.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/
--rw-rw-r--   0 sge       (1000) sge       (1000)       83 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/.coveragerc
--rw-rw-r--   0 sge       (1000) sge       (1000)      131 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/.isort.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     6424 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      505 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)      218 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/Makefile
--rw-rw-r--   0 sge       (1000) sge       (1000)     7520 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      444 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)     2754 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/buildout.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      101 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/ci.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      732 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       57 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1580 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/Extensions/
--rw-rw-r--   0 sge       (1000) sge       (1000)       26 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/Extensions/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     9331 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py
--rw-rw-r--   0 sge       (1000) sge       (1000)   185361 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/Extensions/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     5728 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/QITool.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)    17516 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2970 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/config.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      384 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/data/
--rw-rw-r--   0 sge       (1000) sge       (1000)      248 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/data/robots.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      922 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/fckpatch.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      654 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/hiddenProductsList.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)      336 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/locales/cputils.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)      621 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/model/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7753 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/model/CPUtils.zargo
--rw-rw-r--   0 sge       (1000) sge       (1000)    35679 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/model/archgenxml.log
--rw-rw-r--   0 sge       (1000) sge       (1000)     2978 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/model/generate.conf
--rwxrwxr-x   0 sge       (1000) sge       (1000)       80 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/model/generate.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      491 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/plone3.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)       51 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/default/cputils_default.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      255 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/default/import_steps.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)       78 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      320 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/default/skins.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/profiles/robots/
--rw-rw-r--   0 sge       (1000) sge       (1000)       51 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/robots/cputils_robots.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      378 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles/robots/import_steps.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      648 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/profiles.zcml
--rwxrwxr-x   0 sge       (1000) sge       (1000)      360 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/readme.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/refresh.txt
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/scripts/
--rw-rw-r--   0 sge       (1000) sge       (1000)      235 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/INSTANCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2822 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkInstances.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      280 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkInstances.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     7602 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkPOSKeyErrors.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      289 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkPOSKeyErrors.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)    10049 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_backup_db.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      416 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_backup_db.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     2992 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_db.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      239 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_db.sh
--rwxrwxr-x   0 sge       (1000) sge       (1000)     1197 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_zeo.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      939 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_zeo.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)    11951 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/restore_db.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      264 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/restore_db.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     2251 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/send_log.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      197 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/send_log.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     8598 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/test_db.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      255 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/test_db.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     7491 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/update_awstats.py
--rw-rw-r--   0 sge       (1000) sge       (1000)    10241 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6874 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/zope_restart.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)      334 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/scripts/zope_restart.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)     2152 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/setuphandlers.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products/CPUtils/skins/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/skins/CPUtils/
--rw-rw-r--   0 sge       (1000) sge       (1000)      340 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/skins/CPUtils/readme.txt
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.564391 Products.CPUtils-1.24/src/Products/CPUtils/tests/
--rwxrwxr-x   0 sge       (1000) sge       (1000)     3576 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/CPUtilsTestCase.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)       24 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/__init__.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)     3152 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/framework.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)     4987 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/testMethods.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2252 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/testNewsLetter.py
--rwxrwxr-x   0 sge       (1000) sge       (1000)     1939 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/tests/test_functional.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2267 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/utils.py
--rw-rw-r--   0 sge       (1000) sge       (1000)       12 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/CPUtils/version.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2024-02-12 14:15:22.560391 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     7520 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2996 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        9 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      130 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        9 2024-02-12 14:15:22.000000 Products.CPUtils-1.24/src/Products.CPUtils.egg-info/top_level.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10011 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2996 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      150 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products.CPUtils.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2152 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/skins/CPUtils/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      340 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/skins/CPUtils/readme.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      360 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/readme.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      384 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      491 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/plone3.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      336 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/locales/cputils.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       78 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/default/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/default/cputils_default.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/default/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/robots/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/robots/cputils_robots.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      378 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles/robots/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       12 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/version.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/hiddenProductsList.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2267 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/model/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35679 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/model/archgenxml.log
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7753 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/model/CPUtils.zargo
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       80 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/model/generate.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2978 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/model/generate.conf
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      289 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkPOSKeyErrors.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      416 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_backup_db.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1197 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_zeo.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      239 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_db.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8598 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/test_db.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      280 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkInstances.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6874 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/zope_restart.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      264 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/restore_db.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2822 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkInstances.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11951 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/restore_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10241 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7491 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/update_awstats.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      939 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_zeo.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/test_db.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      197 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/send_log.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      334 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/zope_restart.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10049 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_backup_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7602 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkPOSKeyErrors.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2992 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2251 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/send_log.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/scripts/INSTANCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2970 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/refresh.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   185505 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/Extensions/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9331 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/Extensions/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      922 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/fckpatch.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     4987 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/testMethods.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3576 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/CPUtilsTestCase.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1939 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/test_functional.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3152 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/framework.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       24 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2252 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/tests/testNewsLetter.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/data/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/data/robots.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17516 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5728 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/QITool.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      648 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/CPUtils/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       57 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1611 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10011 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      505 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6520 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       83 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2754 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      101 2024-04-10 07:10:57.000000 Products.CPUtils-1.25/ci.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Products.CPUtils-1.24/CHANGES.rst` & `Products.CPUtils-1.25/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+1.25 (2024-04-10)
+-----------------
+
+- Imported `safe_encode` from imio.pyutils.
+  [sgeulette]
+
 1.24 (2024-02-12)
 -----------------
 
 - Improved `set_attr`.
   [sgeulette]
 - Added `obj_from_uid`
   [sgeulette]
```

### Comparing `Products.CPUtils-1.24/buildout.cfg` & `Products.CPUtils-1.25/buildout.cfg`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/docs/LICENSE.GPL` & `Products.CPUtils-1.25/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/docs/LICENSE.rst` & `Products.CPUtils-1.25/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/setup.py` & `Products.CPUtils-1.25/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     + '\n\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='Products.CPUtils',
-    version='1.24',
+    version='1.25',
     description="Some plone utilities as external methods, monkey patches, etc.",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -35,14 +35,15 @@
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['Products'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'imio.helpers',
+        'imio.pyutils>=1.0.0',
         'plone.api',
         'setuptools',
     ],
     extras_require={
         'test': [
             'plone.app.testing',
             'plone.app.robotframework',
```

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py` & `Products.CPUtils-1.25/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/Extensions/utils.py` & `Products.CPUtils-1.25/src/Products/CPUtils/Extensions/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # utilities
 
-from imio.helpers.content import safe_encode
 from imio.helpers.security import check_zope_admin
+from imio.pyutils.utils import safe_encode
 from plone.app.uuid.utils import uuidToObject
 from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
 
 
 def get_users(self, obj=True):
     from Products.CMFCore.utils import getToolByName
@@ -85,20 +85,21 @@
     return allSiteObj
 
 
 def sendmail(self, mfrom="", to="", body="", subject="", cc="", bcc=""):
     """
         send a mail
     """
+    from email.Header import Header
     from Products.CMFCore.utils import getToolByName
-    from Products.CPUtils.config import PLONE_VERSION
     from Products.CMFPlone.utils import safe_unicode
+    from Products.CPUtils.config import PLONE_VERSION
+
     import email.Message
     import email.Utils
-    from email.Header import Header
 
     portal = getToolByName(self, "portal_url").getPortalObject()
 
     mailMsg = email.Message.Message()
     mailMsg["To"] = to
     mailMsg["From"] = mfrom
     mailMsg["CC"] = cc
@@ -145,16 +146,16 @@
     return u'<a href="%s"%s>%s</a>' % (href, target, safe_unicode(content))
 
 
 def install(self):
     """
         Install cputils methods where the user is (root of zope?)
     """
-    from Products.ExternalMethod.ExternalMethod import manage_addExternalMethod
     from Products.CMFPlone.utils import base_hasattr
+    from Products.ExternalMethod.ExternalMethod import manage_addExternalMethod
 
     if not check_zope_admin():
         return "You must be a zope manager to run this script"
     methods = []
     for method in (
         "add_subject",
         "audit_catalog",
@@ -1212,18 +1213,16 @@
         return "You must have a manager role to run this script"
     lf = "<br />\n"
     out = [
         "<h2>Groups and users checks</h2>",
         "You can call the script with the following parameters:",
         "-> app=xxx => configuration to use (Default: docs){}".format(lf),
     ]
-    from collective.contact.plonegroup.config import (
-        get_registry_organizations,
-        get_registry_functions,
-    )
+    from collective.contact.plonegroup.config import get_registry_functions
+    from collective.contact.plonegroup.config import get_registry_organizations
     from collective.wfadaptations.api import get_applied_adaptations
     from datetime import datetime
     from plone import api
     from zope.component import getUtility
     from zope.schema.interfaces import IVocabularyFactory
 
     out.append(
@@ -1604,17 +1603,15 @@
         passwords = old_acl.source_users._user_passwords
         # Check if password validation is activated, if so deactivate it
         # This is necessary because it will try to validate the hash instead of the real password
         val_deact = False
         plugins = acl.plugins
         val_plugins = plugins.getAllPlugins(plugin_type="IValidationPlugin")
         if "password_strength_plugin" in val_plugins["active"]:
-            from Products.PluggableAuthService.interfaces.plugins import (
-                IValidationPlugin,
-            )
+            from Products.PluggableAuthService.interfaces.plugins import IValidationPlugin
 
             plugins.deactivatePlugin(IValidationPlugin, "password_strength_plugin")
             val_deact = True
         for user in users:
             if user.getUserId() not in [ud["userid"] for ud in acl.searchUsers()]:
                 if change:
                     try:
@@ -1705,16 +1702,16 @@
 
 
 def correctPOSKey(self, dochange=""):
     """
         Correct a DICT like attribute.
         Must be called on site context
     """
-    from ZODB.POSException import POSKeyError
     from Products.CMFCore.utils import getToolByName
+    from ZODB.POSException import POSKeyError
 
     if not check_zope_admin():
         return "You must be a zope manager to run this script"
 
     lf = "<br />\n"
     out = ["<h1>Cleaning POSKey errors</h1>"]
     out.append("You can/must call the script with following parameters:")
@@ -2255,16 +2252,16 @@
         2. in portal_action add new CMF action
         3. edit this action
         >>> url (expression) is : string:${globals_view/getCurrentObjectUrl}/cputils_copy_image_attributes
         >>> Condition (expression) is : python:checkPermission("Delete objects", globals_view.getParentObject()) and
             checkPermission("Copy or Move", object) and checkPermission("Add portal content", object) and
             not globals_view.isPortalOrPortalDefaultPage() and not object.isCanonical()
     """
-    from collective.contentleadimage.utils import hasContentLeadImage
     from collective.contentleadimage.config import IMAGE_FIELD_NAME
+    from collective.contentleadimage.utils import hasContentLeadImage
 
     canonical_obj = self.getCanonical()
     if not canonical_obj or (self == self.getCanonical()):
         return
     if hasContentLeadImage(canonical_obj):
         if canonical_obj.getField(IMAGE_FIELD_NAME) and self.getField(IMAGE_FIELD_NAME):
             self.getField(IMAGE_FIELD_NAME).getMutator(self)(
@@ -2307,16 +2304,16 @@
     out = []
     out.append("<p>You can call the script with the following parameters:<br />")
     out.append(
         "-> unregister=... => name of the adapter to unregister (default to empty => "
         "list all adapters)<br />"
     )
 
-    from zope.component import getSiteManager
     from Products.CMFCore.utils import getToolByName
+    from zope.component import getSiteManager
 
     portal = getToolByName(self, "portal_url").getPortalObject()
 
     params = []
     components = getSiteManager(portal)
     for reg in components.registeredAdapters():
         if unregister:
@@ -2701,19 +2698,20 @@
     if not portlet_name:
         return (
             "You MUST provide a portlet_name to query for. "
             "Add '?portlet_name=myportletname' at the end of the url calling this script. "
             "If you want to see every portlets of this site, use '*' as portlet_name"
         )
 
-    from zope.component import getUtility, getMultiAdapter
-    from plone.portlets.interfaces import IPortletManager
-    from plone.portlets.interfaces import IPortletAssignmentMapping
     from plone.portlets.interfaces import ILocalPortletAssignable
+    from plone.portlets.interfaces import IPortletAssignmentMapping
+    from plone.portlets.interfaces import IPortletManager
     from Products.CMFCore.utils import getToolByName
+    from zope.component import getMultiAdapter
+    from zope.component import getUtility
 
     out = ['<table><tr style="nth-child(odd): background-color: #000000;">']
     left_column = getUtility(IPortletManager, name=u"plone.leftcolumn")
     right_column = getUtility(IPortletManager, name=u"plone.rightcolumn")
 
     brains = self.portal_catalog()
     # Add the portal as it is portlet assignable
@@ -2793,16 +2791,17 @@
 
 def rename_long_ids(self, length="255", dochange="", fromfile=""):
     """
         Renames too long ids, not permitting transmogrifier export
         1) run on orig site first, writing correspondences in output file
         2) renames as orig filenames from correspondences file
     """
-    from Products.CMFCore.utils import getToolByName
     from Acquisition import aq_base
+    from Products.CMFCore.utils import getToolByName
+
     import os.path
 
     if not check_role(self):
         return "You must have a manager role to run this script"
 
     out = []
     out.append("<p>You can call the script with following parameters:</p>")
@@ -3601,14 +3600,15 @@
     if not check_role(self):
         return "You must have a manager role to run this script"
 
     import logging
 
     logger = logging.getLogger("CPUtils")
     from zope.annotation.interfaces import IAnnotations
+
     import cgi
 
     out = ["<h1>Deleting a portlet and displaying some attributes</h1>"]
     out.append("You can/must call the script with following parameters:")
     out.append("-> column='right' : to search left (default) or right portlets")
     out.append(
         "-> portlet='xxx' : the id of the portlet to search (can be seen in url when editing it)"
@@ -3666,16 +3666,16 @@
             "'collective.zipfiletransport.utilities.interfaces.IZipFileTransportUtility' for example)"
         )
 
     brains = self.portal_catalog(object_provides=interface_name)
     if not brains:
         return "No elements provides '%s'" % interface_name
 
-    from zope.interface import noLongerProvides
     from zope.component.interface import getInterface
+    from zope.interface import noLongerProvides
 
     out = []
     interface = getInterface("", interface_name)
     out.append(
         "Following object no longer provides '%s' interface :\n" % interface_name
     )
 
@@ -3752,14 +3752,15 @@
     if not check_role(self):
         return "You must have a manager role to run this script"
 
     import logging
 
     logger = logging.getLogger("CPUtils")
     from Products.CMFCore.utils import getToolByName
+
     import os
 
     purl = getToolByName(self, "portal_url")
     portal = purl.getPortalObject()
     sitePath = "/".join(portal.getPhysicalPath())
 
     out = ["<h1>Adding a subject to objects</h1>"]
@@ -3828,18 +3829,16 @@
     if not check_role(self):
         return "You must have a manager role to run this script"
     try:
         from zope.app.component.hooks import setSite
     except ImportError:
         from zope.component.hooks import setSite
 
+    from collective.zipfiletransport.utilities.interfaces import IZipFileTransportUtility
     from zope.component import getSiteManager
-    from collective.zipfiletransport.utilities.interfaces import (
-        IZipFileTransportUtility,
-    )
 
     setSite(self)
     sm = getSiteManager()
     util = sm.queryUtility(IZipFileTransportUtility, name="zipfiletransport")
     sm.unregisterUtility(component=None, provided=IZipFileTransportUtility)
     sm.utilities.unsubscribe((), IZipFileTransportUtility)
     del util
@@ -4192,16 +4191,17 @@
                 break
 
 
 def dv_images_size(self):
     """
         Return size of documentviewer files
     """
-    from zope.annotation.interfaces import IAnnotations
     from plone.app.blob.utils import openBlob
+    from zope.annotation.interfaces import IAnnotations
+
     import os
 
     sizes = {"large": 0, "normal": 0, "small": 0, "text": 0, "pages": 0, "fmt": ""}
     annot = IAnnotations(self).get("collective.documentviewer", "")
     if (
         not annot
         or not annot.get("successfully_converted")
@@ -4487,17 +4487,19 @@
 
 def change_uuid(self, recursive="", dochange=""):
     """
         Change uuid values.
     """
     if not check_role(self):
         return "You must have a manager role to run this script"
-    from zope.component import getUtility
+    from plone.uuid.interfaces import ATTRIBUTE_NAME
+    from plone.uuid.interfaces import IUUID
+    from plone.uuid.interfaces import IUUIDGenerator
     from Products.CMFPlone.utils import base_hasattr
-    from plone.uuid.interfaces import IUUIDGenerator, ATTRIBUTE_NAME, IUUID
+    from zope.component import getUtility
 
     generator = getUtility(IUUIDGenerator)
 
     out = ["<strong>Creators change</strong>"]
     out.append("You can/must call the script with following parameters:")
     out.append("-> recursive=''  : do it recursively. Default=empty")
     out.append("-> dochange=''  : apply changes. Default=empty")
@@ -4651,22 +4653,22 @@
 
     delt = False
     if delete not in ("", "0", "False", "false"):
         delt = True
     ret = []
 
     from datetime import datetime
-    from ZODB.POSException import POSKeyError
-    from Products.CMFCore.utils import getToolByName
-    from Products.CMFPlone.utils import base_hasattr
-    from Products.Archetypes.Field import FileField
-    from Products.Archetypes.interfaces import IBaseContent
     from plone.app.blob.subtypes.file import ExtensionBlobField
-    from plone.namedfile.interfaces import INamedFile
     from plone.dexterity.content import DexterityContent
+    from plone.namedfile.interfaces import INamedFile
+    from Products.Archetypes.Field import FileField
+    from Products.Archetypes.interfaces import IBaseContent
+    from Products.CMFCore.utils import getToolByName
+    from Products.CMFPlone.utils import base_hasattr
+    from ZODB.POSException import POSKeyError
 
     portal = getToolByName(self, "portal_url").getPortalObject()
     log_list(ret, "Starting check_blobs at %s" % datetime(1973, 02, 12).now())
 
     blob_attrs = {}
     # get all files attributes
     for typ in portal.portal_types:
@@ -4729,21 +4731,21 @@
 
     delt = False
     if delete not in ("", "0", "False", "false"):
         delt = True
     ret = []
 
     from datetime import datetime
-    from ZODB.POSException import POSKeyError
-    from Products.CMFCore.interfaces import IFolderish
-    from Products.CMFCore.utils import getToolByName
+    from plone.dexterity.content import DexterityContent
+    from plone.namedfile.interfaces import INamedFile
     from Products.Archetypes.Field import FileField
     from Products.Archetypes.interfaces import IBaseContent
-    from plone.namedfile.interfaces import INamedFile
-    from plone.dexterity.content import DexterityContent
+    from Products.CMFCore.interfaces import IFolderish
+    from Products.CMFCore.utils import getToolByName
+    from ZODB.POSException import POSKeyError
 
     portal = getToolByName(self, "portal_url").getPortalObject()
     start = datetime(1973, 02, 12).now()
     log_list(ret, "Starting check_blobs at %s" % start)
 
     def check_at_blobs(context):
         """ Archetypes content checker. Return True if purge needed """
@@ -4887,25 +4889,26 @@
 def set_attr(self, attr="", value="", typ="str"):
     """
         Set attribute on context.
         Usefull to change creation_date by example
     """
     if not check_zope_admin():
         return "You must be a zope manager to run this script"
-    from Products.CMFPlone.utils import safe_hasattr
     from cgi import escape
+    from Products.CMFPlone.utils import safe_hasattr
 
     good_types = ["str", "int", "list", "DateTime", "unicode", "datetime", "None"]
 
     sep = "\n<br />"
     out = ["<h2>You can/must call the script with following parameters:</h2>",
            "-> attr=''  : attribute name.",
            "-> value=''  : value to set.",
            "-> typ=''  : value type. Can be %s. Default='str'" % ", ".join(["'%s'" % t for t in good_types]),
            "-> Example: ?attr=creation_date&value=2017-10-13 9:00 GMT%2B1&typ=DateTime<br />"
+           "-> Example: ?attr=_plone.uuid&value=xxx<br />"
     ]
     if not attr:
         out.append("attr parameter is mandatory !")
         return sep.join(out)
     if not safe_hasattr(self, attr):
         out.append("Attr '%s' doesn't exist !" % attr)
         return sep.join(out)
@@ -4929,14 +4932,15 @@
             from Products.CMFPlone.utils import safe_unicode
             new_val = safe_unicode(value)
         elif typ == "DateTime":
             from DateTime import DateTime
             new_val = DateTime(value)  # example '2017-10-13 9:00 GMT%2B1'  %2B = '+'
         elif typ == "datetime":
             from datetime import datetime
+
             import re
             dt = map(int, filter(None, re.split(r"[\- /\\:]+", value)))
             new_val = datetime(*dt)  # example '2017-10-13 9:00'
         elif typ == "None":
             new_val = None
     except Exception as msg:
         out.append("Cannot cast value type to '%s': '%s'" % (typ, msg))
@@ -5016,16 +5020,16 @@
         out.append("No problem found")
     return "\n".join(out)
 
 
 def show_object_relations(self):
     if not check_zope_admin():
         return "You must be a zope manager to run this script"
-    from zope.component import queryUtility
     from zc.relation.interfaces import ICatalog  # noqa
+    from zope.component import queryUtility
     from zope.intid.interfaces import IIntIds
 
     intids = queryUtility(IIntIds)
     catalog = queryUtility(ICatalog)
     out = []
     for way in ("from", "to"):
         out.append("Way = {}".format(way))
@@ -5052,18 +5056,18 @@
     if "collective.documentviewer" in annotations:
         annotations.pop("collective.documentviewer", {})
 
 
 def clear_completed_async_jobs(self):
     """ Remove plone.app.async jobs that are completed, i.e. success or failure.
         Does not remove jobs still in flight """
-    from zope.component import getUtility
-    from Products.CMFCore.interfaces import ISiteRoot
     from plone.app.async.interfaces import IAsyncDatabase
+    from Products.CMFCore.interfaces import ISiteRoot
     from zc.async.interfaces import KEY
+    from zope.component import getUtility
 
     db = getUtility(IAsyncDatabase)
     main_conn = getUtility(ISiteRoot)._p_jar
     async_conn = main_conn.get_connection(db.database_name)
     queue = async_conn.root()[KEY]['']
     for da in queue.dispatchers.values():
         for agent in da.values():
```

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/QITool.txt` & `Products.CPUtils-1.25/src/Products/CPUtils/QITool.txt`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/__init__.py` & `Products.CPUtils-1.25/src/Products/CPUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/config.py` & `Products.CPUtils-1.25/src/Products/CPUtils/config.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/fckpatch.py` & `Products.CPUtils-1.25/src/Products/CPUtils/fckpatch.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/hiddenProductsList.py` & `Products.CPUtils-1.25/src/Products/CPUtils/hiddenProductsList.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po` & `Products.CPUtils-1.25/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/model/CPUtils.zargo` & `Products.CPUtils-1.25/src/Products/CPUtils/model/CPUtils.zargo`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/model/archgenxml.log` & `Products.CPUtils-1.25/src/Products/CPUtils/model/archgenxml.log`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/model/generate.conf` & `Products.CPUtils-1.25/src/Products/CPUtils/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/profiles.zcml` & `Products.CPUtils-1.25/src/Products/CPUtils/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkInstances.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkInstances.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/checkPOSKeyErrors.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/checkPOSKeyErrors.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_backup_db.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_backup_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_db.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_zeo.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_zeo.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/pack_zeo.sh` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/pack_zeo.sh`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/restore_db.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/restore_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/send_log.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/send_log.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/test_db.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/test_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/update_awstats.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/update_awstats.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/utils.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/scripts/zope_restart.py` & `Products.CPUtils-1.25/src/Products/CPUtils/scripts/zope_restart.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/setuphandlers.py` & `Products.CPUtils-1.25/src/Products/CPUtils/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/tests/CPUtilsTestCase.py` & `Products.CPUtils-1.25/src/Products/CPUtils/tests/CPUtilsTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/tests/framework.py` & `Products.CPUtils-1.25/src/Products/CPUtils/tests/framework.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/tests/testMethods.py` & `Products.CPUtils-1.25/src/Products/CPUtils/tests/testMethods.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/tests/testNewsLetter.py` & `Products.CPUtils-1.25/src/Products/CPUtils/tests/testNewsLetter.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/tests/test_functional.py` & `Products.CPUtils-1.25/src/Products/CPUtils/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products/CPUtils/utils.py` & `Products.CPUtils-1.25/src/Products/CPUtils/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.24/src/Products.CPUtils.egg-info/SOURCES.txt` & `Products.CPUtils-1.25/src/Products.CPUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

