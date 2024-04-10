# Comparing `tmp/vnpy_excelrtd-1.0.1.tar.gz` & `tmp/vnpy_excelrtd-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_excelrtd-1.0.1.tar", last modified: Sun Feb 20 12:48:40 2022, max compression
+gzip compressed data, was "vnpy_excelrtd-1.0.2.tar", last modified: Wed Apr 10 06:52:45 2024, max compression
```

## Comparing `vnpy_excelrtd-1.0.1.tar` & `vnpy_excelrtd-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-02-20 12:48:40.288133 vnpy_excelrtd-1.0.1/
--rw-rw-rw-   0        0        0     1109 2021-12-05 03:09:01.000000 vnpy_excelrtd-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1867 2022-02-20 12:48:40.290242 vnpy_excelrtd-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2022-02-20 12:48:11.000000 vnpy_excelrtd-1.0.1/README.md
--rw-rw-rw-   0        0        0      953 2022-02-20 12:48:40.294415 vnpy_excelrtd-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-12-05 03:10:43.000000 vnpy_excelrtd-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-02-20 12:48:40.239185 vnpy_excelrtd-1.0.1/vnpy_excelrtd/
--rw-rw-rw-   0        0        0     1541 2022-02-20 12:47:45.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/__init__.py
--rw-rw-rw-   0        0        0     2171 2021-12-05 02:58:37.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/engine.py
-drwxrwxrwx   0        0        0        0 2022-02-20 12:48:40.285939 vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/
--rw-rw-rw-   0        0        0       32 2021-12-05 02:58:37.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/__init__.py
--rw-rw-rw-   0        0        0    67646 2021-12-05 02:58:37.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/rtd.ico
--rw-rw-rw-   0        0        0     2371 2021-12-05 02:58:37.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/widget.py
--rw-rw-rw-   0        0        0     2769 2021-12-05 02:58:37.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd/vnpy_rtd.py
-drwxrwxrwx   0        0        0        0 2022-02-20 12:48:40.277361 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/
--rw-rw-rw-   0        0        0     1867 2022-02-20 12:48:39.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2022-02-20 12:48:39.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-20 12:48:39.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-05 03:12:07.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2022-02-20 12:48:39.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-02-20 12:48:39.000000 vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:52:45.040215 vnpy_excelrtd-1.0.2/
+-rw-rw-rw-   0        0        0     1109 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1947 2024-04-10 06:52:45.041300 vnpy_excelrtd-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1020 2024-04-10 06:50:48.000000 vnpy_excelrtd-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1112 2024-04-10 06:52:45.052796 vnpy_excelrtd-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:52:44.965909 vnpy_excelrtd-1.0.2/vnpy_excelrtd/
+-rw-rw-rw-   0        0        0     1736 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/__init__.py
+-rw-rw-rw-   0        0        0     2254 2024-04-10 06:48:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/engine.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:52:45.038047 vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/
+-rw-rw-rw-   0        0        0       32 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/__init__.py
+-rw-rw-rw-   0        0        0    67646 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/rtd.ico
+-rw-rw-rw-   0        0        0     2593 2024-04-10 06:47:53.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/widget.py
+-rw-rw-rw-   0        0        0     2826 2024-04-10 06:51:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd/vnpy_rtd.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:52:45.032498 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/
+-rw-rw-rw-   0        0        0     1947 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 06:52:44.000000 vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/top_level.txt
```

### Comparing `vnpy_excelrtd-1.0.1/LICENSE` & `vnpy_excelrtd-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_excelrtd-1.0.1/PKG-INFO` & `vnpy_excelrtd-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: vnpy_excelrtd
-Version: 1.0.1
-Summary: excel RTD application for VeighNa quant trading framework.
+Version: 1.0.2
+Summary: Excel RTD application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeighNa框架的Excel RTD应用模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.1-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.2-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 RTD全称是RealTimeData，是微软提供的主要面向金融行业中实时数据需求设计的Excel数据对接方案.
 
@@ -50,9 +51,7 @@
 
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
-
-
```

### Comparing `vnpy_excelrtd-1.0.1/README.md` & `vnpy_excelrtd-1.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # VeighNa框架的Excel RTD应用模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.1-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.2-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 RTD全称是RealTimeData，是微软提供的主要面向金融行业中实时数据需求设计的Excel数据对接方案.
```

### Comparing `vnpy_excelrtd-1.0.1/setup.cfg` & `vnpy_excelrtd-1.0.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6578 6365 6c72 7464   = vnpy_excelrtd
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
-00000030: 310d 0a75 726c 203d 2068 7474 7073 3a2f  1..url = https:/
+00000030: 320d 0a75 726c 203d 2068 7474 7073 3a2f  2..url = https:/
 00000040: 2f77 7777 2e76 6e70 792e 636f 6d0d 0a6c  /www.vnpy.com..l
 00000050: 6963 656e 7365 203d 204d 4954 0d0a 6175  icense = MIT..au
 00000060: 7468 6f72 203d 2058 6961 6f79 6f75 2043  thor = Xiaoyou C
 00000070: 6865 6e0d 0a61 7574 686f 725f 656d 6169  hen..author_emai
 00000080: 6c20 3d20 7869 616f 796f 752e 6368 656e  l = xiaoyou.chen
 00000090: 406d 6169 6c2e 766e 7079 2e63 6f6d 0d0a  @mail.vnpy.com..
-000000a0: 6465 7363 7269 7074 696f 6e20 3d20 6578  description = ex
+000000a0: 6465 7363 7269 7074 696f 6e20 3d20 4578  description = Ex
 000000b0: 6365 6c20 5254 4420 6170 706c 6963 6174  cel RTD applicat
 000000c0: 696f 6e20 666f 7220 5665 6967 684e 6120  ion for VeighNa 
 000000d0: 7175 616e 7420 7472 6164 696e 6720 6672  quant trading fr
 000000e0: 616d 6577 6f72 6b2e 0d0a 6c6f 6e67 5f64  amework...long_d
 000000f0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000100: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000110: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
@@ -29,32 +29,42 @@
 000001c0: 6c65 0d0a 094f 7065 7261 7469 6e67 2053  le...Operating S
 000001d0: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
 000001e0: 6674 203a 3a20 5769 6e64 6f77 730d 0a09  ft :: Windows...
 000001f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000200: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 00000210: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
 00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000230: 7468 6f6e 203a 3a20 332e 370d 0a09 546f  thon :: 3.7...To
-00000240: 7069 6320 3a3a 204f 6666 6963 652f 4275  pic :: Office/Bu
-00000250: 7369 6e65 7373 203a 3a20 4669 6e61 6e63  siness :: Financ
-00000260: 6961 6c20 3a3a 2049 6e76 6573 746d 656e  ial :: Investmen
-00000270: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
-00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000290: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
-000002a0: 7469 6f6e 203a 3a20 4350 7974 686f 6e0d  tion :: CPython.
-000002b0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000002c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000002d0: 204c 6963 656e 7365 0d0a 094e 6174 7572   License...Natur
-000002e0: 616c 204c 616e 6775 6167 6520 3a3a 2043  al Language :: C
-000002f0: 6869 6e65 7365 2028 5369 6d70 6c69 6669  hinese (Simplifi
-00000300: 6564 290d 0a0d 0a5b 6f70 7469 6f6e 735d  ed)....[options]
-00000310: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000320: 643a 0d0a 7a69 705f 7361 6665 203d 2046  d:..zip_safe = F
-00000330: 616c 7365 0d0a 696e 7374 616c 6c5f 7265  alse..install_re
-00000340: 7175 6972 6573 203d 200d 0a09 696d 706f  quires = ...impo
-00000350: 7274 6c69 625f 6d65 7461 6461 7461 0d0a  rtlib_metadata..
-00000360: 0970 7978 6c6c 0d0a 0d0a 5b6f 7074 696f  .pyxll....[optio
-00000370: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000380: 0d0a 2a20 3d20 2a2e 6963 6f0d 0a0d 0a5b  ..* = *.ico....[
-00000390: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000003a0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000003b0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000230: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000250: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000260: 2033 2e31 310d 0a09 5072 6f67 7261 6d6d   3.11...Programm
+00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000280: 5079 7468 6f6e 203a 3a20 332e 3132 0d0a  Python :: 3.12..
+00000290: 0954 6f70 6963 203a 3a20 4f66 6669 6365  .Topic :: Office
+000002a0: 2f42 7573 696e 6573 7320 3a3a 2046 696e  /Business :: Fin
+000002b0: 616e 6369 616c 203a 3a20 496e 7665 7374  ancial :: Invest
+000002c0: 6d65 6e74 0d0a 0950 726f 6772 616d 6d69  ment...Programmi
+000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002e0: 7974 686f 6e20 3a3a 2049 6d70 6c65 6d65  ython :: Impleme
+000002f0: 6e74 6174 696f 6e20 3a3a 2043 5079 7468  ntation :: CPyth
+00000300: 6f6e 0d0a 094c 6963 656e 7365 203a 3a20  on...License :: 
+00000310: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000320: 4d49 5420 4c69 6365 6e73 650d 0a09 4e61  MIT License...Na
+00000330: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
+00000340: 3a20 4368 696e 6573 6520 2853 696d 706c  : Chinese (Simpl
+00000350: 6966 6965 6429 0d0a 0d0a 5b6f 7074 696f  ified)....[optio
+00000360: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+00000370: 6669 6e64 3a0d 0a7a 6970 5f73 6166 6520  find:..zip_safe 
+00000380: 3d20 4661 6c73 650d 0a69 6e73 7461 6c6c  = False..install
+00000390: 5f72 6571 7569 7265 7320 3d20 0d0a 0969  _requires = ...i
+000003a0: 6d70 6f72 746c 6962 5f6d 6574 6164 6174  mportlib_metadat
+000003b0: 610d 0a09 7079 786c 6c0d 0a0d 0a5b 6f70  a...pyxll....[op
+000003c0: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+000003d0: 7461 5d0d 0a2a 203d 202a 2e69 636f 0d0a  ta]..* = *.ico..
+000003e0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+000003f0: 5f70 6f69 6e74 735d 0d0a 7079 786c 6c20  _points]..pyxll 
+00000400: 3d20 0d0a 096d 6f64 756c 6573 203d 2076  = ...modules = v
+00000410: 6e70 795f 6578 6365 6c72 7464 3a70 7978  npy_excelrtd:pyx
+00000420: 6c6c 5f6d 6f64 756c 6573 0d0a 0d0a 5b65  ll_modules....[e
+00000430: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000440: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000450: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `vnpy_excelrtd-1.0.1/vnpy_excelrtd/engine.py` & `vnpy_excelrtd-1.0.2/vnpy_excelrtd/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-""""""
-
-from typing import Set
+from typing import Optional
 
 from vnpy.event import Event, EventEngine
 from vnpy.rpc import RpcServer
 from vnpy.trader.engine import BaseEngine, MainEngine
-from vnpy.trader.object import TickData, LogData, SubscribeRequest
+from vnpy.trader.object import TickData, ContractData, LogData, SubscribeRequest
 from vnpy.trader.event import EVENT_TICK
 
 
 APP_NAME = "ExcelRtd"
 
 EVENT_RTD_LOG = "eRtdLog"
 
@@ -18,24 +16,24 @@
 
 
 class RtdEngine(BaseEngine):
     """
     The engine for managing RTD objects and data update.
     """
 
-    def __init__(self, main_engine: MainEngine, event_engine: EventEngine):
+    def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """"""
         super().__init__(main_engine, event_engine, APP_NAME)
 
         self.server: RpcServer = RpcServer()
         self.server.register(self.subscribe)
         self.server.register(self.write_log)
         self.server.start(REP_ADDRESS, PUB_ADDRESS)
 
-        self.subscribed: Set[str] = set()
+        self.subscribed: set[str] = set()
 
         self.register_event()
 
     def register_event(self) -> None:
         """
         Register event handler.
         """
@@ -48,33 +46,33 @@
         tick: TickData = event.data
         self.server.publish("tick", tick)
 
     def write_log(self, msg: str) -> None:
         """
         Output RTD related log message.
         """
-        log = LogData(msg=msg, gateway_name=APP_NAME)
-        event = Event(EVENT_RTD_LOG, log)
+        log: LogData = LogData(msg=msg, gateway_name=APP_NAME)
+        event: Event = Event(EVENT_RTD_LOG, log)
         self.event_engine.put(event)
 
     def subscribe(self, vt_symbol: str) -> None:
         """
         Subscribe tick data update.
         """
-        contract = self.main_engine.get_contract(vt_symbol)
+        contract: Optional[ContractData] = self.main_engine.get_contract(vt_symbol)
         if not contract:
             return
 
         if vt_symbol in self.subscribed:
             return
         self.subscribed.add(vt_symbol)
 
-        req = SubscribeRequest(
+        req: SubscribeRequest = SubscribeRequest(
             contract.symbol,
             contract.exchange
         )
         self.main_engine.subscribe(req, contract.gateway_name)
 
-    def close(self):
+    def close(self) -> None:
         """"""
         self.server.stop()
         self.server.join()
```

### Comparing `vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/rtd.ico` & `vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/rtd.ico`

 * *Files identical despite different names*

### Comparing `vnpy_excelrtd-1.0.1/vnpy_excelrtd/ui/widget.py` & `vnpy_excelrtd-1.0.2/vnpy_excelrtd/ui/widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from pathlib import Path
 
 from vnpy.event import EventEngine, Event
 from vnpy.trader.engine import MainEngine
 from vnpy.trader.ui import QtWidgets, QtCore
 from vnpy.trader.object import LogData
-from ..engine import APP_NAME, EVENT_RTD_LOG
+from ..engine import APP_NAME, EVENT_RTD_LOG, BaseEngine
 
 
 class RtdManager(QtWidgets.QWidget):
     """"""
-    signal_log = QtCore.pyqtSignal(Event)
+    signal_log: QtCore.pyqtSignal = QtCore.pyqtSignal(Event)
 
-    def __init__(self, main_engine: MainEngine, event_engine: EventEngine):
+    def __init__(self, main_engine: MainEngine, event_engine: EventEngine) -> None:
         """"""
         super().__init__()
 
-        self.main_engine = main_engine
-        self.event_engine = event_engine
-        self.rm_engine = main_engine.get_engine(APP_NAME)
+        self.main_engine: MainEngine = main_engine
+        self.event_engine: EventEngine = event_engine
+        self.rm_engine: BaseEngine = main_engine.get_engine(APP_NAME)
 
         self.init_ui()
         self.register_event()
 
     def init_ui(self) -> None:
         """
         Init widget ui components.
         """
         self.setWindowTitle("Excel RTD")
         self.resize(600, 600)
 
-        module_path = Path(__file__).parent.parent
-        client_path = module_path.joinpath("vnpy_rtd.py")
-        self.client_line = QtWidgets.QLineEdit(str(client_path))
+        module_path: Path = Path(__file__).parent.parent
+        client_path: Path = module_path.joinpath("vnpy_rtd.py")
+        self.client_line: QtWidgets.QLineEdit = QtWidgets.QLineEdit(str(client_path))
         self.client_line.setReadOnly(True)
 
-        copy_button = QtWidgets.QPushButton("复制")
+        copy_button: QtWidgets.QPushButton = QtWidgets.QPushButton("复制")
         copy_button.clicked.connect(self.copy_client_path)
 
-        self.log_monitor = QtWidgets.QTextEdit()
+        self.log_monitor: QtWidgets.QTextEdit = QtWidgets.QTextEdit()
         self.log_monitor.setReadOnly(True)
 
-        self.port_label = QtWidgets.QLabel(
+        self.port_label: QtWidgets.QLabel = QtWidgets.QLabel(
             "使用Socket端口：请求回应9001、广播推送9002"
         )
 
-        hbox = QtWidgets.QHBoxLayout()
+        hbox: QtWidgets.QHBoxLayout = QtWidgets.QHBoxLayout()
         hbox.addWidget(self.client_line)
         hbox.addWidget(copy_button)
 
-        vbox = QtWidgets.QVBoxLayout()
+        vbox: QtWidgets.QVBoxLayout = QtWidgets.QVBoxLayout()
         vbox.addLayout(hbox)
         vbox.addWidget(self.log_monitor)
         vbox.addWidget(self.port_label)
         self.setLayout(vbox)
 
     def register_event(self) -> None:
         """
@@ -64,15 +64,15 @@
 
     def process_log_event(self, event: Event) -> None:
         """
         Show log message in monitor.
         """
         log: LogData = event.data
 
-        msg = f"{log.time}: {log.msg}"
+        msg: str = f"{log.time}: {log.msg}"
         self.log_monitor.append(msg)
 
     def copy_client_path(self) -> None:
         """
         Copy path of client python file to clipboard.
         """
         self.client_line.selectAll()
```

### Comparing `vnpy_excelrtd-1.0.1/vnpy_excelrtd/vnpy_rtd.py` & `vnpy_excelrtd-1.0.2/vnpy_excelrtd/vnpy_rtd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-""""""
-
-from typing import Dict, Set, Any
 from collections import defaultdict
 
 from pyxll import RTD, xl_func
 
 from vnpy.rpc import RpcClient
 from vnpy.trader.object import TickData
 
@@ -17,82 +14,82 @@
 
 
 class ObjectRtd(RTD):
     """
     RTD proxy for object in Python.
     """
 
-    def __init__(self, engine: "RtdClient", name: str, field: str):
+    def __init__(self, engine: "RtdClient", name: str, field: str) -> None:
         """Constructor"""
         super().__init__(value=0)
 
-        self.engine = engine
-        self.name = name
-        self.field = field
+        self.engine: RtdClient = engine
+        self.name: str = name
+        self.field: str = field
 
     def connect(self) -> None:
         """
         Callback when excel cell rtd is connected.
         """
         self.engine.add_rtd(self)
 
     def disconnect(self) -> None:
         """
         Callback when excel cell rtd is disconncted.
         """
         self.engine.remove_rtd(self)
 
-    def update(self, data: Any) -> None:
+    def update(self, data: object) -> None:
         """
         Update value in excel cell.
         """
         new_value = getattr(data, self.field, "N/A")
 
         if new_value != self.value:
             self.value = new_value
 
 
 class RtdClient(RpcClient):
     """
     The engine for managing RTD objects and data update.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """"""
         super().__init__()
 
-        self.rtds: Dict[str, Set[ObjectRtd]] = defaultdict(set)
+        self.rtds: dict[str, set[ObjectRtd]] = defaultdict(set)
 
         global rtd_client
         rtd_client = self
 
-    def callback(self, topic: str, data: Any) -> None:
+    def callback(self, topic: str, data: object) -> None:
         """"""
         tick: TickData = data
-        buf = self.rtds[tick.vt_symbol]
+        buf: set[ObjectRtd] = self.rtds[tick.vt_symbol]
 
         for rtd in buf:
             rtd.update(tick)
 
     def add_rtd(self, rtd: ObjectRtd) -> None:
         """
         Add a new RTD into the engine..
         """
-        buf = self.rtds[rtd.name]
+        buf: set[ObjectRtd] = self.rtds[rtd.name]
         buf.add(rtd)
         self.write_log(f"新增RTD连接：{rtd.name} {rtd.field}")
 
         # Auto subscribe tick data
         self.subscribe(rtd.name)
 
     def remove_rtd(self, rtd: ObjectRtd) -> None:
         """
         Remove an existing RTD from the engine.
         """
-        buf = self.rtds[self.name]
+        buf: set[ObjectRtd] = self.rtds[self.name]
         if self in buf:
             buf.remove(rtd)
             self.write_log(f"移除RTD连接：{rtd.name} {rtd.field}")
 
 
 def init_client() -> None:
     """Initialize vnpy rtd client"""
@@ -106,9 +103,9 @@
 def rtd_tick_data(vt_symbol: str, field: str) -> ObjectRtd:
     """
     Return the streaming value of the tick data field.
     """
     if not rtd_client:
         init_client()
 
-    rtd = ObjectRtd(rtd_client, vt_symbol, field)
+    rtd: ObjectRtd = ObjectRtd(rtd_client, vt_symbol, field)
     return rtd
```

### Comparing `vnpy_excelrtd-1.0.1/vnpy_excelrtd.egg-info/PKG-INFO` & `vnpy_excelrtd-1.0.2/vnpy_excelrtd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: vnpy-excelrtd
-Version: 1.0.1
-Summary: excel RTD application for VeighNa quant trading framework.
+Version: 1.0.2
+Summary: Excel RTD application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeighNa框架的Excel RTD应用模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.1-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.2-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 RTD全称是RealTimeData，是微软提供的主要面向金融行业中实时数据需求设计的Excel数据对接方案.
 
@@ -50,9 +51,7 @@
 
 
 或者下载源代码后，解压后在cmd中运行：
 
 ```
 pip install .
 ```
-
-
```

