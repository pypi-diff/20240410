# Comparing `tmp/wwpdb.utils.emdb-1.7.1.tar.gz` & `tmp/wwpdb.utils.emdb-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.7.1.tar", last modified: Wed Feb 14 16:07:36 2024, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.8.tar", last modified: Wed Apr 10 17:17:09 2024, max compression
```

## Comparing `wwpdb.utils.emdb-1.7.1.tar` & `wwpdb.utils.emdb-1.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.951547 wwpdb.utils.emdb-1.7.1/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-02-14 16:07:36.951547 wwpdb.utils.emdb-1.7.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-02-14 16:07:36.955547 wwpdb.utils.emdb-1.7.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.947547 wwpdb.utils.emdb-1.7.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.947547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.947547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.947547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.947547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/checkemupload/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/checkemupload/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15818 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/checkemupload/checkemupload.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.951547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2304842 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.951547 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (127)   221391 2024-02-14 16:06:37.000000 wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-14 16:07:36.951547 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-14 16:07:23.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-02-14 16:07:36.000000 wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16058 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/checkemupload.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 17:16:52.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.7.1/PKG-INFO` & `wwpdb.utils.emdb-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.7.1
+Version: 1.8
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.7.1/setup.py` & `wwpdb.utils.emdb-1.8/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/checkemupload/checkemupload.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/checkemupload.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         Raises:
             FileNotFoundError: If the file is not found.
             Exception: If an error occurs during file loading.
         """
         try:
             self.md5_checksum()
-            with mrcfile.open(self.file, mode='r', permissive=True) as mrc:
+            with mrcfile.mmap(self.file, mode='r', permissive=False) as mrc:
                 self.header = mrc.header
                 self.box_size = self.header.cella.tolist()
                 self.pixel_size = mrc.voxel_size.tolist()
                 self.nxyz = np.array((self.header.nx, self.header.ny, self.header.nz)).tolist()
                 nstarts = np.array((self.header.nxstart, self.header.nystart, self.header.nzstart))
                 origin = nstarts * np.array(self.pixel_size)
                 end = origin + np.array(self.box_size)
@@ -184,17 +184,26 @@
 
         Args:
             path2model (str): Path to the MMCIF file.
         """
         # Extracting atom coordinates from the MMCIF file
         mmcif_dict = MMCIF2Dict(path2model)
         self.file = path2model
-        self.structure = [(float(x), float(y), float(z)) for x, y, z in
-                          zip(mmcif_dict['_atom_site.Cartn_x'], mmcif_dict['_atom_site.Cartn_y'],
-                              mmcif_dict['_atom_site.Cartn_z'])]
+        self.structure = [
+            (float(x), float(y), float(z))
+            for x, y, z in zip(
+                mmcif_dict['_atom_site.Cartn_x'],
+                mmcif_dict['_atom_site.Cartn_y'],
+                mmcif_dict['_atom_site.Cartn_z']
+            )
+        ] if (
+            '_atom_site.Cartn_x' in mmcif_dict
+            and '_atom_site.Cartn_y' in mmcif_dict
+            and '_atom_site.Cartn_z' in mmcif_dict
+        ) else None
 
 
 class Validator:
     """
     Class for validating and comparing EM maps and models.
     """
 
@@ -328,15 +337,15 @@
             if not all(os.path.isfile(half_map.file) for half_map in self.half_maps):
                 raise FileNotFoundError("One or more half maps not found.")
             result.update({
                 'half_maps_to_each_other': self._compare_maps(self.half_maps[0], self.half_maps[1]),  # Compare half maps to each other
                 'primary_map_to_half_maps': [self._compare_maps(self.em_map, half_map) for half_map in self.half_maps]  # Compare primary map to each half map
             })
 
-        if self.model:
+        if self.model and self.model.structure:
             num_atoms_outside, fraction_atoms_outside = self._get_atoms_outside()
             result['map_to_model'] = {
                 'num_atoms_outside': num_atoms_outside,
                 # Calculate the fraction of atoms outside the primary map
                 'fraction_atoms_outside': fraction_atoms_outside
             }
```

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.9.2"
+        XML_OUT_VERSION = "3.0.9.3"
         XML_VERSION = XML_OUT_VERSION.replace('.', '_')
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
```

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Mon Feb  5 18:29:43 2024 by generateDS.py version 2.43.3.
+# Generated Wed Mar 27 17:13:50 2024 by generateDS.py version 2.43.3.
 # Python 3.9.7 (default, Sep 16 2021, 08:50:36)  [Clang 10.0.0 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', '/Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_2/emdb.py')
+#   ('-o', '/Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_3/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   /Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_2/emdb.xsd
+#   /Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_3/emdb.xsd
 #
 # Command line:
-#   /Users/sanja/generateDS/generateDS-2.43.3/generateDS.py --root-element="emd" -f -o "/Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_2/emdb.py" --no-warnings --external-encoding="utf-8" /Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_2/emdb.xsd
+#   /Users/sanja/generateDS/generateDS-2.43.3/generateDS.py --root-element="emd" -f -o "/Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_3/emdb.py" --no-warnings --external-encoding="utf-8" /Users/sanja/IdeaProjects/emdb_schemas/emdb_schemas/v3/v3_0_9_3/emdb.xsd
 #
 # Current working directory (os.getcwd()):
-#   sanja
+#   emdb_schemas
 #
 
 import sys
 try:
     ModulenotfoundExp_ = ModuleNotFoundError
 except NameError:
     ModulenotfoundExp_ = ImportError
@@ -1017,14 +1017,15 @@
     TISSUE='tissue'
 
 
 class allowed_film_or_detector_model(str, Enum):
     AGFASCIENTAFILM='AGFA SCIENTA FILM'
     DECTRISSINGLA_1_KX_1_K='DECTRIS SINGLA (1k x 1k)'
     DECTRISELA_1_KX_0_5_K='DECTRIS ELA (1k x 0.5k)'
+    DECTRISARINA_0_2_KX_0_2_K='DECTRIS ARINA (0.2k x 0.2k)'
     DIRECTELECTRONAPOLLO_4_KX_4_K='DIRECT ELECTRON APOLLO (4k x 4k)'
     DIRECTELECTRONDE_10_5_KX_4_K='DIRECT ELECTRON DE-10 (5k x 4k)'
     DIRECTELECTRONDE_12_4_KX_3_K='DIRECT ELECTRON DE-12 (4k x 3k)'
     DIRECTELECTRONDE_16_4_KX_4_K='DIRECT ELECTRON DE-16 (4k x 4k)'
     DIRECTELECTRONDE_20_5_KX_3_K='DIRECT ELECTRON DE-20 (5k x 3k)'
     DIRECTELECTRONDE_64_8_KX_8_K='DIRECT ELECTRON DE-64 (8k x 8k)'
     FEICETA_4_KX_4_K='FEI CETA (4k x 4k)'
@@ -1272,14 +1273,15 @@
 class illumination_modeType(str, Enum):
     FLOODBEAM='FLOOD BEAM'
     SPOTSCAN='SPOT SCAN'
     OTHER='OTHER'
 
 
 class imaging_modeType(str, Enum):
+    _4_DSTEM='4D-STEM'
     BRIGHTFIELD='BRIGHT FIELD'
     DARKFIELD='DARK FIELD'
     DIFFRACTION='DIFFRACTION'
     OTHER='OTHER'
 
 
 class in_frameType(str, Enum):
@@ -1766,15 +1768,15 @@
 #
 # Start data representation classes
 #
 class entry_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.9.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
+    def __init__(self, emdb_id=None, version='3.0.9.3', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.emdb_id_nsprefix_ = None
@@ -1892,15 +1894,15 @@
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='entry_type'):
         if self.emdb_id is not None and 'emdb_id' not in already_processed:
             already_processed.add('emdb_id')
             outfile.write(' emdb_id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.emdb_id), input_name='emdb_id')), ))
-        if self.version != "3.0.9.2" and 'version' not in already_processed:
+        if self.version != "3.0.9.3" and 'version' not in already_processed:
             already_processed.add('version')
             outfile.write(' version=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.version), input_name='version')), ))
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='entry_type', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -14590,15 +14592,15 @@
         # Validate type imaging_modeType, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['BRIGHT FIELD', 'DARK FIELD', 'DIFFRACTION', 'OTHER']
+            enumerations = ['4D-STEM', 'BRIGHT FIELD', 'DARK FIELD', 'DIFFRACTION', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on imaging_modeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
     def validate_electron_sourceType(self, value):
         result = True
@@ -33689,15 +33691,15 @@
         # Validate type allowed_film_or_detector_model, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
-            enumerations = ['AGFA SCIENTA FILM', 'DECTRIS SINGLA (1k x 1k)', 'DECTRIS ELA (1k x 0.5k)', 'DIRECT ELECTRON APOLLO (4k x 4k)', 'DIRECT ELECTRON DE-10 (5k x 4k)', 'DIRECT ELECTRON DE-12 (4k x 3k)', 'DIRECT ELECTRON DE-16 (4k x 4k)', 'DIRECT ELECTRON DE-20 (5k x 3k)', 'DIRECT ELECTRON DE-64 (8k x 8k)', 'FEI CETA (4k x 4k)', 'FEI EAGLE (2k x 2k)', 'FEI EAGLE (4k x 4k)', 'FEI FALCON I (4k x 4k)', 'FEI FALCON II (4k x 4k)', 'FEI FALCON III (4k x 4k)', 'FEI FALCON IV (4k x 4k)', 'GATAN ALPINE (2.3k x 3.2k)', 'GATAN K2 (4k x 4k)', 'GATAN K2 BASE (4k x 4k)', 'GATAN K2 IS (4k x 4k)', 'GATAN K2 QUANTUM (4k x 4k)', 'GATAN K2 SUMMIT (4k x 4k)', 'GATAN K3 (6k x 4k)', 'GATAN K3 BIOCONTINUUM (6k x 4k)', 'GATAN K3 BIOQUANTUM (6k x 4k)', 'GATAN MULTISCAN', 'GATAN ORIUS SC1000 (4k x 2.7k)', 'GATAN ORIUS SC200 (2k x 2k)', 'GATAN ORIUS SC600 (2.7k x 2.7k)', 'GATAN ULTRASCAN 1000 (2k x 2k)', 'GATAN ULTRASCAN 10000 (10k x 10k)', 'GATAN ULTRASCAN 4000 (4k x 4k)', 'GENERIC CCD', 'GENERIC CCD (2k x 2k)', 'GENERIC CCD (4k x 4k)', 'GENERIC FILM', 'GENERIC GATAN', 'GENERIC GATAN (2k x 2k)', 'GENERIC GATAN (4k x 4k)', 'GENERIC IMAGE PLATES', 'GENERIC TVIPS', 'GENERIC TVIPS (2k x 2k)', 'GENERIC TVIPS (4k x 4k)', 'KODAK 4489 FILM', 'KODAK SO-163 FILM', 'OTHER', 'PROSCAN TEM-PIV (2k x 2k)', 'SIA 15C (3k x 3k)', 'TFS FALCON 4i (4k x 4k)', 'TVIPS TEMCAM-F216 (2k x 2k)', 'TVIPS TEMCAM-F224 (2k x 2k)', 'TVIPS TEMCAM-F415 (4k x 4k)', 'TVIPS TEMCAM-F416 (4k x 4k)', 'TVIPS TEMCAM-F816 (8k x 8k)']
+            enumerations = ['AGFA SCIENTA FILM', 'DECTRIS SINGLA (1k x 1k)', 'DECTRIS ELA (1k x 0.5k)', 'DECTRIS ARINA (0.2k x 0.2k)', 'DIRECT ELECTRON APOLLO (4k x 4k)', 'DIRECT ELECTRON DE-10 (5k x 4k)', 'DIRECT ELECTRON DE-12 (4k x 3k)', 'DIRECT ELECTRON DE-16 (4k x 4k)', 'DIRECT ELECTRON DE-20 (5k x 3k)', 'DIRECT ELECTRON DE-64 (8k x 8k)', 'FEI CETA (4k x 4k)', 'FEI EAGLE (2k x 2k)', 'FEI EAGLE (4k x 4k)', 'FEI FALCON I (4k x 4k)', 'FEI FALCON II (4k x 4k)', 'FEI FALCON III (4k x 4k)', 'FEI FALCON IV (4k x 4k)', 'GATAN ALPINE (2.3k x 3.2k)', 'GATAN K2 (4k x 4k)', 'GATAN K2 BASE (4k x 4k)', 'GATAN K2 IS (4k x 4k)', 'GATAN K2 QUANTUM (4k x 4k)', 'GATAN K2 SUMMIT (4k x 4k)', 'GATAN K3 (6k x 4k)', 'GATAN K3 BIOCONTINUUM (6k x 4k)', 'GATAN K3 BIOQUANTUM (6k x 4k)', 'GATAN MULTISCAN', 'GATAN ORIUS SC1000 (4k x 2.7k)', 'GATAN ORIUS SC200 (2k x 2k)', 'GATAN ORIUS SC600 (2.7k x 2.7k)', 'GATAN ULTRASCAN 1000 (2k x 2k)', 'GATAN ULTRASCAN 10000 (10k x 10k)', 'GATAN ULTRASCAN 4000 (4k x 4k)', 'GENERIC CCD', 'GENERIC CCD (2k x 2k)', 'GENERIC CCD (4k x 4k)', 'GENERIC FILM', 'GENERIC GATAN', 'GENERIC GATAN (2k x 2k)', 'GENERIC GATAN (4k x 4k)', 'GENERIC IMAGE PLATES', 'GENERIC TVIPS', 'GENERIC TVIPS (2k x 2k)', 'GENERIC TVIPS (4k x 4k)', 'KODAK 4489 FILM', 'KODAK SO-163 FILM', 'OTHER', 'PROSCAN TEM-PIV (2k x 2k)', 'SIA 15C (3k x 3k)', 'TFS FALCON 4i (4k x 4k)', 'TVIPS TEMCAM-F216 (2k x 2k)', 'TVIPS TEMCAM-F224 (2k x 2k)', 'TVIPS TEMCAM-F415 (4k x 4k)', 'TVIPS TEMCAM-F416 (4k x 4k)', 'TVIPS TEMCAM-F816 (8k x 8k)']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on allowed_film_or_detector_model' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
     def validate_categoryType43(self, value):
         # Validate type categoryType43, a restriction on xs:string.
```

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 0% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.9.2"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.9.3"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -2111,14 +2111,15 @@
             <xs:enumeration value="OTHER"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:element>
       <xs:element name="imaging_mode">
         <xs:simpleType>
           <xs:restriction base="xs:token">
+            <xs:enumeration value="4D-STEM"/>
             <xs:enumeration value="BRIGHT FIELD"/>
             <xs:enumeration value="DARK FIELD"/>
             <xs:enumeration value="DIFFRACTION"/>
             <xs:enumeration value="OTHER"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:element>
@@ -2535,14 +2536,15 @@
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="allowed_film_or_detector_model">
     <xs:restriction base="xs:token">
       <xs:enumeration value="AGFA SCIENTA FILM"/>
       <xs:enumeration value="DECTRIS SINGLA (1k x 1k)"/>
       <xs:enumeration value="DECTRIS ELA (1k x 0.5k)"/>
+      <xs:enumeration value="DECTRIS ARINA (0.2k x 0.2k)"/>
       <xs:enumeration value="DIRECT ELECTRON APOLLO (4k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-10 (5k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-12 (4k x 3k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-16 (4k x 4k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-20 (5k x 3k)"/>
       <xs:enumeration value="DIRECT ELECTRON DE-64 (8k x 8k)"/>
       <xs:enumeration value="FEI CETA (4k x 4k)"/>
```

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.7.1
+Version: 1.8
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.7.1/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

