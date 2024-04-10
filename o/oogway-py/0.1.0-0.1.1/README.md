# Comparing `tmp/oogway_py-0.1.0.tar.gz` & `tmp/oogway_py-0.1.1.tar.gz`

## Comparing `oogway_py-0.1.0.tar` & `oogway_py-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 oogway_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3530 2024-04-06 03:09:33.000000 oogway_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      693 2024-04-06 03:09:33.000000 oogway_py-0.1.0/.gitignore
--rw-r--r--   0     1001      127     1063 2024-04-06 03:09:33.000000 oogway_py-0.1.0/LICENSE
--rw-r--r--   0     1001      127     1975 2024-04-06 03:09:33.000000 oogway_py-0.1.0/README.md
--rw-r--r--   0     1001      127      120 2024-04-06 03:09:33.000000 oogway_py-0.1.0/python/oogway_py/__init__.py
--rw-r--r--   0     1001      127      562 2024-04-06 03:09:33.000000 oogway_py-0.1.0/python/oogway_py/demo.py
--rw-r--r--   0     1001      127     2265 2024-04-06 03:09:33.000000 oogway_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127    55671 2024-04-06 03:09:33.000000 oogway_py-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      472 2024-04-06 03:09:33.000000 oogway_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 oogway_py-0.1.0/PKG-INFO
+-rw-r--r--   0     1001      127      135 2024-04-10 19:53:58.000000 oogway_py-0.1.1/crates/oogway/Cargo.toml
+-rw-r--r--   0     1001      127     3146 2024-04-10 19:53:58.000000 oogway_py-0.1.1/crates/oogway/src/lib.rs
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 oogway_py-0.1.1/py/Cargo.toml
+-rw-r--r--   0     1001      127     2031 2024-04-10 19:53:58.000000 oogway_py-0.1.1/py/README.md
+-rw-r--r--   0     1001      127     1108 2024-04-10 19:53:58.000000 oogway_py-0.1.1/py/example.ipynb
+-rw-r--r--   0     1001      127      120 2024-04-10 19:53:58.000000 oogway_py-0.1.1/py/python/oogway_py/__init__.py
+-rw-r--r--   0     1001      127      562 2024-04-10 19:53:58.000000 oogway_py-0.1.1/py/python/oogway_py/demo.py
+-rw-r--r--   0     1001      127     2198 2024-04-10 19:53:58.000000 oogway_py-0.1.1/py/src/lib.rs
+-rw-r--r--   0     1001      127    58985 2024-04-10 19:53:58.000000 oogway_py-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 oogway_py-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 oogway_py-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      127      562 2024-04-10 19:53:58.000000 oogway_py-0.1.1/python/oogway_py/demo.py
+-rw-r--r--   0     1001      127      120 2024-04-10 19:53:58.000000 oogway_py-0.1.1/python/oogway_py/__init__.py
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 oogway_py-0.1.1/PKG-INFO
```

### Comparing `oogway_py-0.1.0/README.md` & `oogway_py-0.1.1/py/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,12 @@
     ```
 
 That's it! Your application should now be able to allow users to converse with Master Oogway 🐢.
 
 > **Note**
 > You can run the example above from [the demo file](https://github.com/cs50victor/oogway_py/tree/main/python/oogway_py/demo.py).
 
-Run `python python/oogway_py/demo.py`
-
-## Demo 
+Run `python python/oogway_py/demo.py` or checkout the [Jupyter Notebook Example](./example.ipynb)
 
+## Demo
 
 https://github.com/cs50victor/oogway_py/assets/52110451/aa762411-a8a9-4e50-a746-8374f8455700
-
-
```

### Comparing `oogway_py-0.1.0/src/lib.rs` & `oogway_py-0.1.1/py/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::{pin::Pin, sync::Arc};
 
 use async_openai::{error::OpenAIError, types::CreateChatCompletionStreamResponse};
 use async_std::stream::IntoStream;
-use ::oogway::{ask_helper, Oogway as _Oogway};
+use ::oogway::Oogway as _Oogway;
 use futures::{Stream,StreamExt};
 use pyo3::{
     exceptions::{PyKeyError, PyStopAsyncIteration},
     pyclass, pymethods, pymodule,
     types::PyModule,
     PyObject, PyRef, PyResult, Python,
 };
@@ -36,19 +36,17 @@
     }
 
     #[setter(model_name)]
     fn set_model_name(&mut self, model_name: String) {
         self.inner.model(model_name);
     }
 
-    // &PyAny
-    pub fn ask(&mut self, _py: Python, question: String) -> PyResult<RespStream> {
-        let i = self.inner.clone();
+    pub fn ask(&self, _py: Python, question: String) -> PyResult<RespStream> {
         let stream = pyo3_asyncio::tokio::get_runtime()
-            .block_on(async { ask_helper(i, question).await.unwrap().into_stream() });
+            .block_on(async { self.inner.ask(question).await.unwrap().into_stream() });
         Ok(RespStream {
             s: Arc::new(Mutex::new(stream)),
         })
     }
 }
```

### Comparing `oogway_py-0.1.0/Cargo.lock` & `oogway_py-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "aho-corasick"
+version = "1.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "anyhow"
 version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "async-attributes"
@@ -64,17 +73,17 @@
 checksum = "6d416feee97712e43152cd42874de162b8f9b77295b1c85e5d92725cc8310bae"
 dependencies = [
  "async-trait",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.9.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10b3e585719c2358d2660232671ca8ca4ddb4be4ce8a1842d6c2dc8685303316"
+checksum = "5f98c37cf288e302c16ef6c8472aad1e034c6c84ce5ea7b8101c98eb4a802fee"
 dependencies = [
  "async-lock 3.3.0",
  "async-task",
  "concurrent-queue",
  "fastrand 2.0.2",
  "futures-lite 2.3.0",
  "slab",
@@ -159,15 +168,15 @@
 name = "async-openai"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11e97f9c5e0ee3260caee9700ba1bb61a6fdc34d2b6786a31e018c5de5198491"
 dependencies = [
  "async-convert",
  "backoff",
- "base64 0.22.0",
+ "base64",
  "bytes",
  "derive_builder",
  "futures",
  "rand",
  "reqwest",
  "reqwest-eventsource",
  "secrecy",
@@ -299,20 +308,14 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
-
-[[package]]
-name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
@@ -339,46 +342,64 @@
  "futures-lite 2.3.0",
  "piper",
  "tracing",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cli"
+version = "0.1.0"
+dependencies = [
+ "futures",
+ "oogway",
+ "tokio",
+]
+
+[[package]]
 name = "concurrent-queue"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "convert_case"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
+dependencies = [
+ "unicode-segmentation",
+]
+
+[[package]]
 name = "core-foundation"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -393,14 +414,34 @@
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
+name = "cs50victor_oogway"
+version = "0.0.0"
+dependencies = [
+ "napi",
+ "napi-build",
+ "napi-derive",
+ "oogway",
+]
+
+[[package]]
+name = "ctor"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
+dependencies = [
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
 name = "darling"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -693,17 +734,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -907,14 +948,24 @@
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "linux-raw-sys"
@@ -995,14 +1046,72 @@
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "napi"
+version = "2.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4ca998356d8ff9fba7a070dae4508a2298439c98c9f3bc9c07669538b999e8f"
+dependencies = [
+ "bitflags 2.5.0",
+ "ctor",
+ "napi-derive",
+ "napi-sys",
+ "once_cell",
+ "tokio",
+]
+
+[[package]]
+name = "napi-build"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f9130fccc5f763cf2069b34a089a18f0d0883c66aceb81f2fad541a3d823c43"
+
+[[package]]
+name = "napi-derive"
+version = "2.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b138cecf1141ae0ff5d62f4aa0e2f269aec339f66070f346ba6fb4279f1fc178"
+dependencies = [
+ "cfg-if",
+ "convert_case",
+ "napi-derive-backend",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "napi-derive-backend"
+version = "1.0.63"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ce5126b64f6ad9e28e30e6d15213dd378626b38f556454afebc42f7f02a90902"
+dependencies = [
+ "convert_case",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "semver",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "napi-sys"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2503fa6af34dc83fb74888df8b22afe933b58d37daf7d80424b1c60c68196b8b"
+dependencies = [
+ "libloading",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -1032,23 +1141,22 @@
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "oogway"
 version = "0.1.0"
-source = "git+https://github.com/cs50victor/oogway_ai?branch=main#870f87b9dc51776769db9773f244124682733add"
 dependencies = [
  "anyhow",
  "async-openai",
 ]
 
 [[package]]
 name = "oogway_py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "async-openai",
  "async-std",
  "futures",
  "oogway",
  "pyo3",
  "pyo3-asyncio",
@@ -1325,20 +1433,49 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "regex"
+version = "1.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+
+[[package]]
 name = "reqwest"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
 dependencies = [
- "base64 0.22.0",
+ "base64",
  "bytes",
  "futures-core",
  "futures-util",
  "http",
  "http-body",
  "http-body-util",
  "hyper",
@@ -1461,19 +1598,19 @@
  "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "2.1.1"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f48172685e6ff52a556baa527774f61fcaa884f59daf3375c62a3f1cd2549dab"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.21.7",
+ "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1541,14 +1678,20 @@
 checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
+name = "semver"
+version = "1.0.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+
+[[package]]
 name = "serde"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
@@ -1877,14 +2020,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
+name = "unicode-segmentation"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
+
+[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "untrusted"
```

### Comparing `oogway_py-0.1.0/PKG-INFO` & `oogway_py-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.3
 Name: oogway_py
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'tests'
 Provides-Extra: tests
-License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Python SDK for Oogway AI
 
 [![PyPI][pypi-badge]][pypi-url]
 [![Supported Versions][ver-badge]][ver-url]
@@ -65,16 +64,13 @@
     ```
 
 That's it! Your application should now be able to allow users to converse with Master Oogway 🐢.
 
 > **Note**
 > You can run the example above from [the demo file](https://github.com/cs50victor/oogway_py/tree/main/python/oogway_py/demo.py).
 
-Run `python python/oogway_py/demo.py`
-
-## Demo 
+Run `python python/oogway_py/demo.py` or checkout the [Jupyter Notebook Example](./example.ipynb)
 
+## Demo
 
 https://github.com/cs50victor/oogway_py/assets/52110451/aa762411-a8a9-4e50-a746-8374f8455700
 
-
-
```

