# Comparing `tmp/collective.eeafaceted.collectionwidget-1.8.tar.gz` & `tmp/collective.eeafaceted.collectionwidget-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.eeafaceted.collectionwidget-1.8.tar", last modified: Tue Aug 13 08:00:58 2019, max compression
+gzip compressed data, was "dist/collective.eeafaceted.collectionwidget-1.9.tar", last modified: Fri Aug 23 12:55:51 2019, max compression
```

## Comparing `collective.eeafaceted.collectionwidget-1.8.tar` & `collective.eeafaceted.collectionwidget-1.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2771 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/circle.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11137 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11137 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5728 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/not-zip-safe
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      985 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      530 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/categories.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1060 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/upgrades.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3180 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/mk_sync_locales.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      322 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      207 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/collectiveeeafacetedcollectionwidget_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2988 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/types/DashboardCollection.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      207 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/workflows.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      187 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      639 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1027 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/collectiveeeafacetedcollectionwidget_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone5/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone5/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2146 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone5/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone5/collectiveeeafacetedcollectionwidget_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3502 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1184 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3137 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/default_collection.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3828 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/layers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      425 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/testcase.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1085 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/content/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/content/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      513 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/content/dashboardcollection.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/content/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1852 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      253 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2871 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3914 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_categories.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1657 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2201 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1027 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_dashboardcollection.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15338 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_vocabulary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5013 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      640 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_robot.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/robot/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3696 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/robot/test_widget.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14747 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_widget.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1089 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/events.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2863 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/widget.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/view.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7200 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/view.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/edit.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/edit.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9095 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/widget.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      779 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2795 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1833 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7142 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/vocabulary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      564 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/permissions.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3659 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/views.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1265 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/templates/term.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      112 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/templates/category.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      261 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/static/collective.eeafaceted.collectionwidget.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      348 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/static/dashboardcollection.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1295 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       35 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1856 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/collective.eeafaceted.collectionwidget.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1621 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/collective.eeafaceted.collectionwidget.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1686 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/collective.eeafaceted.collectionwidget.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      163 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/update.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      289 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      222 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/travis.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1733 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6342 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/bootstrap.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5698 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      293 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      655 2019-08-13 08:00:58.000000 collective.eeafaceted.collectionwidget-1.8/Makefile
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2771 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      166 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/circle.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11419 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/PKG-INFO
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11419 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5728 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       33 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/not-zip-safe
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      985 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      530 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/categories.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1060 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/upgrades.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3180 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/mk_sync_locales.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      322 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      168 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      207 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      214 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/collectiveeeafacetedcollectionwidget_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2988 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/types/DashboardCollection.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      207 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/workflows.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      187 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      639 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1027 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/collectiveeeafacetedcollectionwidget_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone5/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      189 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone5/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2146 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone5/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone5/collectiveeeafacetedcollectionwidget_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3592 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1184 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3137 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/default_collection.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3828 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/layers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      425 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/testcase.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1085 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      513 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/content/dashboardcollection.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      179 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1852 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      253 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2871 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3914 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_categories.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1657 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2201 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1027 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_dashboardcollection.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15338 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_vocabulary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5013 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      640 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_robot.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/robot/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3696 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/robot/test_widget.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14747 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_widget.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1089 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/events.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2863 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/widget.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      380 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/view.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7200 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/view.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/edit.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/edit.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9095 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/widget.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      779 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      517 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2795 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      264 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1833 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7142 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/vocabulary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      564 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/permissions.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3659 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/views.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1265 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/templates/term.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      112 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/templates/category.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/static/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      261 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/static/collective.eeafaceted.collectionwidget.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      348 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/static/dashboardcollection.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1295 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       35 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1856 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/collective.eeafaceted.collectionwidget.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1621 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/collective.eeafaceted.collectionwidget.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1686 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/collective.eeafaceted.collectionwidget.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      163 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      289 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      222 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/travis.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2019-08-23 12:55:51.000000 collective.eeafaceted.collectionwidget-1.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1733 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6342 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/bootstrap.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5916 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      293 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      655 2019-08-23 12:55:50.000000 collective.eeafaceted.collectionwidget-1.9/Makefile
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/docs/LICENSE.rst` & `collective.eeafaceted.collectionwidget-1.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/docs/LICENSE.GPL` & `collective.eeafaceted.collectionwidget-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/README.rst` & `collective.eeafaceted.collectionwidget-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/PKG-INFO` & `collective.eeafaceted.collectionwidget-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.collectionwidget
-Version: 1.8
+Version: 1.9
 Summary: eea.facetednavigation widget that enables selecting a collection (among several) as base filter
 Home-page: http://pypi.python.org/pypi/collective.eeafaceted.collectionwidget
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Description: 
         .. image:: https://travis-ci.org/collective/collective.eeafaceted.collectionwidget.svg
@@ -54,14 +54,22 @@
         If you are using `eea.facetednavigation` < 10.0, you need to use a version of `collective.eeafaceted.collectionwidget` < 1.0.
         
         
         Changelog
         =========
         
         
+        1.9 (2019-08-23)
+        ----------------
+        
+        - Added parameter `raise_on_error=True` to `utils._get_criterion` so it will
+          return `None` in case passed context is not a faceted context instead
+          raising an error.
+          [gbastien]
+        
         1.8 (2019-08-13)
         ----------------
         
         - Do not store the collection object in `term.value` of vocabulary
           `CollectionVocabulary` because it can be ram cached
           (in `CachedCollectionVocabulary` for example) and ram caching methods
           returning objects is a bad idea.
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/PKG-INFO` & `collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.eeafaceted.collectionwidget
-Version: 1.8
+Version: 1.9
 Summary: eea.facetednavigation widget that enables selecting a collection (among several) as base filter
 Home-page: http://pypi.python.org/pypi/collective.eeafaceted.collectionwidget
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Description: 
         .. image:: https://travis-ci.org/collective/collective.eeafaceted.collectionwidget.svg
@@ -54,14 +54,22 @@
         If you are using `eea.facetednavigation` < 10.0, you need to use a version of `collective.eeafaceted.collectionwidget` < 1.0.
         
         
         Changelog
         =========
         
         
+        1.9 (2019-08-23)
+        ----------------
+        
+        - Added parameter `raise_on_error=True` to `utils._get_criterion` so it will
+          return `None` in case passed context is not a faceted context instead
+          raising an error.
+          [gbastien]
+        
         1.8 (2019-08-13)
         ----------------
         
         - Do not store the collection object in `term.value` of vocabulary
           `CollectionVocabulary` because it can be ram cached
           (in `CachedCollectionVocabulary` for example) and ram caching methods
           returning objects is a bad idea.
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective.eeafaceted.collectionwidget.egg-info/SOURCES.txt` & `collective.eeafaceted.collectionwidget-1.9/src/collective.eeafaceted.collectionwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/events.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/events.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/categories.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/categories.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/upgrades.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/mk_sync_locales.sh` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/common/types/DashboardCollection.xml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/common/types/DashboardCollection.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/jsregistry.xml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone4/cssregistry.xml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone4/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles/plone5/registry.xml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles/plone5/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/utils.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 from zope.annotation.interfaces import IAnnotations
 from zope.event import notify
 from zope.globalrequest import getRequest
 
 import json
 
 
-def _get_criterion(faceted_context, criterion_type):
+def _get_criterion(faceted_context, criterion_type, raise_on_error=True):
     """Return the given criterion_type instance of a
        context with a faceted navigation/search view on it."""
     if not IFacetedNavigable.providedBy(faceted_context):
-        raise NoFacetedViewDefinedException(NO_FACETED_EXCEPTION_MSG)
+        if raise_on_error:
+            raise NoFacetedViewDefinedException(NO_FACETED_EXCEPTION_MSG)
+        else:
+            return None
 
     criteria = ICriteria(faceted_context).criteria
     for criterion in criteria:
         if criterion.widget == criterion_type:
             return criterion
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/events.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/events.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/default_collection.xml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/default_collection.xml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing/layers.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing/layers.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/testing.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/content/dashboardcollection.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/content/dashboardcollection.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/interfaces.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/adapters.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_categories.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_setup.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_views.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_dashboardcollection.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_dashboardcollection.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_vocabulary.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_utils.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_robot.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/robot/test_widget.robot` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/robot/test_widget.robot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/tests/test_widget.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/events.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/events.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/widget.pt` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/widget.pt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/view.js` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/view.js`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/edit.js` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/edit.js`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/widget.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/widgets/configure.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/widgets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/setuphandlers.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/profiles.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/configure.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/vocabulary.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/permissions.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/views.py` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/templates/term.pt` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/templates/term.pt`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/browser/configure.zcml` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/collective.eeafaceted.collectionwidget.po` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/fr/LC_MESSAGES/collective.eeafaceted.collectionwidget.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/collective.eeafaceted.collectionwidget.po` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/en/LC_MESSAGES/collective.eeafaceted.collectionwidget.po`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/src/collective/eeafaceted/collectionwidget/locales/collective.eeafaceted.collectionwidget.pot` & `collective.eeafaceted.collectionwidget-1.9/src/collective/eeafaceted/collectionwidget/locales/collective.eeafaceted.collectionwidget.pot`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/setup.py` & `collective.eeafaceted.collectionwidget-1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 long_description = (
     open('README.rst').read() + '\n' + open('CHANGES.rst').read() + '\n')
 
 setup(
     name='collective.eeafaceted.collectionwidget',
-    version='1.8',
+    version='1.9',
     description=(
         "eea.facetednavigation widget that enables selecting "
         "a collection (among several) as base filter"),
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/bootstrap.py` & `collective.eeafaceted.collectionwidget-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.eeafaceted.collectionwidget-1.8/CHANGES.rst` & `collective.eeafaceted.collectionwidget-1.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog
 =========
 
 
+1.9 (2019-08-23)
+----------------
+
+- Added parameter `raise_on_error=True` to `utils._get_criterion` so it will
+  return `None` in case passed context is not a faceted context instead
+  raising an error.
+  [gbastien]
+
 1.8 (2019-08-13)
 ----------------
 
 - Do not store the collection object in `term.value` of vocabulary
   `CollectionVocabulary` because it can be ram cached
   (in `CachedCollectionVocabulary` for example) and ram caching methods
   returning objects is a bad idea.
```

### Comparing `collective.eeafaceted.collectionwidget-1.8/Makefile` & `collective.eeafaceted.collectionwidget-1.9/Makefile`

 * *Files identical despite different names*

