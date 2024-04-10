# Comparing `tmp/imio.annex-2.8.tar.gz` & `tmp/imio.annex-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.annex-2.8.tar", last modified: Fri Apr 23 12:22:59 2021, max compression
+gzip compressed data, was "dist/imio.annex-2.9.tar", last modified: Fri Jul 16 06:51:23 2021, max compression
```

## Comparing `imio.annex-2.8.tar` & `imio.annex-2.9.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      655 2021-04-23 12:22:58.000000 imio.annex-2.8/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2021-04-23 12:22:58.000000 imio.annex-2.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2021-04-23 12:22:58.000000 imio.annex-2.8/docs/index.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1020 2021-04-23 12:22:58.000000 imio.annex-2.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2021-04-23 12:22:58.000000 imio.annex-2.8/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9128 2021-04-23 12:22:59.000000 imio.annex-2.8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      827 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/quickupload/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/quickupload/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      220 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/templates/form.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/templates/quick_upload.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15008 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/quickupload.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/quickupload/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      899 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/static/quickupload.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2254 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/static/helpers.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1972 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/quickupload/form.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      314 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      316 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      338 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      227 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      139 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      295 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/propertiestool.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/imioannex_default.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/profiles/default/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2331 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/types/annex.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      222 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/default/workflows.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/profiles/zamqp/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/zamqp/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/zamqp/imioannex_amqp.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/profiles/zamqp/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      540 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/profiles/zamqp/types/annex.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3410 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/content/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1721 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/content/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/content/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1668 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/content/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1030 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/content/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      438 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      419 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/behaviors.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      641 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2666 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/columns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      160 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2797 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4118 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/overrides.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/browser/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      448 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/browser/static/view_element.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      416 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/patch.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      275 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/collective.quickupload.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      627 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      531 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/collective.quickupload.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1456 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/imio.annex.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1316 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/imio.annex.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      965 2021-04-23 12:22:58.000000 imio.annex-2.8/src/imio/annex/locales/update.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9128 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2302 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      282 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-04-23 12:22:59.000000 imio.annex-2.8/src/imio.annex.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       95 2021-04-23 12:22:58.000000 imio.annex-2.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-04-23 12:22:59.000000 imio.annex-2.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1868 2021-04-23 12:22:58.000000 imio.annex-2.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6501 2021-04-23 12:22:58.000000 imio.annex-2.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5426 2021-04-23 12:22:58.000000 imio.annex-2.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3414 2021-04-23 12:22:58.000000 imio.annex-2.8/buildout.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9765 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2472 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      282 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio.annex.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1972 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/form.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      899 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/static/quickupload.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2254 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/static/helpers.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      579 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      220 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/templates/form.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3051 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/templates/quick_upload.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15008 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/quickupload.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/quickupload/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      160 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2797 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      641 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3526 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/columns.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      275 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/collective.quickupload.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1150 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      627 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/plone.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1316 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/imio.annex.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1343 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/collective.eeafaceted.batchactions.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1456 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/imio.annex.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      531 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      848 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/collective.quickupload.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1819 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      139 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      314 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      295 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/propertiestool.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2331 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/types/annex.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      338 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      227 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/imioannex_default.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      316 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      222 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/default/workflows.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/zamqp/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/zamqp/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/zamqp/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      540 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/zamqp/types/annex.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/profiles/zamqp/imioannex_amqp.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1030 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1721 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/content/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1668 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/content/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      419 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/behaviors.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      438 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3410 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      827 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5222 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      448 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/static/view_element.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4949 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      634 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      416 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/annex/patch.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2021-07-16 06:51:23.000000 imio.annex-2.9/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2021-07-16 06:51:23.000000 imio.annex-2.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      655 2021-07-16 06:51:23.000000 imio.annex-2.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2021-07-16 06:51:23.000000 imio.annex-2.9/docs/index.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2021-07-16 06:51:23.000000 imio.annex-2.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6501 2021-07-16 06:51:23.000000 imio.annex-2.9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1868 2021-07-16 06:51:23.000000 imio.annex-2.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9765 2021-07-16 06:51:23.000000 imio.annex-2.9/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       95 2021-07-16 06:51:23.000000 imio.annex-2.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5951 2021-07-16 06:51:23.000000 imio.annex-2.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2021-07-16 06:51:23.000000 imio.annex-2.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1020 2021-07-16 06:51:23.000000 imio.annex-2.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2021-07-16 06:51:23.000000 imio.annex-2.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3414 2021-07-16 06:51:23.000000 imio.annex-2.9/buildout.cfg
```

### Comparing `imio.annex-2.8/docs/LICENSE.rst` & `imio.annex-2.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/docs/LICENSE.GPL` & `imio.annex-2.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/README.rst` & `imio.annex-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/PKG-INFO` & `imio.annex-2.9/src/imio.annex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.annex
-Version: 2.8
+Version: 2.9
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/imio.annex
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -62,14 +62,28 @@
         
         - Martin Peeters, Original Author [Affinitic]
         
         Changelog
         =========
         
         
+        2.9 (2021-07-16)
+        ----------------
+        
+        - Override `collective.iconifiedcategory` columns `category-column`,
+          `creation-date-column`, `last-modification-column` and `filesize-column` to
+          use `collective.eeafaceted.z3ctable` based columns instead the original
+          `z3c.table` columns so we have custom CSS classes.
+          [gbastien]
+        - Added `DownloadAnnexesBatchActionForm`, a batch action to download several
+          annexes as a Zip file :
+          - download is handled by an ajax request;
+          - max download size is 50Mb by default.
+          [gbastien]
+        
         2.8 (2021-04-23)
         ----------------
         
         - Fixed `quickupload.ImioAnnexQuickUploadCapableFileFactory` to make sure that
           thread lock is released like it is the case by default in
           `uploadcapable.QuickUploadCapableFileFactory`.
           This should avoid rare cases where instance is stuck while adding an annex.
```

### Comparing `imio.annex-2.8/src/imio/annex/events.py` & `imio.annex-2.9/src/imio/annex/events.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/utils.py` & `imio.annex-2.9/src/imio/annex/quickupload/utils.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/templates/quick_upload.pt` & `imio.annex-2.9/src/imio/annex/quickupload/templates/quick_upload.pt`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/quickupload.py` & `imio.annex-2.9/src/imio/annex/quickupload/quickupload.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/static/quickupload.css` & `imio.annex-2.9/src/imio/annex/quickupload/static/quickupload.css`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/static/helpers.js` & `imio.annex-2.9/src/imio/annex/quickupload/static/helpers.js`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/quickupload/form.py` & `imio.annex-2.9/src/imio/annex/quickupload/form.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/profiles/default/types/annex.xml` & `imio.annex-2.9/src/imio/annex/profiles/default/types/annex.xml`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/profiles/zamqp/types/annex.xml` & `imio.annex-2.9/src/imio/annex/profiles/zamqp/types/annex.xml`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/utils.py` & `imio.annex-2.9/src/imio/annex/utils.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/content/events.py` & `imio.annex-2.9/src/imio/annex/content/events.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/content/annex.py` & `imio.annex-2.9/src/imio/annex/content/annex.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/content/configure.zcml` & `imio.annex-2.9/src/imio/annex/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/adapters.py` & `imio.annex-2.9/src/imio/annex/adapters.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/configure.zcml` & `imio.annex-2.9/src/imio/annex/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/overrides.zcml` & `imio.annex-2.9/src/imio/annex/overrides.zcml`

 * *Files 26% similar despite different names*

```diff
@@ -8,34 +8,63 @@
 
     <adapter
       name="title-column"
       for="zope.interface.Interface
            zope.interface.Interface
            collective.iconifiedcategory.interfaces.ICategorizedTable"
       provides="z3c.table.interfaces.IColumn"
-      factory=".columns.PrettyLinkColumn"
-      />
+      factory=".columns.PrettyLinkColumn" />
 
     <adapter
       name="author-column"
       for="zope.interface.Interface
            zope.interface.Interface
            collective.iconifiedcategory.interfaces.ICategorizedTable"
       provides="z3c.table.interfaces.IColumn"
-      factory=".columns.AuthorColumn"
-      />
+      factory=".columns.AuthorColumn" />
+
+    <adapter
+      name="category-column"
+      for="zope.interface.Interface
+           zope.interface.Interface
+           collective.iconifiedcategory.interfaces.ICategorizedTable"
+      provides="z3c.table.interfaces.IColumn"
+      factory=".columns.CategoryColumn" />
+
+    <adapter
+      name="creation-date-column"
+      for="zope.interface.Interface
+           zope.interface.Interface
+           collective.iconifiedcategory.interfaces.ICategorizedTable"
+      provides="z3c.table.interfaces.IColumn"
+      factory=".columns.CreationDateColumn" />
+
+    <adapter
+      name="last-modification-column"
+      for="zope.interface.Interface
+           zope.interface.Interface
+           collective.iconifiedcategory.interfaces.ICategorizedTable"
+      provides="z3c.table.interfaces.IColumn"
+      factory=".columns.LastModificationColumn" />
+
+    <adapter
+      name="filesize-column"
+      for="zope.interface.Interface
+           zope.interface.Interface
+           collective.iconifiedcategory.interfaces.ICategorizedTable"
+      provides="z3c.table.interfaces.IColumn"
+      factory=".columns.FilesizeColumn" />
 
     <adapter
       name="action-column"
       for="zope.interface.Interface
            zope.interface.Interface
            collective.iconifiedcategory.interfaces.ICategorizedTable"
       provides="z3c.table.interfaces.IColumn"
-      factory=".columns.ActionsColumn"
-      />
+      factory=".columns.ActionsColumn" />
 
     <!-- Use the imio.helpers container view for annex, overrided here because
          already overrided in collective.iconifiedcategory except for ICategoryGroup
          but we do this here to group overrides even if ICategoryGroup could be
          overrided in a configure.zcml -->
     <configure package="imio.helpers">
         <browser:page
```

### Comparing `imio.annex-2.8/src/imio/annex/locales/plone.pot` & `imio.annex-2.9/src/imio/annex/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/plone.po` & `imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/collective.quickupload.po` & `imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/collective.quickupload.po`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/src/imio/annex/locales/fr/LC_MESSAGES/imio.annex.po` & `imio.annex-2.9/src/imio/annex/locales/fr/LC_MESSAGES/imio.annex.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2020-04-21 12:18+0000\n"
+"POT-Creation-Date: 2021-06-01 07:46+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
-#: ../columns.py:56
+#: ../columns.py:62
 msgid "Actions"
 msgstr "Actions"
 
 #: ../configure.zcml:75
 msgid "Adds scan information fields but hides fields to_sign/signed"
 msgstr "Ajoute les champs d'informations de numérisation mais en cachant les champs \"à signer?/signé?\""
 
@@ -42,14 +42,14 @@
 msgid "Installs the zamqp part for imio.annex."
 msgstr ""
 
 #: ../configure.zcml:75
 msgid "Scan metadata (fields to_sign/signed hidden)"
 msgstr "Métadonnées de numérisation (champs \"à signer?/signé?\" cachés)"
 
-#: ../columns.py:17
+#: ../columns.py:19
 msgid "Title"
 msgstr "Titre"
 
 #: ../configure.zcml:35
 msgid "imio.annex"
 msgstr ""
```

### Comparing `imio.annex-2.8/src/imio/annex/locales/imio.annex.pot` & `imio.annex-2.9/src/imio/annex/locales/imio.annex.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2020-04-21 12:18+0000\n"
+"POT-Creation-Date: 2021-06-01 07:46+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: imio.annex\n"
 
-#: ../columns.py:56
+#: ../columns.py:62
 msgid "Actions"
 msgstr ""
 
 #: ../configure.zcml:75
 msgid "Adds scan information fields but hides fields to_sign/signed"
 msgstr ""
 
@@ -45,14 +45,14 @@
 msgid "Installs the zamqp part for imio.annex."
 msgstr ""
 
 #: ../configure.zcml:75
 msgid "Scan metadata (fields to_sign/signed hidden)"
 msgstr ""
 
-#: ../columns.py:17
+#: ../columns.py:19
 msgid "Title"
 msgstr ""
 
 #: ../configure.zcml:35
 msgid "imio.annex"
 msgstr ""
```

### Comparing `imio.annex-2.8/src/imio/annex/locales/update.sh` & `imio.annex-2.9/src/imio/annex/locales/update.sh`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,14 @@
 done
 
 for lang in $(find . -mindepth 1 -maxdepth 1 -type d); do
 		if test -d $lang/LC_MESSAGES; then
 				touch $lang/LC_MESSAGES/$domain.po
 				touch $lang/LC_MESSAGES/plone.po
 				touch $lang/LC_MESSAGES/collective.quickupload.po
+				touch $lang/LC_MESSAGES/collective.eeafaceted.batchactions.po
 				i18ndude sync --pot $domain.pot $lang/LC_MESSAGES/$domain.po
 				i18ndude sync --pot plone.pot $lang/LC_MESSAGES/plone.po
 				i18ndude sync --pot collective.quickupload.pot $lang/LC_MESSAGES/collective.quickupload.po
+				i18ndude sync --pot collective.eeafaceted.batchactions.pot $lang/LC_MESSAGES/collective.eeafaceted.batchactions.po
 		fi
 done
```

### Comparing `imio.annex-2.8/src/imio.annex.egg-info/PKG-INFO` & `imio.annex-2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.annex
-Version: 2.8
+Version: 2.9
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/imio.annex
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -62,14 +62,28 @@
         
         - Martin Peeters, Original Author [Affinitic]
         
         Changelog
         =========
         
         
+        2.9 (2021-07-16)
+        ----------------
+        
+        - Override `collective.iconifiedcategory` columns `category-column`,
+          `creation-date-column`, `last-modification-column` and `filesize-column` to
+          use `collective.eeafaceted.z3ctable` based columns instead the original
+          `z3c.table` columns so we have custom CSS classes.
+          [gbastien]
+        - Added `DownloadAnnexesBatchActionForm`, a batch action to download several
+          annexes as a Zip file :
+          - download is handled by an ajax request;
+          - max download size is 50Mb by default.
+          [gbastien]
+        
         2.8 (2021-04-23)
         ----------------
         
         - Fixed `quickupload.ImioAnnexQuickUploadCapableFileFactory` to make sure that
           thread lock is released like it is the case by default in
           `uploadcapable.QuickUploadCapableFileFactory`.
           This should avoid rare cases where instance is stuck while adding an annex.
```

### Comparing `imio.annex-2.8/src/imio.annex.egg-info/SOURCES.txt` & `imio.annex-2.9/src/imio.annex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 src/imio/annex/interfaces.py
 src/imio/annex/overrides.zcml
 src/imio/annex/patch.py
 src/imio/annex/setuphandlers.py
 src/imio/annex/utils.py
 src/imio/annex/browser/__init__.py
 src/imio/annex/browser/configure.zcml
+src/imio/annex/browser/views.py
 src/imio/annex/browser/static/view_element.png
 src/imio/annex/content/__init__.py
 src/imio/annex/content/annex.py
 src/imio/annex/content/configure.zcml
 src/imio/annex/content/events.py
+src/imio/annex/locales/collective.eeafaceted.batchactions.pot
 src/imio/annex/locales/collective.quickupload.pot
 src/imio/annex/locales/imio.annex.pot
 src/imio/annex/locales/plone.pot
 src/imio/annex/locales/update.sh
+src/imio/annex/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
 src/imio/annex/locales/fr/LC_MESSAGES/collective.quickupload.po
 src/imio/annex/locales/fr/LC_MESSAGES/imio.annex.po
 src/imio/annex/locales/fr/LC_MESSAGES/plone.po
 src/imio/annex/profiles/default/browserlayer.xml
 src/imio/annex/profiles/default/cssregistry.xml
 src/imio/annex/profiles/default/imioannex_default.txt
 src/imio/annex/profiles/default/jsregistry.xml
```

### Comparing `imio.annex-2.8/setup.py` & `imio.annex-2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '\n' +
     open('CHANGES.rst').read() +
     '\n')
 
 
 setup(
     name='imio.annex',
-    version='2.8',
+    version='2.9',
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `imio.annex-2.8/bootstrap.py` & `imio.annex-2.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.annex-2.8/CHANGES.rst` & `imio.annex-2.9/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 Changelog
 =========
 
 
+2.9 (2021-07-16)
+----------------
+
+- Override `collective.iconifiedcategory` columns `category-column`,
+  `creation-date-column`, `last-modification-column` and `filesize-column` to
+  use `collective.eeafaceted.z3ctable` based columns instead the original
+  `z3c.table` columns so we have custom CSS classes.
+  [gbastien]
+- Added `DownloadAnnexesBatchActionForm`, a batch action to download several
+  annexes as a Zip file :
+  - download is handled by an ajax request;
+  - max download size is 50Mb by default.
+  [gbastien]
+
 2.8 (2021-04-23)
 ----------------
 
 - Fixed `quickupload.ImioAnnexQuickUploadCapableFileFactory` to make sure that
   thread lock is released like it is the case by default in
   `uploadcapable.QuickUploadCapableFileFactory`.
   This should avoid rare cases where instance is stuck while adding an annex.
```

### Comparing `imio.annex-2.8/buildout.cfg` & `imio.annex-2.9/buildout.cfg`

 * *Files identical despite different names*

