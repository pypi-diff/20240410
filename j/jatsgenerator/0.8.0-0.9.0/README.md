# Comparing `tmp/jatsgenerator-0.8.0.tar.gz` & `tmp/jatsgenerator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jatsgenerator-0.8.0.tar", last modified: Sat Oct  7 00:56:57 2023, max compression
+gzip compressed data, was "jatsgenerator-0.9.0.tar", last modified: Thu Dec  7 22:44:02 2023, max compression
```

## Comparing `jatsgenerator-0.8.0.tar` & `jatsgenerator-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5910 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5253 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/jatsgenerator/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/jatsgenerator/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    23653 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/jatsgenerator/build.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1531 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/jatsgenerator/conf.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    17217 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/jatsgenerator/generate.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     3083 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/jatsgenerator/utils.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/jatsgenerator.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     5910 2023-10-07 00:56:56.000000 jatsgenerator-0.8.0/jatsgenerator.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      441 2023-10-07 00:56:57.000000 jatsgenerator-0.8.0/jatsgenerator.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-10-07 00:56:56.000000 jatsgenerator-0.8.0/jatsgenerator.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       83 2023-10-07 00:56:56.000000 jatsgenerator-0.8.0/jatsgenerator.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       14 2023-10-07 00:56:56.000000 jatsgenerator-0.8.0/jatsgenerator.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      140 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      910 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-10-07 00:56:57.005518 jatsgenerator-0.8.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    15310 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/tests/test_build.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     2711 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/tests/test_conf.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    15992 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/tests/test_generate.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1852 2023-10-07 00:56:07.000000 jatsgenerator-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5910 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5253 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/jatsgenerator/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/jatsgenerator/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    23763 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/jatsgenerator/build.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1531 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/jatsgenerator/conf.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    17217 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/jatsgenerator/generate.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     3083 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/jatsgenerator/utils.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/jatsgenerator.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5910 2023-12-07 22:44:02.000000 jatsgenerator-0.9.0/jatsgenerator.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      441 2023-12-07 22:44:02.000000 jatsgenerator-0.9.0/jatsgenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-12-07 22:44:02.000000 jatsgenerator-0.9.0/jatsgenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       83 2023-12-07 22:44:02.000000 jatsgenerator-0.9.0/jatsgenerator.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       14 2023-12-07 22:44:02.000000 jatsgenerator-0.9.0/jatsgenerator.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      140 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      910 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-12-07 22:44:02.728388 jatsgenerator-0.9.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    15958 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/tests/test_build.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     2711 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/tests/test_conf.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    15992 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/tests/test_generate.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1852 2023-12-07 22:42:57.000000 jatsgenerator-0.9.0/tests/test_utils.py
```

### Comparing `jatsgenerator-0.8.0/LICENSE` & `jatsgenerator-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/PKG-INFO` & `jatsgenerator-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatsgenerator
-Version: 0.8.0
+Version: 0.9.0
 Summary: JATS XML generator.
 Home-page: https://github.com/elifesciences/jats-generator
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jatsgenerator-0.8.0/README.md` & `jatsgenerator-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/jatsgenerator/build.py` & `jatsgenerator-0.9.0/jatsgenerator/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from xml.etree.ElementTree import Element, SubElement
 from elifearticle import utils as eautils
+from elifetools import utils as etoolsutils
 from jatsgenerator import utils
 
 
 def set_journal_title_group(parent, journal_title):
     # journal-title-group
     journal_title_group = SubElement(parent, "journal-title-group")
 
@@ -111,19 +112,20 @@
     elif contrib_type == "editor":
         role_tag = SubElement(parent, "role")
         role_tag.text = "Reviewing editor"
 
 
 def set_contrib_orcid(parent, contributor):
     if contributor.orcid:
+        orcid_value = etoolsutils.orcid_uri_to_orcid(contributor.orcid)
         orcid_tag = SubElement(parent, "contrib-id")
         if contributor.orcid_authenticated:
             orcid_tag.set("authenticated", "true")
         orcid_tag.set("contrib-id-type", "orcid")
-        orcid_tag.text = "http://orcid.org/" + contributor.orcid
+        orcid_tag.text = "http://orcid.org/" + orcid_value
 
 
 def set_contrib_corresp(parent, rid):
     # Corresponding author xref tag logic
     xref_tag = SubElement(parent, "xref")
     xref_tag.set("ref-type", "corresp")
     xref_tag.set("rid", rid)
```

### Comparing `jatsgenerator-0.8.0/jatsgenerator/conf.py` & `jatsgenerator-0.9.0/jatsgenerator/conf.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/jatsgenerator/generate.py` & `jatsgenerator-0.9.0/jatsgenerator/generate.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/jatsgenerator/utils.py` & `jatsgenerator-0.9.0/jatsgenerator/utils.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/jatsgenerator.egg-info/PKG-INFO` & `jatsgenerator-0.9.0/jatsgenerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatsgenerator
-Version: 0.8.0
+Version: 0.9.0
 Summary: JATS XML generator.
 Home-page: https://github.com/elifesciences/jats-generator
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jatsgenerator-0.8.0/setup.py` & `jatsgenerator-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/tests/test_build.py` & `jatsgenerator-0.9.0/tests/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,25 +108,42 @@
             b'<contrib-id authenticated="true" contrib-id-type="orcid">'
             b"http://orcid.org/0000-00000-0000-0000"
             b"</contrib-id>"
             b"</root>"
         )
         self.assertEqual(xml_string, expected)
 
-    def test_set_contrib_orcid_none(self):
+    def test_not_authenticated(self):
+        "test if ORCID is not authenticated"
         root = Element("root")
         contributor = Contributor("author", "Surname", "Given")
         contributor.orcid = "0000-00000-0000-0000"
         build.set_contrib_orcid(root, contributor)
         xml_string = ElementTree.tostring(root, encoding="utf-8")
         expected = (
             b"<root>"
             b'<contrib-id contrib-id-type="orcid">'
             b"http://orcid.org/0000-00000-0000-0000"
             b"</contrib-id>"
+            b"</root>"
+        )
+        self.assertEqual(xml_string, expected)
+
+    def test_orcid_url(self):
+        "test if ORCID is a URL value"
+        root = Element("root")
+        contributor = Contributor("author", "Surname", "Given")
+        contributor.orcid = "https://orcid.org/0000-00000-0000-0000"
+        build.set_contrib_orcid(root, contributor)
+        xml_string = ElementTree.tostring(root, encoding="utf-8")
+        expected = (
+            b"<root>"
+            b'<contrib-id contrib-id-type="orcid">'
+            b"http://orcid.org/0000-00000-0000-0000"
+            b"</contrib-id>"
             b"</root>"
         )
         self.assertEqual(xml_string, expected)
 
 
 class TestSetAff(unittest.TestCase):
     def setUp(self):
```

### Comparing `jatsgenerator-0.8.0/tests/test_conf.py` & `jatsgenerator-0.9.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/tests/test_generate.py` & `jatsgenerator-0.9.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `jatsgenerator-0.8.0/tests/test_utils.py` & `jatsgenerator-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

