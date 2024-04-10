# Comparing `tmp/collective.iconifiedcategory-0.8.tar.gz` & `tmp/collective.iconifiedcategory-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.iconifiedcategory-0.8.tar", last modified: Wed Jan 25 14:28:10 2017, max compression
+gzip compressed data, was "dist/collective.iconifiedcategory-0.9.tar", last modified: Tue Jan 31 16:10:37 2017, max compression
```

## Comparing `collective.iconifiedcategory-0.8.tar` & `collective.iconifiedcategory-0.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      666 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       84 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/docs/index.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1312 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6099 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/PKG-INFO
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      188 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2498 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6489 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/adapter.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      941 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/widget.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/category_title_hidden.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/collectivecategorize_testing.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/types.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      347 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/testing/types/Document.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      582 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/controlpanel.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      341 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1538 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/actions.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      193 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/collectivecategorize_default.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2193 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryGroup.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryConfiguration.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2073 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2047 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentSubcategory.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12267 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4925 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/category.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1045 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/subcategory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1186 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/categorygroup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      480 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/categoryconfiguration.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1805 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      993 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      878 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/event.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1497 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1583 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1008 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/adapter.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1676 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4638 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_actionview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5747 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_behaviors.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3017 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/file.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3617 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône2.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3742 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône1.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1406 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_browser_subtyper.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      211 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/adapters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6670 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_tabview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10886 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_adapter.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3796 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône3.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2857 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_vocabularies.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6287 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_editview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2226 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4112 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1506 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_css.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16917 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_robot.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3870 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_browser_config.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/robot/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5670 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/robot/test_categorization.robot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1852 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/setuphandlers.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2634 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      605 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/testing-adapters.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1048 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/editview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      277 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/viewlets.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/overrides/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/overrides/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4095 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/views.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2639 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-childs-infos.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1009 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-childs.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-tab-view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      393 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-child-viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/update_categorize_elements.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8600 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/tabview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      618 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/controlpanel.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3317 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/iconifiedcategory.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3989 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/iconifiedcategory.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      644 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/more_infos.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/.gitkeep
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4701 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/actionview.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1123 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/css.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1471 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7673 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1525 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/subtyper.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2972 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/iconifiedcategorization.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      540 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4036 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/collective.iconifiedcategory.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      988 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5360 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      793 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/update.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6099 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6023 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      345 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/requires.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       67 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      152 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1999 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2949 2017-01-25 14:28:10.000000 collective.iconifiedcategory-0.8/CHANGES.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      666 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       84 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/docs/index.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1312 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6793 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/PKG-INFO
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      188 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2498 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6489 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/adapter.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      941 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/widget.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      573 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/category_title_hidden.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/collectivecategorize_testing.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/types.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      347 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/testing/types/Document.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      527 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      292 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      582 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/controlpanel.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      341 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      896 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1538 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/actions.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      355 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      193 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/collectivecategorize_default.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2193 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryGroup.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2165 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryConfiguration.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2073 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2047 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentSubcategory.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12217 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5530 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/category.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1045 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/subcategory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1186 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/categorygroup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      480 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/categoryconfiguration.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1805 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      993 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      878 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/event.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1497 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1583 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1008 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/adapter.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1676 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4638 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_actionview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5747 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_behaviors.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3017 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/file.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3617 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône2.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3742 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône1.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1406 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_browser_subtyper.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      211 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/adapters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6670 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_tabview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10886 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_adapter.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3796 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône3.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2857 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_vocabularies.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6215 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_editview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2226 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8239 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1506 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_css.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16917 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      915 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_robot.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3870 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_browser_config.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5670 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/robot/test_categorization.robot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1852 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2634 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      605 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/testing-adapters.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1048 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/editview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      277 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/viewlets.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/overrides/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/overrides/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4095 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/views.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2639 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-childs-infos.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1009 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-childs.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      337 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-tab-view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      393 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-child-viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      280 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/update_categorize_elements.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8600 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/tabview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      618 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/controlpanel.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3317 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/iconifiedcategory.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4007 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/iconifiedcategory.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      644 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/more_infos.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4701 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/actionview.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1123 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/css.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1471 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7673 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1525 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/subtyper.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2972 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/iconifiedcategorization.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      540 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4036 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/collective.iconifiedcategory.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      988 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5360 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      793 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/update.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6793 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6023 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      345 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/requires.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       67 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      152 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1999 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3523 2017-01-31 16:10:37.000000 collective.iconifiedcategory-0.9/CHANGES.rst
```

### Comparing `collective.iconifiedcategory-0.8/docs/LICENSE.rst` & `collective.iconifiedcategory-0.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/docs/LICENSE.GPL` & `collective.iconifiedcategory-0.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/README.rst` & `collective.iconifiedcategory-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/PKG-INFO` & `collective.iconifiedcategory-0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.iconifiedcategory
-Version: 0.8
+Version: 0.9
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/collective.iconifiedcategory
 Author: IMIO
 Author-email: support@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -53,14 +53,29 @@
         ============
         
         - Martin Peeters, Original Author [Affinitic]
         
         Changelog
         =========
         
+        0.9 (2017-01-31)
+        ----------------
+        
+        - Adapted CSS selector that changes `font-size` of number of categorized
+          elements displayed in the tooltipster
+          [gbastien]
+        - Added a way to defer the categorized_content_created event and to defer
+          call to utils.update_categorized_elements in the categorized_content_updated
+          event.  This way we may manage adding several categorized elements but only
+          updating the categorized_elements dict (including time consuming sorting)
+          at the right time
+          [gbastien]
+        - Fixed tests to work in both Plone 4.3.7 and Plone 4.3.11
+          [gbastien]
+        
         0.8 (2017-01-25)
         ----------------
         
         - Do not fail in `categorized-childs-infos` if current context does not have
           the `categorized_elements` dict
           [gbastien]
```

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/vocabularies.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/adapter.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/adapter.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/widget.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/widget.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/widget/category_title_hidden.pt` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/widget/category_title_hidden.pt`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/metadata.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/controlpanel.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/registry.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/actions.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/cssregistry.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryGroup.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryGroup.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryConfiguration.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategoryConfiguration.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentCategory.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentCategory.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/profiles/default/types/ContentSubcategory.xml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/profiles/default/types/ContentSubcategory.xml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/utils.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,24 +144,24 @@
     uid, infos = get_categorized_infos(obj, category)
     parent.categorized_elements[uid] = infos
     sort_categorized_elements(parent)
     parent._p_changed = True
 
 
 def update_all_categorized_elements(container):
-    if 'categorized_elements' in container.__dict__:
-        container.categorized_elements = OrderedDict()
-        for obj in container.objectValues():
-            if hasattr(obj, 'content_category'):
-                try:
-                    category = get_category_object(obj, obj.content_category)
-                except KeyError:
-                    continue
-                uid, infos = get_categorized_infos(obj, category)
-                container.categorized_elements[uid] = infos
+    container.categorized_elements = OrderedDict()
+    for obj in container.objectValues():
+        if hasattr(obj, 'content_category'):
+            try:
+                category = get_category_object(obj, obj.content_category)
+            except KeyError:
+                continue
+            uid, infos = get_categorized_infos(obj, category)
+            container.categorized_elements[uid] = infos
+    if container.categorized_elements:
         sort_categorized_elements(container)
         container._p_changed = True
 
 
 def get_ordered_categories(context):
     """Return an ordered dict for categories (id and uids)"""
     elements = {}
```

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/events.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 from collective.iconifiedcategory.event import \
     IconifiedConfidentialChangedEvent
 from collective.iconifiedcategory.event import IconifiedPrintChangedEvent
 from collective.iconifiedcategory.interfaces import IIconifiedPrintable
 
 
 def categorized_content_created(event):
+
     if hasattr(event.object, 'content_category'):
+        # if 'to_print' and 'confidential' are managed manually,
+        # we may defer events if relevant value found in the REQUEST
+        if event.object.REQUEST.get('defer_categorized_content_created_event', False):
+            return
+
         if hasattr(event.object, 'confidential'):
             notify(IconifiedConfidentialChangedEvent(
                 event.object,
                 None,
                 event.object.confidential,
             ))
         categorized_content_updated(event)
@@ -63,14 +69,21 @@
             adapter = getAdapter(event.object, IIconifiedPrintable)
             adapter.update_object()
             notify(IconifiedPrintChangedEvent(
                 obj,
                 obj.to_print,
                 obj.to_print,
             ))
+        # we may defer call to utils.update_categorized_elements
+        # if relevant value found in the REQUEST
+        # this is useful when adding several categorized elements without
+        # calling update_categorized_elements between every added element
+        if event.object.REQUEST.get('defer_update_categorized_elements', False):
+            return
+
         utils.update_categorized_elements(obj.aq_parent, obj, target)
 
 
 def categorized_content_removed(event):
     if hasattr(event.object, 'content_category'):
         obj = event.object
         utils.remove_categorized_element(obj.aq_parent, obj)
```

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/category.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/category.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/subcategory.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/subcategory.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/categorygroup.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/categorygroup.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/configure.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/content/base.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/content/base.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/event.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/event.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/testing.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/testing.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/interfaces.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/indexes.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/indexes.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/adapter.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/adapter.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_setup.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_actionview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_actionview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_behaviors.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/file.txt` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/file.txt`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône2.png` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône2.png`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône1.png` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône1.png`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_browser_subtyper.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_browser_subtyper.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_tabview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_tabview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_adapter.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/icône3.png` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/icône3.png`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_vocabularies.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_views.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,18 @@
 class TestCanViewAwareDownload(BaseTestCase):
 
     def test_default(self):
         # by default @@download returns the file, here
         # it is also the case as IIconifiedContent.can_view adapter returns True by default
         file_obj = self.portal['file']
         img_obj = self.portal['image']
-        self.assertTrue(isinstance(file_obj.restrictedTraverse('@@download')(), file))
-        self.assertTrue(isinstance(file_obj.restrictedTraverse('@@display-file')(), file))
-        self.assertTrue(isinstance(img_obj.restrictedTraverse('@@download')(), file))
-        self.assertTrue(isinstance(img_obj.restrictedTraverse('@@display-file')(), file))
+        self.assertTrue(file_obj.restrictedTraverse('@@download')())
+        self.assertTrue(file_obj.restrictedTraverse('@@display-file')())
+        self.assertTrue(img_obj.restrictedTraverse('@@download')())
+        self.assertTrue(img_obj.restrictedTraverse('@@display-file')())
 
     def test_can_not_view(self):
         # register an adapter that will return False
         zcml.load_config('testing-adapters.zcml', collective_iconifiedcategory)
         file_obj = self.portal['file']
         img_obj = self.portal['image']
         self.assertRaises(Unauthorized, file_obj.restrictedTraverse('@@download'))
```

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_editview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_editview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/base.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/base.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_css.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_utils.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_robot.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/test_browser_config.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/test_browser_config.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/tests/robot/test_categorization.robot` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/tests/robot/test_categorization.robot`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/setuphandlers.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/configure.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/testing-adapters.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/testing-adapters.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/editview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/editview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/views.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-childs-infos.pt` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-childs-infos.pt`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/templates/categorized-childs.pt` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/templates/categorized-childs.pt`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/tabview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/tabview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/controlpanel.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/iconifiedcategory.js` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/iconifiedcategory.js`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/iconifiedcategory.css` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/iconifiedcategory.css`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 }
 
 #content div.categorized-elements h2 {
     margin-bottom: 0.3em;
 }
 
 /* display number of elements smaller */
-.tooltip.deactivated.tooltipstered > span {
-    font-size: 80%;
+div.categorized-elements a.deactivated.tooltipstered > span {
+    font-size: 90%;
 }
 
 #content div.categorized-elements a:link,
 #content div.categorized-elements a:hover,
 #content div.categorized-elements a:visited {
     color: #666;
     /* added !important to override default behavior of base.css that removes border-bottom in table.listing a */
```

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/static/more_infos.png` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/static/more_infos.png`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/actionview.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/actionview.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/css.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/css.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/config.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/config.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/configure.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/browser/subtyper.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/browser/subtyper.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/iconifiedcategorization.py` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/iconifiedcategorization.py`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/behaviors/configure.zcml` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/collective.iconifiedcategory.pot` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/collective.iconifiedcategory.pot`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/manual.pot` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/fr/LC_MESSAGES/collective.iconifiedcategory.po`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective/iconifiedcategory/locales/update.sh` & `collective.iconifiedcategory-0.9/src/collective/iconifiedcategory/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/PKG-INFO` & `collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: collective.iconifiedcategory
-Version: 0.8
+Version: 0.9
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/collective.iconifiedcategory
 Author: IMIO
 Author-email: support@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -53,14 +53,29 @@
         ============
         
         - Martin Peeters, Original Author [Affinitic]
         
         Changelog
         =========
         
+        0.9 (2017-01-31)
+        ----------------
+        
+        - Adapted CSS selector that changes `font-size` of number of categorized
+          elements displayed in the tooltipster
+          [gbastien]
+        - Added a way to defer the categorized_content_created event and to defer
+          call to utils.update_categorized_elements in the categorized_content_updated
+          event.  This way we may manage adding several categorized elements but only
+          updating the categorized_elements dict (including time consuming sorting)
+          at the right time
+          [gbastien]
+        - Fixed tests to work in both Plone 4.3.7 and Plone 4.3.11
+          [gbastien]
+        
         0.8 (2017-01-25)
         ----------------
         
         - Do not fail in `categorized-childs-infos` if current context does not have
           the `categorized_elements` dict
           [gbastien]
```

### Comparing `collective.iconifiedcategory-0.8/src/collective.iconifiedcategory.egg-info/SOURCES.txt` & `collective.iconifiedcategory-0.9/src/collective.iconifiedcategory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.iconifiedcategory-0.8/setup.py` & `collective.iconifiedcategory-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '\n' +
     open('CHANGES.rst').read() +
     '\n')
 
 
 setup(
     name='collective.iconifiedcategory',
-    version='0.8',
+    version='0.9',
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `collective.iconifiedcategory-0.8/CHANGES.rst` & `collective.iconifiedcategory-0.9/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+0.9 (2017-01-31)
+----------------
+
+- Adapted CSS selector that changes `font-size` of number of categorized
+  elements displayed in the tooltipster
+  [gbastien]
+- Added a way to defer the categorized_content_created event and to defer
+  call to utils.update_categorized_elements in the categorized_content_updated
+  event.  This way we may manage adding several categorized elements but only
+  updating the categorized_elements dict (including time consuming sorting)
+  at the right time
+  [gbastien]
+- Fixed tests to work in both Plone 4.3.7 and Plone 4.3.11
+  [gbastien]
+
 0.8 (2017-01-25)
 ----------------
 
 - Do not fail in `categorized-childs-infos` if current context does not have
   the `categorized_elements` dict
   [gbastien]
```

