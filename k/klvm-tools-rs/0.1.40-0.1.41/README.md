# Comparing `tmp/klvm_tools_rs-0.1.40-cp38-abi3-win_amd64.whl.zip` & `tmp/klvm_tools_rs-0.1.41-cp38-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1320674 bytes, number of entries: 6
--rw-r--r--  4.6 unx     7376 b- defN 24-Feb-22 08:49 klvm_tools_rs-0.1.40.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Feb-22 08:49 klvm_tools_rs-0.1.40.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 24-Feb-22 08:49 klvm_tools_rs-0.1.40.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 24-Feb-22 08:49 klvm_tools_rs/__init__.py
--rwxr-xr-x  4.6 unx  3751424 b- defN 24-Feb-22 08:49 klvm_tools_rs/klvm_tools_rs.pyd
--rw-r--r--  4.6 unx      509 b- defN 24-Feb-22 08:49 klvm_tools_rs-0.1.40.dist-info/RECORD
-6 files, 3771096 bytes uncompressed, 1319756 bytes compressed:  65.0%
+Zip file size: 1337168 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     7189 b- defN 24-Apr-10 09:02 klvm_tools_rs-0.1.41.dist-info/METADATA
+-rw-r--r--  4.6 unx      127 b- defN 24-Apr-10 09:02 klvm_tools_rs-0.1.41.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11357 b- defN 24-Apr-10 09:02 klvm_tools_rs-0.1.41.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 24-Apr-10 09:02 klvm_tools_rs/__init__.py
+-rwxr-xr-x  4.6 unx  3205696 b- defN 24-Apr-10 09:02 klvm_tools_rs/klvm_tools_rs.abi3.so
+-rw-r--r--  4.6 unx      514 b- defN 24-Apr-10 09:02 klvm_tools_rs-0.1.41.dist-info/RECORD
+6 files, 3225018 bytes uncompressed, 1336242 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: klvm_tools_rs-0.1.40.dist-info/METADATA
+Filename: klvm_tools_rs-0.1.41.dist-info/METADATA
 Comment: 
 
-Filename: klvm_tools_rs-0.1.40.dist-info/WHEEL
+Filename: klvm_tools_rs-0.1.41.dist-info/WHEEL
 Comment: 
 
-Filename: klvm_tools_rs-0.1.40.dist-info/license_files/LICENSE
+Filename: klvm_tools_rs-0.1.41.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: klvm_tools_rs/__init__.py
 Comment: 
 
-Filename: klvm_tools_rs/klvm_tools_rs.pyd
+Filename: klvm_tools_rs/klvm_tools_rs.abi3.so
 Comment: 
 
-Filename: klvm_tools_rs-0.1.40.dist-info/RECORD
+Filename: klvm_tools_rs-0.1.41.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `klvm_tools_rs-0.1.40.dist-info/METADATA` & `klvm_tools_rs-0.1.41.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,201 +1,201 @@
 Metadata-Version: 2.1
 Name: klvm_tools_rs
-Version: 0.1.40
+Version: 0.1.41
 License-File: LICENSE
 Summary: tools for working with chiklisp language; compiler, repl, python and wasm bindings
 Keywords: chik,chiklisp,klvm
 Home-Page: https://prozacchiwawa.github.io/klvm_tools_rs/
 Author: Art Yerkes <art.yerkes@gmail.com>
 Author-email: Art Yerkes <art.yerkes@gmail.com>
 License: Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/Chik-Network/klvm_tools_rs
 
-klvm_tools_rs
-=
-
-Theory of operation of the modern compiler: ./HOW_CHIKLISP_IS_COMPILED.md
--
-This repo can be installed via cargo
-
-    cargo install klvm_tools_rs
-
-or via pip
-
-    pip install klvm_tools_rs@git+https://github.com/Chik-Network/klvm_tools_rs.git@e17412032aa7d3b8b1d1f931893fb5802eee626a
-
-Note: `pip` installs a subset of the tools installed by `cargo`, including `brun`, `run`, `opc` and `opd`.
-
-
-The most current version of the language is in the nightly branch:
-
-    [nightly](https://github.com/Chik-Network/klvm_tools_rs/tree/nightly)
-
-To install from a specific branch:
-
-    cargo install --no-default-features --git 'https://github.com/Chik-Network/klvm_tools_rs' --branch nightly
-    
-To install a git checkout into your current python environment (must be in some kind of venv or conda environment):
-
-    git clone https://github.com/Chik-Network/klvm_tools_rs
-    cd klvm_tools_rs
-    maturin develop
-
-Install from PYPI:
-
-    pip install -i https://pypi.chiknetwork.com/nightlies/ klvm_tools_rs
-    
-Most people still compile chiklisp via python.  One way to set up compilation
-in that way is like this:
-
-    import json
-    from klvm_tools_rs import compile_klvm
-
-    def compile_module_with_symbols(include_paths,source):
-        path_obj = Path(source)
-        file_path = path_obj.parent
-        file_stem = path_obj.stem
-        target_file = file_path / (file_stem + ".klvm.hex")
-        sym_file = file_path / (file_stem + ".sym")
-        compile_result = compile_klvm(source, str(target_file.absolute()), include_paths, True)
-        symbols = compile_result['symbols']
-        if len(symbols) != 0:
-            with open(str(sym_file.absolute()),'w') as symfile:
-                symfile.write(json.dumps(symbols))
-
-The command line tools provided:
-
-    - run -- Compiles KLVM code from chiklisp
-
-    Most commonly, you'll compile chiklisp like this:
-
-      ./target/debug/run -O -i include_dir chiklisp.clsp
-    
-    'run' outputs the code resulting from compiling the program, or an error.
-    
-    - repl -- Accepts chiklisp forms and expressions and produces results
-              interactively.
-              
-    Run like:
-    
-      ./target/debug/repl
-      
-    Example session:
-    
-    >>> (defmacro assert items
-       (if (r items)
-           (list if (f items) (c assert (r items)) (q . (x)))
-         (f items)
-         )
-       )
-    (q)
-    >>> (assert 1 1 "hello")
-    (q . hello)
-    >>> (assert 1 0 "bye")
-    failed: CompileErr(Srcloc { file: "*macros*", line: 2, col: 26, until: Some(Until { line: 2, col: 82 }) }, "klvm raise in (8) (())")
-    >>> 
-
-    - cldb -- Stepwise run chiklisp programs with program readable yaml output.
-    
-      ./target/debug/cldb '(mod (X) (x X))' '(4)'
-      ---
-      - Arguments: (() (4))
-        Operator: "4"
-        Operator-Location: "*command*(1):11"
-        Result-Location: "*command*(1):11"
-        Row: "0"
-        Value: (() 4)
-      - Env: "4"
-        Env-Args: ()
-        Operator: "2"
-        Operator-Location: "*command*(1):11"
-        Result-Location: "*command*(1):13"
-        Row: "1"
-        Value: "4"
-      - Arguments: (4)
-        Failure: klvm raise in (8 5) (() 4)
-        Failure-Location: "*command*(1):11"
-        Operator: "8"
-        Operator-Location: "*command*(1):13"
-
-    - brun -- Runs a "binary" program.  Instead of serving as a chiklisp
-      compiler, instead runs klvm programs.
-    
-    As 'brun' from the python code:
-    
-    $ ./target/debug/run '(mod (X) (defun fact (N X) (if (> 2 X) N (fact (* X N) (- X 1)))) (fact 1 X))'
-    (a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))
-    $ ./target/debug/brun '(a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))' '(5)'
-    120
-    
-    - opc -- crush klvm s-expression form to hex.
-    
-    As 'opc' from the python code.
-    
-    opc '(a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))'
-    ff02ffff01ff02ff02ffff04ff02ffff04ffff0101ffff04ff05ff8080808080ffff04ffff01ff02ffff03ffff15ffff0102ff0b80ffff0105ffff01ff02ff02ffff04ff02ffff04ffff12ff0bff0580ffff04ffff11ff0bffff010180ff808080808080ff0180ff018080
-    
-    - opd -- disassemble hex to s-expression form.
-    
-    As 'opd' from the python code.
-    
-    opd 'ff02ffff01ff02ff02ffff04ff02ffff04ffff0101ffff04ff05ff8080808080ffff04ffff01ff02ffff03ffff15ffff0102ff0b80ffff0105ffff01ff02ff02ffff04ff02ffff04ffff12ff0bff0580ffff04ffff11ff0bffff010180ff808080808080ff0180ff018080'
-    (a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))
-
-History
-=
-
-This is a second-hand port of chik's [klvm tools](https://github.com/Chik-Network/klvm_tools/) to rust via the work of
-ChikMineJP porting to typescript.  This would have been a lot harder to
-get to where it is without prior work mapping out the types of various
-semi-dynamic things (thanks, ChikMineJP).
-
-Some reasons for doing this are:
-
- - Chik switched the klvm implementation to rust: [klvm_rs](https://github.com/Chik-Network/klvm_rs), and this code may both pick up speed and track klvm better being in the same language.
- 
- - I wrote a new compiler with a simpler, less intricate structure that should be easier to improve and verify in the future in ocaml: [ochiklisp](https://github.com/prozacchiwawa/ochiklisp).
-
- - Also it's faster even in this unoptimized form.
-
-All acceptance tests i've brought over so far work, and more are being added.
-As of now, I'm not aware of anything that shouldn't be authentic when running
-these command line tools from klvm_tools in their equivalents in this repository
-
- - opc
- 
- - opd
- 
- - run
- 
- - brun
-
- - repl
- 
-argparse was ported to javascript and I believe I have faithfully reproduced it
-as it is used in cmds, so command line parsing should work similarly in all three
-versions.
-
-The directory structure is expected to be:
-
-    src/classic  <-- any ported code with heritage pointing back to
-                     the original chik repo.
-                    
-    src/compiler <-- a newer compiler (ochiklisp) with a simpler
-                     structure.  Select new style compilation by
-                     including a `(include *standard-cl-21*)`
-                     form in your toplevel `mod` form.
-
-Mac M1
-===
-
-Use ```cargo build --no-default-features``` due to differences in how mac m1 and
-other platforms handle python extensions.
-
-Use with chik-blockchain
-===
-
-    # Activate your venv, then
-    $ maturin develop --release
-
+klvm_tools_rs
+=
+
+Theory of operation of the modern compiler: ./HOW_CHIKLISP_IS_COMPILED.md
+-
+This repo can be installed via cargo
+
+    cargo install klvm_tools_rs
+
+or via pip
+
+    pip install klvm_tools_rs@git+https://github.com/Chik-Network/klvm_tools_rs.git@e17412032aa7d3b8b1d1f931893fb5802eee626a
+
+Note: `pip` installs a subset of the tools installed by `cargo`, including `brun`, `run`, `opc` and `opd`.
+
+
+The most current version of the language is in the nightly branch:
+
+    [nightly](https://github.com/Chik-Network/klvm_tools_rs/tree/nightly)
+
+To install from a specific branch:
+
+    cargo install --no-default-features --git 'https://github.com/Chik-Network/klvm_tools_rs' --branch nightly
+    
+To install a git checkout into your current python environment (must be in some kind of venv or conda environment):
+
+    git clone https://github.com/Chik-Network/klvm_tools_rs
+    cd klvm_tools_rs
+    maturin develop
+
+Install from PYPI:
+
+    pip install -i https://pypi.chiknetwork.com/nightlies/ klvm_tools_rs
+    
+Most people still compile chiklisp via python.  One way to set up compilation
+in that way is like this:
+
+    import json
+    from klvm_tools_rs import compile_klvm
+
+    def compile_module_with_symbols(include_paths,source):
+        path_obj = Path(source)
+        file_path = path_obj.parent
+        file_stem = path_obj.stem
+        target_file = file_path / (file_stem + ".klvm.hex")
+        sym_file = file_path / (file_stem + ".sym")
+        compile_result = compile_klvm(source, str(target_file.absolute()), include_paths, True)
+        symbols = compile_result['symbols']
+        if len(symbols) != 0:
+            with open(str(sym_file.absolute()),'w') as symfile:
+                symfile.write(json.dumps(symbols))
+
+The command line tools provided:
+
+    - run -- Compiles KLVM code from chiklisp
+
+    Most commonly, you'll compile chiklisp like this:
+
+      ./target/debug/run -O -i include_dir chiklisp.clsp
+    
+    'run' outputs the code resulting from compiling the program, or an error.
+    
+    - repl -- Accepts chiklisp forms and expressions and produces results
+              interactively.
+              
+    Run like:
+    
+      ./target/debug/repl
+      
+    Example session:
+    
+    >>> (defmacro assert items
+       (if (r items)
+           (list if (f items) (c assert (r items)) (q . (x)))
+         (f items)
+         )
+       )
+    (q)
+    >>> (assert 1 1 "hello")
+    (q . hello)
+    >>> (assert 1 0 "bye")
+    failed: CompileErr(Srcloc { file: "*macros*", line: 2, col: 26, until: Some(Until { line: 2, col: 82 }) }, "klvm raise in (8) (())")
+    >>> 
+
+    - cldb -- Stepwise run chiklisp programs with program readable yaml output.
+    
+      ./target/debug/cldb '(mod (X) (x X))' '(4)'
+      ---
+      - Arguments: (() (4))
+        Operator: "4"
+        Operator-Location: "*command*(1):11"
+        Result-Location: "*command*(1):11"
+        Row: "0"
+        Value: (() 4)
+      - Env: "4"
+        Env-Args: ()
+        Operator: "2"
+        Operator-Location: "*command*(1):11"
+        Result-Location: "*command*(1):13"
+        Row: "1"
+        Value: "4"
+      - Arguments: (4)
+        Failure: klvm raise in (8 5) (() 4)
+        Failure-Location: "*command*(1):11"
+        Operator: "8"
+        Operator-Location: "*command*(1):13"
+
+    - brun -- Runs a "binary" program.  Instead of serving as a chiklisp
+      compiler, instead runs klvm programs.
+    
+    As 'brun' from the python code:
+    
+    $ ./target/debug/run '(mod (X) (defun fact (N X) (if (> 2 X) N (fact (* X N) (- X 1)))) (fact 1 X))'
+    (a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))
+    $ ./target/debug/brun '(a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))' '(5)'
+    120
+    
+    - opc -- crush klvm s-expression form to hex.
+    
+    As 'opc' from the python code.
+    
+    opc '(a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))'
+    ff02ffff01ff02ff02ffff04ff02ffff04ffff0101ffff04ff05ff8080808080ffff04ffff01ff02ffff03ffff15ffff0102ff0b80ffff0105ffff01ff02ff02ffff04ff02ffff04ffff12ff0bff0580ffff04ffff11ff0bffff010180ff808080808080ff0180ff018080
+    
+    - opd -- disassemble hex to s-expression form.
+    
+    As 'opd' from the python code.
+    
+    opd 'ff02ffff01ff02ff02ffff04ff02ffff04ffff0101ffff04ff05ff8080808080ffff04ffff01ff02ffff03ffff15ffff0102ff0b80ffff0105ffff01ff02ff02ffff04ff02ffff04ffff12ff0bff0580ffff04ffff11ff0bffff010180ff808080808080ff0180ff018080'
+    (a (q 2 2 (c 2 (c (q . 1) (c 5 ())))) (c (q 2 (i (> (q . 2) 11) (q . 5) (q 2 2 (c 2 (c (* 11 5) (c (- 11 (q . 1)) ()))))) 1) 1))
+
+History
+=
+
+This is a second-hand port of chik's [klvm tools](https://github.com/Chik-Network/klvm_tools/) to rust via the work of
+ChikMineJP porting to typescript.  This would have been a lot harder to
+get to where it is without prior work mapping out the types of various
+semi-dynamic things (thanks, ChikMineJP).
+
+Some reasons for doing this are:
+
+ - Chik switched the klvm implementation to rust: [klvm_rs](https://github.com/Chik-Network/klvm_rs), and this code may both pick up speed and track klvm better being in the same language.
+ 
+ - I wrote a new compiler with a simpler, less intricate structure that should be easier to improve and verify in the future in ocaml: [ochiklisp](https://github.com/prozacchiwawa/ochiklisp).
+
+ - Also it's faster even in this unoptimized form.
+
+All acceptance tests i've brought over so far work, and more are being added.
+As of now, I'm not aware of anything that shouldn't be authentic when running
+these command line tools from klvm_tools in their equivalents in this repository
+
+ - opc
+ 
+ - opd
+ 
+ - run
+ 
+ - brun
+
+ - repl
+ 
+argparse was ported to javascript and I believe I have faithfully reproduced it
+as it is used in cmds, so command line parsing should work similarly in all three
+versions.
+
+The directory structure is expected to be:
+
+    src/classic  <-- any ported code with heritage pointing back to
+                     the original chik repo.
+                    
+    src/compiler <-- a newer compiler (ochiklisp) with a simpler
+                     structure.  Select new style compilation by
+                     including a `(include *standard-cl-21*)`
+                     form in your toplevel `mod` form.
+
+Mac M1
+===
+
+Use ```cargo build --no-default-features``` due to differences in how mac m1 and
+other platforms handle python extensions.
+
+Use with chik-blockchain
+===
+
+    # Activate your venv, then
+    $ maturin develop --release
+
```

## Comparing `klvm_tools_rs-0.1.40.dist-info/license_files/LICENSE` & `klvm_tools_rs-0.1.41.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

