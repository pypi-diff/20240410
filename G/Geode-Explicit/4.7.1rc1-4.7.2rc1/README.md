# Comparing `tmp/Geode_Explicit-4.7.1rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.7.2rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3150566 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-Apr-09 15:40 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-09 15:40 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-Apr-09 15:40 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4040192 b- defN 24-Apr-09 15:41 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-Apr-09 15:41 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-Apr-09 15:41 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153088 b- defN 24-Apr-09 15:41 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-Apr-09 15:41 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2211 b- defN 24-Apr-09 15:41 Geode_Explicit-4.7.1rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-09 15:41 Geode_Explicit-4.7.1rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-09 15:41 Geode_Explicit-4.7.1rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 24-Apr-09 15:41 Geode_Explicit-4.7.1rc1.dist-info/RECORD
-12 files, 8081994 bytes uncompressed, 3148642 bytes compressed:  61.0%
+Zip file size: 375182 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 24-Apr-10 13:11 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 24-Apr-10 13:11 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 24-Apr-10 13:11 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   175680 b- defN 24-Apr-10 13:12 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   138752 b- defN 24-Apr-10 13:12 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   488472 b- defN 24-Apr-10 13:12 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    35368 b- defN 24-Apr-10 13:12 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    77000 b- defN 24-Apr-10 13:12 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2148 b- defN 24-Apr-10 13:12 Geode_Explicit-4.7.2rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-Apr-10 13:12 Geode_Explicit-4.7.2rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-10 13:12 Geode_Explicit-4.7.2rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1166 b- defN 24-Apr-10 13:12 Geode_Explicit-4.7.2rc1.dist-info/RECORD
+12 files, 919294 bytes uncompressed, 373178 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-4.7.1rc1.dist-info/METADATA
+Filename: Geode_Explicit-4.7.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.7.1rc1.dist-info/WHEEL
+Filename: Geode_Explicit-4.7.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.7.1rc1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.7.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.7.1rc1.dist-info/RECORD
+Filename: Geode_Explicit-4.7.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

## Comparing `Geode_Explicit-4.7.1rc1.dist-info/METADATA` & `Geode_Explicit-4.7.2rc1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1
-Name: Geode-Explicit
-Version: 4.7.1rc1
-Summary: Geode-solutions OpenGeode module for building explicit models
-Home-page: https://github.com/Geode-solutions/Geode-Explicit
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.9.6
-Requires-Dist: geode-common ==31.*,>=31.0.6rc1
-Requires-Dist: geode-conversion ==5.*,>=5.2.8
-Requires-Dist: opengeode-core ==14.*,>=14.18.1
-Requires-Dist: opengeode-inspector ==5.*,>=5.0.5
-
-<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://geode-solutions.com/#slack">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2024, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Explicit
+Version: 4.7.2rc1
+Summary: Geode-solutions OpenGeode module for building explicit models
+Home-page: https://github.com/Geode-solutions/Geode-Explicit
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background ==7.*,>=7.9.6
+Requires-Dist: geode-common ==31.*,>=31.0.6
+Requires-Dist: geode-conversion ==5.*,>=5.2.8
+Requires-Dist: opengeode-core ==14.*,>=14.18.2rc1
+Requires-Dist: opengeode-inspector ==5.*,>=5.0.5
+
+<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://geode-solutions.com/#slack">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2024, Geode-solutions
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.7.1rc1 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.7.2rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.9.6
-Requires-Dist: geode-common ==31.*,>=31.0.6rc1 Requires-Dist: geode-conversion
-==5.*,>=5.2.8 Requires-Dist: opengeode-core ==14.*,>=14.18.1 Requires-Dist:
-opengeode-inspector ==5.*,>=5.0.5
+contact@geode-solutions.com License: Proprietary Description-Content-Type:
+text/markdown Requires-Dist: geode-background ==7.*,>=7.9.6 Requires-Dist:
+geode-common ==31.*,>=31.0.6 Requires-Dist: geode-conversion ==5.*,>=5.2.8
+Requires-Dist: opengeode-core ==14.*,>=14.18.2rc1 Requires-Dist: opengeode-
+inspector ==5.*,>=5.0.5
                 ************ GGeeooddee--EExxpplliicciittbbyy GGeeooddee--ssoolluuttiioonnss ************
     ******** GGeeooddee--ssoolluuttiioonnss OOppeennGGeeooddee mmoodduullee ffoorr bbuuiillddiinngg eexxpplliicciitt mmooddeellss ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

## Comparing `Geode_Explicit-4.7.1rc1.dist-info/RECORD` & `Geode_Explicit-4.7.2rc1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-geode_explicit/__init__.py,sha256=3IEZJDMtMfFSTtDJOl8tpLIg5P9Iytnx2bE1I6Gg8qo,194
-geode_explicit/brep.py,sha256=i4sDZvKY0NnpwATBxQHOq2egAGLbxDH5u4iZqCHMOlk,271
-geode_explicit/section.py,sha256=k_Q35aAqi_ZAP004Xc86lQf4FSYA2u0kU6y1_iR9Ahk,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=EdRrK9st2uvkHOoKFYVKBJ1MoxlpJ-B9s571_siAKvM,4040192
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=p-n1sNf4f7Dxs_kBNTTmtvq7fa8pXJetK5g1bLFPYFo,33792
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=V_XlU_8LGdTuVv88383H34pY4_nDGHpEZwV3lENt_88,3715072
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=flPwEj1Re84koaHvIhF5BBLLThO0DbFCN1xJNdc6mT8,153088
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=95LSi0Sj4j7QN-eehf5s5HFUpi8YV_f0c2BzTTHmqZU,135680
-Geode_Explicit-4.7.1rc1.dist-info/METADATA,sha256=pGBU2wradsrrgpmw5HU3HpaXIT672Se3oqGEZUBtXQ0,2211
-Geode_Explicit-4.7.1rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Explicit-4.7.1rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.7.1rc1.dist-info/RECORD,,
+geode_explicit/__init__.py,sha256=08Jv_j6l55nLaa6-0g_1kSAFNTm8bJxZIhj1Su7ykhg,89
+geode_explicit/brep.py,sha256=AGSr4GiHYA2yA300pQq5aSAPY-cKbjxOzdYukAtEJNw,261
+geode_explicit/section.py,sha256=iYPIWWs6fo3bNWTBkUqJ7-J0FI9w3mXN3NovuSZaL6o,240
+geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so,sha256=HoWAIFaXusWPqPR91Un-uTmfMqIXmFwau-yjToK6Ih8,175680
+geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so,sha256=IfwGcXp4iL7bIDwK7_t552SsbxPncerepBL1WYZocLM,138752
+geode_explicit/lib64/libGeode-Explicit_brep.so,sha256=i651XKdz2fyArRAMpq1cRILDNzjPmVhRoEJEwCOgBGo,488472
+geode_explicit/lib64/libGeode-Explicit_common.so,sha256=hHm39rTH4cuTCYe-mFiO7UxoXyIGH4lkn9Jmk7DENvo,35368
+geode_explicit/lib64/libGeode-Explicit_section.so,sha256=nREziECHjaKJ2PAUYzXu9xv8am6F3B4-oB1UCtO_r4Y,77000
+Geode_Explicit-4.7.2rc1.dist-info/METADATA,sha256=mxSXE599lDr0zelwwh_m7-KGHCOsHxgeF44mnC5qHGg,2148
+Geode_Explicit-4.7.2rc1.dist-info/WHEEL,sha256=cPiEulY4lHJMdGCxx29HxfDkwhV9C6172sJgZUA9dSs,103
+Geode_Explicit-4.7.2rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.7.2rc1.dist-info/RECORD,,
```

