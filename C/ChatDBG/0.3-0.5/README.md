# Comparing `tmp/chatdbg-0.3.tar.gz` & `tmp/chatdbg-0.5.tar.gz`

## Comparing `chatdbg-0.3.tar` & `chatdbg-0.5.tar`

### file list

```diff
@@ -1,64 +1,85 @@
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chatdbg-0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chatdbg-0.3/.github/workflows/sanity.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.3/rust-support/Cargo.toml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chatdbg-0.3/rust-support/chatdbg/Cargo.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.3/rust-support/chatdbg/src/lib.rs
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 chatdbg-0.3/rust-support/chatdbg_macros/Cargo.toml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.3/rust-support/chatdbg_macros/src/lib.rs
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/__main__.py
--rw-r--r--   0        0        0     8759 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/chatdbg_gdb.py
--rw-r--r--   0        0        0    29814 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/chatdbg_lldb.py
--rw-r--r--   0        0        0    25684 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/chatdbg_pdb.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/chatdbg_utils.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/clangd_lsp_integration.py
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/assistant/assistant.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/assistant/lite_assistant.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/capture.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/chatlog.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/config.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/locals.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/prompts.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/ipdb_util/text.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/CMakeLists.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/build-chatdbg.bat
--rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/chatdbg.cpp
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/vcpkg-configuration.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/vcpkg.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/include/appendlines.hpp
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/include/getmodel.hpp
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/include/joinstrings.hpp
--rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/include/openai.hpp
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/include/wordwrap.hpp
--rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.3/src/chatdbg/windbg/nlohmann/json.hpp
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-deep-recursion.cpp
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-definition-likely.cpp
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-failed-assert.cpp
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-failed-assert.why.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-overflow.cpp
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-overflow.why.txt
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-pointers-loop.cpp
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-pointers.cpp
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-stack-overflow.cpp
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-stack-overflow.why.txt
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-use-after-free.cpp
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.3/test/test-use-after-free.why.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.3/test/testme.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/bootstrap.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/bootstrap2.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/ds101.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/marble-sample.csv
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/marbles.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/mean.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/nb.ipynb
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/requirements.txt
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.3/test/python/sample.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.3/test/rust/.gitignore
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.3/test/rust/Cargo.toml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.3/test/rust/test-failed-assert.rs
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 chatdbg-0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.3/LICENSE
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 chatdbg-0.3/README.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 chatdbg-0.3/pyproject.toml
--rw-r--r--   0        0        0    10845 2020-02-02 00:00:00.000000 chatdbg-0.3/PKG-INFO
+-rw-r--r--   0        0        0   431302 2020-02-02 00:00:00.000000 chatdbg-0.5/ChatDBG-arxiv-2403.16354.pdf
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 chatdbg-0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 chatdbg-0.5/.github/workflows/sanity.yml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/Cargo.toml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg/Cargo.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg/src/lib.rs
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg_macros/Cargo.toml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chatdbg-0.5/rust-support/chatdbg_macros/src/lib.rs
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/__main__.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_gdb.py
+-rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_lldb.py
+-rw-r--r--   0        0        0    22964 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/chatdbg_pdb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/__init__.py
+-rw-r--r--   0        0        0    12775 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/assistant.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/assistant/listeners.py
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/clangd_lsp_integration.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/code.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/dbg_dialog.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/native_util/stacks.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/chatdbg_utils.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/gdb_print_test.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/lldb_print_test.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/lldb_why.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/old_stuff/prompts.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb/prompts.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb/text.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/capture.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/locals.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/pdb_util/paths.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/config.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/history.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/instructions.txt
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/jupyter.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/log.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/markdown.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/plog.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/printer.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/prompts.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/stream.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/text.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/trim.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/util/wrap.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/CMakeLists.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/build-chatdbg.bat
+-rw-r--r--   0        0        0    11421 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/chatdbg.cpp
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/vcpkg-configuration.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/vcpkg.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/appendlines.hpp
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/getmodel.hpp
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/joinstrings.hpp
+-rw-r--r--   0        0        0    25429 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/openai.hpp
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/include/wordwrap.hpp
+-rw-r--r--   0        0        0   915040 2020-02-02 00:00:00.000000 chatdbg-0.5/src/chatdbg/windbg/nlohmann/json.hpp
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-deep-recursion.cpp
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-definition-likely.cpp
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-failed-assert.cpp
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-failed-assert.why.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-overflow.cpp
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-overflow.why.txt
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-pointers-loop.cpp
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-pointers.cpp
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-stack-overflow.cpp
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-stack-overflow.why.txt
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-use-after-free.cpp
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 chatdbg-0.5/test/test-use-after-free.why.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.5/test/testme.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/bootstrap.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/bootstrap2.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/ds101.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/marble-sample.csv
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/marbles.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/mean.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/nb.ipynb
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/requirements.txt
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 chatdbg-0.5/test/python/sample.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/.gitignore
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/Cargo.toml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 chatdbg-0.5/test/rust/test-failed-assert.rs
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 chatdbg-0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 chatdbg-0.5/LICENSE
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 chatdbg-0.5/README.md
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 chatdbg-0.5/pyproject.toml
+-rw-r--r--   0        0        0    11096 2020-02-02 00:00:00.000000 chatdbg-0.5/PKG-INFO
```

### Comparing `chatdbg-0.3/.github/workflows/release.yml` & `chatdbg-0.5/.github/workflows/release.yml`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   release:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
```

### Comparing `chatdbg-0.3/.github/workflows/sanity.yml` & `chatdbg-0.5/.github/workflows/sanity.yml`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/rust-support/chatdbg/src/lib.rs` & `chatdbg-0.5/rust-support/chatdbg/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/rust-support/chatdbg_macros/src/lib.rs` & `chatdbg-0.5/rust-support/chatdbg_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/chatdbg_pdb.py` & `chatdbg-0.5/src/chatdbg/chatdbg_pdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,162 +6,169 @@
 import pdb
 import pydoc
 import sys
 import textwrap
 import traceback
 from io import StringIO
 from pathlib import Path
-from pprint import pprint
 
 import IPython
-import llm_utils
-from traitlets import TraitError
 
-from chatdbg.ipdb_util.capture import CaptureInput
-
-from .assistant.assistant import Assistant
-from .ipdb_util.chatlog import ChatDBGLog, CopyingTextIOWrapper
-from .ipdb_util.config import Chat
-from .ipdb_util.locals import *
-from .ipdb_util.prompts import pdb_instructions
-from .ipdb_util.text import *
-
-_valid_models = [
-    "gpt-4-turbo-preview",
-    "gpt-4-0125-preview",
-    "gpt-4-1106-preview",
-    "gpt-3.5-turbo-0125",
-    "gpt-3.5-turbo-1106",
-    "gpt-4",  # no parallel calls
-    "gpt-3.5-turbo",  # no parallel calls
-]
-
-chatdbg_config: Chat = None
+from chatdbg.util.prompts import (
+    build_followup_prompt,
+    build_initial_prompt,
+    initial_instructions,
+)
+
+from chatdbg.assistant.assistant import Assistant, AssistantError
+from chatdbg.pdb_util.capture import CaptureInput, CaptureOutput
+from chatdbg.pdb_util.locals import print_locals
+from chatdbg.util.text import strip_ansi, truncate_proportionally
+from chatdbg.util.config import chatdbg_config
+from chatdbg.util.log import ChatDBGLog
+from chatdbg.util.history import CommandHistory
 
 
 def load_ipython_extension(ipython):
-    # Create an instance of your configuration class with IPython's config
     global chatdbg_config
-    from chatdbg.chatdbg_pdb import Chat, ChatDBG
+    from chatdbg.chatdbg_pdb import ChatDBG
+    from chatdbg.util.config import ChatDBGConfig, chatdbg_config
 
     ipython.InteractiveTB.debugger_cls = ChatDBG
-    chatdbg_config = Chat(config=ipython.config)
+    chatdbg_config = ChatDBGConfig(config=ipython.config)
     print("*** Loaded ChatDBG ***")
 
 
+_special_config = []
 try:
     ipython = IPython.get_ipython()
     if ipython != None:
         from IPython.terminal.interactiveshell import TerminalInteractiveShell
 
         if isinstance(ipython, TerminalInteractiveShell):
             # ipython --pdb
             from IPython.terminal.debugger import TerminalPdb
 
             ChatDBGSuper = TerminalPdb
-            _user_file_prefixes = [os.getcwd(), "<ipython"]
         else:
             # inside jupyter
             from IPython.core.debugger import InterruptiblePdb
 
             ChatDBGSuper = InterruptiblePdb
-            _user_file_prefixes = [os.getcwd(), IPython.paths.tempfile.gettempdir()]
+            _special_config += ["--format=jupyter"]
     else:
         # ichatpdb on command line
         from IPython.terminal.debugger import TerminalPdb
 
         ChatDBGSuper = TerminalPdb
-        _user_file_prefixes = [os.getcwd()]
 except NameError as e:
-    print(f"Error {e}:IPython not found. Defaulting to pdb plugin.")
+    print(f"Error {e}: IPython not found. Defaulting to pdb plugin.")
     ChatDBGSuper = pdb.Pdb
 
 
 class ChatDBG(ChatDBGSuper):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        chatdbg_config.parse_only_user_flags(_special_config)
+
         self.prompt = "(ChatDBG) "
         self._chat_prefix = "   "
-        self._text_width = 80
+        self._text_width = 120
         self._assistant = None
-        self._history = []
-        self._error_specific_prompt = ""
+        atexit.register(lambda: self._close_assistant())
 
-        global chatdbg_config
-        if chatdbg_config == None:
-            chatdbg_config = Chat()
+        self._history = CommandHistory(self.prompt)
+        self._error_message = ""
+        self._error_details = ""
 
         sys.stdin = CaptureInput(sys.stdin)
 
+        self._supports_flow = self.can_support_flow()
+
+        self.do_context(chatdbg_config.context)
+        self.rcLines += ast.literal_eval(chatdbg_config.rc_lines)
+
+        # set this to True ONLY AFTER we have had access to stack frames
+        self._show_locals = False
+
+        self._library_paths = [os.path.dirname(os.__file__)] + [
+            path
+            for path in sys.path
+            if "site-packages" in path or "dist-packages" in path
+        ]
+
+        self._log = ChatDBGLog(
+            log_filename=chatdbg_config.log,
+            config=chatdbg_config.to_json(),
+            capture_streams=True,
+        )
+
+    def _close_assistant(self):
+        if self._assistant != None:
+            self._assistant.close()
+
+    def can_support_flow(self):
         # Only use flow when we are in jupyter or using stdin in ipython.   In both
         # cases, there will be no python file at the start of argv after the
         # ipython commands.
-        self._supports_flow = chatdbg_config.show_slices
-        if self._supports_flow:
+        if chatdbg_config.show_slices:
             if ChatDBGSuper is not IPython.core.debugger.InterruptiblePdb:
                 for arg in sys.argv:
                     if arg.endswith("ipython") or arg.endswith("ipython3"):
                         continue
                     if arg.startswith("-"):
                         continue
                     if Path(arg).suffix in [".py", ".ipy"]:
-                        self._supports_flow = False
-                    break
-
-        self.do_context(chatdbg_config.context)
-        self.rcLines += ast.literal_eval(chatdbg_config.rc_lines)
-
-        # set this to True ONLY AFTER we have had stack frames
-        self._show_locals = False
-
-        self._log = ChatDBGLog(chatdbg_config)
-        atexit.register(lambda: self._log.dump())
+                        return False
+            return True
+        else:
+            return False
 
     def _is_user_frame(self, frame):
         if not self._is_user_file(frame.f_code.co_filename):
             return False
         name = frame.f_code.co_name
         return not name.startswith("<") or name == "<module>"
 
     def _is_user_file(self, file_name):
         if file_name.endswith(".pyx"):
             return False
-        if file_name == "<string>":
+        elif file_name == "<string>":
             return False
-        for prefix in _user_file_prefixes:
-            if file_name.startswith(prefix):
-                return True
-        return False
 
-    def format_stack_trace(self, context=None):
+        for path in self._library_paths:
+            if os.path.commonpath([file_name, path]) == path:
+                return False
+
+        return True
+
+    def enriched_stack_trace(self, context=None):
         old_stdout = self.stdout
         buf = StringIO()
         self.stdout = buf
         try:
             self.print_stack_trace(context)
         finally:
             self.stdout = old_stdout
-        return strip_color(buf.getvalue())
+        return strip_ansi(buf.getvalue())
 
     def interaction(self, frame, tb_or_exc):
         if isinstance(tb_or_exc, BaseException):
             exception = tb_or_exc
         elif sys.exc_info()[1] != None:
             exception = sys.exc_info()[1]
         else:
             exception = None
 
         if exception != None:
             details = "".join(
                 traceback.format_exception_only(type(exception), exception)
             ).rstrip()
-            self._error_specific_prompt = (
-                f"The program encountered the following error:\n```\n{details}\n```\n"
-            )
+            self._error_message = details
 
         super().interaction(frame, tb_or_exc)
 
     def _hide_lib_frames(self):
         # hide lib frames
         for s in self.stack:
             s[0].f_locals["__tracebackhide__"] = not self._is_user_frame(s[0])
@@ -180,93 +187,82 @@
 
         # Assume assertions are correct and the code leading to them is not!
         if self.curframe.f_lineno != None:
             current_line = linecache.getline(
                 self.curframe.f_code.co_filename, self.curframe.f_lineno
             )
             if current_line.strip().startswith("assert"):
-                self._error_specific_prompt += f"The code `{current_line.strip()}` is correct and MUST remain unchanged in your fix.\n"
+                self._error_details = f"The code `{current_line.strip()}` is correct and MUST remain unchanged in your fix."
 
     def execRcLines(self):
-
         # do before running rclines -- our stack should be set up by now.
-
         if not chatdbg_config.show_libs:
             self._hide_lib_frames()
-        self._error_stack_trace = f"The program has the following stack trace:\n```\n{self.format_stack_trace()}\n```\n"
 
         # finally safe to enable this.
         self._show_locals = chatdbg_config.show_locals and not chatdbg_config.show_libs
 
         return super().execRcLines()
 
     def onecmd(self, line: str) -> bool:
         """
         Override to stash the results in our history.
         """
         if not line:
             # blank -- let super call back to into onecmd
             return super().onecmd(line)
         else:
-            hist_file = CopyingTextIOWrapper(self.stdout)
+            hist_file = CaptureOutput(self.stdout)
             self.stdout = hist_file
             try:
-                self.was_chat = False
+                self.was_chat_or_renew = False
                 return super().onecmd(line)
             finally:
                 self.stdout = hist_file.getfile()
-                if not line.startswith("config") and not line.startswith("mark"):
-                    output = strip_color(hist_file.getvalue())
-                    if line not in ["quit", "EOF"]:
-                        self._log.user_command(line, output)
-                    if (
-                        line not in ["hist", "test_prompt", "c", "continue"]
-                        and not self.was_chat
-                    ):
-                        self._history += [(line, output)]
+                output = strip_ansi(hist_file.getvalue())
+                if not self.was_chat_or_renew:
+                    self._log.on_function_call(line, output)
+                    if line.split()[0] not in [
+                        "hist",
+                        "test_prompt",
+                        "c",
+                        "cont",
+                        "continue",
+                        "config",
+                    ]:
+                        self._history.append(line, output)
 
     def message(self, msg) -> None:
         """
         Override to remove tabs for messages so we can indent them.
         """
         return super().message(str(msg).expandtabs())
 
     def error(self, msg) -> None:
         """
         Override to remove tabs for messages so we can indent them.
         """
         return super().error(str(msg).expandtabs())
-        # return super().error('If the name is undefined, be sure you are in the right frame.  Use up and down to do that, and then print the variable again'.expandtabs())
 
     def _capture_onecmd(self, line):
         """
         Run one Pdb command, but capture and return stdout.
         """
         stdout = self.stdout
         lastcmd = self.lastcmd
         try:
             self.stdout = StringIO()
             super().onecmd(line)
             result = self.stdout.getvalue().rstrip()
+            result = strip_ansi(result)
             return result
         finally:
             self.stdout = stdout
             self.lastcmd = lastcmd
 
-    def _format_history_entry(self, entry, indent=""):
-        line, output = entry
-        if output:
-            entry = f"{self.prompt}{line}\n{output}"
-        else:
-            entry = f"{self.prompt}{line}"
-        return textwrap.indent(entry, indent, lambda _: True)
-
-    def _clear_history(self):
-        self._history = []
-
     def default(self, line):
         if line[:1] == "!":
             super().default(line)
         else:
             if line[:1] == ":":
                 line = line[1:].strip()
             self.do_chat(line)
@@ -277,17 +273,15 @@
             line = super(IPython.core.debugger.Pdb, self).precmd(line)
         return line
 
     def do_hist(self, arg):
         """hist
         Print the history of user-issued commands since the last chat.
         """
-        entry_strs = [self._format_history_entry(x) for x in self._history]
-        history_str = "\n".join(entry_strs)
-        self.message(history_str)
+        self.message(self._history)
 
     def do_pydoc(self, arg):
         """pydoc name
         Print the pydoc string for a name.
         """
         try:
             obj = self._getval(arg)
@@ -314,17 +308,15 @@
                 except:
                     # fail silently, try the next name
                     pass
 
             # didn't find anything
             if obj == None:
                 self.message(f"No name `{arg}` is visible in the current frame.")
-                return
-
-            if self._is_user_file(inspect.getfile(obj)):
+            elif self._is_user_file(inspect.getfile(obj)):
                 self.do_source(x)
             else:
                 self.do_pydoc(x)
                 self.message(
                     f"You MUST assume that `{x}` is specified and implemented correctly."
                 )
         except OSError:
@@ -335,14 +327,19 @@
         except Exception:
             self.do_pydoc(x)
             self.message(
                 f"You MUST assume that `{x}` is specified and implemented correctly."
             )
 
     def do_slice(self, arg):
+        """
+        slice
+        Print the backwards slice for a variable used in the current cell but
+        defined in an earlier cell.  [interactive IPython / Jupyter only]
+        """
         if not self._supports_flow:
             self.message("*** `slice` is only supported in Jupyter notebooks")
             return
 
         try:
             from ipyflow import cells, singletons
             from ipyflow.models import statements
@@ -357,19 +354,14 @@
                     cell = cells().at_counter(pos)
                     # print(cell.used_symbols)
                     _x = next((x for x in cell.used_symbols if x.name == arg), None)
                 if _x != None:
                     break
                 index -= 1
             if _x != None:
-                # print('found it')
-                # print(_x)
-                # print(_x.__dict__)
-                # print(_x._get_timestamps_for_version(version=-1))
-                # print(code(_x))
                 time_stamps = _x._get_timestamps_for_version(version=-1)
                 time_stamps = [ts for ts in time_stamps if ts.cell_num > -1]
                 result = str(
                     statements().format_multi_slice(
                         time_stamps, blacken=True, format_type=None
                     )
                 ).rstrip()
@@ -393,17 +385,15 @@
         self.message(result)
 
     def do_test_prompt(self, arg):
         """test_prompt
         [For debugging] Prints the prompts to be sent to the assistant.
         """
         self.message("Instructions:")
-        self.message(
-            pdb_instructions(self._supports_flow, chatdbg_config.take_the_wheel)
-        )
+        self.message(self._initial_prompt_instructions())
         self.message("-" * 80)
         self.message("Prompt:")
         self.message(self._build_prompt(arg, False))
 
     def _hidden_predicate(self, frame):
         """
         Given a frame return whether it it should be hidden or not by IPython.
@@ -430,15 +420,15 @@
             frame_locals = self._get_frame_locals(frame)
             if "__tracebackhide__" not in frame_locals:
                 return False
             return frame_locals["__tracebackhide__"]
         return False
 
     def print_stack_trace(self, context=None, locals=None):
-        # override to print the skips into stdout...
+        # override to print the skips into stdout instead of stderr...
         Colors = self.color_scheme_table.active_colors
         ColorsNormal = Colors.Normal
         if context is None:
             context = self.context
         try:
             context = int(context)
             if context <= 0:
@@ -461,262 +451,218 @@
                     print(
                         f"{Colors.excName}    [... skipping {skipped} hidden frame(s)]{ColorsNormal}\n",
                         file=self.stdout,
                     )
                     skipped = 0
                 self.print_stack_entry(frame_lineno, context=context)
                 if locals:
-                    self._print_locals(frame_lineno[0])
+                    print_locals(self.stdout, frame_lineno[0])
             if skipped:
                 print(
                     f"{Colors.excName}    [... skipping {skipped} hidden frame(s)]{ColorsNormal}\n",
                     file=self.stdout,
                 )
         except KeyboardInterrupt:
             pass
 
-    def _print_locals(self, frame):
-        locals = frame.f_locals
-        in_global_scope = locals is frame.f_globals
-        defined_locals = extract_locals(frame)
-        # Unclear benefit: possibly some benefit w/ stack only runs, but large context...
-        # if in_global_scope and "In" in locals:  # in notebook
-        #     defined_locals = defined_locals | extract_nb_globals(locals)
-        if len(defined_locals) > 0:
-            if in_global_scope:
-                print(f"    Global variables:", file=self.stdout)
-            else:
-                print(f"    Variables in this frame:", file=self.stdout)
-            for name in sorted(defined_locals):
-                value = locals[name]
-                t = type(value).__name__
-                prefix = f"      {name}: {t} = "
-                rep = format_limited(value, limit=20).split("\n")
-                if len(rep) > 1:
-                    rep = (
-                        prefix
-                        + rep[0]
-                        + "\n"
-                        + textwrap.indent("\n".join(rep[1:]), prefix=" " * len(prefix))
-                    )
-                else:
-                    rep = prefix + rep[0]
-                print(rep, file=self.stdout)
-            print(file=self.stdout)
-
-    def _stack_prompt(self):
+    def _prompt_stack(self):
         stdout = self.stdout
         buffer = StringIO()
         self.stdout = buffer
         try:
             self.print_stack_trace(context=1, locals=False)
             stack_frames = buffer.getvalue()
             stack_frames = "\n".join(
                 line for line in stack_frames.splitlines() if line.strip()
             )
             stack = (
                 textwrap.dedent(
-                    f"""
+                    f"""\
                 This is the current stack.  The current frame is indicated by 
                 an arrow '>' at the start of the line.
                 ```"""
                 )
                 + f"\n{stack_frames}\n```"
             )
             return stack
         finally:
             self.stdout = stdout
 
-    def _build_prompt(self, arg, conversing):
-        prompt = ""
+    def _initial_prompt_instructions(self):
+        functions = self._supported_functions()
+        return initial_instructions(functions)
 
-        if not conversing:
-            stack_dump = f"The program has this stack trace:\n```\n{self.format_stack_trace()}\n```\n\n"
-            prompt = "\n" + stack_dump + self._error_specific_prompt
-            if len(sys.argv) > 1:
-                prompt += f"\nThese were the command line options:\n```\n{' '.join(sys.argv)}\n```\n"
-            input = sys.stdin.get_captured_input()
-            if len(input) > 0:
-                prompt += f"\nThis was the program's input :\n```\n{input}```\n"
-
-        if len(self._history) > 0:
-            hist = textwrap.indent(self._capture_onecmd("hist"), "")
-            self._clear_history()
-            hist = f"\nThis is the history of some pdb commands I ran and the results.\n```\n{hist}\n```\n"
-            prompt += hist
+    def _initial_prompt_enchriched_stack_trace(self):
+        return self.enriched_stack_trace()
+
+    def _initial_prompt_error_message(self):
+        return self._error_message
+
+    def _initial_prompt_error_details(self):
+        return self._error_details
 
-        if arg == "why":
-            arg = "Explain the root cause of the error."
+    def _initial_prompt_command_line(self):
+        return " ".join(sys.argv)
 
-        stack = self._stack_prompt()
-        prompt += stack + "\n" + arg
+    def _initial_prompt_input(self):
+        return sys.stdin.get_captured_input()
 
-        return prompt
+    def _prompt_history(self):
+        return str(self._history)
+
+    def _build_prompt(self, arg, conversing):
+        if not conversing:
+            return build_initial_prompt(
+                self._initial_prompt_enchriched_stack_trace(),
+                self._initial_prompt_error_message(),
+                self._initial_prompt_error_details(),
+                self._initial_prompt_command_line(),
+                self._initial_prompt_input(),
+                self._prompt_history(),
+                None,
+                arg,
+            )
+        else:
+            return build_followup_prompt(
+                self._prompt_history(), self._prompt_stack(), arg
+            )
 
     def do_chat(self, arg):
-        """chat/:
+        """chat
         Send a chat message.
         """
-        self.was_chat = True
+        self.was_chat_or_renew = True
 
         full_prompt = self._build_prompt(arg, self._assistant != None)
+        full_prompt = strip_ansi(full_prompt)
+        full_prompt = truncate_proportionally(full_prompt)
 
-        if self._assistant == None:
-            self._make_assistant()
-
-        def client_print(line=""):
-            line = llm_utils.word_wrap_except_code_blocks(line, self._text_width - 10)
-            self._log.message(line)
-            line = textwrap.indent(line, self._chat_prefix, lambda _: True)
-            print(line, file=self.stdout, flush=True)
+        self._history.clear()
 
-        full_prompt = strip_color(full_prompt)
-        full_prompt = truncate_proportionally(full_prompt)
+        try:
+            if self._assistant == None:
+                self._make_assistant()
 
-        self._log.push_chat(arg, full_prompt)
-        stats = self._assistant.run(full_prompt, client_print)
-        self._log.pop_chat(stats)
-
-    def do_mark(self, arg):
-        marks = ["Full", "Partial", "Wrong", "None", "?"]
-        if arg == None or arg == "":
-            arg = input(f"mark? (one of {marks}): ")
-            while arg not in marks:
-                arg = input(f"mark? (one of {marks}): ")
-        if arg not in marks:
-            self.error(
-                f"answer must be in { ['Full', 'Partial', 'Wrong', '?', 'None'] }"
-            )
-        else:
-            self._log.add_mark(arg)
+            stats = self._assistant.query(full_prompt, user_text=arg)
+            self.message(stats["message"])
+        except AssistantError as e:
+            for line in str(e).split("\n"):
+                self.error(line)
+
+    def do_renew(self, arg):
+        """renew
+        End the current chat dialog and prepare to start a new one.
+        """
+        if self._assistant != None:
+            self._assistant.close()
+            self._assistant = None
+        self.was_chat_or_renew = True
+        self.message(f"Ready to start a new dialog.")
 
     def do_config(self, arg):
+        """
+        config
+        Print out the ChatDBG config options.
+        """
         args = arg.split()
-        if len(args) == 0:
-            pprint(chatdbg_config.to_json(), sort_dicts=True, stream=self.stdout)
-            return
-
-        if len(args) != 2:
-            self.error("Usage: config <option> <value>")
-            self.error("   or: config")
-            return
+        message = chatdbg_config.parse_only_user_flags(args)
+        self.message(message)
 
-        option, value = args
-        try:
-            chatdbg_config.set_trait(option, value)
-            pprint(chatdbg_config.to_json(), sort_dicts=True, stream=self.stdout)
-        except TraitError as e:
-            self.error(f"{e}")
+    def _supported_functions(self):
+        if chatdbg_config.take_the_wheel:
+            functions = [self.debug, self.info]
+            if self._supports_flow:
+                functions += [self.slice]
+        else:
+            functions = []
 
-            # Get the documentation and source code (if available) for any function or method visible in the current frame.  The argument to info can be the name of the function or an expression of the form `obj.method_name`  to see the information for the method_name method of object obj.",
+        return functions
 
     def _make_assistant(self):
-        def info(value):
-            """
-            {
-                "name": "info",
-                "description": "Get the documentation and source code for a reference, which may be a variable, function, method reference, field reference, or dotted reference visible in the current frame.  Examples include n, e.n where e is an expression, and t.n where t is a type.",
-                "parameters": {
-                    "type": "object",
-                    "properties": {
-                        "value": {
-                            "type": "string",
-                            "description": "The reference to get the information for."
-                        }
-                    },
-                    "required": [ "value"  ]
-                }
-            }
-            """
-            command = f"info {value}"
-            result = self._capture_onecmd(command)
-            self.message(
-                self._format_history_entry((command, result), indent=self._chat_prefix)
-            )
-            result = strip_color(result)
-            self._log.function(command, result)
-            return truncate_proportionally(result, top_proportion=1)
-
-        def debug(command):
-            """
-            {
-                "name": "debug",
-                "description": "Run a pdb command and get the response.",
-                "parameters": {
-                    "type": "object",
-                    "properties": {
-                        "command": {
-                            "type": "string",
-                            "description": "The pdb command to run."
-                        }
-                    },
-                    "required": [ "command" ]
-                }
-            }
-            """
-            cmd = command if command != "list" else "ll"
-            result = self._capture_onecmd(cmd)
-
-            self.message(
-                self._format_history_entry((command, result), indent=self._chat_prefix)
-            )
-
-            result = strip_color(result)
-            self._log.function(command, result)
-
-            # help the LLM know where it is...
-            result += strip_color(self._stack_prompt())
-            return truncate_proportionally(result, maxlen=8000, top_proportion=0.9)
-
-        def slice(name):
-            """
-            {
-                "name": "slice",
-                "description": "Return the code to compute a global variable used in the current frame",
-                "parameters": {
-                    "type": "object",
-                    "properties": {
-                        "name": {
-                            "type": "string",
-                            "description": "The variable to look at."
-                        }
-                    },
-                    "required": [ "name"  ]
-                }
-            }
-
-            """
-            command = f"slice {name}"
-            result = self._capture_onecmd(command)
-            self.message(
-                self._format_history_entry((command, result), indent=self._chat_prefix)
-            )
-            result = strip_color(result)
-            self._log.function(command, result)
-            return truncate_proportionally(result, top_proportion=0.5)
-
-        self._clear_history()
-        instruction_prompt = pdb_instructions(
-            self._supports_flow, chatdbg_config.take_the_wheel
-        )
-
-        self._log.instructions(instruction_prompt)
-
-        if not chatdbg_config.model in _valid_models:
-            print(
-                f"'{chatdbg_config.model}' is not a valid OpenAI model.  Choose from: {_valid_models}."
-            )
-            sys.exit(0)
+        instruction_prompt = self._initial_prompt_instructions()
+        functions = self._supported_functions()
 
         self._assistant = Assistant(
-            "ChatDBG",
             instruction_prompt,
             model=chatdbg_config.model,
             debug=chatdbg_config.debug,
+            functions=functions,
+            stream=not chatdbg_config.no_stream,
+            max_call_response_tokens=8192,
+            listeners=[
+                chatdbg_config.make_printer(
+                    self.stdout, self.prompt, self._chat_prefix, self._text_width
+                ),
+                self._log,
+            ],
         )
 
-        if chatdbg_config.take_the_wheel:
-            self._assistant.add_function(debug)
-            self._assistant.add_function(info)
+    ### Callbacks for LLM
 
-            if self._supports_flow:
-                self._assistant.add_function(slice)
+    def info(self, value):
+        """
+        {
+            "name": "info",
+            "description": "Call the `info` function to get the documentation and source code for any variable, function, package, class, method reference, field reference, or dotted reference visible in the current frame.  Examples include: n, e.n where e is an expression, and t.n where t is a type. Unless it is from a common, widely-used library, you MUST call `info` exactly once on any symbol that is referenced in code leading up to the error.",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "value": {
+                        "type": "string",
+                        "description": "The reference to get the information for."
+                    }
+                },
+                "required": [ "value"  ]
+            }
+        }
+        """
+        command = f"info {value}"
+        result = self._capture_onecmd(command)
+        return command, truncate_proportionally(result, top_proportion=1)
+
+    def debug(self, command):
+        """
+        {
+            "name": "debug",
+            "description": "Call the `debug` function to run Pdb debugger commands on the stopped program. You may call the `pdb` function to run the following commands: `bt`, `up`, `down`, `p expression`, `list`.  Call `debug` to print any variable value or expression that you believe may contribute to the error.",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "command": {
+                        "type": "string",
+                        "description": "The pdb command to run."
+                    }
+                },
+                "required": [ "command" ]
+            }
+        }
+        """
+        cmd = command if command != "list" else "ll"
+        # old_curframe = self.curframe
+        result = self._capture_onecmd(cmd)
+
+        # help the LLM know where it is...
+        # if old_curframe != self.curframe:
+        #     result += strip_color(self._stack_prompt())
+
+        return command, truncate_proportionally(result, maxlen=8000, top_proportion=0.9)
+
+    def slice(self, name):
+        """
+        {
+            "name": "slice",
+            "description": "Call the `slice` function to get the code used to produce the value currently stored a variable.  You MUST call `slice` exactly once on any variable used but not defined in the current frame's code.",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "name": {
+                        "type": "string",
+                        "description": "The variable to look at."
+                    }
+                },
+                "required": [ "name"  ]
+            }
+        }
+        """
+        command = f"slice {name}"
+        result = self._capture_onecmd(command)
+        return command, truncate_proportionally(result, top_proportion=0.5)
```

### Comparing `chatdbg-0.3/src/chatdbg/chatdbg_utils.py` & `chatdbg-0.5/src/chatdbg/old_stuff/chatdbg_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import argparse
-import textwrap
-import time
-from typing import Any, Callable, List, Optional, Tuple
-
-import llm_utils
-import openai
-from rich.console import Console
-
-
-class RichArgParser(argparse.ArgumentParser):
-    def __init__(self, *args: Any, **kwargs: Any):
-        self.console = Console(highlight=False)
-        super().__init__(*args, **kwargs)
-
-    def _print_message(self, message: Optional[str], file: Any = None) -> None:
-        if message:
-            self.console.print(message)
-
-
-class ChatDBGArgumentFormatter(argparse.HelpFormatter):
-    # RawDescriptionHelpFormatter.
-    def _fill_text(self, text, width, indent):
-        return "".join(indent + line for line in text.splitlines(keepends=True))
-
-    # RawTextHelpFormatter.
-    def _split_lines(self, text, width):
-        return text.splitlines()
-
-    # ArgumentDefaultsHelpFormatter.
-    # Ignore if help message is multiline.
-    def _get_help_string(self, action):
-        help = action.help
-        if "\n" not in help and "%(default)" not in action.help:
-            if action.default is not argparse.SUPPRESS:
-                defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
-                if action.option_strings or action.nargs in defaulting_nargs:
-                    help += " (default: %(default)s)"
-        return help
-
-
-def parse_known_args(argv: List[str]) -> Tuple[argparse.Namespace, List[str]]:
-    description = textwrap.dedent(
-        rf"""
-            [b]ChatDBG[/b]: A Python debugger that uses AI to tell you `why`.
-            [blue][link=https://github.com/plasma-umass/ChatDBG]https://github.com/plasma-umass/ChatDBG[/link][/blue]
-        """
-    ).strip()
-    parser = RichArgParser(
-        prog="chatdbg",
-        usage=argparse.SUPPRESS,
-        description=description,
-        formatter_class=ChatDBGArgumentFormatter,
-    )
-    parser.add_argument(
-        "--llm",
-        type=str,
-        default="gpt-4-turbo-preview",
-        help="the language model to use, e.g., 'gpt-3.5-turbo' or 'gpt-4'",
-    )
-    parser.add_argument(
-        "--debug",
-        action="store_true",
-        help="when enabled, only print prompt and exit with `why`, and output to a log file with `chat`",
-    )
-    parser.add_argument(
-        "--tool-call-max-result-tokens",
-        default=512,  # Arbitrary.
-        help="the maximum number of tokens to send in any tool call response",
-    )
-    parser.add_argument(
-        "--fresh",
-        action="store_true",
-        default=False,
-        help="in `chat` mode, reset the chat history to start a new conversation",
-    )
-    parser.add_argument(
-        "--timeout",
-        type=int,
-        default=60,
-        help="the timeout for API calls in seconds",
-    )
-
-    return parser.parse_known_args(argv)
-
-
-def explain(
-    source_code: str,
-    traceback: str,
-    exception: str,
-    args: argparse.Namespace,
-    append_message: Callable[[str], None] = print,
-    append_warning: Callable[[str], None] = print,
-    set_error: Callable[[str], None] = print,
-) -> None:
-    user_prompt = f"""
-Explain what the root cause of this error is, given the following source code
-context for each stack frame and a traceback, and propose a fix. In your
-response, never refer to the frames given below (as in, 'frame 0'). Instead,
-always refer only to specific lines and filenames of source code.
-
-Source code for each stack frame:
-```
-{source_code}
-```
-
-Traceback:
-{traceback}
-
-Stop reason: {exception}
-    """.strip()
-
-    input_tokens = llm_utils.count_tokens(args.llm, user_prompt)
-
-    if args.debug:
-        append_message(f"{user_prompt}\n\nTotal input tokens: {input_tokens}.")
-        return
-
-    start = time.time()
-
-    try:
-        client = openai.OpenAI(timeout=args.timeout)
-    except openai.OpenAIError:
-        append_warning("you need an OpenAI key to use this tool.")
-        append_warning("You can get a key here: https://platform.openai.com/api-keys.")
-        append_warning("set the environment variable OPENAI_API_KEY to your key value.")
-        return
-
-    try:
-        completion = client.chat.completions.create(
-            model=args.llm, messages=[{"role": "user", "content": user_prompt}]
-        )
-    except openai.NotFoundError:
-        set_error(f"'{args.llm}' does not exist or you do not have access to it.")
-        return
-    except openai.RateLimitError:
-        set_error("you have exceeded a rate limit or have no remaining funds.")
-        return
-    except openai.APITimeoutError:
-        set_error("the OpenAI API timed out.")
-        return
-
-    text = completion.choices[0].message.content
-    elapsed = time.time() - start
-    input_tokens = completion.usage.prompt_tokens
-    output_tokens = completion.usage.completion_tokens
-    cost = llm_utils.calculate_cost(input_tokens, output_tokens, args.llm)
-
-    append_message(
-        llm_utils.word_wrap_except_code_blocks(text)
-        + "\n\n"
-        + f"Elapsed time: {elapsed:.2f} seconds"
-        + "\n"
-        + f"Total cost: {cost:.2f}$"
-    )
+# import argparse
+# import textwrap
+# import time
+# from typing import Any, Callable, List, Optional, Tuple
+
+# import llm_utils
+# import openai
+# from rich.console import Console
+
+
+# class RichArgParser(argparse.ArgumentParser):
+#     def __init__(self, *args: Any, **kwargs: Any):
+#         self.console = Console(highlight=False)
+#         super().__init__(*args, **kwargs)
+
+#     def _print_message(self, message: Optional[str], file: Any = None) -> None:
+#         if message:
+#             self.console.print(message)
+
+
+# class ChatDBGArgumentFormatter(argparse.HelpFormatter):
+#     # RawDescriptionHelpFormatter.
+#     def _fill_text(self, text, width, indent):
+#         return "".join(indent + line for line in text.splitlines(keepends=True))
+
+#     # RawTextHelpFormatter.
+#     def _split_lines(self, text, width):
+#         return text.splitlines()
+
+#     # ArgumentDefaultsHelpFormatter.
+#     # Ignore if help message is multiline.
+#     def _get_help_string(self, action):
+#         help = action.help
+#         if "\n" not in help and "%(default)" not in action.help:
+#             if action.default is not argparse.SUPPRESS:
+#                 defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
+#                 if action.option_strings or action.nargs in defaulting_nargs:
+#                     help += " (default: %(default)s)"
+#         return help
+
+
+# def parse_known_args(argv: List[str]) -> Tuple[argparse.Namespace, List[str]]:
+#     description = textwrap.dedent(
+#         rf"""
+#             [b]ChatDBG[/b]: A Python debugger that uses AI to tell you `why`.
+#             [blue][link=https://github.com/plasma-umass/ChatDBG]https://github.com/plasma-umass/ChatDBG[/link][/blue]
+#         """
+#     ).strip()
+#     parser = RichArgParser(
+#         prog="chatdbg",
+#         usage=argparse.SUPPRESS,
+#         description=description,
+#         formatter_class=ChatDBGArgumentFormatter,
+#     )
+#     parser.add_argument(
+#         "--llm",
+#         type=str,
+#         default="gpt-4-turbo-preview",
+#         help="the language model to use, e.g., 'gpt-3.5-turbo' or 'gpt-4'",
+#     )
+#     parser.add_argument(
+#         "--debug",
+#         action="store_true",
+#         help="when enabled, only print prompt and exit with `why`, and output to a log file with `chat`",
+#     )
+#     parser.add_argument(
+#         "--tool-call-max-result-tokens",
+#         default=512,  # Arbitrary.
+#         help="the maximum number of tokens to send in any tool call response",
+#     )
+#     parser.add_argument(
+#         "--fresh",
+#         action="store_true",
+#         default=False,
+#         help="in `chat` mode, reset the chat history to start a new conversation",
+#     )
+#     parser.add_argument(
+#         "--timeout",
+#         type=int,
+#         default=60,
+#         help="the timeout for API calls in seconds",
+#     )
+
+#     return parser.parse_known_args(argv)
+
+
+# def explain(
+#     source_code: str,
+#     traceback: str,
+#     exception: str,
+#     args: argparse.Namespace,
+#     append_message: Callable[[str], None] = print,
+#     append_warning: Callable[[str], None] = print,
+#     set_error: Callable[[str], None] = print,
+# ) -> None:
+#     user_prompt = f"""
+# Explain what the root cause of this error is, given the following source code
+# context for each stack frame and a traceback, and propose a fix. In your
+# response, never refer to the frames given below (as in, 'frame 0'). Instead,
+# always refer only to specific lines and filenames of source code.
+
+# Source code for each stack frame:
+# ```
+# {source_code}
+# ```
+
+# Traceback:
+# {traceback}
+
+# Stop reason: {exception}
+#     """.strip()
+
+#     input_tokens = llm_utils.count_tokens(args.llm, user_prompt)
+
+#     if args.debug:
+#         append_message(f"{user_prompt}\n\nTotal input tokens: {input_tokens}.")
+#         return
+
+#     start = time.time()
+
+#     try:
+#         client = openai.OpenAI(timeout=args.timeout)
+#     except openai.OpenAIError:
+#         append_warning("you need an OpenAI key to use this tool.")
+#         append_warning("You can get a key here: https://platform.openai.com/api-keys.")
+#         append_warning("set the environment variable OPENAI_API_KEY to your key value.")
+#         return
+
+#     try:
+#         completion = client.chat.completions.create(
+#             model=args.llm, messages=[{"role": "user", "content": user_prompt}]
+#         )
+#     except openai.NotFoundError:
+#         set_error(f"'{args.llm}' does not exist or you do not have access to it.")
+#         return
+#     except openai.RateLimitError:
+#         set_error("you have exceeded a rate limit or have no remaining funds.")
+#         return
+#     except openai.APITimeoutError:
+#         set_error("the OpenAI API timed out.")
+#         return
+
+#     text = completion.choices[0].message.content
+#     elapsed = time.time() - start
+#     input_tokens = completion.usage.prompt_tokens
+#     output_tokens = completion.usage.completion_tokens
+#     cost = llm_utils.calculate_cost(input_tokens, output_tokens, args.llm)
+
+#     append_message(
+#         llm_utils.word_wrap_except_code_blocks(text)
+#         + "\n\n"
+#         + f"Elapsed time: {elapsed:.2f} seconds"
+#         + "\n"
+#         + f"Total cost: {cost:.2f}$"
+#     )
```

### Comparing `chatdbg-0.3/src/chatdbg/ipdb_util/chatlog.py` & `chatdbg-0.5/src/chatdbg/util/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,153 @@
 import sys
 import uuid
 from datetime import datetime
-from io import StringIO
 
 import yaml
 
-from .config import Chat
+from ..assistant.listeners import BaseAssistantListener
+from ..pdb_util.capture import CaptureOutput
+from .wrap import word_wrap_except_code_blocks
 
 
-class CopyingTextIOWrapper:
-    """
-    File wrapper that will stash a copy of everything written.
-    """
-
-    def __init__(self, file):
-        self.file = file
-        self.buffer = StringIO()
-
-    def write(self, data):
-        self.buffer.write(data)
-        return self.file.write(data)
-
-    def getvalue(self):
-        return self.buffer.getvalue()
-
-    def getfile(self):
-        return self.file
-
-    def __getattr__(self, attr):
-        # Delegate attribute access to the file object
-        return getattr(self.file, attr)
+class ChatDBGLog(BaseAssistantListener):
+
+    def __init__(self, log_filename, config, capture_streams=True):
+        self._log_filename = log_filename
+        self.config = config
+        if capture_streams:
+            self._stdout_wrapper = CaptureOutput(sys.stdout)
+            self._stderr_wrapper = CaptureOutput(sys.stderr)
+            sys.stdout = self._stdout_wrapper
+            sys.stderr = self._stdout_wrapper
+        else:
+            self._stderr_wrapper = None
+            self._stderr_wrapper = None
 
+        self._log = self._make_log()
+        self._current_chat = None
 
-class ChatDBGLog:
-    def __init__(self, config: Chat):
-        self.steps = []
-        self.meta = {
-            "time": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+    def _make_log(self):
+        meta = {
+            "time": datetime.now(),
             "command_line": " ".join(sys.argv),
             "uid": str(uuid.uuid4()),
-            "config": config.to_json(),
-            "mark": "?",
+            "config": self.config,
         }
-        self.log = config.log
-        self._instructions = ""
-        self.stdout_wrapper = CopyingTextIOWrapper(sys.stdout)
-        self.stderr_wrapper = CopyingTextIOWrapper(sys.stderr)
-        sys.stdout = self.stdout_wrapper
-        sys.stderr = self.stdout_wrapper
-        self.chat_step = None
-        self.mark = "?"
-
-    def add_mark(self, value):
-        if value not in ["Fix", "Partial", "None", "?"]:
-            print(f"answer must be in { ['Fix', 'Partial', 'None', '?'] }")
-        else:
-            self.meta["mark"] = value
-
-    def total(self, key):
-        return sum(
-            [x["stats"][key] for x in self.steps if x["output"]["type"] == "chat"]
-        )
-
-    def dump(self):
-        self.meta["total_tokens"] = self.total("tokens")
-        self.meta["total_time"] = self.total("time")
-        self.meta["total_cost"] = self.total("cost")
-
-        full_json = [
-            {
-                "meta": self.meta,
-                "steps": self.steps,
-                "instructions": self._instructions,
-                "stdout": self.stdout_wrapper.getvalue(),
-                "stderr": self.stderr_wrapper.getvalue(),
-            }
-        ]
-
-        print(f"*** Write ChatDBG log to {self.log}")
-        with open(self.log, "a") as file:
-            yaml.dump(full_json, file, default_flow_style=False)
-
-    def instructions(self, instructions):
-        self._instructions = instructions
-
-    def user_command(self, line, output):
-        if self.chat_step != None:
-            x = self.chat_step
-            self.chat_step = None
-        else:
-            x = {"input": line, "output": {"type": "text", "output": output}}
-        self.steps.append(x)
-
-    def push_chat(self, line, full_prompt):
-        self.chat_step = {
-            "input": line,
-            "full_prompt": full_prompt,
-            "output": {"type": "chat", "outputs": []},
-            "stats": {"tokens": 0, "cost": 0, "time": 0},
+        return {
+            "steps": [],
+            "meta": meta,
+            "instructions": None,
+            "stdout": (
+                None
+                if self._stderr_wrapper == None
+                else self._stdout_wrapper.getvalue()
+            ),
+            "stderr": (
+                None
+                if self._stderr_wrapper == None
+                else self._stderr_wrapper.getvalue()
+            ),
         }
 
-    def pop_chat(self, stats):
-        self.chat_step["stats"] = stats
-
-    def message(self, text):
-        self.chat_step["output"]["outputs"].append({"type": "text", "output": text})
+    def _dump(self):
+        log = self._log
 
-    def function(self, line, output):
-        x = {
-            "type": "call",
-            "input": line,
-            "output": {"type": "text", "output": output},
+        def total(key):
+            return sum(
+                x["stats"][key]
+                for x in log["steps"]
+                if x["output"]["type"] == "chat" and "stats" in x["output"]
+            )
+
+        log["meta"]["total_tokens"] = total("tokens")
+        log["meta"]["total_time"] = total("time")
+        log["meta"]["total_cost"] = total("cost")
+
+        print(f"*** Writing ChatDBG dialog log to {self._log_filename}")
+
+        with open(self._log_filename, "a") as file:
+
+            def literal_presenter(dumper, data):
+                if "\n" in data:
+                    return dumper.represent_scalar(
+                        "tag:yaml.org,2002:str", data, style="|"
+                    )
+                else:
+                    return dumper.represent_scalar("tag:yaml.org,2002:str", data)
+
+            yaml.add_representer(str, literal_presenter)
+            yaml.dump([log], file, default_flow_style=False, indent=2)
+
+    def on_begin_dialog(self, instructions):
+        log = self._log
+        assert log != None
+        log["instructions"] = instructions
+
+    def on_end_dialog(self):
+        if self._log != None:
+            self._dump()
+        self._log = self._make_log()
+
+    def on_begin_query(self, prompt, extra):
+        log = self._log
+        assert log != None
+        assert self._current_chat == None
+        self._current_chat = {
+            "input": extra,
+            "prompt": prompt,
+            "output": {"type": "chat", "outputs": []},
         }
-        self.chat_step["output"]["outputs"].append(x)
-
 
-# Custom representer for literal scalar representation
-def literal_presenter(dumper, data):
-    if "\n" in data:
-        return dumper.represent_scalar("tag:yaml.org,2002:str", data, style="|")
-    return dumper.represent_scalar("tag:yaml.org,2002:str", data)
-
-
-yaml.add_representer(str, literal_presenter)
+    def on_end_query(self, stats):
+        log = self._log
+        assert log != None
+        assert self._current_chat != None
+        log["steps"] += [self._current_chat]
+        log["stats"] = stats
+        self._current_chat = None
+
+    def _post(self, text, kind):
+        log = self._log
+        assert log != None
+        if self._current_chat != None:
+            self._current_chat["output"]["outputs"].append(
+                {"type": "text", "output": f"*** {kind}: {text}"}
+            )
+        else:
+            log["steps"].append(
+                {
+                    "type": "call",
+                    "input": f"*** {kind}",
+                    "output": {"type": "text", "output": text},
+                }
+            )
+
+    def on_warn(self, text):
+        self._post(text, "Warning")
+
+    def on_response(self, text):
+        log = self._log
+        assert log != None
+        assert self._current_chat != None
+        text = word_wrap_except_code_blocks(text)
+        self._current_chat["output"]["outputs"].append({"type": "text", "output": text})
+
+    def on_function_call(self, call, result):
+        log = self._log
+        assert log != None
+        if self._current_chat != None:
+            self._current_chat["output"]["outputs"].append(
+                {
+                    "type": "call",
+                    "input": call,
+                    "output": {"type": "text", "output": result},
+                }
+            )
+        else:
+            log["steps"].append(
+                {
+                    "type": "call",
+                    "input": call,
+                    "output": {"type": "text", "output": result},
+                }
+            )
```

### Comparing `chatdbg-0.3/src/chatdbg/ipdb_util/prompts.py` & `chatdbg-0.5/src/chatdbg/pdb/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import os
+
 _intro = f"""\
 You are a debugging assistant. You will be given a Python stack trace for an
 error and answer questions related to the root cause of the error.
 """
 
 _pdb_function = f"""\
 Call the `pdb` function to run Pdb debugger commands on the stopped program. You 
 may call the `pdb` function to run the following commands: `bt`, `up`, `down`, 
 `p expression`, `list`.
 
 Call `pdb` to print any variable value or expression that you believe may
 contribute to the error.
 """
 
+
 _info_function = """\
 Call the `info` function to get the documentation and source code for any
 variable, function, package, class, method reference, field reference, or 
 dotted reference visible in the current frame.  Examples include: n, e.n  
 where e is an expression, and t.n where t is a type.
 
 Unless it is from a common, widely-used library, you MUST call `info` exactly once on any
@@ -66,15 +69,15 @@
 
 _no_wheel = f"""\
 {_intro}
 {_general_instructions}
 """
 
 
-def pdb_instructions(supports_flow, take_the_wheel):
+def pdb_instructions(supports_flow: bool, take_the_wheel: bool) -> str:
     if take_the_wheel:
         if supports_flow:
             return _wheel_and_slice
         else:
             return _wheel_no_slice
     else:
         return _no_wheel
```

### Comparing `chatdbg-0.3/src/chatdbg/windbg/CMakeLists.txt` & `chatdbg-0.5/src/chatdbg/windbg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/windbg/chatdbg.cpp` & `chatdbg-0.5/src/chatdbg/windbg/chatdbg.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/windbg/include/appendlines.hpp` & `chatdbg-0.5/src/chatdbg/windbg/include/appendlines.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/windbg/include/openai.hpp` & `chatdbg-0.5/src/chatdbg/windbg/include/openai.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/windbg/include/wordwrap.hpp` & `chatdbg-0.5/src/chatdbg/windbg/include/wordwrap.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/src/chatdbg/windbg/nlohmann/json.hpp` & `chatdbg-0.5/src/chatdbg/windbg/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/test-deep-recursion.cpp` & `chatdbg-0.5/test/test-deep-recursion.cpp`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/test-failed-assert.why.txt` & `chatdbg-0.5/test/test-failed-assert.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/test-overflow.why.txt` & `chatdbg-0.5/test/test-overflow.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/test-use-after-free.why.txt` & `chatdbg-0.5/test/test-use-after-free.why.txt`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/python/bootstrap.py` & `chatdbg-0.5/test/python/bootstrap.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/python/bootstrap2.py` & `chatdbg-0.5/test/python/bootstrap2.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/python/ds101.py` & `chatdbg-0.5/test/python/ds101.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/python/mean.py` & `chatdbg-0.5/test/python/mean.py`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/test/python/nb.ipynb` & `chatdbg-0.5/test/python/nb.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976438492063492%*

 * *Differences: {"'metadata'": "{'ipyflow': {'cell_children': {'cf1aa8d4-c2fb-4c68-9861-3431df761d1a': []}, "*

 * *               "'cell_parents': {'cf1aa8d4-c2fb-4c68-9861-3431df761d1a': []}}, 'language_info': "*

 * *               "{'version': '3.11.7'}}"}*

```diff
@@ -66,14 +66,15 @@
                     "b46dc5a5-c376-40b3-a98d-da0ea012c80a"
                 ],
                 "a0ef25d9-d30c-4577-8285-c21fdd1fac2d": [],
                 "b46dc5a5-c376-40b3-a98d-da0ea012c80a": [],
                 "c13a73c3-68cb-4172-8f9d-0b0387b0c927": [
                     "f7c07ae1-735d-4093-bd3e-7efa9291f2d2"
                 ],
+                "cf1aa8d4-c2fb-4c68-9861-3431df761d1a": [],
                 "f7c07ae1-735d-4093-bd3e-7efa9291f2d2": []
             },
             "cell_parents": {
                 "11a5ccf7-17d6-4600-ad3b-4369d00eac1a": [],
                 "44d121b5-07d7-4b90-8fa5-bd0ad7ee2623": [],
                 "45d9fcde-3d09-4bd0-a1ac-f8470fc81250": [],
                 "637bdd5a-8e45-4f1d-8ad6-6e4d75e60d66": [],
@@ -82,14 +83,15 @@
                 "802a3ab2-599d-49dd-a5b4-3139d5e34269": [],
                 "a0ef25d9-d30c-4577-8285-c21fdd1fac2d": [],
                 "b46dc5a5-c376-40b3-a98d-da0ea012c80a": [
                     "66b2ebbf-584a-4c5f-885d-f2ad667cadd1",
                     "802a3ab2-599d-49dd-a5b4-3139d5e34269"
                 ],
                 "c13a73c3-68cb-4172-8f9d-0b0387b0c927": [],
+                "cf1aa8d4-c2fb-4c68-9861-3431df761d1a": [],
                 "f7c07ae1-735d-4093-bd3e-7efa9291f2d2": [
                     "c13a73c3-68cb-4172-8f9d-0b0387b0c927"
                 ]
             }
         },
         "kernelspec": {
             "display_name": "Python 3 (ipyflow)",
@@ -102,13 +104,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.19"
+            "version": "3.11.7"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `chatdbg-0.3/.gitignore` & `chatdbg-0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -156,7 +156,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 a.out
+log.yaml
```

### Comparing `chatdbg-0.3/LICENSE` & `chatdbg-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatdbg-0.3/README.md` & `chatdbg-0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 by [Emery Berger](https://emeryberger.com), [Stephen Freund](https://www.cs.williams.edu/~freund/index.html), [Kyla Levin](https://ravenblood000.github.io/KylaHLevin/index.html), [Nicolas van Kempen](https://nvankempen.com/) (ordered alphabetically)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/chatdbg.svg)](https://pypi.org/project/chatdbg/)
 [![Downloads](https://static.pepy.tech/badge/chatdbg)](https://pepy.tech/project/chatdbg)
 [![Downloads](https://static.pepy.tech/badge/chatdbg/month)](https://pepy.tech/project/chatdbg)
 
-ChatDBG is an experimental debugger for C/C++/Python/Rust code that integrates large language models into a standard debugger (`pdb`, `lldb`, `gdb`, and `windbg`) to help debug your code. With ChatDBG, you can engage in a dialog with your debugger, asking open-ended questions about your program, like `why is x null?`. ChatDBG will _take the wheel_ and steer the debugger to answer your queries. ChatDBG can provide error diagnoses and suggest fixes.
+ChatDBG is an AI-based debugging assistant for C/C++/Python/Rust code that integrates large language models into a standard debugger (`pdb`, `lldb`, `gdb`, and `windbg`) to help debug your code. With ChatDBG, you can engage in a dialog with your debugger, asking open-ended questions about your program, like `why is x null?`. ChatDBG will _take the wheel_ and steer the debugger to answer your queries. ChatDBG can provide error diagnoses and suggest fixes.
 
 As far as we are aware, ChatDBG is the *first* debugger to automatically perform root cause analysis and to provide suggested fixes.
 
+For technical details and a complete evaluation, see our arXiv paper, [_ChatDBG: An AI-Powered Debugging Assistant_](https://arxiv.org/abs/2403.16354) ([PDF](https://github.com/plasma-umass/ChatDBG/blob/main/ChatDBG-arxiv-2403.16354.pdf)).
+
 ## Installation
 
 > **Note**
 >
-> ChatDBG needs to be connected to an [OpenAI account](https://openai.com/api/). _Your account will need to have a positive balance for this to work_ ([check your balance](https://platform.openai.com/account/usage)). If you have never purchased credits, you will need to purchase at least $1 in credits (if your API account was created before August 13, 2023) or $0.50 (if you have a newer API account) in order to have access to GPT-4, which ChatDBG uses. [Get a key here.](https://platform.openai.com/account/api-keys)
+> ChatDBG needs to be connected to an [OpenAI account](https://openai.com/api/). _Your account will need to have a positive balance for this to work_ ([check your balance](https://platform.openai.com/account/usage)). If you have never purchased credits, you will need to purchase at least \$1 in credits (if your API account was created before August 13, 2023) or \$0.50 (if you have a newer API account) in order to have access to GPT-4, which ChatDBG uses. [Get a key here.](https://platform.openai.com/account/api-keys)
 >
 > Once you have an API key, set it as an environment variable called `OPENAI_API_KEY`.
 >
 > ```bash
 > export OPENAI_API_KEY=<your-api-key>
 > ```
```

### Comparing `chatdbg-0.3/pyproject.toml` & `chatdbg-0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChatDBG"
-version = "0.3"
+version = "0.5"
 authors = [
   { name="Emery Berger", email="emery.berger@gmail.com" },
   { name="Stephen Freund", email="sfreund@williams.edu" },
   { name="Kyla Levin", email="khlevin@umass.edu" },
   { name="Nicolas van Kempen", email="nvankemp@gmail.com" },
 ]
 dependencies = [
   "llm-utils>=0.2.8",
   "openai>=1.6.1",
   "rich>=13.7.0",
   "ansicolors>=1.1.8",
   "traitlets>=5.14.1",
   "ipdb>=0.13.13",
   "ipython>=8.18.1",
-  "litellm>=1.26.6",
+  "litellm>=1.34.12",
   "PyYAML>=6.0.1", 
   "ipyflow>=0.0.130",
   "numpy>=1.26.3"
 ]
 description = "AI-assisted debugging. Uses AI to answer 'why'."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -31,11 +31,12 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 chatdbg = "chatdbg.__main__:main"
+print_chatdbg_log = "chatdbg.util.plog:main"
 
 [project.urls]
 "Homepage" = "https://github.com/plasma-umass/ChatDBG"
 "Bug Tracker" = "https://github.com/plasma-umass/ChatDBG/issues"
```

### Comparing `chatdbg-0.3/PKG-INFO` & `chatdbg-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: ChatDBG
-Version: 0.3
+Version: 0.5
 Summary: AI-assisted debugging. Uses AI to answer 'why'.
 Project-URL: Homepage, https://github.com/plasma-umass/ChatDBG
 Project-URL: Bug Tracker, https://github.com/plasma-umass/ChatDBG/issues
 Author-email: Emery Berger <emery.berger@gmail.com>, Stephen Freund <sfreund@williams.edu>, Kyla Levin <khlevin@umass.edu>, Nicolas van Kempen <nvankemp@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: ansicolors>=1.1.8
 Requires-Dist: ipdb>=0.13.13
 Requires-Dist: ipyflow>=0.0.130
 Requires-Dist: ipython>=8.18.1
-Requires-Dist: litellm>=1.26.6
+Requires-Dist: litellm>=1.34.12
 Requires-Dist: llm-utils>=0.2.8
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: openai>=1.6.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: rich>=13.7.0
 Requires-Dist: traitlets>=5.14.1
 Description-Content-Type: text/markdown
@@ -27,23 +27,25 @@
 
 by [Emery Berger](https://emeryberger.com), [Stephen Freund](https://www.cs.williams.edu/~freund/index.html), [Kyla Levin](https://ravenblood000.github.io/KylaHLevin/index.html), [Nicolas van Kempen](https://nvankempen.com/) (ordered alphabetically)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/chatdbg.svg)](https://pypi.org/project/chatdbg/)
 [![Downloads](https://static.pepy.tech/badge/chatdbg)](https://pepy.tech/project/chatdbg)
 [![Downloads](https://static.pepy.tech/badge/chatdbg/month)](https://pepy.tech/project/chatdbg)
 
-ChatDBG is an experimental debugger for C/C++/Python/Rust code that integrates large language models into a standard debugger (`pdb`, `lldb`, `gdb`, and `windbg`) to help debug your code. With ChatDBG, you can engage in a dialog with your debugger, asking open-ended questions about your program, like `why is x null?`. ChatDBG will _take the wheel_ and steer the debugger to answer your queries. ChatDBG can provide error diagnoses and suggest fixes.
+ChatDBG is an AI-based debugging assistant for C/C++/Python/Rust code that integrates large language models into a standard debugger (`pdb`, `lldb`, `gdb`, and `windbg`) to help debug your code. With ChatDBG, you can engage in a dialog with your debugger, asking open-ended questions about your program, like `why is x null?`. ChatDBG will _take the wheel_ and steer the debugger to answer your queries. ChatDBG can provide error diagnoses and suggest fixes.
 
 As far as we are aware, ChatDBG is the *first* debugger to automatically perform root cause analysis and to provide suggested fixes.
 
+For technical details and a complete evaluation, see our arXiv paper, [_ChatDBG: An AI-Powered Debugging Assistant_](https://arxiv.org/abs/2403.16354) ([PDF](https://github.com/plasma-umass/ChatDBG/blob/main/ChatDBG-arxiv-2403.16354.pdf)).
+
 ## Installation
 
 > **Note**
 >
-> ChatDBG needs to be connected to an [OpenAI account](https://openai.com/api/). _Your account will need to have a positive balance for this to work_ ([check your balance](https://platform.openai.com/account/usage)). If you have never purchased credits, you will need to purchase at least $1 in credits (if your API account was created before August 13, 2023) or $0.50 (if you have a newer API account) in order to have access to GPT-4, which ChatDBG uses. [Get a key here.](https://platform.openai.com/account/api-keys)
+> ChatDBG needs to be connected to an [OpenAI account](https://openai.com/api/). _Your account will need to have a positive balance for this to work_ ([check your balance](https://platform.openai.com/account/usage)). If you have never purchased credits, you will need to purchase at least \$1 in credits (if your API account was created before August 13, 2023) or \$0.50 (if you have a newer API account) in order to have access to GPT-4, which ChatDBG uses. [Get a key here.](https://platform.openai.com/account/api-keys)
 >
 > Once you have an API key, set it as an environment variable called `OPENAI_API_KEY`.
 >
 > ```bash
 > export OPENAI_API_KEY=<your-api-key>
 > ```
```

