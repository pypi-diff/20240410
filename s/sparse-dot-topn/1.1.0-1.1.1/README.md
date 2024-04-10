# Comparing `tmp/sparse-dot-topn-1.1.0.tar.gz` & `tmp/sparse-dot-topn-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-dot-topn-1.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "sparse-dot-topn-1.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `sparse-dot-topn-1.1.0.tar` & `sparse-dot-topn-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.clang-format
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.clang-tidy
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.clangd
--rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/ISSUE_TEMPLATE/Bug_report.yml
--rw-r--r--   0        0        0      331 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1509 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/workflows/nonvendored_wheels.yml
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/workflows/test_all_python.yml
--rw-r--r--   0        0        0     3957 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/.gitignore
--rw-r--r--   0        0        0     3385 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/CHANGES.md
--rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/CMakeLists.txt
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2487 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/INSTALLATION.md
--rw-r--r--   0        0        0    11375 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/LICENSE
--rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/NOTICE
--rw-r--r--   0        0        0     8817 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/README.md
--rw-r--r--   0        0        0    17263 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/bench/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/bench/__init__.py
--rw-r--r--   0        0        0     5083 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/bench/bench_scipy_csr.py
--rwxr-xr-x   0        0        0      568 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/mbuild.sh
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      542 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn/__init__.py
--rw-r--r--   0        0        0    14485 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn/api.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn/lib/.gitkeep
--rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn/types.py
--rw-r--r--   0        0        0     3796 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn/unchecked.py
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/CleanUp.cmake
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/ConfigureBuildType.cmake
--rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/ConfigureTarget.cmake
--rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindAvx.cmake
--rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindDependencies.cmake
--rw-r--r--   0        0        0     7670 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindSse.cmake
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/GetCatch2.cmake
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/GetEigen.cmake
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/InstallTarget.cmake
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/SetHomebrew.cmake
--rw-r--r--   0        0        0     1933 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/common.hpp
--rw-r--r--   0        0        0     3744 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/maxheap.hpp
--rw-r--r--   0        0        0    10209 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul.hpp
--rw-r--r--   0        0        0     3636 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_bindings.hpp
--rw-r--r--   0        0        0    14897 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn.hpp
--rw-r--r--   0        0        0     4324 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn_bindings.hpp
--rw-r--r--   0        0        0     4554 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn.hpp
--rw-r--r--   0        0        0     2727 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn_bindings.hpp
--rw-r--r--   0        0        0     1507 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/extension.cpp
--rw-r--r--   0        0        0     8562 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/sp_matmul_bindings.cpp
--rw-r--r--   0        0        0    19297 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/sp_matmul_topn_bindings.cpp
--rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/zip_sp_matmul_topn_bindings.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/tests/_resources.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0    10784 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/tests/test_api.py
--rw-r--r--   0        0        0     9479 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.clang-format
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.clang-tidy
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.clangd
+-rw-r--r--   0        0        0      145 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/ISSUE_TEMPLATE/Bug_report.yml
+-rw-r--r--   0        0        0      331 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/linux.yml
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/macos.yml
+-rw-r--r--   0        0        0     1509 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/nonvendored_wheels.yml
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      647 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/test_all_python.yml
+-rw-r--r--   0        0        0     3957 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.github/workflows/windows.yml
+-rw-r--r--   0        0        0      206 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/.gitignore
+-rw-r--r--   0        0        0     3489 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/CHANGES.md
+-rw-r--r--   0        0        0     2293 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2487 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/INSTALLATION.md
+-rw-r--r--   0        0        0    11375 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/NOTICE
+-rw-r--r--   0        0        0     9799 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/README.md
+-rw-r--r--   0        0        0    17263 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/bench/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/bench/__init__.py
+-rw-r--r--   0        0        0     5083 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/bench/bench_scipy_csr.py
+-rwxr-xr-x   0        0        0      568 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/mbuild.sh
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      542 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn/__init__.py
+-rw-r--r--   0        0        0    14495 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn/api.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn/lib/.gitkeep
+-rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn/types.py
+-rw-r--r--   0        0        0     3796 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn/unchecked.py
+-rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/CleanUp.cmake
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/ConfigureBuildType.cmake
+-rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/ConfigureTarget.cmake
+-rw-r--r--   0        0        0     2097 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindAvx.cmake
+-rw-r--r--   0        0        0      657 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindDependencies.cmake
+-rw-r--r--   0        0        0     7670 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindSse.cmake
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/GetCatch2.cmake
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/GetEigen.cmake
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/InstallTarget.cmake
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/SetHomebrew.cmake
+-rw-r--r--   0        0        0     1933 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/common.hpp
+-rw-r--r--   0        0        0     3744 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/maxheap.hpp
+-rw-r--r--   0        0        0    10209 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul.hpp
+-rw-r--r--   0        0        0     3636 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_bindings.hpp
+-rw-r--r--   0        0        0    14897 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn.hpp
+-rw-r--r--   0        0        0     4324 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn_bindings.hpp
+-rw-r--r--   0        0        0     4554 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn.hpp
+-rw-r--r--   0        0        0     2727 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn_bindings.hpp
+-rw-r--r--   0        0        0     1507 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/extension.cpp
+-rw-r--r--   0        0        0     8562 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/sp_matmul_bindings.cpp
+-rw-r--r--   0        0        0    19297 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/sp_matmul_topn_bindings.cpp
+-rw-r--r--   0        0        0     4373 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/zip_sp_matmul_topn_bindings.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/tests/_resources.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    10792 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/tests/test_api.py
+-rw-r--r--   0        0        0    10461 2022-11-09 12:37:21.000000 sparse-dot-topn-1.1.1/PKG-INFO
```

### Comparing `sparse-dot-topn-1.1.0/.clang-format` & `sparse-dot-topn-1.1.1/.clang-format`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/.github/ISSUE_TEMPLATE/Bug_report.yml` & `sparse-dot-topn-1.1.1/.github/ISSUE_TEMPLATE/Bug_report.yml`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/.github/workflows/nonvendored_wheels.yml` & `sparse-dot-topn-1.1.1/.github/workflows/nonvendored_wheels.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - uses: actions/checkout@v4
       with:
         submodules: true
 
     - uses: actions/setup-python@v5
 
     - name: Install cibuildwheel
-      run: python -m pip install cibuildwheel==2.16.5
+      run: python -m pip install cibuildwheel==2.17.0
 
     - name: Build wheels
       run: python -m cibuildwheel --output-dir wheelhouse
 
     - name: Verify clean directory
       run: git diff --exit-code
       shell: bash
```

### Comparing `sparse-dot-topn-1.1.0/.github/workflows/test.yml` & `sparse-dot-topn-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/.github/workflows/test_all_python.yml` & `sparse-dot-topn-1.1.1/.github/workflows/test_all_python.yml`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/.github/workflows/wheels.yml` & `sparse-dot-topn-1.1.1/.github/workflows/wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - uses: actions/checkout@v4
       with:
         submodules: true
 
     - uses: actions/setup-python@v5
 
     - name: Install cibuildwheel
-      run: python -m pip install cibuildwheel==2.16.5
+      run: python -m pip install cibuildwheel==2.17.0
 
     - name: Build wheels
       run: python -m cibuildwheel --output-dir wheelhouse
       env:
         CIBW_ENVIRONMENT: CMAKE_ARGS="-DSDTN_ENABLE_ARCH_FLAGS=OFF -DSDTN_ENABLE_OPENMP=ON -DSDTN_DISABLE_OPENMP=OFF"
         CIBW_TEST_COMMAND: pytest {project}/tests && python -c "from sparse_dot_topn import _has_openmp_support;assert _has_openmp_support"
         # only build for x86_64; ARM wheels are build seperately
@@ -103,15 +103,15 @@
             -DCMAKE_OSX_DEPLOYMENT_TARGET="10.14" \
             -DCMAKE_BUILD_TYPE=Release \
             -DCMAKE_C_COMPILER=clang \
             -DCMAKE_CXX_COMPILER=clang++ \
             -DCMAKE_INSTALL_PREFIX="/usr/local"
         cmake --build openmp_build --target install --config Release
 
-    - uses: pypa/cibuildwheel@v2.16.5
+    - uses: pypa/cibuildwheel@v2.17.0
       env:
         # only build for ARM; x86_64wheels are build seperately
         CIBW_ARCHS: "arm64"
         CIBW_ENVIRONMENT_MACOS: MACOSX_DEPLOYMENT_TARGET="10.14" CMAKE_ARGS="-DSDTN_ENABLE_ARCH_FLAGS=OFF -DSDTN_ENABLE_OPENMP=ON -DSDTN_DISABLE_OPENMP=OFF -DOpenMP_ROOT=/usr/local"
 
     - name: Verify clean directory
       run: git diff --exit-code
```

### Comparing `sparse-dot-topn-1.1.0/CHANGES.md` & `sparse-dot-topn-1.1.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release history:
 
+## v1.1.1
+
+### Internal
+
+- FIX: Prevent Scipy from dropping columns that are all zero for sub-matrices
+
 ## v1.1.0
 
 Add new function to select top-n from blocks of a sparse matrix matmul.
 Function will return a zipped matrix Z, where Z = [sorted top n results > lower_bound for each row of C_j], where C_j = A.dot(B_j) and where B has been split row-wise into sub-matrices B_j.
 
 ### API
```

### Comparing `sparse-dot-topn-1.1.0/CMakeLists.txt` & `sparse-dot-topn-1.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/CONTRIBUTING.md` & `sparse-dot-topn-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/INSTALLATION.md` & `sparse-dot-topn-1.1.1/INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/LICENSE` & `sparse-dot-topn-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/NOTICE` & `sparse-dot-topn-1.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/README.md` & `sparse-dot-topn-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # sparse\_dot\_topn
 
--------------------------------**WARNING**-------------------------------
+[![MacOS](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/macos.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/macos.yml)
+[![Linux](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/linux.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/linux.yml)
+[![Windows](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/windows.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/windows.yml)
+[![License](https://img.shields.io/github/license/ing-bank/sparse_dot_topn)](https://github.com/ing-bank/sparse_dot_topn/blob/master/LICENSE)
+[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
-Version 1.0 introduces major and potentially breaking changes to the API.
 
-Please see the Migrating section below.
-
--------------------------------**WARNING**-------------------------------
+[![Release_date](https://img.shields.io/github/release-date/ing-bank/sparse_dot_topn)](https://github.com/ing-bank/sparse_dot_topn/releases)
+[![PyPi](https://img.shields.io/pypi/v/sparse-dot-topn.svg)](https://pypi.org/project/sparse-dot-topn/)
+[![Downloads](https://pepy.tech/badge/sparse_dot_topn)](https://pepy.tech/project/sparse_dot_topn)
 
 **sparse\_dot\_topn** provides a fast way to performing a sparse matrix multiplication followed by top-n multiplication result selection.
 
 Comparing very large feature vectors and picking the best matches, in practice often results in performing a sparse matrix multiplication followed by selecting the top-n multiplication results.
 
 **sparse\_dot\_topn** provides a (parallelised) sparse matrix multiplication implementation that integrates selecting the top-n values, resulting in a significantly lower memory footprint and improved performance.
 On Apple M2 Pro over two 20k x 193k TF-IDF matrices **sparse\_dot\_topn** can be up to 6 times faster when retaining the top 10 values per row and utilising 8 cores.
@@ -20,14 +23,16 @@
 
 `sp_matmul_topn` supports `{CSR, CSC, COO}` matrices with `{32, 64}bit {int, float}` data.
 Note that `COO` and `CSC` inputs are converted to the `CSR` format and are therefore slower.
 Two options to further reduce memory requirements are `threshold` and `density`.
 Optionally, the values can be sorted such that the first column for a given row contains the largest value.
 Note that `sp_matmul_topn(A, B, top_n=B.shape[1])` is equal to `sp_matmul(A, B)` and `A.dot(B)`.
 
+**If you are migrating from `v0.*` please see the migration guide below for details.**
+
 ```python
 import scipy.sparse as sparse
 from sparse_dot_topn import sp_matmul, sp_matmul_topn
 
 A = sparse.random(1000, 100, density=0.1, format="csr")
 B = sparse.random(100, 2000, density=0.1, format="csr")
 
@@ -185,8 +190,7 @@
 
 * [Zhe Sun](https://github.com/ymwdalex/)
 * [Ahmet Erdem](https://github.com/aerdem4)
 * [Stephane Collet](https://github.com/stephanecollot)
 * [Particular Miner](https://github.com/ParticularMiner) (no ING affiliation)
 * [Ralph Urlus](https://github.com/RUrlus)
 * [Max Baak](https://github.com/mbaak)
-
```

### Comparing `sparse-dot-topn-1.1.0/bench/README.md` & `sparse-dot-topn-1.1.1/bench/README.md`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/bench/bench_scipy_csr.py` & `sparse-dot-topn-1.1.1/bench/bench_scipy_csr.py`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/mbuild.sh` & `sparse-dot-topn-1.1.1/mbuild.sh`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/pyproject.toml` & `sparse-dot-topn-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core >=0.4.3", "nanobind >=1.3.2"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "sparse_dot_topn"
-version = "1.1.0"
+version = "1.1.1"
 description = "This package boosts a sparse matrix multiplication followed by selecting the top-n multiplication"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     {name = "ING Analytics Wholesale Banking", email = "wbaa@ing.com"},
 ]
 classifiers = [
```

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn/__init__.py` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn/__init__.py`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn/api.py` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -320,22 +320,19 @@
         nrows, c_nc = C.shape
         _nrows.append(nrows)
         ncols.append(c_nc)
         data.append(C.data)
         indptr.append(C.indptr)
         indices.append(C.indices)
 
+    ncols = np.asarray(ncols, int)
+    total_cols = ncols.sum()
     if not np.all(np.diff(_nrows) == 0):
         msg = "Each `C` in `C_mats` should have the same number of rows."
         raise ValueError(msg)
 
     return csr_matrix(
         _core.zip_sp_matmul_topn(
-            top_n=top_n,
-            Z_max_nnz=nrows * top_n,
-            nrows=nrows,
-            B_ncols=np.asarray(ncols, int),
-            data=data,
-            indptr=indptr,
-            indices=indices,
-        )
+            top_n=top_n, Z_max_nnz=nrows * top_n, nrows=nrows, B_ncols=ncols, data=data, indptr=indptr, indices=indices
+        ),
+        shape=(nrows, total_cols),
     )
```

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn/types.py` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn/types.py`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn/unchecked.py` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn/unchecked.py`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/ConfigureBuildType.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/ConfigureBuildType.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/ConfigureTarget.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/ConfigureTarget.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindAvx.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindAvx.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindDependencies.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindDependencies.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/FindSse.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/FindSse.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/cmake/GetEigen.cmake` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/cmake/GetEigen.cmake`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/common.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/common.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/maxheap.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/maxheap.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_bindings.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_bindings.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn_bindings.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/sp_matmul_topn_bindings.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn_bindings.hpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/include/sparse_dot_topn/zip_sp_matmul_topn_bindings.hpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/extension.cpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/extension.cpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/sp_matmul_bindings.cpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/sp_matmul_bindings.cpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/sp_matmul_topn_bindings.cpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/sp_matmul_topn_bindings.cpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/src/sparse_dot_topn_core/src/zip_sp_matmul_topn_bindings.cpp` & `sparse-dot-topn-1.1.1/src/sparse_dot_topn_core/src/zip_sp_matmul_topn_bindings.cpp`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/tests/_resources.py` & `sparse-dot-topn-1.1.1/tests/_resources.py`

 * *Files identical despite different names*

### Comparing `sparse-dot-topn-1.1.0/tests/test_api.py` & `sparse-dot-topn-1.1.1/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     A = sparse.random(1000, 2000, density=0.1, format="csr", dtype=dtype, random_state=rng)
     B = sparse.random(600, 2000, density=0.1, format="csr", dtype=dtype, random_state=rng)
 
     # reference
     C_ref = sp_matmul_topn(A, B.T, top_n=10, threshold=0.01, sort=True)
 
     # zipped C-matrix
-    As = [A[i*200:(i+1)*200] for i in range(5)]  # names-to-match split
+    As = [A[i * 200 : (i + 1) * 200] for i in range(5)]  # names-to-match split
     Bs = [B[:100], B[100:300], B[300:]]  # GT split
 
     Cs = [[sp_matmul_topn(Aj, Bi.T, top_n=10, threshold=0.01, sort=True) for Bi in Bs] for Aj in As]
     C_zips = [zip_sp_matmul_topn(top_n=10, C_mats=Cis) for Cis in Cs]
 
     # stack over names-to-match subparts
     C_stack = sparse.vstack(C_zips, dtype=dtype)
```

### Comparing `sparse-dot-topn-1.1.0/PKG-INFO` & `sparse-dot-topn-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-dot-topn
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package boosts a sparse matrix multiplication followed by selecting the top-n multiplication
 Author-Email: ING Analytics Wholesale Banking <wbaa@ing.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/ing-bank/sparse_dot_topn
 Requires-Python: >=3.8
@@ -13,21 +13,24 @@
 Requires-Dist: psutil
 Requires-Dist: pytest>=4.0.2; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # sparse\_dot\_topn
 
--------------------------------**WARNING**-------------------------------
+[![MacOS](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/macos.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/macos.yml)
+[![Linux](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/linux.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/linux.yml)
+[![Windows](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/windows.yml/badge.svg)](https://github.com/ing-bank/sparse_dot_topn/actions/workflows/windows.yml)
+[![License](https://img.shields.io/github/license/ing-bank/sparse_dot_topn)](https://github.com/ing-bank/sparse_dot_topn/blob/master/LICENSE)
+[![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
-Version 1.0 introduces major and potentially breaking changes to the API.
 
-Please see the Migrating section below.
-
--------------------------------**WARNING**-------------------------------
+[![Release_date](https://img.shields.io/github/release-date/ing-bank/sparse_dot_topn)](https://github.com/ing-bank/sparse_dot_topn/releases)
+[![PyPi](https://img.shields.io/pypi/v/sparse-dot-topn.svg)](https://pypi.org/project/sparse-dot-topn/)
+[![Downloads](https://pepy.tech/badge/sparse_dot_topn)](https://pepy.tech/project/sparse_dot_topn)
 
 **sparse\_dot\_topn** provides a fast way to performing a sparse matrix multiplication followed by top-n multiplication result selection.
 
 Comparing very large feature vectors and picking the best matches, in practice often results in performing a sparse matrix multiplication followed by selecting the top-n multiplication results.
 
 **sparse\_dot\_topn** provides a (parallelised) sparse matrix multiplication implementation that integrates selecting the top-n values, resulting in a significantly lower memory footprint and improved performance.
 On Apple M2 Pro over two 20k x 193k TF-IDF matrices **sparse\_dot\_topn** can be up to 6 times faster when retaining the top 10 values per row and utilising 8 cores.
@@ -37,14 +40,16 @@
 
 `sp_matmul_topn` supports `{CSR, CSC, COO}` matrices with `{32, 64}bit {int, float}` data.
 Note that `COO` and `CSC` inputs are converted to the `CSR` format and are therefore slower.
 Two options to further reduce memory requirements are `threshold` and `density`.
 Optionally, the values can be sorted such that the first column for a given row contains the largest value.
 Note that `sp_matmul_topn(A, B, top_n=B.shape[1])` is equal to `sp_matmul(A, B)` and `A.dot(B)`.
 
+**If you are migrating from `v0.*` please see the migration guide below for details.**
+
 ```python
 import scipy.sparse as sparse
 from sparse_dot_topn import sp_matmul, sp_matmul_topn
 
 A = sparse.random(1000, 100, density=0.1, format="csr")
 B = sparse.random(100, 2000, density=0.1, format="csr")
 
@@ -202,8 +207,7 @@
 
 * [Zhe Sun](https://github.com/ymwdalex/)
 * [Ahmet Erdem](https://github.com/aerdem4)
 * [Stephane Collet](https://github.com/stephanecollot)
 * [Particular Miner](https://github.com/ParticularMiner) (no ING affiliation)
 * [Ralph Urlus](https://github.com/RUrlus)
 * [Max Baak](https://github.com/mbaak)
-
```

