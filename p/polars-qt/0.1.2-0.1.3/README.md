# Comparing `tmp/polars_qt-0.1.2.tar.gz` & `tmp/polars_qt-0.1.3.tar.gz`

## Comparing `polars_qt-0.1.2.tar` & `polars_qt-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 polars_qt-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      100 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-08 06:47:06.000000 polars_qt-0.1.2/.python-version
--rw-r--r--   0     1001      127      541 2024-04-08 06:47:06.000000 polars_qt-0.1.2/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-08 06:47:06.000000 polars_qt-0.1.2/README.md
--rw-r--r--   0     1001      127       38 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/__init__.py
--rw-r--r--   0     1001      127     2893 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/funcs.py
--rw-r--r--   0     1001      127     1408 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/qt.py
--rw-r--r--   0     1001      127     2567 2024-04-08 06:47:06.000000 polars_qt-0.1.2/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-08 06:47:06.000000 polars_qt-0.1.2/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-08 06:47:06.000000 polars_qt-0.1.2/rust-toolchain.toml
--rw-r--r--   0     1001      127    13255 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/if_then.rs
--rw-r--r--   0     1001      127      276 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-08 06:47:06.000000 polars_qt-0.1.2/src/rolling_rank.rs
--rw-r--r--   0     1001      127     1375 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-08 06:47:06.000000 polars_qt-0.1.2/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127    33830 2024-04-08 06:47:21.000000 polars_qt-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127     1726 2024-04-08 06:47:06.000000 polars_qt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 polars_qt-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-10 05:28:13.000000 polars_qt-0.1.3/.python-version
+-rw-r--r--   0     1001      127      645 2024-04-10 05:28:13.000000 polars_qt-0.1.3/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-10 05:28:13.000000 polars_qt-0.1.3/README.md
+-rw-r--r--   0     1001      127       38 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     2898 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     2105 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/qt.py
+-rw-r--r--   0     1001      127     1917 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-10 05:28:13.000000 polars_qt-0.1.3/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-10 05:28:13.000000 polars_qt-0.1.3/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-10 05:28:13.000000 polars_qt-0.1.3/rust-toolchain.toml
+-rw-r--r--   0     1001      127    13211 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/if_then.rs
+-rw-r--r--   0     1001      127      319 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     7926 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/strategy/boll.rs
+-rw-r--r--   0     1001      127      617 2024-04-10 05:28:13.000000 polars_qt-0.1.3/src/strategy/mod.rs
+-rw-r--r--   0     1001      127     1375 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1227 2024-04-10 05:28:13.000000 polars_qt-0.1.3/tests/test_strategy.py
+-rw-r--r--   0     1001      127    41876 2024-04-10 05:28:25.000000 polars_qt-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-10 05:28:13.000000 polars_qt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.3/PKG-INFO
```

### Comparing `polars_qt-0.1.2/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.3/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/Makefile` & `polars_qt-0.1.3/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 
 pre-commit: .venv
 	cargo fmt --all && cargo clippy --all-features
 	ruff check . --fix --exit-non-zero-on-fix
 	ruff format polars_qt tests
 	# .venv/bin/mypy polars_qt tests
 
+format:
+	cargo fmt --all
+	cargo clippy --all-features
+	ruff check
+
 test: .venv
 	pytest tests
 
 debug: 
 	maturin develop
 
+release:
+	maturin develop --release
+
```

### Comparing `polars_qt-0.1.2/README.md` & `polars_qt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/polars_qt/funcs.py` & `polars_qt-0.1.3/polars_qt/funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     contract_chg_signal: IntoExpr | None = None,
 ) -> pl.Expr:
     open = parse_into_expr(open).cast(pl.Float64)
     close = parse_into_expr(close).cast(pl.Float64)
     signal = parse_into_expr(signal).cast(pl.Float64)
     pos = signal.shift(fill_value=0) if is_signal else signal
     base_config = {
-        "init_cash": init_cash,
+        "init_cash": int(init_cash),
         "multiplier": multiplier,
         "leverage": leverage,
         "c_rate": c_rate,
         "blowup": blowup,
         "commision_type": commision_type,
     }
     assert commision_type in ["percent", "absolute"]
```

### Comparing `polars_qt-0.1.2/polars_qt/qt.py` & `polars_qt-0.1.3/polars_qt/qt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import polars as pl
 
 from .funcs import *
+from .strategy import boll
 
 
 @pl.api.register_expr_namespace("qt")
 class ExprQuantExtend:
     def __init__(self, expr: pl.Expr):
         self.expr = expr
 
@@ -45,7 +46,29 @@
             slippage=slippage,
             ticksize=ticksize,
             c_rate=c_rate,
             blowup=blowup,
             commision_type=commision_type,
             contract_chg_signal=contract_chg_signal,
         )
+
+    def boll(
+        self,
+        params: tuple[int, float, float] | tuple[int, float] | int,
+        min_periods: int | None = None,
+        filters: tuple[IntoExpr, IntoExpr, IntoExpr, IntoExpr] | None = None,
+        *,
+        delay_open: bool = False,
+        long_signal: float = 1,
+        short_signal: float = -1,
+        close_signal: float = 0,
+    ) -> pl.Expr:
+        return boll(
+            self.expr,
+            params=params,
+            min_periods=min_periods,
+            filters=filters,
+            delay_open=delay_open,
+            long_signal=long_signal,
+            short_signal=short_signal,
+            close_signal=close_signal,
+    )
```

### Comparing `polars_qt-0.1.2/polars_qt/utils.py` & `polars_qt-0.1.3/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/src/equity.rs` & `polars_qt-0.1.3/src/equity.rs`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     Ok(
         impl_calc_future_ret(pos, opening_cost, closing_cost, contract_chg_signal, kwargs)
             .into_series(),
     )
 }
 
 fn impl_calc_future_ret(
-    pos_se: &ChunkedArray<Float64Type>,
-    opening_cost_se: &ChunkedArray<Float64Type>,
-    closing_cost_se: &ChunkedArray<Float64Type>,
-    contract_chg_signal_se: Option<&ChunkedArray<BooleanType>>,
+    pos_se: &Float64Chunked,
+    opening_cost_se: &Float64Chunked,
+    closing_cost_se: &Float64Chunked,
+    contract_chg_signal_se: Option<&BooleanChunked>,
     kwargs: FutureRetKwargs,
 ) -> Float64Chunked {
     let mut cash = kwargs.init_cash as f64;
     let mut last_pos = 0_f64; // pos_arr[0];
     let mut last_lot_num = 0.;
     if pos_se.is_empty() {
         return Float64Chunked::from_vec(pos_se.name(), vec![]);
```

### Comparing `polars_qt-0.1.2/src/if_then.rs` & `polars_qt-0.1.3/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/src/rolling_rank.rs` & `polars_qt-0.1.3/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/tests/test_equity.py` & `polars_qt-0.1.3/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/tests/test_if_then.py` & `polars_qt-0.1.3/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/tests/test_rolling_rank.py` & `polars_qt-0.1.3/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.2/Cargo.lock` & `polars_qt-0.1.3/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,29 @@
 [[package]]
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "argminmax"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52424b59d69d69d5056d508b260553afd91c57e21849579cd1f50ee8b8b88eaa"
 dependencies = [
  "num-traits",
 ]
@@ -42,14 +57,23 @@
 [[package]]
 name = "array-init-cursor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
 [[package]]
+name = "atoi"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
@@ -73,17 +97,17 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
@@ -110,26 +134,54 @@
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
+name = "cc"
+version = "1.0.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+dependencies = [
+ "jobserver",
+ "libc",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
  "num-traits",
+ "windows-targets 0.52.4",
+]
+
+[[package]]
+name = "core-foundation-sys"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
+name = "crossbeam-channel"
+version = "0.5.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+dependencies = [
+ "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
@@ -144,14 +196,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "crossbeam-queue"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dyn-clone"
@@ -162,14 +223,26 @@
 [[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
+name = "enum_dispatch"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
+dependencies = [
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "ethnum"
@@ -193,26 +266,32 @@
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "getrandom"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
  "allocator-api2",
@@ -231,14 +310,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows-core",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
@@ -253,20 +355,38 @@
 [[package]]
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
+name = "jobserver"
+version = "0.1.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -296,14 +416,34 @@
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "lz4"
+version = "1.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
+dependencies = [
+ "libc",
+ "lz4-sys",
+]
+
+[[package]]
+name = "lz4-sys"
+version = "1.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
@@ -342,14 +482,32 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "target-features",
 ]
 
 [[package]]
+name = "now"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
+dependencies = [
+ "chrono",
+]
+
+[[package]]
+name = "ntapi"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -413,14 +571,20 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pkg-config"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
@@ -431,15 +595,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f01006048a264047d6cba081fed8e11adbd69c15956f9e53185a9ac4a541853c"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
+ "polars-io",
+ "polars-lazy",
  "polars-parquet",
+ "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
 version = "0.38.3"
@@ -454,24 +621,26 @@
  "either",
  "ethnum",
  "fast-float",
  "foreign_vec",
  "getrandom",
  "hashbrown",
  "itoa",
+ "lz4",
  "multiversion",
  "num-traits",
  "polars-arrow-format",
  "polars-error",
  "polars-utils",
  "ryu",
  "simdutf8",
  "streaming-iterator",
  "strength_reduce",
  "version_check",
+ "zstd",
 ]
 
 [[package]]
 name = "polars-arrow-format"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b0ef2474af9396b19025b189d96e992311e6a47f90c53cd998b36c4c64b84c"
@@ -501,40 +670,43 @@
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f20d3c227186f74aa3c228c64ef72f5a15617322fed30b4323eaf53b25f8e7b"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "bytemuck",
+ "chrono",
  "either",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-arrow",
  "polars-compute",
  "polars-error",
  "polars-row",
  "polars-utils",
  "rand",
  "rand_distr",
  "rayon",
+ "regex",
  "smartstring",
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d66dd0ce51f8bd620eb8bd376502fe68a2b1a446d5433ecd2e75270b0755ce76"
 dependencies = [
  "polars-arrow-format",
+ "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-ffi"
 version = "0.38.3"
@@ -549,30 +721,55 @@
 name = "polars-io"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b40bef2edcdc58394792c4d779465144283a09ff1836324e7b72df7978a6e992"
 dependencies = [
  "ahash",
  "bytes",
+ "chrono",
  "home",
  "memchr",
  "memmap2",
  "num-traits",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-error",
+ "polars-time",
  "polars-utils",
  "rayon",
  "regex",
  "smartstring",
 ]
 
 [[package]]
+name = "polars-lazy"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c27df26a19d3092298d31d47614ad84dc330c106e38aa8cd53727cd91c07cf56"
+dependencies = [
+ "ahash",
+ "bitflags 2.5.0",
+ "glob",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-pipe",
+ "polars-plan",
+ "polars-time",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+ "version_check",
+]
+
+[[package]]
 name = "polars-ops"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f8a51c3bdc9e7c34196ff6f5c3cb17da134e5aafb1756aaf24b76c7118e63dc"
 dependencies = [
  "ahash",
  "argminmax",
@@ -609,38 +806,65 @@
  "polars-utils",
  "seq-macro",
  "simdutf8",
  "streaming-decompression",
 ]
 
 [[package]]
+name = "polars-pipe"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c5e2c1f14e81d60cfa9afe4e611a9bad9631a2cb7cd19b7c0094d0dc32f0231"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-queue",
+ "enum_dispatch",
+ "hashbrown",
+ "num-traits",
+ "polars-arrow",
+ "polars-compute",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-plan",
+ "polars-row",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+ "uuid",
+ "version_check",
+]
+
+[[package]]
 name = "polars-plan"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff48362bd1b078bbbec7e7ba9ec01fea58fee2887db22a8e3deaf78f322fa3c4"
 dependencies = [
  "ahash",
  "bytemuck",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
+ "polars-time",
  "polars-utils",
  "rayon",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
+ "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
 ]
 
 [[package]]
@@ -652,14 +876,33 @@
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
+name = "polars-time"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86eb74ea6ddfe675aa5c3f33c00dadbe2b85f0e8e3887b85db1fd5a3397267fd"
+dependencies = [
+ "atoi",
+ "chrono",
+ "now",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-error",
+ "polars-ops",
+ "polars-utils",
+ "regex",
+ "smartstring",
+]
+
+[[package]]
 name = "polars-utils"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "694656a7d2b0cd8f07660dbc8d0fb7a81066ff57a452264907531d805c1e58c4"
 dependencies = [
  "ahash",
  "bytemuck",
@@ -667,14 +910,15 @@
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
  "raw-cpuid",
  "rayon",
  "smartstring",
+ "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -787,17 +1031,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1044,14 +1288,28 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "sysinfo"
+version = "0.30.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e9a84fe4cfc513b41cb2596b624e561ec9e7e1c4b46328e496ed56a53514ef2a"
+dependencies = [
+ "cfg-if",
+ "core-foundation-sys",
+ "libc",
+ "ntapi",
+ "once_cell",
+ "windows",
+]
+
+[[package]]
 name = "target-features"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1bbb9f3c5c463a01705937a24fdabc5047929ac764b2d5b9cf681c1f5041ed5"
 
 [[package]]
 name = "target-lexicon"
@@ -1088,14 +1346,23 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
@@ -1154,14 +1421,55 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
+name = "windows"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.4",
+]
+
+[[package]]
+name = "windows-core"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
+dependencies = [
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
  "windows-targets 0.52.4",
 ]
@@ -1301,7 +1609,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
+
+[[package]]
+name = "zstd"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "7.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
+dependencies = [
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.10+zstd.1.5.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
+dependencies = [
+ "cc",
+ "pkg-config",
+]
```

### Comparing `polars_qt-0.1.2/pyproject.toml` & `polars_qt-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 
 [build-system]
 requires = ["maturin>=1.0,<2.0", "polars>=0.20.16"]
 build-backend = "maturin"
 
 [tool.rye]
 managed = true
+virtual = true
 dev-dependencies = [
     "maturin>=1.5.1",
     "pip>=24.0",
     "ruff>=0.3.5",
     "spyder-kernels>=2.5.1",
     "pytest>=7.4.3",
+    "pandas[feather]>=2.2.1",
 ]
 
 [tool.ruff]
 line-length = 88
-fix = true
+fix = false
 
 [tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "W", # pycodestyle
   "F", # Pyflakes
   "B", # flake8-bugbear
@@ -60,8 +62,8 @@
 ignore = [
     "F401", # imported but unused
     "F403", # unable to detect undefined names
     "F405", # name may be undefined, or defined from star imports
     "EM101", # Exception must not use a string literal, assign to variable first
     "TRY003", # Avoid specifying long messages outside the exception class
     "E501", # line too long
-]
+]
```

### Comparing `polars_qt-0.1.2/PKG-INFO` & `polars_qt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

