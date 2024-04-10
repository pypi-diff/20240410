# Comparing `tmp/go_vendor_tools-0.3.0.tar.gz` & `tmp/go_vendor_tools-0.4.0b1.tar.gz`

## Comparing `go_vendor_tools-0.3.0.tar` & `go_vendor_tools-0.4.0b1.tar`

### file list

```diff
@@ -1,70 +1,79 @@
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/.packit.yaml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/NEWS.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/docs-requirements.txt
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/go-vendor-tools.spec
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/noxfile.py
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/rpmeval.sh
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/ruff.toml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/.reuse/dep5
--rwxr-xr-x   0        0        0      610 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/contrib/integration-archive.sh
--rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/contrib/main-archive.sh
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/contrib/verify-license.sh
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/contrib/wait-for-copr.sh
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/README.md -> ../README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/architecture.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/config.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/contributing.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/example-specfile.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/news.md -> ../NEWS.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/doc/scenarios.md
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/rpm/macros.go_vendor_tools
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/__init__.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/archive.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/exceptions.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/gomod.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/hashing.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/licensing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/py.typed
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/specfile_sources.py
--rwxr-xr-x   0        0        0     7491 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/cli/go_vendor_archive.py
--rwxr-xr-x   0        0        0    19756 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/cli/go_vendor_license.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/cli/utils.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/config/archive.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/config/base.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/config/licenses.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/config/utils.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/__init__.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/askalono.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/base.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/load.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/trivy.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/.gitignore
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/autorestic/CHECKSUMS
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/autorestic/autorestic.spec
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/autorestic/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/autorestic/expected-licenses.list.license
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/autorestic/go-vendor-tools.toml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/fzf/CHECKSUMS
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/fzf/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/fzf/expected-licenses.list.license
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/fzf/fzf.spec
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/integration/fzf/go-vendor-tools.toml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/conftest.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_archive.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_go_vendor_tools.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_licensing.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_data/case1/config-broken.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_data/case1/config.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/tests/pytests/test_data/case2/licenses/LICENSE
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/.gitignore
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/README.md
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 go_vendor_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.packit.yaml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSE.md
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/NEWS.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/docs-requirements.txt
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/go-vendor-tools.spec
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/mkdocs.yml
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/noxfile.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json.license
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpmeval.sh
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/ruff.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.reuse/dep5
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/integration-archive.sh
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/main-archive.sh
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/verify-license.sh
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/wait-for-copr.sh
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/README.md -> ../README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/architecture.md
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/config.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/contributing.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/example-specfile.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/news.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/scenarios.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/.gitignore
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive.1.scd
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_create.1.scd
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_override.1.scd
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkdocs_mangen.py
+-rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkman.sh
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/py.typed
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py
+-rwxr-xr-x   0        0        0     9832 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py
+-rwxr-xr-x   0        0        0    20400 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/utils.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/utils.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/__init__.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/.gitignore
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/CHECKSUMS
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list.license
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS.license
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list.license
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/go-vendor-tools.toml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/conftest.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_archive.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config-broken.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitignore
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/README.md
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/PKG-INFO
```

### Comparing `go_vendor_tools-0.3.0/.gitlab-ci.yml` & `go_vendor_tools-0.4.0b1/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
       go-rpm-macros
       golang-bin
       pipx
       python3-devel
       redhat-rpm-config
       rpm-build
       rpmdevtools
+      /usr/bin/unshare
     - >-
       test "$SHOULD_RPMBUILD" = "false" ||
       sudo dnf install
       --setopt=install_weak_deps=0 -y
       python3.9
       python3.10-devel
       python3.11-devel
@@ -93,13 +94,18 @@
           SHOULD_RPMBUILD: "false"
         - IMAGE: "quay.io/centos/centos:stream9"
           PACKAGES: "fzf"
           SHOULD_RPMBUILD: "false"
 
 pages:
   script:
+    - >-
+      sudo dnf install
+      --setopt=install_weak_deps=0 -y
+      pandoc
+      scd2html
     - nox -e mkdocs -- build -d public
   artifacts:
     paths:
       - public
   rules:
     - if: $CI_COMMIT_BRANCH == "main"
```

### Comparing `go_vendor_tools-0.3.0/.packit.yaml` & `go_vendor_tools-0.4.0b1/.packit.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 upstream_package_name: go-vendor-tools
 srpm_build_deps:
   - golang-bin
   - git-core
   - pipx
   - rpmdevtools
   - wait-for-copr
+  - /usr/bin/unshare
 packages:
   # Main package
   go-vendor-tools:
     specfile_path: go-vendor-tools.spec
     actions:
       fix-spec-file:
         - "./contrib/main-archive.sh go-vendor-tools.spec"
@@ -42,25 +43,26 @@
         - bash -x ../../../contrib/wait-for-copr.sh
 jobs:
   - job: copr_build
     packages:
       - go-vendor-tools
       - autorestic
       - fzf
-    targets: &targets
+    targets:
       fedora-all-x86_64:
-        additional_packages:
-          # TODO: Remove this once trivy is packaged in Fedora!
-          - https://github.com/aquasecurity/trivy/releases/download/v0.49.1/trivy_0.49.1_Linux-64bit.rpm
-      # - epel-9-x86_64
+        # Extra dependencies (trivy, python-zstarfile) not packaged in Fedora
+        additional_repos:
+          - "copr://@go-sig/go-vendor-tools-dev"
     trigger: pull_request
 
   - job: copr_build
     packages:
       - go-vendor-tools
       - autorestic
       - fzf
-    targets: *targets
+    targets:
+      - fedora-all-x86_64
+      - fedora-all-aarch64
     owner: "@go-sig"
     project: go-vendor-tools-dev
     trigger: commit
     branch: main
```

### Comparing `go_vendor_tools-0.3.0/CONTRIBUTING.md` & `go_vendor_tools-0.4.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/NEWS.md` & `go_vendor_tools-0.4.0b1/NEWS.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 <!--
 Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 SPDX-License-Identifier: MIT
 -->
 
 # NEWS
 
+## 0.4.0b1 - 2024-04-10 <a id='0.4.0b1'></a>
+
+### Added
+
+- `cli`: support compression algorithms other than `xz` (#7, #45)
+- `doc`: add manpages for go_vendor_archive commands (#40)
+- `go_vendor_archive create`: add `--idempotent` flag
+- `go_vendor_archive create`: add `--write-config` flag
+- `go_vendor_archive create`: add missing `--no-use-module-proxy` flag to
+    disable default `--use-module-proxy`.
+- `go_vendor_archive create`: change default output file to `vendor.tar.bz2`
+    (#7, #46)
+- `go_vendor_archive create`: handle projects without any dependencies (#29)
+
+### Fixed
+
+- `doc config`: fix markdown syntax error
+- `doc config`: remove stray backtick in archive section
+- `go_vendor_license install`: properly own intermediate directories
+
 ## 0.3.0 - 2024-03-28 <a id='0.3.0'></a>
 
 ### Added
 
 - `LICENSES`: add Copyright
 - `doc`: add documentation site at
   <https://fedora.gitlab.io/sigs/go/go-vendor-tools>
```

### Comparing `go_vendor_tools-0.3.0/go-vendor-tools.spec` & `go_vendor_tools-0.4.0b1/go-vendor-tools.spec`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT
 
-%global forgeurl https://gitlab.com/gotmax23/go-vendor-tools
-%define tag v%{version}
+%bcond manpages 1
+%global forgeurl https://gitlab.com/fedora/sigs/go/go-vendor-tools
+%define tag v%{version_no_tilde %{quote:%nil}}
 
 Name:           go-vendor-tools
-Version:        0.3.0
+Version:        0.4.0b1
 %forgemeta
 Release:        1%{?dist}
 Summary:        Tools for handling Go library vendoring in Fedora
 
 # BSD-3-Clause: src/go_vendor_tools/archive.py
 License:        MIT AND BSD-3-Clause
 URL:            %{forgeurl}
 Source0:        %{forgesource}
 
 BuildArch:      noarch
 
 BuildRequires:  python3-devel
 
+%if %{with manpages}
+BuildRequires:  scdoc
+%endif
+
 Recommends:     (askalono-cli or trivy)
 
 
 %global common_description %{expand:
 go-vendor-tools provides tools and macros for handling Go library vendoring in
 Fedora.}
 
@@ -43,46 +48,60 @@
 
 %generate_buildrequires
 %pyproject_buildrequires -x test
 
 
 %build
 %pyproject_wheel
+%if %{with manpages}
+./doc/man/mkman.sh
+%endif
 
 
 %install
 %pyproject_install
 # TODO(anyone): Use -l flag once supported by EL 9.
 %pyproject_save_files go_vendor_tools
 
 # Install RPM macros
 install -Dpm 0644 rpm/macros.go_vendor_tools -t %{buildroot}%{_rpmmacrodir}
 
 # Install documentation
 mkdir -p %{buildroot}%{_docdir}/go-vendor-tools-doc
 cp -rL doc/* %{buildroot}%{_docdir}/go-vendor-tools-doc
 
+# Install manpages
+%if %{with manpages}
+install -Dpm 0644 doc/man/*.1 -t %{buildroot}%{_mandir}/man1/
+%endif
+
 
 %check
 %pytest
 
 
 %files -f %{pyproject_files}
 # Install top-level markdown files
 %doc *.md
 %license LICENSES/*
 %{_bindir}/go_vendor*
 %{_rpmmacrodir}/macros.go_vendor_tools
+%if %{with manpages}
+%{_mandir}/man1/go*.1*
+%endif
 
 %files doc
 %doc %{_docdir}/go-vendor-tools-doc/
 
 %pyproject_extras_subpkg -n go-vendor-tools all
 
 %changelog
+* Wed Apr 10 2024 Maxwell G <maxwell@gtmx.me> - 0.4.0b1-1
+- Release 0.4.0b1.
+
 * Thu Mar 28 2024 Maxwell G <maxwell@gtmx.me> - 0.3.0-1
 - Release 0.3.0.
 
 * Sat Mar 16 2024 Maxwell G <maxwell@gtmx.me> - 0.2.0-1
 - Release 0.2.0.
 
 * Sat Mar 09 2024 Maxwell G <maxwell@gtmx.me> - 0.1.0-1
```

### Comparing `go_vendor_tools-0.3.0/mkdocs.yml` & `go_vendor_tools-0.4.0b1/mkdocs.yml`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 site_url: https://gotmax23.gitlab.io/go-vendor-tools
 repo_url: https://gitlab.com/gotmax23/go-vendor-tools
 theme:
   name: material
   features:
     - content.code.copy
     - navigation.footer
+    - navigation.sections
 # REUSE-IgnoreStart
 copyright: >
   Copyright (C) 2024 Maxwell G and contributors |
   SPDX-License-Identifier: <a style="text-decoration: underline;" href="https://gitlab.com/gotmax23/go-vendor-tools/-/blob/main/LICENSES/MIT.txt?ref_type=heads">MIT</a>
 # REUSE-IgnoreEnd
 markdown_extensions:
   # Builtin
@@ -21,16 +22,34 @@
   - attr_list
   - footnotes
   - toc:
       permalink: true
   # pymdownx
   - pymdownx.highlight:
       anchor_linenums: true
+  - pymdownx.magiclink:
+      repo_url_shorthand: true
+      provider: gitlab
+      user: "fedora/sigs/go"
+      repo: "go-vendor-tools"
   - pymdownx.superfences
+plugins:
+  - exclude:
+      glob:
+        - "man/**"
+        - ".gitignore"
+  - gen-files:
+      scripts:
+        - doc/man/mkdocs_mangen.py
+
 nav:
   - README.md
   - news.md
   - contributing.md
+  - Manpages:
+    - "go_vendor_archive(1)": man/go_vendor_archive1.md
+    - "go_vendor_archive_create(1)": man/go_vendor_archive_create1.md
+    - "go_vendor_archive_override(1)": man/go_vendor_archive_override1.md
   - scenarios.md
   - config.md
   - architecture.md
   - example-specfile.md
```

### Comparing `go_vendor_tools-0.3.0/noxfile.py` & `go_vendor_tools-0.4.0b1/noxfile.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/rpmeval.sh` & `go_vendor_tools-0.4.0b1/rpmeval.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/ruff.toml` & `go_vendor_tools-0.4.0b1/ruff.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/contrib/integration-archive.sh` & `go_vendor_tools-0.4.0b1/contrib/integration-archive.sh`

 * *Files 16% similar despite different names*

```diff
@@ -14,8 +14,12 @@
 
 spectool -g ./*.spec
 ls
 if [ -f "go-vendor-tools.toml" ]; then
     command+=("--config" "$(pwd)/go-vendor-tools.toml")
 fi
 time "${command[@]}" "$@" ./*.spec
+# Test idempotency by running again with networking disabled and a timeout
+# to make sure nothing is downloaded.
+command+=("--idempotent")
+timeout 5 unshare -rn "${command[@]}" "$@" ./*.spec | grep 'already exists'
 sha512sum -c CHECKSUMS
```

### Comparing `go_vendor_tools-0.3.0/contrib/verify-license.sh` & `go_vendor_tools-0.4.0b1/contrib/verify-license.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/doc/architecture.md` & `go_vendor_tools-0.4.0b1/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/doc/config.md` & `go_vendor_tools-0.4.0b1/doc/config.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 > **Environment variable**: `GO_VENDOR_LICENSE_DETECTOR`
 
 Explicitly choose a license detector.
 Currently supported detectors are:
 
 1. trivy
-2. askalono`
+2. askalono
 
 If no detector is specified, `go_vendor_license` will attempt to load the first
 available license detector from first to last in the above list.
 `go_vendor_license` will error if neither `trivy` nor `askalono` is installed.
 
 #### `licenses` (list of license entry tables)
 
@@ -58,15 +58,15 @@
 
 #### `exclude_directories` (list of strings)
 
 List of directories to ignore when scanning for license files
 
 ### `archive`
 
-The configuration for `go_vendor_archive` is stored under the `archive` table`.
+The configuration for `go_vendor_archive` is stored under the `archive` table.
 
 #### `use_module_proxy` (boolean)
 
 > **Default**: `true`
 >
 > **Environment variable**: `GO_VENDOR_ARCHIVE_USE_MODULE_PROXY`
 
@@ -85,10 +85,27 @@
 Whether to run `go tidy` before `go mod vendor` when creating the archive.
 You should leave this enabled.
 
 #### `dependency_overrides` (string mapping)
 
 See [*Security updates*](./scenarios.md#security-updates).
 
+#### `compression_type` (string)
+
+> **CLI flag**: `--compression`
+
+Compression type, such as `tar` (uncompressed), `gz`, `bz2`, or `zstd`.
+By default, the compression type is detected based on the extension of
+`--output` passed on the CLI.
+
+#### compresslevel (int)
+
+> **Environment variable**: `GO_VENDOR_ARCHIVE_COMPRESSLEVEL`
+>
+> **CLI flag**: `--compresslevel`
+
+Compression level as an integer for compression algorithms that support the
+setting
+
 [^1]: This is done for security reasons. `pre_commands` and `post_commands` can
     run arbitrary code, so we do not want to blindly load configuration from
     the current working directory.
```

### Comparing `go_vendor_tools-0.3.0/doc/example-specfile.md` & `go_vendor_tools-0.4.0b1/doc/example-specfile.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/doc/scenarios.md` & `go_vendor_tools-0.4.0b1/doc/scenarios.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/rpm/macros.go_vendor_tools` & `go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Tools for creating tar archives
 """
 
 from __future__ import annotations
 
 import os
 import tarfile
-from collections.abc import Sequence
+from collections.abc import Collection, Sequence
 from pathlib import Path, PurePath
 
 
 ### normalize_file_permissions is derived from flit_core
 # Copyright (c) 2015, Thomas Kluyver and contributors
 # SPDX-License-Identifier: BSD-3-Clause
 def normalize_file_permissions(st_mode: int) -> int:
@@ -43,18 +43,21 @@
 
 
 def add_files_to_archive(
     tf: tarfile.TarFile,
     directory: Path,
     files: Sequence[Path],
     top_level_dir: bool = False,
+    optional_files: Collection[Path] = frozenset(),
 ) -> None:
     for file in files:
         if file.is_absolute():
             raise ValueError(f"{file} is not a relative path!")
+        if not (directory / file).exists() and file in optional_files:
+            continue
         dest = (directory.resolve().name / file) if top_level_dir else file
         tf.add(directory / file, dest, filter=reproducible_filter)
 
 
 def get_toplevel_directory(tar: tarfile.TarFile) -> str | None:
     first_parent = {PurePath(info.name).parts[0] for info in tar.getmembers()}
     if len(first_parent) == 1:
```

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/exceptions.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/gomod.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/hashing.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/licensing.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/specfile_sources.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/cli/go_vendor_archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 import argparse
 import dataclasses
 import os
 import shlex
 import shutil
 import subprocess
 import sys
-import tarfile
 import tempfile
 from collections.abc import Callable, Sequence
-from contextlib import AbstractContextManager, nullcontext
-from functools import cache, partial
+from contextlib import ExitStack
+from functools import partial
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, ClassVar
 
+from zstarfile import ZSTarfile
+from zstarfile.extra import open_write_compressed
+
 from go_vendor_tools import __version__
 from go_vendor_tools.archive import add_files_to_archive
 from go_vendor_tools.config.archive import get_go_dependency_update_commands
 from go_vendor_tools.config.base import BaseConfig, load_config
 from go_vendor_tools.exceptions import ArchiveError
 from go_vendor_tools.specfile_sources import get_path_and_output_from_specfile
 
@@ -34,23 +36,23 @@
 else:
     HAS_TOMLKIT = True
     from go_vendor_tools.cli.utils import load_tomlkit_if_exists
 
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
-DEFAULT_OUTPUT = "vendor.tar.xz"
+DEFAULT_OUTPUT = "vendor.tar.bz2"
 ARCHIVE_FILES = (Path("go.mod"), Path("go.sum"), Path("vendor"))
+OPTIONAL_FILES = frozenset({Path("go.sum")})
 GO_PROXY_ENV = {
     "GOPROXY": "https://proxy.golang.org,direct",
     "GOSUMDB": "sum.golang.org",
 }
 
 
-@cache
 def need_tomlkit(action="this action"):
     if not HAS_TOMLKIT:
         message = f"tomlkit is required for {action}. Please install it!"
         sys.exit(message)
 
 
 def run_command(
@@ -65,38 +67,57 @@
 @dataclasses.dataclass()
 class CreateArchiveArgs:
     path: Path
     output: Path
     use_top_level_dir: bool
     use_module_proxy: bool
     tidy: bool
+    idempotent: bool
+    compresslevel: int | None
+    compression_type: str | None
     config_path: Path
     config: BaseConfig
+    write_config: bool
+    _explicitly_passed: list[str] = dataclasses.field(default_factory=list, repr=False)
 
     CONFIG_OPTS: ClassVar[tuple[str, ...]] = (
         "use_module_proxy",
         "use_top_level_dir",
         "tidy",
+        "compresslevel",
+        "compression_type",
     )
 
     @classmethod
     def construct(cls, **kwargs: Any) -> CreateArchiveArgs:
         if kwargs.pop("subcommand") != "create":
             raise AssertionError  # pragma: no cover
-        kwargs["config"] = load_config(kwargs["config_path"])
+        _explicitly_passed = list(kwargs)
+        kwargs["config"] = load_config(kwargs["config_path"], kwargs["write_config"])
         for opt in cls.CONFIG_OPTS:
-            if kwargs[opt] is None:
+            if kwargs.get(opt) is None:
                 kwargs[opt] = kwargs["config"]["archive"][opt]
-
-        if kwargs["output"] and not kwargs["output"].name.endswith((".tar.xz", "txz")):
-            raise ValueError(f"{kwargs['output']} must end with '.tar.xz' or '.txz'")
-
         if not kwargs["path"].exists():
             raise ArchiveError(f"{kwargs['path']} does not exist!")
-        return CreateArchiveArgs(**kwargs)
+        if kwargs["write_config"]:
+            need_tomlkit("--write-config")
+            if not kwargs["config_path"]:
+                raise ArchiveError("--write-config requires --config to be set")
+        return CreateArchiveArgs(**kwargs, _explicitly_passed=_explicitly_passed)
+
+    def write_config_opts(self) -> None:
+        need_tomlkit("write_config_opts")
+        loaded = load_tomlkit_if_exists(self.config_path)
+        config = loaded.setdefault("archive", {})
+        for opt in self._explicitly_passed:
+            if opt not in self.CONFIG_OPTS:
+                continue
+            config[opt] = getattr(self, opt)
+        with open(self.config_path, "w", encoding="utf-8") as fp:
+            tomlkit.dump(loaded, fp)
 
 
 @dataclasses.dataclass()
 class OverrideArgs:
     config_path: Path
     import_path: str
     version: str
@@ -115,29 +136,50 @@
     create_subparser = subparsers.add_parser("create")
     create_subparser.add_argument("--version", action="version", version=__version__)
     create_subparser.add_argument(
         "-O", "--output", type=Path, default=None, help=f"Default: {DEFAULT_OUTPUT}"
     )
     create_subparser.add_argument(
         "--top-level-dir",
-        default=None,
         dest="use_top_level_dir",
         action=argparse.BooleanOptionalAction,
+        default=argparse.SUPPRESS,
+    )
+    create_subparser.add_argument(
+        "--use-module-proxy",
+        action=argparse.BooleanOptionalAction,
+        default=argparse.SUPPRESS,
     )
     create_subparser.add_argument(
-        "--use-module-proxy", action="store_true", default=None
+        "-p", action="store_true", dest="use_module_proxy", default=argparse.SUPPRESS
     )
-    create_subparser.add_argument("-p", action="store_true", dest="use_module_proxy")
     create_subparser.add_argument("-c", "--config", type=Path, dest="config_path")
     create_subparser.add_argument(
         "--tidy",
         help="%(default)s",
         action=argparse.BooleanOptionalAction,
-        default=None,
+        default=argparse.SUPPRESS,
+    )
+    create_subparser.add_argument(
+        "-I",
+        "--idempotent",
+        action="store_true",
+        help="Only generate archive if OUTPUT does not already exist",
     )
+    create_subparser.add_argument(
+        "--compresslevel", type=int, default=argparse.SUPPRESS
+    )
+    create_subparser.add_argument(
+        "--compression",
+        dest="compression_type",
+        metavar="COMPRESSION_TYPE",
+        help=f"Choices: {list(ZSTarfile.OPEN_METH)}",
+        default=argparse.SUPPRESS,
+    )
+    create_subparser.add_argument("--write-config", action="store_true")
     create_subparser.add_argument("path", type=Path)
     override_subparser = subparsers.add_parser("override")
     override_subparser.add_argument(
         "--config", type=Path, dest="config_path", required=True
     )
     override_subparser.add_argument("import_path")
     override_subparser.add_argument("version")
@@ -162,48 +204,68 @@
             f" Run 'spectool -g {spec_path}' and try again!"
         )
 
 
 def create_archive(args: CreateArchiveArgs) -> None:
     _already_checked_is_file = False
     cwd = args.path
-    cm: AbstractContextManager[str] = nullcontext(str(args.path))
     if args.path.suffix == ".spec":
         _create_archive_read_from_specfile(args)
         _already_checked_is_file = True
     else:
         args.output = Path(DEFAULT_OUTPUT)
-    # Treat as an archive if it's not a directory
-    if _already_checked_is_file or args.path.is_file():
-        print(f"* Treating {args.path} as an archive. Unpacking...")
-        cm = tempfile.TemporaryDirectory()
-        shutil.unpack_archive(args.path, cm.name)
-        cwd = Path(cm.name)
-        cwd /= next(cwd.iterdir())
-    with cm:
+    if args.idempotent and args.output.exists():
+        print(f"{args.output} already exists")
+        sys.exit()
+    with ExitStack() as stack:
+        try:
+            tf = stack.enter_context(
+                open_write_compressed(
+                    args.output,
+                    compression_type=args.compression_type,
+                    compresslevel=args.compresslevel,
+                )
+            )
+        except ValueError as exc:
+            sys.exit(f"Invalid --output value: {exc}")
+        # Treat as an archive if it's not a directory
+        if _already_checked_is_file or args.path.is_file():
+            print(f"* Treating {args.path} as an archive. Unpacking...")
+            cwd = Path(stack.enter_context(tempfile.TemporaryDirectory()))
+            shutil.unpack_archive(args.path, cwd)
+            cwd /= next(cwd.iterdir())
         env = os.environ | GO_PROXY_ENV if args.use_module_proxy else None
         runner = partial(subprocess.run, cwd=cwd, check=True, env=env)
         pre_commands = chain(
             args.config["archive"]["pre_commands"],
             get_go_dependency_update_commands(
                 args.config["archive"]["dependency_overrides"]
             ),
         )
         for command in pre_commands:
             run_command(runner, command)
         if args.tidy:
             run_command(runner, ["go", "mod", "tidy"])
         run_command(runner, ["go", "mod", "vendor"])
+        # Create vendor directory so it is there even if there are no
+        # dependencies to download
+        (vdir := cwd / "vendor").mkdir(exist_ok=True)
+        (vdir / "modules.txt").touch(exist_ok=True)
         for command in args.config["archive"]["post_commands"]:
             run_command(runner, command)
         print("Creating archive...")
-        with tarfile.open(args.output, "w:xz") as tf:
-            add_files_to_archive(
-                tf, Path(cwd), ARCHIVE_FILES, top_level_dir=args.use_top_level_dir
-            )
+        add_files_to_archive(
+            tf,
+            Path(cwd),
+            ARCHIVE_FILES,
+            top_level_dir=args.use_top_level_dir,
+            optional_files=OPTIONAL_FILES,
+        )
+        if args.write_config:
+            args.write_config_opts()
 
 
 def override_command(args: OverrideArgs) -> None:
     need_tomlkit()
     loaded = load_tomlkit_if_exists(args.config_path)
     overrides = loaded.setdefault("archive", {}).setdefault("dependency_overrides", {})
     overrides[args.import_path] = args.version
```

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/cli/go_vendor_license.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from __future__ import annotations
 
 import argparse
 import json
 import os
 import shutil
 import sys
-import tarfile
 from collections.abc import Collection, Iterable, Iterator, MutableSequence, Sequence
 from contextlib import contextmanager
 from functools import cache
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from textwrap import dedent
 from typing import IO, Any, cast
 
 import license_expression
+from zstarfile import ZSTarfile
 
 from go_vendor_tools import __version__
 from go_vendor_tools.archive import get_toplevel_directory
 from go_vendor_tools.config.base import load_config
 from go_vendor_tools.config.licenses import (
     LicenseConfig,
     LicenseEntry,
@@ -39,15 +39,15 @@
     import tomlkit
 except ImportError:
     HAS_TOMLKIT = False
 else:
     HAS_TOMLKIT = True
     from go_vendor_tools.cli.utils import load_tomlkit_if_exists
 
-COLOR = None
+COLOR: bool | None = None
 RED = "\033[31m"  # ]
 CLEAR = "\033[0m"  # ]
 
 
 def red(__msg: str, /, *, file: IO[str] = sys.stdout) -> None:
     color = COLOR
     if color is None:
@@ -396,22 +396,22 @@
     if directories[0].suffix == ".spec":
         directories[:] = get_path_and_output_from_specfile(directories[0])
         is_archive = True
     if is_archive:
         with TemporaryDirectory() as _tmp:
             tmp = Path(_tmp)
             # Extract the first archive
-            with tarfile.open(directories[0]) as tar:
+            with ZSTarfile.open(directories[0]) as tar:
                 first_toplevel = get_toplevel_directory(tar)
                 if not first_toplevel:
                     sys.exit(f"{directories[0]} does not have a top-level directory!")
                 print(f"Extracting {directories[0]}", file=sys.stderr)
                 tar.extractall(tmp)
             for directory in directories[1:]:
-                with tarfile.open(directory) as tar:
+                with ZSTarfile.open(directory) as tar:
                     toplevel = get_toplevel_directory(tar)
                     print(f"Extracting {directory}", file=sys.stderr)
                     tar.extractall(tmp if toplevel else tmp / first_toplevel)
             yield tmp / first_toplevel
 
     else:
         yield directories[0]
@@ -462,32 +462,52 @@
             (license_data.undetected_licenses and not ignore_undetected)
             or (unlicensed_mods and not ignore_unlicensed_mods)
             or license_data.unmatched_extra_licenses
         )
     )
 
 
+def _get_intermediate_directories(
+    directory_parts: Collection[Sequence[str]],
+) -> set[Path]:
+    inter_parts = set()
+    for parts in directory_parts:
+        for i in range(len(parts)):
+            inter_parts.add(Path(*parts[: i + 1]))
+    return inter_parts
+
+
 def copy_licenses(
     base_directory: Path,
     license_paths: Iterable[Path],
     install_destdir: Path,
     install_directory: Path,
     install_filelist: Path,
 ) -> None:
     installdir = install_destdir / install_directory.relative_to("/")
     base_directory = base_directory.resolve()
 
-    with install_filelist.open("w", encoding="utf-8") as fp:
-        installdir.mkdir(parents=True, exist_ok=True)
-        fp.write(f"%license %dir {install_directory}\n")
-        for lic in license_paths:
-            relpath = lic.resolve().relative_to(base_directory)
-            (installdir / relpath).parent.mkdir(parents=True, exist_ok=True)
-            shutil.copy2(lic, installdir / relpath)
-            fp.write(f"%license {install_directory / relpath}\n")
+    entries: list[str] = []
+    directory_parts: set[Sequence[str]] = set()
+    installdir.mkdir(parents=True, exist_ok=True)
+    entries.append(f"%license %dir {install_directory}")
+    for lic in license_paths:
+        resolvedpath = lic.resolve()
+        relpath = resolvedpath.relative_to(base_directory)
+        if len(relpath.parts) > 1:
+            directory_parts.add(relpath.parts[:-1])
+        (installdir / relpath).parent.mkdir(parents=True, exist_ok=True)
+        shutil.copy2(lic, installdir / relpath)
+        entries.append(f"%license {install_directory / relpath}")
+    entries.extend(
+        f"%license %dir {install_directory / path}"
+        for path in _get_intermediate_directories(directory_parts)
+    )
+    entries.sort()
+    install_filelist.write_text("\n".join(entries) + "\n")
 
 
 def install_command(args: argparse.Namespace) -> None:
     """
     Install license files into the license directory
     """
     directory: Path = args.directory[0]
```

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/config/archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,46 +3,57 @@
 
 """
 Configuration for the go_vendor_archive command
 """
 
 from __future__ import annotations
 
+import os
 from collections.abc import Iterator
 from typing import Any, Mapping, TypedDict, cast
 
 from .utils import get_envvar_boolean
 
 DEFAULT_USE_TOP_LEVEL_DIR = False
 DEFAULT_USE_MODULE_PROXY = get_envvar_boolean(
     "GO_VENDOR_ARCHIVE_USE_MODULE_PROXY", True
 )
 DEFAULT_TIDY = True
+DEFAULT_COMPRESSLEVEL_STR = os.environ.get("GO_VENDOR_ARCHIVE_COMPRESSLEVEL")
 
 
 class ArchiveConfig(TypedDict):
     use_module_proxy: bool
     use_top_level_dir: bool
     # Commands to run before downloading modules
     pre_commands: list[list[str]]
     # Commands to run after downloading modules
     post_commands: list[list[str]]
     tidy: bool
     dependency_overrides: dict[str, str]
+    compresslevel: int | None
+    compression_type: str | None
 
 
 def create_archive_config(config: dict[str, Any] | None = None) -> ArchiveConfig:
     # Keep the same order here as in ArchiveConfig definition
     config = {} if config is None else config.copy()
     config.setdefault("use_module_proxy", DEFAULT_USE_MODULE_PROXY)
     config.setdefault("use_top_level_dir", DEFAULT_USE_TOP_LEVEL_DIR)
     config.setdefault("pre_commands", [])
     config.setdefault("post_commands", [])
     config.setdefault("tidy", DEFAULT_TIDY)
     config.setdefault("dependency_overrides", {})
+    config.setdefault(
+        "compresslevel",
+        DEFAULT_COMPRESSLEVEL_STR if DEFAULT_COMPRESSLEVEL_STR else None,
+    )
+    if config["compresslevel"] is not None:
+        config["compresslevel"] = int(config["compresslevel"])
+    config.setdefault("compression_type", None)
     return cast(ArchiveConfig, config)
 
 
 def get_go_dependency_update_commands(
     dependency_overrides: Mapping[str, str]
 ) -> Iterator[tuple[str, ...]]:
     for ipath, version in dependency_overrides.items():
```

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/config/base.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/config/licenses.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/askalono.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/base.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/load.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/src/go_vendor_tools/license_detection/trivy.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/integration/autorestic/autorestic.spec` & `go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/integration/autorestic/go-vendor-tools.toml` & `go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/integration/fzf/expected-licenses.list` & `go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,31 @@
 %license %dir /usr/share/licenses/not-fzf
+%license %dir /usr/share/licenses/not-fzf/src
+%license %dir /usr/share/licenses/not-fzf/vendor
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/gdamore
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/gdamore/encoding
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/gdamore/tcell
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/gdamore/tcell/v2
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/lucasb-eyer
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/lucasb-eyer/go-colorful
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/mattn
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/mattn/go-isatty
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/mattn/go-runewidth
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/mattn/go-shellwords
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/rivo
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/rivo/uniseg
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/saracen
+%license %dir /usr/share/licenses/not-fzf/vendor/github.com/saracen/walker
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org/x
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org/x/sync
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org/x/sys
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org/x/term
+%license %dir /usr/share/licenses/not-fzf/vendor/golang.org/x/text
 %license /usr/share/licenses/not-fzf/LICENSE
 %license /usr/share/licenses/not-fzf/src/LICENSE
 %license /usr/share/licenses/not-fzf/vendor/github.com/gdamore/encoding/LICENSE
 %license /usr/share/licenses/not-fzf/vendor/github.com/gdamore/tcell/v2/AUTHORS
 %license /usr/share/licenses/not-fzf/vendor/github.com/gdamore/tcell/v2/LICENSE
 %license /usr/share/licenses/not-fzf/vendor/github.com/lucasb-eyer/go-colorful/LICENSE
 %license /usr/share/licenses/not-fzf/vendor/github.com/mattn/go-isatty/LICENSE
```

### Comparing `go_vendor_tools-0.3.0/tests/integration/fzf/fzf.spec` & `go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 %if %{undefined el9}
 SourceLicense:  MIT
 %endif
 License:        Apache-2.0 AND BSD-3-Clause AND MIT
 URL:            %{gourl}
 Source0:        %{gosource}
-Source1:        fzf-%{version}-vendor.tar.xz
+Source1:        fzf-%{version}-vendor.tar.bz2
 Source2:        expected-licenses.list
 
 BuildRequires:  go-vendor-tools
 
 %description %{common_description}
 
 %prep
```

### Comparing `go_vendor_tools-0.3.0/tests/pytests/test_go_vendor_tools.py` & `go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/pytests/test_licensing.py` & `go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/tests/pytests/test_data/case2/licenses/LICENSE` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/README.md` & `go_vendor_tools-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/pyproject.toml` & `go_vendor_tools-0.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
 ]
 dependencies = [
+    "zstarfile",
     "license_expression",
     "tomli; python_version<'3.11'"
 ]
 requires-python = ">=3.9"
 
 [project.scripts]
 go_vendor_archive = "go_vendor_tools.cli.go_vendor_archive:main"
```

### Comparing `go_vendor_tools-0.3.0/LICENSES/BSD-3-Clause.txt` & `go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/LICENSES/MIT.txt` & `go_vendor_tools-0.4.0b1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.3.0/PKG-INFO` & `go_vendor_tools-0.4.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: go-vendor-tools
-Version: 0.3.0
+Version: 0.4.0b1
 Summary: Tools for handling Go library vendoring in Fedora
 Project-URL: Homepage, https://fedora.gitlab.io/sigs/go/go-vendor-tools/
 Project-URL: Source, https://gitlab.com/fedora/sigs/go/go-vendor-tools
 Project-URL: Issue Tracker, https://gitlab.com/fedora/sigs/go/go-vendor-tools/-/issues
 Project-URL: Changelog, https://fedora.gitlab.io/sigs/go/go-vendor-tools/news/
 Author-email: Maxwell G <maxwell@gtmx.me>
 Maintainer-email: Maxwell G <maxwell@gtmx.me>, Fedora Go SIG <golang@lists.fedoraproject.org>
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: license-expression
 Requires-Dist: tomli; python_version < '3.11'
+Requires-Dist: zstarfile
 Provides-Extra: all
 Requires-Dist: tomlkit; extra == 'all'
 Provides-Extra: codeqa
 Requires-Dist: pymarkdownlnt; extra == 'codeqa'
 Requires-Dist: reuse; extra == 'codeqa'
 Requires-Dist: ruff>=0.3.0; extra == 'codeqa'
 Requires-Dist: shellcheck-py; extra == 'codeqa'
```

