# Comparing `tmp/collective.listmonk-1.0.0a3.tar.gz` & `tmp/collective.listmonk-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.listmonk-1.0.0a3.tar", last modified: Mon Apr  8 03:24:59 2024, max compression
+gzip compressed data, was "collective.listmonk-1.0.0a4.tar", last modified: Tue Apr  9 22:06:13 2024, max compression
```

## Comparing `collective.listmonk-1.0.0a3.tar` & `collective.listmonk-1.0.0a4.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.187487 collective.listmonk-1.0.0a3/
--rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)      670 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/CONTRIBUTORS.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/LICENSE.md
--rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     6668 2024-04-08 03:24:59.187243 collective.listmonk-1.0.0a3/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/constraints.txt
--rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/docker-compose.yml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.179613 collective.listmonk-1.0.0a3/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/docs/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/docs/dlr.svg
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.179870 collective.listmonk-1.0.0a3/news/
--rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/news/.changelog_template.jinja
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/news/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-08 03:24:59.187525 collective.listmonk-1.0.0a3/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.176454 collective.listmonk-1.0.0a3/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.179998 collective.listmonk-1.0.0a3/src/collective/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.181984 collective.listmonk-1.0.0a3/src/collective/listmonk/
--rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.182238 collective.listmonk-1.0.0a3/src/collective/listmonk/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.182496 collective.listmonk-1.0.0a3/src/collective/listmonk/content/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2675 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/content/newsletter.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.182720 collective.listmonk-1.0.0a3/src/collective/listmonk/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/controlpanel/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/controlpanel/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/dependencies.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/interfaces.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1445 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/listmonk.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.183233 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2679 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/collective.listmonk.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.176961 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.183447 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     2664 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.177086 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.183610 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     2234 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
--rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/locales/update.py
--rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/permissions.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.177359 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.184189 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/rolemap.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.184314 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/types/Newsletter.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.184471 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/profiles.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.185209 collective.listmonk-1.0.0a3/src/collective/listmonk/services/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/services/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/services/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1254 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/services/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/services/mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5246 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/services/subscriptions.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.185349 collective.listmonk-1.0.0a3/src/collective/listmonk/setuphandlers/
--rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/setuphandlers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3184 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.185608 collective.listmonk-1.0.0a3/src/collective/listmonk/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/upgrades/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/src/collective/listmonk/upgrades/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.186668 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     6668 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     2409 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-08 03:24:59.000000 collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.185754 collective.listmonk-1.0.0a3/tests/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.186026 collective.listmonk-1.0.0a3/tests/api/
--rw-r--r--   0 davisagli   (501) staff       (20)     5036 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/api/test_mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4273 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/api/test_subscriptions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2699 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.186308 collective.listmonk-1.0.0a3/tests/setup/
--rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/setup/test_setup_install.py
--rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-08 03:24:59.186455 collective.listmonk-1.0.0a3/tests/setup/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-08 03:24:58.000000 collective.listmonk-1.0.0a3/tests/setup/upgrades/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.019106 collective.listmonk-1.0.0a4/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)      783 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/CONTRIBUTORS.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/LICENSE.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     6781 2024-04-09 22:06:13.018797 collective.listmonk-1.0.0a4/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/constraints.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docker-compose.yml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.008615 collective.listmonk-1.0.0a4/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docs/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/docs/dlr.svg
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.008962 collective.listmonk-1.0.0a4/news/
+-rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/news/.changelog_template.jinja
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/news/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-09 22:06:13.019152 collective.listmonk-1.0.0a4/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.004640 collective.listmonk-1.0.0a4/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.009118 collective.listmonk-1.0.0a4/src/collective/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.011607 collective.listmonk-1.0.0a4/src/collective/listmonk/
+-rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.011911 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.012547 collective.listmonk-1.0.0a4/src/collective/listmonk/content/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/content/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2742 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/content/newsletter.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.012969 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/controlpanel/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/interfaces.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1445 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/listmonk.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013507 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3074 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/collective.listmonk.pot
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005232 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013701 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3171 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005384 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.013893 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2581 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/locales/update.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/permissions.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.005712 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.014623 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/rolemap.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.014832 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/Newsletter.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.015041 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/profiles.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.015907 collective.listmonk-1.0.0a4/src/collective/listmonk/services/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1254 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     6397 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/services/subscriptions.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016088 collective.listmonk-1.0.0a4/src/collective/listmonk/setuphandlers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/setuphandlers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3185 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016423 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective/listmonk/upgrades/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.018051 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     6781 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     2449 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.016751 collective.listmonk-1.0.0a4/tests/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017258 collective.listmonk-1.0.0a4/tests/api/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4657 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/test_mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5182 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/api/test_subscriptions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3116 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017616 collective.listmonk-1.0.0a4/tests/setup/
+-rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/test_setup_install.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-09 22:06:13.017792 collective.listmonk-1.0.0a4/tests/setup/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-09 22:06:12.000000 collective.listmonk-1.0.0a4/tests/setup/upgrades/conftest.py
```

### Comparing `collective.listmonk-1.0.0a3/.editorconfig` & `collective.listmonk-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/CHANGES.md` & `collective.listmonk-1.0.0a4/CHANGES.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-04-09)
+
+
+### New features:
+
+- Send an email confirmation of a new subscription. @davisagli #12
+
 ## 1.0.0a3 (2024-04-07)
 
 
 ### Bug fixes:
 
 - Don't add header and footer to the email automatically, so the editor has control. @davisagli #11
```

### Comparing `collective.listmonk-1.0.0a3/LICENSE.GPL` & `collective.listmonk-1.0.0a4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/LICENSE.md` & `collective.listmonk-1.0.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/PKG-INFO` & `collective.listmonk-1.0.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-04-09)
+
+
+### New features:
+
+- Send an email confirmation of a new subscription. @davisagli #12
+
 ## 1.0.0a3 (2024-04-07)
 
 
 ### Bug fixes:
 
 - Don't add header and footer to the email automatically, so the editor has control. @davisagli #11
```

### Comparing `collective.listmonk-1.0.0a3/README.md` & `collective.listmonk-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/docker-compose.yml` & `collective.listmonk-1.0.0a4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/docs/dlr.svg` & `collective.listmonk-1.0.0a4/docs/dlr.svg`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/pyproject.toml` & `collective.listmonk-1.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/setup.py` & `collective.listmonk-1.0.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {Path("CONTRIBUTORS.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="collective.listmonk",
-    version="1.0.0a3",
+    version="1.0.0a4",
     description="A Listmonk newsletter integration for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/content/newsletter.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/content/newsletter.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,24 +68,27 @@
         )
         return formataddr((from_name, from_address))
 
     def get_email_body(self, content):
         parts = [content]
 
         request = getRequest()
-        unsubscribe_path = translate(
-            _("path_unsubscribe", default="newsletter-unsubscribe"),
-            context=request,
-        )
-        unsubscribe_link = f"{self.absolute_url()}/{unsubscribe_path}"
         parts.append(
             translate(
                 _(
                     "email_mailing_footer",
                     default="---\nUnsubscribe: ${unsubscribe_link}",
-                    mapping={"unsubscribe_link": unsubscribe_link},
+                    mapping={"unsubscribe_link": self.get_unsubscribe_link()},
                 ),
                 request,
             )
         )
 
         return "\n\n".join(parts)
+
+    def get_unsubscribe_link(self):
+        request = getRequest()
+        unsubscribe_path = translate(
+            _("path_unsubscribe", default="newsletter-unsubscribe"),
+            context=request,
+        )
+        return f"{self.absolute_url()}/{unsubscribe_path}"
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/listmonk.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/listmonk.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/locales/collective.listmonk.pot` & `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/collective.listmonk.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 #SOME DESCRIPTIVE TITLE.
 #FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-04-08 03:15+0000\n"
+"POT-Creation-Date: 2024-04-09 21:59+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -34,28 +34,38 @@
 msgstr ""
 
 #: collective-listmonk/src/collective/listmonk/profiles.zcml:21
 msgid "Uninstall collective.listmonk"
 msgstr ""
 
 #. Default: "Someone has requested a subscription to ${newsletter}\n\nTo confirm this subscription, click this link:\n${confirm_link}\n\nIf you did not request this subscription, you can ignore this email.\n"
-#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:154
+#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:87
 msgid "email_confirm_body"
 msgstr ""
 
 #. Default: "Confirm Subscription"
-#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:151
+#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:83
 msgid "email_confirm_subject"
 msgstr ""
 
 #. Default: "---\nUnsubscribe: ${unsubscribe_link}"
-#: collective-listmonk/src/collective/listmonk/content/newsletter.py:82
+#: collective-listmonk/src/collective/listmonk/content/newsletter.py:77
 msgid "email_mailing_footer"
 msgstr ""
 
+#. Default: "You are now subscribed to the ${newsletter}\n\nYou can unsubscribe using this link:\n${unsubscribe_link}\n"
+#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:146
+msgid "email_subscribed_body"
+msgstr ""
+
+#. Default: "Subscription confirmed"
+#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:142
+msgid "email_subscribed_subject"
+msgstr ""
+
 #. Default: "E-mail Footer"
 #: collective-listmonk/src/collective/listmonk/content/newsletter.py:55
 msgid "label_email_footer"
 msgstr ""
 
 #. Default: "E-mail Sender Name (From)"
 #: collective-listmonk/src/collective/listmonk/content/newsletter.py:45
@@ -69,15 +79,15 @@
 
 #. Default: "Topics"
 #: collective-listmonk/src/collective/listmonk/content/newsletter.py:19
 msgid "label_topics"
 msgstr ""
 
 #. Default: "newsletter-confirm"
-#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:74
+#: collective-listmonk/src/collective/listmonk/services/subscriptions.py:77
 msgid "path_confirm"
 msgstr ""
 
 #. Default: "newsletter-unsubscribe"
-#: collective-listmonk/src/collective/listmonk/content/newsletter.py:76
+#: collective-listmonk/src/collective/listmonk/content/newsletter.py:91
 msgid "path_unsubscribe"
 msgstr ""
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-04-08 03:15+0000\n"
+"POT-Creation-Date: 2024-04-09 21:56+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -31,28 +31,38 @@
 msgstr ""
 
 #: collective/listmonk/profiles.zcml:21
 msgid "Uninstall collective.listmonk"
 msgstr ""
 
 #. Default: "Someone has requested a subscription to ${newsletter}\n\nTo confirm this subscription, click this link:\n${confirm_link}\n\nIf you did not request this subscription, you can ignore this email.\n"
-#: collective/listmonk/services/subscriptions.py:154
+#: collective/listmonk/services/subscriptions.py:87
 msgid "email_confirm_body"
 msgstr "Jemand hat ein Abonnement für ${newsletter} angefordert\n\nUm dieses Abonnement zu bestätigen, klicken Sie auf diesen Link:\n${confirm_link}\n\nWenn Sie dieses Abonnement nicht angefordert haben, können Sie diese E-Mail ignorieren.\n"
 
 #. Default: "Confirm Subscription"
-#: collective/listmonk/services/subscriptions.py:151
+#: collective/listmonk/services/subscriptions.py:83
 msgid "email_confirm_subject"
 msgstr "Abonnement bestätigen"
 
 #. Default: "---\nUnsubscribe: ${unsubscribe_link}"
-#: collective/listmonk/content/newsletter.py:82
+#: collective/listmonk/content/newsletter.py:77
 msgid "email_mailing_footer"
 msgstr "---\nZur Abbestellung dieses Newsletters bitte auf folgenden Link klicken:\n${unsubscribe_link}"
 
+#. Default: "You are now subscribed to the ${newsletter}\n\nYou can unsubscribe using this link:\n${unsubscribe_link}\n"
+#: collective/listmonk/services/subscriptions.py:146
+msgid "email_subscribed_body"
+msgstr "Sie haben jetzt den ${newsletter} abonniert\n\nZur Abbestellung dieses Newsletters bitte auf folgenden Link klicken:\n${unsubscribe_link}\n"
+
+#. Default: "Subscription confirmed"
+#: collective/listmonk/services/subscriptions.py:142
+msgid "email_subscribed_subject"
+msgstr "Abonnement bestätigt"
+
 #. Default: "E-mail Footer"
 #: collective/listmonk/content/newsletter.py:55
 msgid "label_email_footer"
 msgstr ""
 
 #. Default: "E-mail Sender Name (From)"
 #: collective/listmonk/content/newsletter.py:45
@@ -66,15 +76,15 @@
 
 #. Default: "Topics"
 #: collective/listmonk/content/newsletter.py:19
 msgid "label_topics"
 msgstr "Themen"
 
 #. Default: "newsletter-confirm"
-#: collective/listmonk/services/subscriptions.py:74
+#: collective/listmonk/services/subscriptions.py:77
 msgid "path_confirm"
 msgstr "newsletter-bestaetigen"
 
 #. Default: "newsletter-unsubscribe"
-#: collective/listmonk/content/newsletter.py:76
+#: collective/listmonk/content/newsletter.py:91
 msgid "path_unsubscribe"
 msgstr "newsletter-abbestellen"
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2024-04-08 03:15+0000\n"
+"POT-Creation-Date: 2024-04-09 21:59+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -31,28 +31,38 @@
 msgstr ""
 
 #: collective/listmonk/profiles.zcml:21
 msgid "Uninstall collective.listmonk"
 msgstr ""
 
 #. Default: "Someone has requested a subscription to ${newsletter}\n\nTo confirm this subscription, click this link:\n${confirm_link}\n\nIf you did not request this subscription, you can ignore this email.\n"
-#: collective/listmonk/services/subscriptions.py:154
+#: collective/listmonk/services/subscriptions.py:87
 msgid "email_confirm_body"
 msgstr ""
 
 #. Default: "Confirm Subscription"
-#: collective/listmonk/services/subscriptions.py:151
+#: collective/listmonk/services/subscriptions.py:83
 msgid "email_confirm_subject"
 msgstr ""
 
 #. Default: "---\nUnsubscribe: ${unsubscribe_link}"
-#: collective/listmonk/content/newsletter.py:82
+#: collective/listmonk/content/newsletter.py:77
 msgid "email_mailing_footer"
 msgstr ""
 
+#. Default: "You are now subscribed to the ${newsletter}\n\nYou can unsubscribe using this link:\n${unsubscribe_link}\n"
+#: collective/listmonk/services/subscriptions.py:146
+msgid "email_subscribed_body"
+msgstr ""
+
+#. Default: "Subscription confirmed"
+#: collective/listmonk/services/subscriptions.py:142
+msgid "email_subscribed_subject"
+msgstr ""
+
 #. Default: "E-mail Footer"
 #: collective/listmonk/content/newsletter.py:55
 msgid "label_email_footer"
 msgstr ""
 
 #. Default: "E-mail Sender Name (From)"
 #: collective/listmonk/content/newsletter.py:45
@@ -66,15 +76,15 @@
 
 #. Default: "Topics"
 #: collective/listmonk/content/newsletter.py:19
 msgid "label_topics"
 msgstr ""
 
 #. Default: "newsletter-confirm"
-#: collective/listmonk/services/subscriptions.py:74
+#: collective/listmonk/services/subscriptions.py:77
 msgid "path_confirm"
 msgstr ""
 
 #. Default: "newsletter-unsubscribe"
-#: collective/listmonk/content/newsletter.py:76
+#: collective/listmonk/content/newsletter.py:91
 msgid "path_unsubscribe"
 msgstr ""
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/locales/update.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/rolemap.xml` & `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/profiles/default/types/Newsletter.xml` & `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles/default/types/Newsletter.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/profiles.zcml` & `collective.listmonk-1.0.0a4/src/collective/listmonk/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/services/base.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/services/base.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/services/configure.zcml` & `collective.listmonk-1.0.0a4/src/collective/listmonk/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/services/mailings.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/services/mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/services/subscriptions.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/services/subscriptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,21 +66,51 @@
                     "lists": list_ids,
                 },
             )
             subscriber = result["data"]
 
         pc = create_pending_confirmation(subscriber["id"], data)
         transaction.commit()
+        self.send_confirmation(data, pc)
+
+    def send_confirmation(self, data: SubscriptionRequest, pc: PendingConfirmation):
         confirm_path = translate(
             _("path_confirm", default="newsletter-confirm"), context=self.request
         )
         confirm_link = (
             f"{self.context.absolute_url()}/{confirm_path}?token={quote(pc.token)}"
         )
-        send_confirmation(self.context, self.request, data, confirm_link)
+        subject = translate(
+            _("email_confirm_subject", default="Confirm Subscription"),
+            context=self.request,
+        )
+        body = translate(
+            _(
+                "email_confirm_body",
+                default="""Someone has requested a subscription to ${newsletter}
+
+To confirm this subscription, click this link:
+${confirm_link}
+
+If you did not request this subscription, you can ignore this email.
+""",
+                mapping={
+                    "newsletter": self.context.title,
+                    "confirm_link": confirm_link,
+                },
+            ),
+            context=self.request,
+        )
+        api.portal.send_email(
+            sender=self.context.get_email_sender(),
+            recipient=data.email,
+            subject=subject,
+            body=body,
+            immediate=True,
+        )
 
 
 class ConfirmSubscriptionRequest(pydantic.BaseModel):
     token: str
 
 
 class ConfirmSubscription(PydanticService):
@@ -98,14 +128,46 @@
                 "ids": [pc.sub_id],
                 "action": "add",
                 "target_list_ids": pc.list_ids,
                 "status": "confirmed",
             },
         )
         del storage[data.token]
+        transaction.commit()
+        self.send_confirmation(pc)
+
+    def send_confirmation(self, pc: PendingConfirmation):
+        subscriber = listmonk.call_listmonk("get", f"/subscribers/{pc.sub_id}")
+        email = subscriber["data"]["email"]
+        subject = translate(
+            _("email_subscribed_subject", default="Subscription confirmed"),
+            context=self.request,
+        )
+        body = translate(
+            _(
+                "email_subscribed_body",
+                default="""You are now subscribed to the ${newsletter}
+
+You can unsubscribe using this link:
+${unsubscribe_link}
+""",
+                mapping={
+                    "newsletter": self.context.title,
+                    "unsubscribe_link": self.context.get_unsubscribe_link(),
+                },
+            ),
+            context=self.request,
+        )
+        api.portal.send_email(
+            sender=self.context.get_email_sender(),
+            recipient=email,
+            subject=subject,
+            body=body,
+            immediate=True,
+        )
 
 
 class UnsubscribeRequest(pydantic.BaseModel):
     list_ids: list[int]
     email: str
 
 
@@ -138,36 +200,7 @@
     sub_id: int, data: SubscriptionRequest
 ) -> PendingConfirmation:
     storage = get_pending_confirmation_storage()
     token = uuid.uuid4().hex
     pc = PendingConfirmation(token=token, sub_id=sub_id, list_ids=data.list_ids)
     storage[token] = pc.model_dump()
     return pc
-
-
-def send_confirmation(
-    newsletter: Newsletter, request, data: SubscriptionRequest, confirm_link: str
-):
-    subject = translate(
-        _("email_confirm_subject", default="Confirm Subscription"), context=request
-    )
-    body = translate(
-        _(
-            "email_confirm_body",
-            default="""Someone has requested a subscription to ${newsletter}
-
-To confirm this subscription, click this link:
-${confirm_link}
-
-If you did not request this subscription, you can ignore this email.
-""",
-            mapping={"newsletter": newsletter.title, "confirm_link": confirm_link},
-        ),
-        context=request,
-    )
-    api.portal.send_email(
-        sender=newsletter.get_email_sender(),
-        recipient=data.email,
-        subject=subject,
-        body=body,
-        immediate=True,
-    )
```

### Comparing `collective.listmonk-1.0.0a3/src/collective/listmonk/testing.py` & `collective.listmonk-1.0.0a4/src/collective/listmonk/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 "auth_protocol": "none",
                 "tls_type": "none",
             }
         )
         settings.update({"smtp": [smtp], "privacy.unsubscribe_header": False})
         listmonk.call_listmonk("put", "/settings", json=settings)
 
-        # Configure template
+        # Configure templates
         listmonk.call_listmonk(
             "put",
             "/templates/1",
             json={
                 "name": "Default campaign template",
                 "type": "campaign",
                 "body": '{{ template "content" . }}',
```

### Comparing `collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/PKG-INFO` & `collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,21 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-04-09)
+
+
+### New features:
+
+- Send an email confirmation of a new subscription. @davisagli #12
+
 ## 1.0.0a3 (2024-04-07)
 
 
 ### Bug fixes:
 
 - Don't add header and footer to the email automatically, so the editor has control. @davisagli #11
```

### Comparing `collective.listmonk-1.0.0a3/src/collective.listmonk.egg-info/SOURCES.txt` & `collective.listmonk-1.0.0a4/src/collective.listmonk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,13 +52,15 @@
 src/collective/listmonk/services/base.py
 src/collective/listmonk/services/configure.zcml
 src/collective/listmonk/services/mailings.py
 src/collective/listmonk/services/subscriptions.py
 src/collective/listmonk/setuphandlers/__init__.py
 src/collective/listmonk/upgrades/__init__.py
 src/collective/listmonk/upgrades/configure.zcml
+tests/__init__.py
 tests/conftest.py
+tests/api/__init__.py
 tests/api/test_mailings.py
 tests/api/test_subscriptions.py
 tests/setup/test_setup_install.py
 tests/setup/test_setup_uninstall.py
 tests/setup/upgrades/conftest.py
```

### Comparing `collective.listmonk-1.0.0a3/tests/api/test_mailings.py` & `collective.listmonk-1.0.0a4/tests/api/test_mailings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from ..conftest import poll_for_mail
+
 import email
 import pytest
-import time
 
 
 class TestNewsletterMailingsService:
     list_id = 1
 
     @pytest.fixture(autouse=True)
     def load_functional_layer(self, functional):
@@ -119,19 +120,7 @@
         assert item["newsletter"]["@id"] == newsletter.absolute_url()
         assert item["newsletter"]["title"] == newsletter.title
         assert item["topics"] == ["Test topic"]
         assert item["based_on"]["@id"] == portal.absolute_url()
         assert item["sent_by"] == "admin"
         assert item["subject"] == "Test mailing"
         assert "sent_at" in item
-
-
-def poll_for_mail(mailhog_client, expected=1, retries=15):
-    messages = mailhog_client.get("/messages").json()
-    orig_retries = retries
-    while retries > 0:
-        messages = mailhog_client.get("/messages").json()
-        if len(messages) == expected:
-            return messages
-        retries -= 1
-        time.sleep(1)
-    raise Exception(f"Timed out waiting for mail after {orig_retries}s")
```

### Comparing `collective.listmonk-1.0.0a3/tests/api/test_subscriptions.py` & `collective.listmonk-1.0.0a4/tests/api/test_subscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ..conftest import poll_for_mail
 from collective.listmonk import listmonk
 from urllib.parse import unquote
 
 import email
 import json
 import pytest
 import re
@@ -44,15 +45,17 @@
         # Assert unconfirmed subscription was created in listmonk
         subscriber = listmonk.get_subscriber("subscriber@example.com")
         subscription = [
             lst for lst in subscriber["lists"] if lst["id"] == self.list_id
         ][0]
         assert subscription["subscription_status"] == "unconfirmed"
 
-    def test_create_subscription_again(self, url, anon_plone_client, mailhog_client):
+    def test_create_subscription_again(
+        self, newsletter, url, anon_plone_client, mailhog_client
+    ):
         # Trying to create it a second time re-sends the confirmation.
         response = anon_plone_client.post(
             url,
             json={
                 "name": "Jean-Luc Picard",
                 "email": "subscriber@example.com",
                 "list_ids": [self.list_id],
@@ -77,14 +80,35 @@
         # Confirm status was updated in listmonk
         subscriber = listmonk.get_subscriber("subscriber@example.com")
         subscription = [
             lst for lst in subscriber["lists"] if lst["id"] == self.list_id
         ][0]
         assert subscription["subscription_status"] == "confirmed"
 
+        # Confirm email was sent to confirm subscription
+        poll_for_mail(mailhog_client, 3)
+        resp = mailhog_client.get("/messages")
+        messages = resp.json()
+        assert len(messages) == 3
+        msg = email.message_from_string(
+            messages[0]["Raw"]["Data"], policy=email.policy.default
+        )
+        body = msg.get_content()
+        assert msg["From"] == '"collective.listmonk tests" <testplone@example.com>'
+        assert msg["To"] == "subscriber@example.com"
+        assert msg["Subject"] == "Subscription confirmed"
+        assert msg["Content-Type"] == 'text/plain; charset="utf-8"'
+        assert (
+            msg.get_content()
+            == f"""You are now subscribed to the Test Newsletter\r
+\r
+You can unsubscribe using this link:\r
+{newsletter.absolute_url()}/newsletter-unsubscribe"""
+        )
+
     def test_create_subscription__bad_request(self, url, anon_plone_client):
         response = anon_plone_client.post(
             url,
             json={},
         )
         assert response.status_code == 400
         # Make sure it's in the format that volto expects
```

### Comparing `collective.listmonk-1.0.0a3/tests/conftest.py` & `collective.listmonk-1.0.0a4/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from plone.restapi.testing import RelativeSession
 from pytest_plone import fixtures_factory
 from pythongettext.msgfmt import Msgfmt
 from pythongettext.msgfmt import PoSyntaxError
 from typing import Generator
 
 import pytest
+import time
 import transaction
 
 
 pytest_plugins = ["pytest_plone"]
 
 
 globals().update(
@@ -94,7 +95,19 @@
     session.auth = ("admin", "admin")
     return session
 
 
 @pytest.fixture()
 def mailhog_client():
     return RelativeSession("http://localhost:8025/api/v1")
+
+
+def poll_for_mail(mailhog_client, expected=1, retries=15):
+    messages = mailhog_client.get("/messages").json()
+    orig_retries = retries
+    while retries > 0:
+        messages = mailhog_client.get("/messages").json()
+        if len(messages) == expected:
+            return messages
+        retries -= 1
+        time.sleep(1)
+    raise Exception(f"Timed out waiting for mail after {orig_retries}s")
```

### Comparing `collective.listmonk-1.0.0a3/tests/setup/test_setup_install.py` & `collective.listmonk-1.0.0a4/tests/setup/test_setup_install.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/tests/setup/test_setup_uninstall.py` & `collective.listmonk-1.0.0a4/tests/setup/test_setup_uninstall.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a3/tests/setup/upgrades/conftest.py` & `collective.listmonk-1.0.0a4/tests/setup/upgrades/conftest.py`

 * *Files identical despite different names*

