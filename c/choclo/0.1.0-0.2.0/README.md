# Comparing `tmp/choclo-0.1.0.tar.gz` & `tmp/choclo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "choclo-0.1.0.tar", last modified: Fri May 12 20:36:31 2023, max compression
+gzip compressed data, was "choclo-0.2.0.tar", last modified: Tue Apr  9 23:04:55 2024, max compression
```

## Comparing `choclo-0.1.0.tar` & `choclo-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.179335 choclo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:36:16.000000 choclo-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-12 20:36:16.000000 choclo-0.1.0/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-12 20:36:16.000000 choclo-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-12 20:36:16.000000 choclo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-12 20:36:31.179335 choclo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-12 20:36:16.000000 choclo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/dipole/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/dipole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/dipole/_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/point/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/point/_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/prism/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_magnetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.179335 choclo-0.1.0/choclo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    26624 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_point_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)    66599 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_prism_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34717 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_prism_magnetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:36:30.000000 choclo-0.1.0/choclo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 20:36:16.000000 choclo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-12 20:36:31.179335 choclo-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.113724 choclo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 23:04:41.000000 choclo-0.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 23:04:41.000000 choclo-0.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 23:04:41.000000 choclo-0.2.0/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-09 23:04:41.000000 choclo-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 23:04:41.000000 choclo-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-09 23:04:55.113724 choclo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 23:04:41.000000 choclo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.109724 choclo-0.2.0/choclo/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 23:04:54.000000 choclo-0.2.0/choclo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.109724 choclo-0.2.0/choclo/dipole/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/dipole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/dipole/_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.113724 choclo-0.2.0/choclo/point/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22079 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/point/_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/point/_kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.113724 choclo-0.2.0/choclo/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46789 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/prism/_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/prism/_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30129 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/prism/_magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/prism/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.113724 choclo-0.2.0/choclo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27024 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/test_dipole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/test_point_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66599 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/test_prism_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34717 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/test_prism_magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-09 23:04:41.000000 choclo-0.2.0/choclo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:55.113724 choclo-0.2.0/choclo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-09 23:04:55.000000 choclo-0.2.0/choclo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 23:04:55.000000 choclo-0.2.0/choclo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:04:55.000000 choclo-0.2.0/choclo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 23:04:55.000000 choclo-0.2.0/choclo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 23:04:55.000000 choclo-0.2.0/choclo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 23:04:41.000000 choclo-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:04:55.113724 choclo-0.2.0/setup.cfg
```

### Comparing `choclo-0.1.0/LICENSE.txt` & `choclo-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/PKG-INFO` & `choclo-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: choclo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Kernel functions for your geophysical models
-Home-page: https://github.com/fatiando/choclo
-Author: The Choclo Developers
-Author-email: fatiandoaterra@protonmail.com
-Maintainer: Santiago Soler
-Maintainer-email: santiago.r.soler@gmail.com
-License: BSD 3-Clause License
+Author-email: The Choclo Developers <fatiandoaterra@protonmail.com>
+Maintainer-email: Santiago Soler <santisoler@fastmail.com>
+License: BSD-3-Clause
 Project-URL: Documentation, https://www.fatiando.org/choclo
-Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
+Project-URL: Changelog, https://www.fatiando.org/choclo/latest/changes.html
 Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues
 Project-URL: Source Code, https://github.com/fatiando/choclo
-Keywords: geophysics,geoscience
-Platform: any
-Classifier: Development Status :: 3 - Alpha
+Keywords: geoscience,geophysics
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: AUTHORS.md
+Requires-Dist: numpy>=1.19
+Requires-Dist: numba>=0.52
 
 <img src="https://github.com/fatiando/choclo/raw/main/doc/_static/readme-banner.png" alt="Choclo">
 
 <h2 align="center">Kernel functions for your geophysical models</h2>
 
 <p align="center">
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
 <a href="https://www.fatiando.org/contact/"><strong>Contact</strong></a>
 </p>
 
 <p align="center">
-Part of the <a href="https://www.fatiando.org"><strong>Fatiando a Terra</strong></a> project
+Part of the <a href="https://www.fatiando.org"><strong>Fatiando
+a Terra</strong></a> project, built in collaboration with <a
+href="https://simpeg.xyz"><strong>SimPEG</strong></a>
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: choclo Version: 0.1.0 Summary: Kernel functions for
-your geophysical models Home-page: https://github.com/fatiando/choclo Author:
-The Choclo Developers Author-email: fatiandoaterra@protonmail.com Maintainer:
-Santiago Soler Maintainer-email: santiago.r.soler@gmail.com License: BSD 3-
-Clause License Project-URL: Documentation, https://www.fatiando.org/choclo
-Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
-Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues Project-
-URL: Source Code, https://github.com/fatiando/choclo Keywords:
-geophysics,geoscience Platform: any Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Developers Classifier: Intended Audience :: Education Classifier: License ::
-OSI Approved :: BSD License Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE.txt[Choclo]
+Metadata-Version: 2.1 Name: choclo Version: 0.2.0 Summary: Kernel functions for
+your geophysical models Author-email: The Choclo Developers
+protonmail.com> Maintainer-email: Santiago Soler
+fastmail.com> License: BSD-3-Clause Project-URL: Documentation, https://
+www.fatiando.org/choclo Project-URL: Changelog, https://www.fatiando.org/
+choclo/latest/changes.html Project-URL: Bug Tracker, https://github.com/
+fatiando/choclo/issues Project-URL: Source Code, https://github.com/fatiando/
+choclo Keywords: geoscience,geophysics Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
+Libraries Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE.txt License-File: AUTHORS.md Requires-Dist: numpy>=1.19
+Requires-Dist: numba>=0.52[Choclo]
            ********** KKeerrnneell ffuunnccttiioonnss ffoorr yyoouurr ggeeoopphhyyssiiccaall mmooddeellss **********
   _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_l_a_t_e_s_t_) â¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_m_a_i_n_ _b_r_a_n_c_h_) â¢ _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg â¢
                                     _CC_oo_nn_tt_aa_cc_tt
-                     Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project
+   Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project, built in collaboration with _SS_ii_mm_PP_EE_GG
  _[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _P_y_P_I_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _c_o_n_d_a_-_f_o_r_g_e_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _s_t_a_t_u_s_]
             _[_C_o_m_p_a_t_i_b_l_e_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_._]_[_D_O_I_ _u_s_e_d_ _t_o_ _c_i_t_e_ _C_h_o_c_l_o_]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
```

### Comparing `choclo-0.1.0/README.md` & `choclo-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
 <a href="https://www.fatiando.org/contact/"><strong>Contact</strong></a>
 </p>
 
 <p align="center">
-Part of the <a href="https://www.fatiando.org"><strong>Fatiando a Terra</strong></a> project
+Part of the <a href="https://www.fatiando.org"><strong>Fatiando
+a Terra</strong></a> project, built in collaboration with <a
+href="https://simpeg.xyz"><strong>SimPEG</strong></a>
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [Choclo]
            ********** KKeerrnneell ffuunnccttiioonnss ffoorr yyoouurr ggeeoopphhyyssiiccaall mmooddeellss **********
   _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_l_a_t_e_s_t_) â¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_m_a_i_n_ _b_r_a_n_c_h_) â¢ _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg â¢
                                     _CC_oo_nn_tt_aa_cc_tt
-                     Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project
+   Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project, built in collaboration with _SS_ii_mm_PP_EE_GG
  _[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _P_y_P_I_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _c_o_n_d_a_-_f_o_r_g_e_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _s_t_a_t_u_s_]
             _[_C_o_m_p_a_t_i_b_l_e_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_._]_[_D_O_I_ _u_s_e_d_ _t_o_ _c_i_t_e_ _C_h_o_c_l_o_]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
```

### Comparing `choclo-0.1.0/choclo/dipole/_forward.py` & `choclo-0.2.0/choclo/dipole/_forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,15 @@
     c_m = VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi
     b_e = c_m * (
         3 * dotproduct * r_e / distance**5 - magnetic_moment_east / distance**3
     )
     b_n = c_m * (
         3 * dotproduct * r_n / distance**5 - magnetic_moment_north / distance**3
     )
-    b_u = c_m * (
-        3 * dotproduct * r_u / distance**5 - magnetic_moment_up / distance**3
-    )
+    b_u = c_m * (3 * dotproduct * r_u / distance**5 - magnetic_moment_up / distance**3)
     return b_e, b_n, b_u
 
 
 @jit(nopython=True)
 def magnetic_e(
     easting_p,
     northing_p,
@@ -293,17 +291,15 @@
     r_u = upward_p - upward_q
     distance = np.sqrt(r_e**2 + r_n**2 + r_u**2)
     dotproduct = (
         magnetic_moment_east * r_e
         + magnetic_moment_north * r_n
         + magnetic_moment_up * r_u
     )
-    result = (
-        3 * dotproduct * r_n / distance**5 - magnetic_moment_north / distance**3
-    )
+    result = 3 * dotproduct * r_n / distance**5 - magnetic_moment_north / distance**3
     return VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi * result
 
 
 @jit(nopython=True)
 def magnetic_u(
     easting_p,
     northing_p,
```

### Comparing `choclo-0.1.0/choclo/point/_forward.py` & `choclo-0.2.0/choclo/point/_forward.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 """
 Forward modelling function for point sources
 """
 from numba import jit
 
 from ..constants import GRAVITATIONAL_CONST
 from ..utils import distance_cartesian
+from ._kernels import (
+    kernel_e,
+    kernel_ee,
+    kernel_en,
+    kernel_eu,
+    kernel_n,
+    kernel_nn,
+    kernel_nu,
+    kernel_pot,
+    kernel_u,
+    kernel_uu,
+)
 
 
 @jit(nopython=True)
 def gravity_pot(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Gravitational potential field due to a point source
 
@@ -58,15 +70,18 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    return GRAVITATIONAL_CONST * mass / distance
+    kernel = kernel_pot(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
+    return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_e(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting component of the gravitational acceleration due to a point source
 
@@ -115,15 +130,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = -(easting_p - easting_q) / distance**3
+    kernel = kernel_e(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_n(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing component of the gravitational acceleration due to a point source
@@ -173,15 +190,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = -(northing_p - northing_q) / distance**3
+    kernel = kernel_n(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_u(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Upward component of the gravitational acceleration due to a point source
@@ -231,15 +250,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = -(upward_p - upward_q) / distance**3
+    kernel = kernel_u(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_ee(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-easting component of the gravitational tensor due to a point source
@@ -296,15 +317,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (easting_p - easting_q) ** 2 / distance**5 - 1 / distance**3
+    kernel = kernel_ee(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_nn(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing-northing component of the gravitational tensor due to point source
@@ -361,15 +384,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (northing_p - northing_q) ** 2 / distance**5 - 1 / distance**3
+    kernel = kernel_nn(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_uu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Upward-upward component of the gravitational tensor due to a point source
@@ -426,15 +451,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (upward_p - upward_q) ** 2 / distance**5 - 1 / distance**3
+    kernel = kernel_uu(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_en(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-northing component of the gravitational tensor due to point source
@@ -486,15 +513,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (easting_p - easting_q) * (northing_p - northing_q) / distance**5
+    kernel = kernel_en(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_eu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-upward component of the gravitational tensor due to point source
@@ -546,15 +575,17 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (easting_p - easting_q) * (upward_p - upward_q) / distance**5
+    kernel = kernel_eu(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_nu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing-upward component of the gravitational tensor due to point source
@@ -606,9 +637,11 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = 3 * (northing_p - northing_q) * (upward_p - upward_q) / distance**5
+    kernel = kernel_nu(
+        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
+    )
     return GRAVITATIONAL_CONST * mass * kernel
```

### Comparing `choclo-0.1.0/choclo/prism/__init__.py` & `choclo-0.2.0/choclo/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/prism/_gravity.py` & `choclo-0.2.0/choclo/prism/_gravity.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/prism/_kernels.py` & `choclo-0.2.0/choclo/prism/_kernels.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/prism/_magnetic.py` & `choclo-0.2.0/choclo/prism/_magnetic.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/prism/_utils.py` & `choclo-0.2.0/choclo/prism/_utils.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/test_dipole.py` & `choclo-0.2.0/choclo/tests/test_dipole.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/test_distance.py` & `choclo-0.2.0/choclo/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/test_point_gravity.py` & `choclo-0.2.0/choclo/tests/test_point_gravity.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/test_prism_gravity.py` & `choclo-0.2.0/choclo/tests/test_prism_gravity.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/test_prism_magnetic.py` & `choclo-0.2.0/choclo/tests/test_prism_magnetic.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/tests/utils.py` & `choclo-0.2.0/choclo/tests/utils.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo/utils.py` & `choclo-0.2.0/choclo/utils.py`

 * *Files identical despite different names*

### Comparing `choclo-0.1.0/choclo.egg-info/PKG-INFO` & `choclo-0.2.0/choclo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: choclo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Kernel functions for your geophysical models
-Home-page: https://github.com/fatiando/choclo
-Author: The Choclo Developers
-Author-email: fatiandoaterra@protonmail.com
-Maintainer: Santiago Soler
-Maintainer-email: santiago.r.soler@gmail.com
-License: BSD 3-Clause License
+Author-email: The Choclo Developers <fatiandoaterra@protonmail.com>
+Maintainer-email: Santiago Soler <santisoler@fastmail.com>
+License: BSD-3-Clause
 Project-URL: Documentation, https://www.fatiando.org/choclo
-Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
+Project-URL: Changelog, https://www.fatiando.org/choclo/latest/changes.html
 Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues
 Project-URL: Source Code, https://github.com/fatiando/choclo
-Keywords: geophysics,geoscience
-Platform: any
-Classifier: Development Status :: 3 - Alpha
+Keywords: geoscience,geophysics
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: AUTHORS.md
+Requires-Dist: numpy>=1.19
+Requires-Dist: numba>=0.52
 
 <img src="https://github.com/fatiando/choclo/raw/main/doc/_static/readme-banner.png" alt="Choclo">
 
 <h2 align="center">Kernel functions for your geophysical models</h2>
 
 <p align="center">
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
 <a href="https://www.fatiando.org/contact/"><strong>Contact</strong></a>
 </p>
 
 <p align="center">
-Part of the <a href="https://www.fatiando.org"><strong>Fatiando a Terra</strong></a> project
+Part of the <a href="https://www.fatiando.org"><strong>Fatiando
+a Terra</strong></a> project, built in collaboration with <a
+href="https://simpeg.xyz"><strong>SimPEG</strong></a>
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: choclo Version: 0.1.0 Summary: Kernel functions for
-your geophysical models Home-page: https://github.com/fatiando/choclo Author:
-The Choclo Developers Author-email: fatiandoaterra@protonmail.com Maintainer:
-Santiago Soler Maintainer-email: santiago.r.soler@gmail.com License: BSD 3-
-Clause License Project-URL: Documentation, https://www.fatiando.org/choclo
-Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
-Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues Project-
-URL: Source Code, https://github.com/fatiando/choclo Keywords:
-geophysics,geoscience Platform: any Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Developers Classifier: Intended Audience :: Education Classifier: License ::
-OSI Approved :: BSD License Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE.txt[Choclo]
+Metadata-Version: 2.1 Name: choclo Version: 0.2.0 Summary: Kernel functions for
+your geophysical models Author-email: The Choclo Developers
+protonmail.com> Maintainer-email: Santiago Soler
+fastmail.com> License: BSD-3-Clause Project-URL: Documentation, https://
+www.fatiando.org/choclo Project-URL: Changelog, https://www.fatiando.org/
+choclo/latest/changes.html Project-URL: Bug Tracker, https://github.com/
+fatiando/choclo/issues Project-URL: Source Code, https://github.com/fatiando/
+choclo Keywords: geoscience,geophysics Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Scientific/Engineering Classifier: Topic :: Software Development ::
+Libraries Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE.txt License-File: AUTHORS.md Requires-Dist: numpy>=1.19
+Requires-Dist: numba>=0.52[Choclo]
            ********** KKeerrnneell ffuunnccttiioonnss ffoorr yyoouurr ggeeoopphhyyssiiccaall mmooddeellss **********
   _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_l_a_t_e_s_t_) â¢ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _(_m_a_i_n_ _b_r_a_n_c_h_) â¢ _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg â¢
                                     _CC_oo_nn_tt_aa_cc_tt
-                     Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project
+   Part of the _FF_aa_tt_ii_aa_nn_dd_oo_ _aa_ _TT_ee_rr_rr_aa project, built in collaboration with _SS_ii_mm_PP_EE_GG
  _[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _P_y_P_I_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_n_ _c_o_n_d_a_-_f_o_r_g_e_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _s_t_a_t_u_s_]
             _[_C_o_m_p_a_t_i_b_l_e_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_._]_[_D_O_I_ _u_s_e_d_ _t_o_ _c_i_t_e_ _C_h_o_c_l_o_]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
```

### Comparing `choclo-0.1.0/choclo.egg-info/SOURCES.txt` & `choclo-0.2.0/choclo.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+.flake8
 AUTHORS.md
 CITATION.rst
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 choclo/__init__.py
 choclo/_version.py
-choclo/_version_generated.py
 choclo/constants.py
 choclo/utils.py
 choclo.egg-info/PKG-INFO
 choclo.egg-info/SOURCES.txt
 choclo.egg-info/dependency_links.txt
 choclo.egg-info/requires.txt
 choclo.egg-info/top_level.txt
-choclo.egg-info/zip-safe
 choclo/dipole/__init__.py
 choclo/dipole/_forward.py
 choclo/point/__init__.py
 choclo/point/_forward.py
+choclo/point/_kernels.py
 choclo/prism/__init__.py
 choclo/prism/_gravity.py
 choclo/prism/_kernels.py
 choclo/prism/_magnetic.py
 choclo/prism/_utils.py
 choclo/tests/__init__.py
 choclo/tests/test_dipole.py
```

