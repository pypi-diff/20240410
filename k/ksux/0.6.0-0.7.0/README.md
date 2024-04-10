# Comparing `tmp/ksux-0.6.0.tar.gz` & `tmp/ksux-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksux-0.6.0.tar", last modified: Mon Oct 30 11:27:55 2023, max compression
+gzip compressed data, was "ksux-0.7.0.tar", last modified: Wed Apr 10 12:33:04 2024, max compression
```

## Comparing `ksux-0.6.0.tar` & `ksux-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.688352 ksux-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-30 11:27:43.000000 ksux-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-30 11:27:43.000000 ksux-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2023-10-30 11:27:55.684352 ksux-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2023-10-30 11:27:43.000000 ksux-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-10-30 11:27:48.000000 ksux-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 11:27:55.688352 ksux-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.684352 ksux-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:43.000000 ksux-0.6.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.684352 ksux-0.6.0/src/ksux/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2023-10-30 11:27:48.000000 ksux-0.6.0/src/ksux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.684352 ksux-0.6.0/src/ksux/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/src/create_manifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/src/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/src/read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/src/save_manifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/src/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.684352 ksux-0.6.0/src/ksux/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/tests/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-10-30 11:27:43.000000 ksux-0.6.0/src/ksux/tests/test_read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:27:55.684352 ksux-0.6.0/src/ksux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-30 11:27:55.000000 ksux-0.6.0/src/ksux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.267994 ksux-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 12:32:57.000000 ksux-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 12:32:57.000000 ksux-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-10 12:33:04.267994 ksux-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-10 12:32:57.000000 ksux-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-10 12:33:02.000000 ksux-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:33:04.267994 ksux-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.263994 ksux-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:32:57.000000 ksux-0.7.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.267994 ksux-0.7.0/src/ksux/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 12:33:02.000000 ksux-0.7.0/src/ksux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.267994 ksux-0.7.0/src/ksux/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/src/create_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/src/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/src/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/src/save_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.267994 ksux-0.7.0/src/ksux/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/tests/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-10 12:32:57.000000 ksux-0.7.0/src/ksux/tests/test_read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:33:04.267994 ksux-0.7.0/src/ksux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 12:33:04.000000 ksux-0.7.0/src/ksux.egg-info/top_level.txt
```

### Comparing `ksux-0.6.0/LICENSE` & `ksux-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/PKG-INFO` & `ksux-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksux
-Version: 0.6.0
+Version: 0.7.0
 Summary: Easy customization of kubernetes manifests
 Author: Tomas Sladecek
 License: MIT License
         
         Copyright (c) 2022 Tomáš Sládeček
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,18 +24,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/tsladecek/ksux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<2,>=1.10
+Requires-Dist: pydantic<3,>2
 Requires-Dist: ruamel.yaml<1,>=0.17.21
 
 <p align="center">
   <img src="misc/logo.svg" width="75%">
 </p>
 
 <p align=center>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.6.0 Summary: Easy customization of
+Metadata-Version: 2.1 Name: ksux Version: 0.7.0 Summary: Easy customization of
 kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
 2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -11,17 +11,17 @@
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
 https://github.com/tsladecek/ksux Classifier: Programming Language :: Python ::
-3 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+3 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pydantic<2,>=1.10 Requires-Dist: ruamel.yaml<1,>=0.17.21
+pydantic<3,>2 Requires-Dist: ruamel.yaml<1,>=0.17.21
                                 [misc/logo.svg]
                AA ssiimmppllee wwaayy ffoorr tteemmppllaattiinngg kkuubbeerrnneetteess mmaanniiffeessttss..
          [License: MIT][https://img.shields.io/github/v/tag/tsladecek/
   ksux?color=yellow&label=version&logo=GitHub]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
       _k_s_u_x_?_l_o_g_o_=_P_y_p_i_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_s_l_a_d_e_c_e_k_/
  _k_s_u_x_?_l_o_g_o_=_D_o_c_k_e_r_&_s_o_r_t_=_d_a_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_l_i_n_k_-
                                     _g_r_e_e_n_]
```

### Comparing `ksux-0.6.0/README.md` & `ksux-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/pyproject.toml` & `ksux-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ksux"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
     { name = "Tomas Sladecek" }
 ]
 description = "Easy customization of kubernetes manifests"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.6"
+requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pydantic >= 1.10, < 2",
+    "pydantic > 2, < 3",
     "ruamel.yaml >= 0.17.21, < 1",
 ]
 [project.urls]
 "Homepage" = "https://github.com/tsladecek/ksux"
 [project.scripts]
-ksux = "ksux:main"
+ksux = "ksux:main"
```

### Comparing `ksux-0.6.0/src/ksux/__init__.py` & `ksux-0.7.0/src/ksux/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser.add_argument('--dry-run', help='Print manifests to stdout', action="store_true")
     parser.add_argument('-q', '--quiet', help='Do not print debug, info and warning messages', action='store_true')
     parser.add_argument('--version', help='Package version', action="store_true")
 
     args = parser.parse_args()
 
     if args.version:
-        print('0.6.0')
+        print('0.7.0')
         exit(0)
 
     if args.quiet:
         logging.root.setLevel(logging.ERROR)
     else:
         logging.root.setLevel(logging.INFO)
```

### Comparing `ksux-0.6.0/src/ksux/src/create_manifests.py` & `ksux-0.7.0/src/ksux/src/create_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux/src/patch.py` & `ksux-0.7.0/src/ksux/src/patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux/src/read_file.py` & `ksux-0.7.0/src/ksux/src/read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux/src/save_manifests.py` & `ksux-0.7.0/src/ksux/src/save_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux/src/schemas.py` & `ksux-0.7.0/src/ksux/src/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 from typing import Optional, Union, List
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, ValidationInfo, field_validator
 from ruamel.yaml import CommentedSeq, CommentedMap
 
 
 class Target(BaseModel):
     """
     Target object used to find a manifest. This should be a unique
     combination able to detect only one manifest
@@ -31,21 +31,22 @@
           you can use item names instead of indexes
     value: value to be added or which will replace old value. Not
            required for action = remove
     action: Action
     """
     name: str
     path: str
-    value: Optional[Union[str, int, dict, list]]
+    value: Optional[Union[str, int, dict, list]] = None
     enforce_integer: bool = False
     action: Action
     list_key: str = 'name'
 
-    @validator('action')
-    def check_value(cls, v, values, **kwargs):
+    @field_validator('action')
+    def check_value(cls, v, info: ValidationInfo):
+        values = info.data
         if v == Action.add or v == Action.replace:
             if 'value' not in values or values['value'] is None:
                 raise ValueError(f'Value needs to be present for action {v}')
 
             # For add the value needs to be an object
             if v == Action.add and type(values['value']) not in [list, dict, CommentedMap, CommentedSeq]:
                 raise ValueError('For add, the value needs to be a dict or a list')
```

### Comparing `ksux-0.6.0/src/ksux/tests/test_patch.py` & `ksux-0.7.0/src/ksux/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux/tests/test_read_file.py` & `ksux-0.7.0/src/ksux/tests/test_read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.6.0/src/ksux.egg-info/PKG-INFO` & `ksux-0.7.0/src/ksux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksux
-Version: 0.6.0
+Version: 0.7.0
 Summary: Easy customization of kubernetes manifests
 Author: Tomas Sladecek
 License: MIT License
         
         Copyright (c) 2022 Tomáš Sládeček
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,18 +24,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/tsladecek/ksux
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<2,>=1.10
+Requires-Dist: pydantic<3,>2
 Requires-Dist: ruamel.yaml<1,>=0.17.21
 
 <p align="center">
   <img src="misc/logo.svg" width="75%">
 </p>
 
 <p align=center>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.6.0 Summary: Easy customization of
+Metadata-Version: 2.1 Name: ksux Version: 0.7.0 Summary: Easy customization of
 kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
 2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -11,17 +11,17 @@
 IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
 https://github.com/tsladecek/ksux Classifier: Programming Language :: Python ::
-3 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+3 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pydantic<2,>=1.10 Requires-Dist: ruamel.yaml<1,>=0.17.21
+pydantic<3,>2 Requires-Dist: ruamel.yaml<1,>=0.17.21
                                 [misc/logo.svg]
                AA ssiimmppllee wwaayy ffoorr tteemmppllaattiinngg kkuubbeerrnneetteess mmaanniiffeessttss..
          [License: MIT][https://img.shields.io/github/v/tag/tsladecek/
   ksux?color=yellow&label=version&logo=GitHub]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
       _k_s_u_x_?_l_o_g_o_=_P_y_p_i_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_s_l_a_d_e_c_e_k_/
  _k_s_u_x_?_l_o_g_o_=_D_o_c_k_e_r_&_s_o_r_t_=_d_a_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_l_i_n_k_-
                                     _g_r_e_e_n_]
```

### Comparing `ksux-0.6.0/src/ksux.egg-info/SOURCES.txt` & `ksux-0.7.0/src/ksux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

