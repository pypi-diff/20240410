# Comparing `tmp/coreforecast-0.0.7.tar.gz` & `tmp/coreforecast-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreforecast-0.0.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "coreforecast-0.0.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `coreforecast-0.0.7.tar` & `coreforecast-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.github/workflows/build-docs.yaml
--rw-r--r--   0        0        0     2624 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1641 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.github/workflows/release.yaml
--rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.gitignore
--rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 coreforecast-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 coreforecast-0.0.7/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 coreforecast-0.0.7/LICENSE
--rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 coreforecast-0.0.7/README.md
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/__init__.py
--rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/_lib.py
--rw-r--r--   0        0        0     2029 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/differences.py
--rw-r--r--   0        0        0    14913 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/grouped_array.py
--rw-r--r--   0        0        0    12313 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/lag_transforms.py
--rw-r--r--   0        0        0    23057 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/scalers.py
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/seasonal.py
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 coreforecast-0.0.7/coreforecast/utils.py
--rw-r--r--   0        0        0     2883 2022-11-09 12:37:21.000000 coreforecast-0.0.7/docs/mintlify/dark.png
--rw-r--r--   0        0        0     1633 2022-11-09 12:37:21.000000 coreforecast-0.0.7/docs/mintlify/favicon.svg
--rw-r--r--   0        0        0     2851 2022-11-09 12:37:21.000000 coreforecast-0.0.7/docs/mintlify/light.png
--rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 coreforecast-0.0.7/docs/mintlify/mint.json
--rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 coreforecast-0.0.7/docs/to_mdx.py
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/brent.h
--rw-r--r--   0        0        0     3545 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/diff.h
--rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/expanding.h
--rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/exponentially_weighted.h
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/export.h
--rw-r--r--   0        0        0     5456 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/grouped_array.h
--rw-r--r--   0        0        0     2529 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/grouped_array_functions.h
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/kpss.h
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/lag.h
--rw-r--r--   0        0        0    12968 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/rolling.h
--rw-r--r--   0        0        0     4467 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/scalers.h
--rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/seasonal.h
--rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 coreforecast-0.0.7/include/stats.h
--rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 coreforecast-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 coreforecast-0.0.7/requirements-test.txt
--rwxr-xr-x   0        0        0      199 2022-11-09 12:37:21.000000 coreforecast-0.0.7/scripts/switch_xcode
--rw-r--r--   0        0        0     8132 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/diff.cpp
--rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/expanding.cpp
--rw-r--r--   0        0        0      872 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/exponentially_weighted.cpp
--rw-r--r--   0        0        0     4287 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/grouped_array_functions.cpp
--rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/lag.cpp
--rw-r--r--   0        0        0    26212 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/rolling.cpp
--rw-r--r--   0        0        0    13389 2022-11-09 12:37:21.000000 coreforecast-0.0.7/src/scalers.cpp
--rw-r--r--   0        0        0     3403 2022-11-09 12:37:21.000000 coreforecast-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/build-docs.yaml
+-rw-r--r--   0        0        0     2624 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1641 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      313 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.gitignore
+-rw-r--r--   0        0        0      255 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 coreforecast-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 coreforecast-0.0.8/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 coreforecast-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 coreforecast-0.0.8/README.md
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/__init__.py
+-rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/_lib.py
+-rw-r--r--   0        0        0     2029 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/differences.py
+-rw-r--r--   0        0        0    15261 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/grouped_array.py
+-rw-r--r--   0        0        0    12313 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/lag_transforms.py
+-rw-r--r--   0        0        0    23057 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/scalers.py
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/seasonal.py
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 coreforecast-0.0.8/coreforecast/utils.py
+-rw-r--r--   0        0        0     2883 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/dark.png
+-rw-r--r--   0        0        0     1633 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/favicon.svg
+-rw-r--r--   0        0        0     2851 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/light.png
+-rw-r--r--   0        0        0      694 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/mintlify/mint.json
+-rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 coreforecast-0.0.8/docs/to_mdx.py
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/brent.h
+-rw-r--r--   0        0        0     3545 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/diff.h
+-rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/expanding.h
+-rw-r--r--   0        0        0      353 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/exponentially_weighted.h
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/export.h
+-rw-r--r--   0        0        0     5456 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/grouped_array.h
+-rw-r--r--   0        0        0     2529 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/grouped_array_functions.h
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/kpss.h
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/lag.h
+-rw-r--r--   0        0        0    12968 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/rolling.h
+-rw-r--r--   0        0        0     4467 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/scalers.h
+-rw-r--r--   0        0        0     1701 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/seasonal.h
+-rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 coreforecast-0.0.8/include/stats.h
+-rw-r--r--   0        0        0     1501 2022-11-09 12:37:21.000000 coreforecast-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 coreforecast-0.0.8/requirements-test.txt
+-rwxr-xr-x   0        0        0      199 2022-11-09 12:37:21.000000 coreforecast-0.0.8/scripts/switch_xcode
+-rw-r--r--   0        0        0     8132 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/diff.cpp
+-rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/expanding.cpp
+-rw-r--r--   0        0        0      872 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/exponentially_weighted.cpp
+-rw-r--r--   0        0        0     4287 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/grouped_array_functions.cpp
+-rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/lag.cpp
+-rw-r--r--   0        0        0    26212 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/rolling.cpp
+-rw-r--r--   0        0        0    13389 2022-11-09 12:37:21.000000 coreforecast-0.0.8/src/scalers.cpp
+-rw-r--r--   0        0        0     3403 2022-11-09 12:37:21.000000 coreforecast-0.0.8/PKG-INFO
```

### Comparing `coreforecast-0.0.7/.github/workflows/build-docs.yaml` & `coreforecast-0.0.8/.github/workflows/build-docs.yaml`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/.github/workflows/ci.yaml` & `coreforecast-0.0.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/.github/workflows/release.yaml` & `coreforecast-0.0.8/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/CMakeLists.txt` & `coreforecast-0.0.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/LICENSE` & `coreforecast-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/README.md` & `coreforecast-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/coreforecast/differences.py` & `coreforecast-0.0.8/coreforecast/differences.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/coreforecast/grouped_array.py` & `coreforecast-0.0.8/coreforecast/grouped_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,23 +79,25 @@
             self._handle,
             _data_as_void_ptr(stats),
         )
         return stats
 
     def _scaler_transform(self, stats: np.ndarray) -> np.ndarray:
         out = np.empty_like(self.data)
+        stats = stats.astype(self.data.dtype, copy=False)
         _LIB[f"{self.prefix}_ScalerTransform"](
             self._handle,
             _data_as_void_ptr(stats),
             _data_as_void_ptr(out),
         )
         return out
 
     def _scaler_inverse_transform(self, stats: np.ndarray) -> np.ndarray:
         out = np.empty_like(self.data)
+        stats = stats.astype(self.data.dtype, copy=False)
         _LIB[f"{self.prefix}_ScalerInverseTransform"](
             self._handle,
             _data_as_void_ptr(stats),
             _data_as_void_ptr(out),
         )
         return out
 
@@ -362,23 +364,25 @@
                 _pyfloat_to_np_c(upper, self.data.dtype),
                 _data_as_void_ptr(out),
             )
         return out
 
     def _boxcox_transform(self, stats: np.ndarray) -> np.ndarray:
         out = np.empty_like(self.data)
+        stats = stats.astype(self.data.dtype, copy=False)
         _LIB[f"{self.prefix}_BoxCoxTransform"](
             self._handle,
             _data_as_void_ptr(stats),
             _data_as_void_ptr(out),
         )
         return out
 
     def _boxcox_inverse_transform(self, stats: np.ndarray) -> np.ndarray:
         out = np.empty_like(self.data)
+        stats = stats.astype(self.data.dtype, copy=False)
         _LIB[f"{self.prefix}_BoxCoxInverseTransform"](
             self._handle,
             _data_as_void_ptr(stats),
             _data_as_void_ptr(out),
         )
         return out
 
@@ -436,18 +440,20 @@
             _data_as_void_ptr(ds),
             _data_as_void_ptr(out),
         )
         return out
 
     def _inv_diff(self, d: int, tails: np.ndarray) -> np.ndarray:
         ds = np.full(len(self), d, dtype=_indptr_dtype)
+        tails = tails.astype(self.data.dtype, copy=False)
         return self._inv_diffs(ds, tails)
 
     def _inv_diffs(self, ds: np.ndarray, tails: np.ndarray) -> np.ndarray:
         tails_indptr = _diffs_to_indptr(ds)
+        tails = tails.astype(self.data.dtype, copy=False)
         tails_ga = GroupedArray(tails, tails_indptr)
         out = np.empty_like(self.data)
         _LIB[f"{self.prefix}_InvertDifferences"](
             self._handle,
             tails_ga._handle,
             _data_as_void_ptr(self.indptr),
             _data_as_void_ptr(out),
```

### Comparing `coreforecast-0.0.7/coreforecast/lag_transforms.py` & `coreforecast-0.0.8/coreforecast/lag_transforms.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/coreforecast/scalers.py` & `coreforecast-0.0.8/coreforecast/scalers.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/coreforecast/seasonal.py` & `coreforecast-0.0.8/coreforecast/seasonal.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/coreforecast/utils.py` & `coreforecast-0.0.8/coreforecast/utils.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/docs/mintlify/dark.png` & `coreforecast-0.0.8/docs/mintlify/dark.png`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/docs/mintlify/favicon.svg` & `coreforecast-0.0.8/docs/mintlify/favicon.svg`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/docs/mintlify/light.png` & `coreforecast-0.0.8/docs/mintlify/light.png`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/docs/mintlify/mint.json` & `coreforecast-0.0.8/docs/mintlify/mint.json`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/docs/to_mdx.py` & `coreforecast-0.0.8/docs/to_mdx.py`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/brent.h` & `coreforecast-0.0.8/include/brent.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/diff.h` & `coreforecast-0.0.8/include/diff.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/expanding.h` & `coreforecast-0.0.8/include/expanding.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/grouped_array.h` & `coreforecast-0.0.8/include/grouped_array.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/grouped_array_functions.h` & `coreforecast-0.0.8/include/grouped_array_functions.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/kpss.h` & `coreforecast-0.0.8/include/kpss.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/rolling.h` & `coreforecast-0.0.8/include/rolling.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/scalers.h` & `coreforecast-0.0.8/include/scalers.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/seasonal.h` & `coreforecast-0.0.8/include/seasonal.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/include/stats.h` & `coreforecast-0.0.8/include/stats.h`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/pyproject.toml` & `coreforecast-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coreforecast"
-version = "0.0.7"
+version = "0.0.8"
 requires-python = ">=3.8"
 dependencies = [
     "importlib_resources ; python_version < '3.10'",
     "numpy>=1.20.0",
 ]
 license = { text = "Apache-2.0" }
 classifiers = [
```

### Comparing `coreforecast-0.0.7/src/diff.cpp` & `coreforecast-0.0.8/src/diff.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/expanding.cpp` & `coreforecast-0.0.8/src/expanding.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/exponentially_weighted.cpp` & `coreforecast-0.0.8/src/exponentially_weighted.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/grouped_array_functions.cpp` & `coreforecast-0.0.8/src/grouped_array_functions.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/lag.cpp` & `coreforecast-0.0.8/src/lag.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/rolling.cpp` & `coreforecast-0.0.8/src/rolling.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/src/scalers.cpp` & `coreforecast-0.0.8/src/scalers.cpp`

 * *Files identical despite different names*

### Comparing `coreforecast-0.0.7/PKG-INFO` & `coreforecast-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreforecast
-Version: 0.0.7
+Version: 0.0.8
 Summary: Fast implementations of common forecasting routines
 Keywords: forecasting time-series
 Home-page: https://nixtla.github.io/coreforecast
 Author-Email: José Morales <jmoralz92@gmail.com>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

