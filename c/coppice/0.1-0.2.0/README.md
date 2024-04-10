# Comparing `tmp/coppice-0.1.tar.gz` & `tmp/coppice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coppice-0.1.tar", last modified: Tue Jan  2 21:17:23 2024, max compression
+gzip compressed data
```

## Comparing `coppice-0.1.tar` & `coppice-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:17:23.442912 coppice-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-01-02 21:17:12.000000 coppice-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-02 21:17:23.442912 coppice-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-02 21:17:12.000000 coppice-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:17:23.438912 coppice-0.1/coppice/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-02 21:17:12.000000 coppice-0.1/coppice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:17:23.438912 coppice-0.1/coppice/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-02 21:17:12.000000 coppice-0.1/coppice/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-02 21:17:12.000000 coppice-0.1/coppice/scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:17:23.438912 coppice-0.1/coppice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-02 21:17:23.000000 coppice-0.1/coppice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-02 21:17:12.000000 coppice-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 21:17:23.442912 coppice-0.1/setup.cfg
+-rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 coppice-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-10 11:47:46.000000 coppice-0.2.0/.github/workflows/python-publish.yml
+-rwxr-xr-x   0     1001      127     3301 2024-04-10 11:47:46.000000 coppice-0.2.0/.gitignore
+-rwxr-xr-x   0     1001      127      740 2024-04-10 11:47:46.000000 coppice-0.2.0/.pre-commit-config.yaml
+-rwxr-xr-x   0     1001      127    10912 2024-04-10 11:47:46.000000 coppice-0.2.0/LICENSE
+-rwxr-xr-x   0     1001      127      949 2024-04-10 11:47:46.000000 coppice-0.2.0/README.md
+-rwxr-xr-x   0     1001      127       75 2024-04-10 11:47:46.000000 coppice-0.2.0/coppice/__init__.py
+-rwxr-xr-x   0     1001      127      110 2024-04-10 11:47:46.000000 coppice-0.2.0/coppice/scripts/__init__.py
+-rwxr-xr-x   0     1001      127     2115 2024-04-10 11:47:46.000000 coppice-0.2.0/coppice/scripts/cli.py
+-rwxr-xr-x   0     1001      127   510331 2024-04-10 11:47:46.000000 coppice-0.2.0/demo_data/x_bin_1000.csv
+-rwxr-xr-x   0     1001      127     2000 2024-04-10 11:47:46.000000 coppice-0.2.0/demo_data/y_bin_1000.csv
+-rwxr-xr-x   0     1001      127     1568 2024-04-10 11:47:46.000000 coppice-0.2.0/src/criteria.rs
+-rwxr-xr-x   0     1001      127     2274 2024-04-10 11:47:46.000000 coppice-0.2.0/src/forest.rs
+-rwxr-xr-x   0     1001      127     1686 2024-04-10 11:47:46.000000 coppice-0.2.0/src/io.rs
+-rwxr-xr-x   0     1001      127     1581 2024-04-10 11:47:46.000000 coppice-0.2.0/src/lib.rs
+-rwxr-xr-x   0     1001      127     1511 2024-04-10 11:47:46.000000 coppice-0.2.0/src/metrics.rs
+-rwxr-xr-x   0     1001      127     2689 2024-04-10 11:47:46.000000 coppice-0.2.0/src/splitting.rs
+-rwxr-xr-x   0     1001      127     3231 2024-04-10 11:47:46.000000 coppice-0.2.0/src/tree.rs
+-rwxr-xr-x   0     1001      127    12642 2024-04-10 11:47:46.000000 coppice-0.2.0/Cargo.lock
+-rwxr-xr-x   0     1001      127     1145 2024-04-10 11:47:46.000000 coppice-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 coppice-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `coppice-0.1/LICENSE` & `coppice-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,188 +1,188 @@
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
-   Copyright 2024 Jake Bowden
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
+   Copyright 2024 Jake Bowden
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

### Comparing `coppice-0.1/pyproject.toml` & `coppice-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 [build-system]
-requires = [ "setuptools>=61",]
-build-backend = "setuptools.build_meta"
+requires = [ "maturin<2.0,>=1.4",]
+build-backend = "maturin"
 
 [project]
 name = "coppice"
-version = "0.1"
-description = "Decision trees and ensembles using a rust backend"
+version = "0.2.0"
+description = "A python and rust decision tree library"
 readme = "README.md"
 requires-python = ">=3.10"
+classifiers = [
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Programming Language :: Rust",
+]
 dependencies = [ "jsonschema", "numpy", "scikit-learn",]
-dynamic = []
+dynamic = [ "version",]
 
 [project.urls]
 Homepage = "https://github.com/JBwdn/coppice"
 
 [project.scripts]
 coppice = "coppice.scripts:cli_main"
 coppice_ = "coppice.scripts:cli_main"
 
 [project.optional-dependencies]
-dev = [ "black", "ipython", "isort", "pre-commit", "pylint", "pyright", "pytest",]
+dev = [ "black", "ipython", "isort", "maturin", "pre-commit", "pylint", "pyright", "pytest",]
+
+[tool.maturin]
+features = [ "pyo3/extension-module",]
+python-souce = "coppice"
+module-name = "coppice._coppice"
 
 [tool.pylint]
 disable = [ "import-error", "fixme",]
+extension-pkg-whitelist = [ "_coppice",]
 
 [tool.pyright]
 reportMissingImports = false
 pythonVersion = "3.10"
 
 [tool.black]
 target-version = [ "py310",]
 
 [tool.isort]
 profile = "black"
 filter_files = true
-
-[tool.setuptools.packages.find]
```

