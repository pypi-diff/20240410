# Comparing `tmp/anyhedge-0.8.2.tar.gz` & `tmp/anyhedge-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-0.8.2.tar", last modified: Sun Mar 24 06:26:11 2024, max compression
+gzip compressed data, was "anyhedge-2.0.0.tar", last modified: Wed Apr 10 20:26:58 2024, max compression
```

## Comparing `anyhedge-0.8.2.tar` & `anyhedge-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-03-24 06:26:11.171506 anyhedge-0.8.2/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.8.2/LICENSE
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-03-24 06:26:11.171506 anyhedge-0.8.2/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.8.2/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-03-24 06:26:11.167506 anyhedge-0.8.2/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.8.2/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2425 2023-12-05 19:11:48.000000 anyhedge-0.8.2/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    45338 2024-03-24 06:17:01.000000 anyhedge-0.8.2/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.8.2/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.8.2/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-03-24 06:26:11.171506 anyhedge-0.8.2/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    43176 2024-03-24 06:20:55.000000 anyhedge-0.8.2/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.8.2/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.8.2/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-03-24 06:26:11.171506 anyhedge-0.8.2/anyhedge.egg-info/
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-03-24 06:26:11.000000 anyhedge-0.8.2/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      512 2024-03-24 06:26:11.000000 anyhedge-0.8.2/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-03-24 06:26:11.000000 anyhedge-0.8.2/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-03-24 06:26:11.000000 anyhedge-0.8.2/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-03-24 06:26:11.000000 anyhedge-0.8.2/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-03-24 06:21:27.000000 anyhedge-0.8.2/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-03-24 06:26:11.171506 anyhedge-0.8.2/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-04-10 20:26:58.339672 anyhedge-2.0.0/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-2.0.0/LICENSE
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-04-10 20:26:58.339672 anyhedge-2.0.0/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-2.0.0/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-04-10 20:26:58.335672 anyhedge-2.0.0/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-2.0.0/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2426 2024-04-10 20:22:29.000000 anyhedge-2.0.0/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    45310 2024-04-10 20:24:54.000000 anyhedge-2.0.0/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-2.0.0/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-2.0.0/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-04-10 20:26:58.339672 anyhedge-2.0.0/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    43176 2024-03-24 06:20:55.000000 anyhedge-2.0.0/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-2.0.0/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-2.0.0/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-04-10 20:26:58.339672 anyhedge-2.0.0/anyhedge.egg-info/
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-04-10 20:26:58.000000 anyhedge-2.0.0/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      512 2024-04-10 20:26:58.000000 anyhedge-2.0.0/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-04-10 20:26:58.000000 anyhedge-2.0.0/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-04-10 20:26:58.000000 anyhedge-2.0.0/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-04-10 20:26:58.000000 anyhedge-2.0.0/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-04-10 20:26:10.000000 anyhedge-2.0.0/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-04-10 20:26:58.339672 anyhedge-2.0.0/setup.cfg
```

### Comparing `anyhedge-0.8.2/LICENSE` & `anyhedge-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/PKG-INFO` & `anyhedge-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.8.2
+Version: 2.0.0
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.8.2/README.md` & `anyhedge-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/bch_primitives.py` & `anyhedge-2.0.0/anyhedge/bch_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Library imports
 from arrow import Arrow
 
 # Local imports
 from . import validators
 
-DUST = 546
+DUST = 1332
 PUBLIC_KEY_BYTES_LENGTH = 33
 SCRIPT_INT_MAX_WHEN_JAVASCRIPT = int(2 ** 53)
 SCRIPT_INT_MAX = int(2 ** 63 - 1)
 SATS_PER_BCH = int(1e8)
 MAX_REASONABLE_SATS = int(100_000 * SATS_PER_BCH)  # 100k BCH
 MIN_NLOCKTIME_TIMESTAMP = 500_000_000
 MIN_REASONABLE_DIVISION_STEPS = 500
```

### Comparing `anyhedge-0.8.2/anyhedge/contract.py` & `anyhedge-2.0.0/anyhedge/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
     @property
     def effective_nominal_value_oracleUnits(self) -> OracleUnit:
         return self.oracle_unit_cls(self.nominal_oracleUnits_x_satsPerBch / SATS_PER_BCH)
 
     @property
     def cost_sats_for_nominal_value_at_start(self) -> UtxoSats:
-        return UtxoSats(round_half_up(float(self.nominal_oracleUnits_x_satsPerBch) / float(self.start_price_oracleUnits_per_bch)))
+        return UtxoSats(self.nominal_oracleUnits_x_satsPerBch // self.start_price_oracleUnits_per_bch)
 
     @property
     def effective_short_leverage(self) -> ShortLeverage:
         # There is a special case where even if the liquidation price must be recorded at some max value,
         # The fundamental cost for the position at liquidation is hard-lined at zero. That is the definition
         # of a hard hedge position, emulating the original anyhedge contract behavior.
         if self.cost_sats_for_nominal_value_at_high_liquidation == 0:
```

### Comparing `anyhedge-0.8.2/anyhedge/fee.py` & `anyhedge-2.0.0/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/oracle.py` & `anyhedge-2.0.0/anyhedge/oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/tests/test_bch_primitives.py` & `anyhedge-2.0.0/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/tests/test_contract.py` & `anyhedge-2.0.0/anyhedge/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/tests/test_fee.py` & `anyhedge-2.0.0/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge/tests/test_oracle.py` & `anyhedge-2.0.0/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/anyhedge.egg-info/PKG-INFO` & `anyhedge-2.0.0/anyhedge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.8.2
+Version: 2.0.0
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.8.2/anyhedge.egg-info/SOURCES.txt` & `anyhedge-2.0.0/anyhedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyhedge-0.8.2/pyproject.toml` & `anyhedge-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '0.8.2'
+version = '2.0.0'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

