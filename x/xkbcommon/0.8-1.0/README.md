# Comparing `tmp/xkbcommon-0.8.tar.gz` & `tmp/xkbcommon-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xkbcommon-0.8.tar", last modified: Wed Jan 11 23:55:11 2023, max compression
+gzip compressed data, was "xkbcommon-1.0.tar", last modified: Wed Apr 10 14:12:16 2024, max compression
```

## Comparing `xkbcommon-0.8.tar` & `xkbcommon-1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-01-11 23:55:11.186813 xkbcommon-0.8/
--rw-rw-r--   0 steve     (1000) steve     (1000)     1077 2023-01-11 17:51:59.000000 xkbcommon-0.8/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2021-07-18 15:34:22.000000 xkbcommon-0.8/MANIFEST.in
--rw-rw-r--   0 steve     (1000) steve     (1000)     1910 2023-01-11 23:55:11.186813 xkbcommon-0.8/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     1089 2023-01-11 23:54:47.000000 xkbcommon-0.8/README.rst
--rw-rw-r--   0 steve     (1000) steve     (1000)       89 2023-01-11 17:51:59.000000 xkbcommon-0.8/pyproject.toml
--rw-rw-r--   0 steve     (1000) steve     (1000)      943 2023-01-11 23:55:11.186813 xkbcommon-0.8/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)       95 2023-01-11 17:51:59.000000 xkbcommon-0.8/setup.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-01-11 23:55:11.186813 xkbcommon-0.8/tests/
--rw-r--r--   0 steve     (1000) steve     (1000)        0 2018-07-25 10:33:28.000000 xkbcommon-0.8/tests/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    65393 2020-02-01 15:53:05.000000 xkbcommon-0.8/tests/data.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    19690 2023-01-11 22:00:20.000000 xkbcommon-0.8/tests/test_xkb.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-01-11 23:55:11.186813 xkbcommon-0.8/xkbcommon/
--rw-r--r--   0 steve     (1000) steve     (1000)      224 2018-07-25 10:33:28.000000 xkbcommon-0.8/xkbcommon/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    14468 2023-01-11 21:50:54.000000 xkbcommon-0.8/xkbcommon/ffi_build.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    38715 2023-01-11 21:52:55.000000 xkbcommon-0.8/xkbcommon/xkb.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-01-11 23:55:11.186813 xkbcommon-0.8/xkbcommon.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)     1910 2023-01-11 23:55:11.000000 xkbcommon-0.8/xkbcommon.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      340 2023-01-11 23:55:11.000000 xkbcommon-0.8/xkbcommon.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-01-11 23:55:11.000000 xkbcommon-0.8/xkbcommon.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       12 2023-01-11 23:55:11.000000 xkbcommon-0.8/xkbcommon.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       10 2023-01-11 23:55:11.000000 xkbcommon-0.8/xkbcommon.egg-info/top_level.txt
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-10 14:12:16.277598 xkbcommon-1.0/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1077 2023-01-11 17:51:59.000000 xkbcommon-1.0/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2021-07-18 15:34:22.000000 xkbcommon-1.0/MANIFEST.in
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1861 2024-04-10 14:12:16.277598 xkbcommon-1.0/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1089 2023-01-11 23:54:47.000000 xkbcommon-1.0/README.rst
+-rw-rw-r--   0 steve     (1000) steve     (1000)       89 2023-01-11 17:51:59.000000 xkbcommon-1.0/pyproject.toml
+-rw-rw-r--   0 steve     (1000) steve     (1000)      905 2024-04-10 14:12:16.277598 xkbcommon-1.0/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)       95 2023-01-11 17:51:59.000000 xkbcommon-1.0/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-10 14:12:16.273598 xkbcommon-1.0/tests/
+-rw-r--r--   0 steve     (1000) steve     (1000)        0 2018-07-25 10:33:28.000000 xkbcommon-1.0/tests/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    65393 2020-02-01 15:53:05.000000 xkbcommon-1.0/tests/data.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    20138 2024-04-10 14:10:58.000000 xkbcommon-1.0/tests/test_xkb.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-10 14:12:16.273598 xkbcommon-1.0/xkbcommon/
+-rw-r--r--   0 steve     (1000) steve     (1000)      224 2018-07-25 10:33:28.000000 xkbcommon-1.0/xkbcommon/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    14825 2024-04-10 14:10:58.000000 xkbcommon-1.0/xkbcommon/ffi_build.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    39750 2024-04-10 14:10:58.000000 xkbcommon-1.0/xkbcommon/xkb.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2024-04-10 14:12:16.277598 xkbcommon-1.0/xkbcommon.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1861 2024-04-10 14:12:16.000000 xkbcommon-1.0/xkbcommon.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      340 2024-04-10 14:12:16.000000 xkbcommon-1.0/xkbcommon.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2024-04-10 14:12:16.000000 xkbcommon-1.0/xkbcommon.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       12 2024-04-10 14:12:16.000000 xkbcommon-1.0/xkbcommon.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       10 2024-04-10 14:12:16.000000 xkbcommon-1.0/xkbcommon.egg-info/top_level.txt
```

### Comparing `xkbcommon-0.8/LICENSE` & `xkbcommon-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xkbcommon-0.8/PKG-INFO` & `xkbcommon-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: xkbcommon
-Version: 0.8
+Version: 1.0
 Summary: Bindings for libxkbcommon using cffi
 Home-page: https://github.com/sde1000/python-xkbcommon
 Author: Stephen Early
 Author-email: steve@assorted.org.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 xkbcommon
 =========
 
 Python bindings for libxkbcommon_ using cffi_.
```

### Comparing `xkbcommon-0.8/README.rst` & `xkbcommon-1.0/README.rst`

 * *Files identical despite different names*

### Comparing `xkbcommon-0.8/setup.cfg` & `xkbcommon-1.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [metadata]
 name = xkbcommon
-version = 0.8
+version = 1.0
 description = Bindings for libxkbcommon using cffi
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Stephen Early
 author_email = steve@assorted.org.uk
 url = https://github.com/sde1000/python-xkbcommon
 license = MIT
 license_files = 
 	LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development :: Libraries
 	Intended Audience :: Developers
 
 [options]
-python_requires = >= 3.6
+python_requires = >= 3.8
 packages = 
 	xkbcommon
 setup_requires = 
 	cffi >= 1.5.0
 install_requires = 
 	cffi >= 1.5.0
```

### Comparing `xkbcommon-0.8/tests/data.py` & `xkbcommon-1.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `xkbcommon-0.8/tests/test_xkb.py` & `xkbcommon-1.0/tests/test_xkb.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,23 @@
         key = next(iter(self.km))
         self.assertEqual(self.km.num_layouts_for_key(key), 1)
 
     def test_keymap_num_levels_for_key(self):
         key = next(iter(self.km))
         self.assertEqual(self.km.num_levels_for_key(key, 0), 1)
 
+    def test_keymap_key_get_mods_for_level(self):
+        first_invalid_mask = 1 << self.km.num_mods()
+        for key in self.km:
+            for layout in range(self.km.num_layouts_for_key(key)):
+                for level in range(self.km.num_levels_for_key(key, layout)):
+                    r = self.km.key_get_mods_for_level(key, layout, level)
+                    for mm in r:
+                        self.assertLess(mm, first_invalid_mask)
+
     def test_keymap_key_get_syms_by_level(self):
         for key in self.km:
             r = self.km.key_get_syms_by_level(key, 0, 0)
             for k in r:
                 # If we are returned an invalid keysym, this will raise
                 # XKBInvalidKeysym
                 self.assertTrue(xkb.keysym_get_name(k))
```

### Comparing `xkbcommon-0.8/xkbcommon/ffi_build.py` & `xkbcommon-1.0/xkbcommon/ffi_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cffi import FFI
 ffibuilder = FFI()
 
-# Currently implemented with reference to libxkbcommon-0.6.0
+# Currently implemented with reference to libxkbcommon-1.0.0
 
 ffibuilder.set_source("xkbcommon._ffi", """
 #include <stdarg.h>
 #include <xkbcommon/xkbcommon.h>
 #include <xkbcommon/xkbcommon-keysyms.h>
 #include <xkbcommon/xkbcommon-compose.h>
 
@@ -249,14 +249,22 @@
 xkb_layout_index_t
 xkb_keymap_num_layouts_for_key(struct xkb_keymap *keymap, xkb_keycode_t key);
 
 xkb_level_index_t
 xkb_keymap_num_levels_for_key(struct xkb_keymap *keymap, xkb_keycode_t key,
                               xkb_layout_index_t layout);
 
+size_t
+xkb_keymap_key_get_mods_for_level(struct xkb_keymap *keymap,
+                                  xkb_keycode_t key,
+                                  xkb_layout_index_t layout,
+                                  xkb_level_index_t level,
+                                  xkb_mod_mask_t *masks_out,
+                                  size_t masks_size);
+
 int
 xkb_keymap_key_get_syms_by_level(struct xkb_keymap *keymap,
                                  xkb_keycode_t key,
                                  xkb_layout_index_t layout,
                                  xkb_level_index_t level,
                                  const xkb_keysym_t **syms_out);
```

### Comparing `xkbcommon-0.8/xkbcommon/xkb.py` & `xkbcommon-1.0/xkbcommon/xkb.py`

 * *Files 2% similar despite different names*

```diff
@@ -614,14 +614,37 @@
         If layout is out of range for this key (that is, larger or
         equal to the value returned by Keymap.num_layouts_for_key()),
         it is brought back into range in a manner consistent with
         State.key_get_layout().
         """
         return lib.xkb_keymap_num_levels_for_key(self._keymap, key, layout)
 
+    def key_get_mods_for_level(self, key, layout, level):
+        """Retrieves every possible modifier mask that produces the specified
+        shift level for a specific key and layout.
+
+        This API is useful for inverse key transformation;
+        i.e. finding out which modifiers need to be active in order to
+        be able to type the keysym(s) corresponding to the specific
+        key code, layout and level.
+
+        If layout is out of range for this key (that is, larger or
+        equal to the value returned by Keymap.num_layouts_for_key()),
+        it is brought back into range in a manner consistent with
+        State.key_get_layout().
+        """
+        masks_size = 4
+        while True:
+            masks_out = ffi.new(f"xkb_mod_mask_t[{masks_size}]")
+            r = lib.xkb_keymap_key_get_mods_for_level(
+                self._keymap, key, layout, level, masks_out, masks_size)
+            if r < masks_size:
+                return [masks_out[n] for n in range(r)]
+            masks_size = masks_size << 1
+
     def key_get_syms_by_level(self, key, layout, level):
         """Get the keysyms obtained from pressing a key in a given layout and
         shift level.
 
         This function is like State.key_get_syms(), only the layout
         and shift level are not derived from the keyboard state but
         are instead specified explicitly.
```

### Comparing `xkbcommon-0.8/xkbcommon.egg-info/PKG-INFO` & `xkbcommon-1.0/xkbcommon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: xkbcommon
-Version: 0.8
+Version: 1.0
 Summary: Bindings for libxkbcommon using cffi
 Home-page: https://github.com/sde1000/python-xkbcommon
 Author: Stephen Early
 Author-email: steve@assorted.org.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 xkbcommon
 =========
 
 Python bindings for libxkbcommon_ using cffi_.
```

