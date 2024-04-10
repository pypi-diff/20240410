# Comparing `tmp/imio.directory.core-1.2.8.tar.gz` & `tmp/imio.directory.core-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.directory.core-1.2.8.tar", last modified: Mon Feb 12 13:31:40 2024, max compression
+gzip compressed data, was "imio.directory.core-1.2.9.tar", last modified: Tue Feb 27 13:40:36 2024, max compression
```

## Comparing `imio.directory.core-1.2.8.tar` & `imio.directory.core-1.2.9.tar`

### file list

```diff
@@ -1,125 +1,131 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4939 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      128 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      670 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10548 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4458 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7996 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-02-12 13:31:40.848940 imio.directory.core-1.2.8/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2811 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.836940 imio.directory.core-1.2.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      335 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      972 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1363 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/import.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11997 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/import.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      897 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       53 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/config.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1016 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      107 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      136 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1925 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11584 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2013 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4503 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4136 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1737 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1710 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7229 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/export.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.836940 imio.directory.core-1.2.8/src/imio/directory/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/faceted/config/entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3709 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1357 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      284 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1070 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/monkey.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      668 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/monkey.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      640 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.836940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1538 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      182 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2099 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      730 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      661 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      456 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      325 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    96418 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1884 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1598 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      242 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/testing/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      162 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/testing/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      507 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/testing/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1218 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/profiles.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      785 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5170 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1166 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1825 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1802 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/resources/json_contact.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9847 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/resources/logo.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2007 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    21464 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_contact.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2431 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7090 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7013 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_export.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1591 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10334 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      930 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2026 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2709 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      508 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4743 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      290 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/imio.directory.Entity.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.844940 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8546 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2138 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3612 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1168 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio/directory/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-02-12 13:31:40.840940 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10548 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4126 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       20 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      511 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-02-12 13:31:40.000000 imio.directory.core-1.2.8/src/imio.directory.core.egg-info/top_level.txt
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.420677 imio.directory.core-1.2.9/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5136 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/CHANGES.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)      128 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)      586 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/DEVELOP.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)    18092 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/LICENSE.GPL
+-rw-rw-r--   0 remi      (1000) remi      (1000)      670 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/LICENSE.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)      106 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/MANIFEST.in
+-rw-r--r--   0 remi      (1000) remi      (1000)    11757 2024-02-27 13:40:36.420677 imio.directory.core-1.2.9/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4458 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/README.rst
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/docs/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7996 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/docs/conf.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       80 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/docs/index.rst
+-rw-rw-r--   0 remi      (1000) remi      (1000)       64 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/requirements.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)      518 2024-02-27 13:40:36.420677 imio.directory.core-1.2.9/setup.cfg
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2811 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/setup.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       80 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/
+-rw-rw-r--   0 remi      (1000) remi      (1000)       80 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      335 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/browser/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      972 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1363 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/import.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)    11997 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/import.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/browser/overrides/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/browser/static/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/static/.gitkeep
+-rw-rw-r--   0 remi      (1000) remi      (1000)      897 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/browser/utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)       53 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/config.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1016 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/configure.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/contents/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      107 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      136 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/configure.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1925 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)    11584 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/content.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2013 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/forms.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4503 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/serializer.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4136 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/view.pt
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1737 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/view.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      562 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/configure.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1710 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/content.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7229 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/export.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      487 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/converters.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/core/faceted/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/faceted/config/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7958 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/faceted/config/entity.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3709 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/indexers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1357 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/indexers.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      284 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/interfaces.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1070 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/monkey.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      668 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/monkey.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      350 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/overrides.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      640 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/permissions.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1538 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/actions.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      182 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2099 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/catalog.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      730 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/metadata.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1275 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/registry.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      456 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/taxonomies/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      325 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.cfg
+-rw-rw-r--   0 remi      (1000) remi      (1000)    96418 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1920 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1634 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      242 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/testing/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      162 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/testing/metadata.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      507 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/testing/registry.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/profiles/uninstall/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      129 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1218 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/profiles.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      785 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/setuphandlers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     5170 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/subscribers.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1166 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/subscribers.zcml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1825 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/testing.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/tests/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/__init__.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/tests/resources/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1802 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/resources/json_contact.json
+-rw-rw-r--   0 remi      (1000) remi      (1000)     9847 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/resources/logo.png
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/tests/robot/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2007 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/robot/test_example.robot
+-rw-rw-r--   0 remi      (1000) remi      (1000)    21464 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_contact.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2431 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_cropping.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7090 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_entity.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     7013 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_export.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1591 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_local_roles.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)    10334 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_multilingual.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      930 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_robot.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2026 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_setup.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2876 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2709 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/test_vocabularies.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)      508 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/tests/utils.py
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/
+-rw-rw-r--   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/__init__.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     6001 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/configure.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      290 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1003_to_1004/types/imio.directory.Entity.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1066 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1013_to_1014/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      743 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1013_to_1014/registry.xml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.412677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1014_to_1015/
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1014_to_1015/types/
+-rw-rw-r--   0 remi      (1000) remi      (1000)      319 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1014_to_1015/types/imio.directory.Contact.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)      318 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1014_to_1015/types/imio.directory.Entity.xml
+-rw-rw-r--   0 remi      (1000) remi      (1000)     8546 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/upgrades/upgrades.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     2138 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/utils.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     3612 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/vocabularies.py
+-rw-rw-r--   0 remi      (1000) remi      (1000)     1168 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio/directory/core/vocabularies.zcml
+drwxrwxr-x   0 remi      (1000) remi      (1000)        0 2024-02-27 13:40:36.416677 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/
+-rw-r--r--   0 remi      (1000) remi      (1000)    11757 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/PKG-INFO
+-rw-rw-r--   0 remi      (1000) remi      (1000)     4369 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)       20 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        1 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/not-zip-safe
+-rw-rw-r--   0 remi      (1000) remi      (1000)      511 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/requires.txt
+-rw-rw-r--   0 remi      (1000) remi      (1000)        5 2024-02-27 13:40:36.000000 imio.directory.core-1.2.9/src/imio.directory.core.egg-info/top_level.txt
```

### Comparing `imio.directory.core-1.2.8/CHANGES.rst` & `imio.directory.core-1.2.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changelog
 =========
 
 
+1.2.9 (2024-02-27)
+------------------
+
+- WEB-4072, WEB-4073 : Enable solr.fields behavior on some content types
+  [remdub]
+
+- WEB-4006 : Exclude some content types from search results
+  [remdub]
+
+
 1.2.8 (2024-02-12)
 ------------------
 
 - MWEBRCHA-14 : Add view to export contacts to csv file
   [boulch]
```

### Comparing `imio.directory.core-1.2.8/DEVELOP.rst` & `imio.directory.core-1.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/LICENSE.GPL` & `imio.directory.core-1.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/LICENSE.rst` & `imio.directory.core-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/PKG-INFO` & `imio.directory.core-1.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.directory.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio contacts Directory websites
 Home-page: https://github.com/imio/imio.directory.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.directory.core
 Project-URL: Source, https://github.com/imio/imio.directory.core
@@ -16,17 +16,43 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: z3c.unconfigure
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.gallery
+Requires-Dist: plone.restapi
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: pandas
+Requires-Dist: collective.taxonomy
+Requires-Dist: embeddify
+Requires-Dist: imio.smartweb.common
+Requires-Dist: imio.smartweb.locales
+Requires-Dist: collective.instancebehavior
+Requires-Dist: collective.z3cform.datagridfield>=2.0
+Requires-Dist: collective.geolocationbehavior
+Requires-Dist: collective.monkeypatcher
+Requires-Dist: collective.schedulefield
+Requires-Dist: vobject
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
+Requires-Dist: beautifulsoup4; extra == "test"
+Requires-Dist: plone.restapi[test]; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://github.com/IMIO/imio.directory.core/workflows/Tests/badge.svg
     :target: https://github.com/IMIO/imio.directory.core/actions?query=workflow%3ATests
@@ -186,14 +212,24 @@
 - Laurent Lasudry, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-02-27)
+------------------
+
+- WEB-4072, WEB-4073 : Enable solr.fields behavior on some content types
+  [remdub]
+
+- WEB-4006 : Exclude some content types from search results
+  [remdub]
+
+
 1.2.8 (2024-02-12)
 ------------------
 
 - MWEBRCHA-14 : Add view to export contacts to csv file
   [boulch]
```

### Comparing `imio.directory.core-1.2.8/README.rst` & `imio.directory.core-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/docs/conf.py` & `imio.directory.core-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/setup.cfg` & `imio.directory.core-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/setup.py` & `imio.directory.core-1.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.directory.core",
-    version="1.2.8",
+    version="1.2.9",
     description="Core product for iMio contacts Directory websites",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/browser/configure.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/browser/import.pt` & `imio.directory.core-1.2.9/src/imio/directory/core/browser/import.pt`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/browser/import.py` & `imio.directory.core-1.2.9/src/imio/directory/core/browser/import.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/browser/utils.py` & `imio.directory.core-1.2.9/src/imio/directory/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/configure.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/configure.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/content.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/content.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/forms.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/forms.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/serializer.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/view.pt` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/view.pt`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/contact/view.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/contact/view.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/configure.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/content.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/contents/entity/export.py` & `imio.directory.core-1.2.9/src/imio/directory/core/contents/entity/export.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/faceted/config/entity.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/faceted/config/entity.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/indexers.py` & `imio.directory.core-1.2.9/src/imio/directory/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/indexers.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/monkey.py` & `imio.directory.core-1.2.9/src/imio/directory/core/monkey.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/monkey.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/monkey.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/permissions.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/actions.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/catalog.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/metadata.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/metadata.xml`

 * *Files 10% similar despite different names*

#### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/metadata.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>1013</version>
+  <version>1014</version>
   <dependencies>
     <dependency>profile-plone.app.dexterity:default</dependency>
     <dependency>profile-plone.gallery:default</dependency>
     <dependency>profile-plone.restapi:default</dependency>
     <dependency>profile-plone.app.imagecropping:default</dependency>
     <dependency>profile-collective.z3cform.datagridfield:default</dependency>
     <dependency>profile-collective.schedulefield:default</dependency>
```

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/taxonomies/contact_category.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml`

 * *Files 7% similar despite different names*

#### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Contact.xml`

```diff
@@ -25,14 +25,15 @@
     <element value="geolocatable"/>
     <element value="collective.schedulefield.behavior.IMultiScheduledContent"/>
     <element value="collective.schedulefield.behavior.IExceptionalClosureContent"/>
     <element value="collective.taxonomy.generated.contact_category"/>
     <element value="imio.smartweb.topics"/>
     <element value="imio.smartweb.iam"/>
     <element value="plone.categorization"/>
+    <element value="solr.fields"/>
   </property>
   <!-- View information -->
   <property name="default_view">view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
     <element value="view"/>
```

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml`

 * *Files 9% similar despite different names*

#### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles/default/types/imio.directory.Entity.xml`

```diff
@@ -20,14 +20,15 @@
     <element value="plone.shortname"/>
     <element value="plone.excludefromnavigation"/>
     <element value="plone.categorization"/>
     <element value="plone.basic"/>
     <element value="plone.locking"/>
     <element value="plone.leadimage"/>
     <element value="eea.faceted.navigable"/>
+    <element value="solr.fields"/>
   </property>
   <!-- View information -->
   <property name="default_view">view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
     <element value="view"/>
```

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/profiles.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/setuphandlers.py` & `imio.directory.core-1.2.9/src/imio/directory/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/subscribers.py` & `imio.directory.core-1.2.9/src/imio/directory/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/subscribers.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/testing.py` & `imio.directory.core-1.2.9/src/imio/directory/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/resources/json_contact.json` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/resources/json_contact.json`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/resources/logo.png` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/resources/logo.png`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/robot/test_example.robot` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_contact.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_cropping.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_entity.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_export.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_local_roles.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_multilingual.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_robot.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_setup.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_utils.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/tests/test_vocabularies.py` & `imio.directory.core-1.2.9/src/imio/directory/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/upgrades/configure.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/upgrades/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,30 @@
     name="upgrade_1006_to_1007"
     title="Upgrade core from 1006 to 1007"
     directory="profiles/1006_to_1007"
     description="Add more missing translations indexes / metadata"
     provides="Products.GenericSetup.interfaces.EXTENSION"
     />
 
+    <genericsetup:registerProfile
+      name="upgrade_1013_to_1014"
+      title="Upgrade core from 1013 to 1014"
+      directory="profiles/1013_to_1014"
+      description="Exclude some content_types from search results"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
+    <genericsetup:registerProfile
+      name="upgrade_1014_to_1015"
+      title="Upgrade core from 1014 to 1015"
+      directory="profiles/1014_to_1015"
+      description="Add solr.fields behavior to some content types"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:upgradeStep
       title="Add selected_entities to existing contacts"
       description="Every contact should have its current entity in selected_entities"
       source="1000"
       destination="1001"
       handler=".upgrades.add_current_entity_on_contacts"
       profile="imio.directory.core:default"
@@ -143,8 +159,28 @@
             />
         <genericsetup:upgradeStep
             title="Reindex SolR"
             handler=".upgrades.reindex_solr"
             />
     </genericsetup:upgradeSteps>
 
+    <genericsetup:upgradeSteps
+      source="1013"
+      destination="1014"
+      profile="imio.directory.core:default">
+      <genericsetup:upgradeDepends
+        title="Exclude some content_types from search results"
+        import_profile="imio.directory.core.upgrades:upgrade_1013_to_1014"
+        />
+    </genericsetup:upgradeSteps>
+
+    <genericsetup:upgradeSteps
+      source="1014"
+      destination="1015"
+      profile="imio.directory.core:default">
+      <genericsetup:upgradeDepends
+        title="Add solr.fields behavior to some content types"
+        import_profile="imio.directory.core.upgrades:upgrade_1014_to_1015"
+        />
+    </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml` & `imio.directory.core-1.2.9/src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/upgrades/upgrades.py` & `imio.directory.core-1.2.9/src/imio/directory/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/utils.py` & `imio.directory.core-1.2.9/src/imio/directory/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/vocabularies.py` & `imio.directory.core-1.2.9/src/imio/directory/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio/directory/core/vocabularies.zcml` & `imio.directory.core-1.2.9/src/imio/directory/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.directory.core-1.2.8/src/imio.directory.core.egg-info/PKG-INFO` & `imio.directory.core-1.2.9/src/imio.directory.core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.directory.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio contacts Directory websites
 Home-page: https://github.com/imio/imio.directory.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.directory.core
 Project-URL: Source, https://github.com/imio/imio.directory.core
@@ -16,17 +16,43 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: z3c.unconfigure
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.gallery
+Requires-Dist: plone.restapi
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: pandas
+Requires-Dist: collective.taxonomy
+Requires-Dist: embeddify
+Requires-Dist: imio.smartweb.common
+Requires-Dist: imio.smartweb.locales
+Requires-Dist: collective.instancebehavior
+Requires-Dist: collective.z3cform.datagridfield>=2.0
+Requires-Dist: collective.geolocationbehavior
+Requires-Dist: collective.monkeypatcher
+Requires-Dist: collective.schedulefield
+Requires-Dist: vobject
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
+Requires-Dist: beautifulsoup4; extra == "test"
+Requires-Dist: plone.restapi[test]; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://github.com/IMIO/imio.directory.core/workflows/Tests/badge.svg
     :target: https://github.com/IMIO/imio.directory.core/actions?query=workflow%3ATests
@@ -186,14 +212,24 @@
 - Laurent Lasudry, laurent.lasudry@affinitic.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-02-27)
+------------------
+
+- WEB-4072, WEB-4073 : Enable solr.fields behavior on some content types
+  [remdub]
+
+- WEB-4006 : Exclude some content types from search results
+  [remdub]
+
+
 1.2.8 (2024-02-12)
 ------------------
 
 - MWEBRCHA-14 : Add view to export contacts to csv file
   [boulch]
```

### Comparing `imio.directory.core-1.2.8/src/imio.directory.core.egg-info/SOURCES.txt` & `imio.directory.core-1.2.9/src/imio.directory.core.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -88,8 +88,11 @@
 src/imio/directory/core/tests/resources/json_contact.json
 src/imio/directory/core/tests/resources/logo.png
 src/imio/directory/core/tests/robot/test_example.robot
 src/imio/directory/core/upgrades/__init__.py
 src/imio/directory/core/upgrades/configure.zcml
 src/imio/directory/core/upgrades/upgrades.py
 src/imio/directory/core/upgrades/profiles/1003_to_1004/types/imio.directory.Entity.xml
-src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
+src/imio/directory/core/upgrades/profiles/1006_to_1007/catalog.xml
+src/imio/directory/core/upgrades/profiles/1013_to_1014/registry.xml
+src/imio/directory/core/upgrades/profiles/1014_to_1015/types/imio.directory.Contact.xml
+src/imio/directory/core/upgrades/profiles/1014_to_1015/types/imio.directory.Entity.xml
```

