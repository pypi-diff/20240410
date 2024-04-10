# Comparing `tmp/setuptools_pybind11-0.3.2-py3-none-any.whl.zip` & `tmp/setuptools_pybind11-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5097 bytes, number of entries: 6
--rw-r--r--  2.0 unx     7652 b- defN 24-Mar-19 21:39 setuptools_pybind11.py
--rw-r--r--  2.0 unx     1070 b- defN 24-Mar-19 21:40 setuptools_pybind11-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1374 b- defN 24-Mar-19 21:40 setuptools_pybind11-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-19 21:40 setuptools_pybind11-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Mar-19 21:40 setuptools_pybind11-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      525 b- defN 24-Mar-19 21:40 setuptools_pybind11-0.3.2.dist-info/RECORD
-6 files, 10733 bytes uncompressed, 4137 bytes compressed:  61.5%
+Zip file size: 6120 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    11180 b- defN 24-Apr-10 02:26 setuptools_pybind11.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-Apr-10 02:43 setuptools_pybind11-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1782 b- defN 24-Apr-10 02:43 setuptools_pybind11-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 02:43 setuptools_pybind11-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-10 02:43 setuptools_pybind11-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      526 b- defN 24-Apr-10 02:43 setuptools_pybind11-0.4.0.dist-info/RECORD
+6 files, 14679 bytes uncompressed, 5160 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: setuptools_pybind11.py
 Comment: 
 
-Filename: setuptools_pybind11-0.3.2.dist-info/LICENSE
+Filename: setuptools_pybind11-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: setuptools_pybind11-0.3.2.dist-info/METADATA
+Filename: setuptools_pybind11-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: setuptools_pybind11-0.3.2.dist-info/WHEEL
+Filename: setuptools_pybind11-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: setuptools_pybind11-0.3.2.dist-info/top_level.txt
+Filename: setuptools_pybind11-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: setuptools_pybind11-0.3.2.dist-info/RECORD
+Filename: setuptools_pybind11-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## setuptools_pybind11.py

```diff
@@ -2,18 +2,24 @@
 from typing import List, Optional, Tuple
 import os
 import shutil
 import pathlib
 import sys
 import subprocess
 
+if sys.version_info.major == 3 and sys.version_info.minor < 11:
+    import tomli  # type: ignore
+else:
+    import tomllib as tomli  # type: ignore
+
 import setuptools
 from setuptools.command.build_ext import build_ext
 
-SOURCE_DIR, _ = os.path.split(__file__)
+from setuptools import build_meta
+
 IS_WINDOWS = sys.platform == "win32"
 
 
 class PyBindModule(setuptools.Extension):
     """
     Defines a single pybind11 module
     """
@@ -230,7 +236,117 @@
         ext_modules=modules,
         *args,
         cmdclass={
             'build_ext': _Build
         },
         **kwargs,
     )
+
+
+__all__ = [
+    'get_requires_for_build_sdist',
+    'get_requires_for_build_wheel',
+    'prepare_metadata_for_build_wheel',
+    'build_wheel',
+    'build_sdist'
+]
+
+
+# subclass the normal setuptools backend
+class _BuildBackend(build_meta._BuildMetaBackend):
+    SOURCE_DIR = "source_dir"
+    BIN_PREFIX = "bin_prefix"
+    DEP_BIN_PREFIXES = "dep_bin_prefixes"
+    INC_DIRS = "inc_dirs"
+    CMAKE_CONFIG = "cmake_config_options"
+    CMAKE_BUILD = "cmake_build_options"
+
+    VALID_KEYS = {
+        SOURCE_DIR,
+        BIN_PREFIX,
+        DEP_BIN_PREFIXES,
+        INC_DIRS,
+        CMAKE_CONFIG,
+        CMAKE_BUILD
+    }
+
+    def run_setup(self, setup_script: str = "setup.py") -> None:
+        # ignore the passed arg, and just directly call
+        # setup here after loading the pyproject args
+        with open("pyproject.toml", mode='rb') as f:
+            project = tomli.load(f)
+
+        try:
+            moduleConfigs = project["tool"]["setuptools-pybind11"]["modules"]
+        except KeyError:
+            logging.warn("No pybind11 modules defined, exitting")
+            return
+
+        modules = []
+
+        for moduleName, configs in moduleConfigs.items():
+            badKey = False
+            for key in configs.keys():
+                if key not in self.VALID_KEYS:
+                    logging.error(
+                        f"Unknown config key tools.setuptools-pybind11.modules.{moduleName}.{key}"
+                    )
+                    badKey = True
+
+            if badKey:
+                raise RuntimeError("Invalid config keys")
+
+            try:
+                sourceDir = configs["source_dir"]
+            except KeyError:
+                sourceDir = "."
+
+            # make source dir relative to pyproject.toml
+            if not os.path.isabs(sourceDir):
+                sourceDir = os.path.abspath(sourceDir)
+
+            try:
+                binPrefix = configs["bin_prefix"]
+            except KeyError:
+                binPrefix = ""
+
+            try:
+                depBinPrefixes = configs['dep_bin_prefixes']
+            except KeyError:
+                depBinPrefixes = []
+
+            try:
+                incDirs = configs["inc_dirs"]
+            except KeyError:
+                incDirs = []
+
+            try:
+                cmakeConfigOptions = configs["cmake_config_options"]
+            except KeyError:
+                cmakeConfigOptions = []
+
+            try:
+                cmakeBuildOptions = configs["cmake_build_options"]
+            except KeyError:
+                cmakeBuildOptions = []
+
+            modules.append(
+                PyBindModule(
+                    module_name=moduleName,
+                    source_dir=sourceDir,
+                    bin_prefix=binPrefix,
+                    dep_bin_prefixes=depBinPrefixes,
+                    inc_dirs=incDirs,
+                    cmake_config_options=cmakeConfigOptions,
+                    cmake_build_options=cmakeBuildOptions
+                )
+            )
+
+        setup(modules=modules)
+
+
+build_meta._BACKEND = _BuildBackend()
+get_requires_for_build_wheel = build_meta._BACKEND.get_requires_for_build_wheel
+get_requires_for_build_sdist = build_meta._BACKEND.get_requires_for_build_sdist
+prepare_metadata_for_build_wheel = build_meta._BACKEND.prepare_metadata_for_build_wheel
+build_wheel = build_meta._BACKEND.build_wheel
+build_sdist = build_meta._BACKEND.build_sdist
```

## Comparing `setuptools_pybind11-0.3.2.dist-info/LICENSE` & `setuptools_pybind11-0.4.0.dist-info/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Ben Kimbrough
+Copyright (c) 2024 Ben "Alagyn" Kimbrough
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

