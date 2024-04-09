# Comparing `tmp/foamlib-0.2.5.tar.gz` & `tmp/foamlib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.5.tar", last modified: Mon Apr  8 19:15:25 2024, max compression
+gzip compressed data, was "foamlib-0.2.6.tar", last modified: Tue Apr  9 18:30:49 2024, max compression
```

## Comparing `foamlib-0.2.5.tar` & `foamlib-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-08 19:15:15.000000 foamlib-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 19:15:25.248138 foamlib-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-08 19:15:15.000000 foamlib-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.244138 foamlib-0.2.5/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.244138 foamlib-0.2.5/foamlib/_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_dictionaries/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:15.000000 foamlib-0.2.5/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 19:15:25.000000 foamlib-0.2.5/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-08 19:15:15.000000 foamlib-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:15:25.248138 foamlib-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:15:25.248138 foamlib-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_flange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_flange_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_pitz.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 19:15:15.000000 foamlib-0.2.5/tests/test_pitz_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:49.396471 foamlib-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-09 18:30:44.000000 foamlib-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 18:30:49.396471 foamlib-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 18:30:44.000000 foamlib-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:49.392471 foamlib-0.2.6/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:49.392471 foamlib-0.2.6/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:44.000000 foamlib-0.2.6/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:49.392471 foamlib-0.2.6/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 18:30:49.000000 foamlib-0.2.6/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 18:30:49.000000 foamlib-0.2.6/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:30:49.000000 foamlib-0.2.6/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 18:30:49.000000 foamlib-0.2.6/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:30:49.000000 foamlib-0.2.6/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 18:30:44.000000 foamlib-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:30:49.396471 foamlib-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:30:49.392471 foamlib-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-09 18:30:44.000000 foamlib-0.2.6/tests/test_serialization.py
```

### Comparing `foamlib-0.2.5/LICENSE.txt` & `foamlib-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.5/PKG-INFO` & `foamlib-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.5/README.md` & `foamlib-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.5/foamlib/_cases.py` & `foamlib-0.2.6/foamlib/_cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import sys
-import os
 import asyncio
 import multiprocessing
+import os
 import shutil
-
-from pathlib import Path
+import sys
 from contextlib import asynccontextmanager
+from pathlib import Path
 from typing import (
     Optional,
     Union,
     overload,
 )
 
 if sys.version_info >= (3, 9):
     from collections.abc import (
-        Collection,
-        Mapping,
-        Set,
-        Sequence,
         AsyncGenerator,
         Callable,
+        Collection,
         Iterator,
+        Mapping,
+        Sequence,
+        Set,
     )
 else:
-    from typing import Collection, Mapping, Sequence, AsyncGenerator, Callable, Iterator
     from typing import AbstractSet as Set
+    from typing import AsyncGenerator, Callable, Collection, Iterator, Mapping, Sequence
 
 import aioshutil
 
-from ._util import is_sequence, run_process, run_process_async, CalledProcessError
-from ._dictionaries import FoamFile, FoamFieldFile
+from ._dictionaries import FoamFieldFile, FoamFile
+from ._util import CalledProcessError, is_sequence, run_process, run_process_async
 
 
 class FoamCaseBase(Sequence["FoamCaseBase.TimeDirectory"]):
     def __init__(self, path: Union[Path, str]):
         self.path = Path(path).absolute()
         if not self.path.is_dir():
             raise NotADirectoryError(f"{self.path} is not a directory")
@@ -50,24 +49,20 @@
         def __init__(self, path: Union[Path, str]):
             self.path = Path(path).absolute()
             if not self.path.is_dir():
                 raise NotADirectoryError(f"{self.path} is not a directory")
 
         @property
         def time(self) -> float:
-            """
-            The time that corresponds to this directory.
-            """
+            """The time that corresponds to this directory."""
             return float(self.path.name)
 
         @property
         def name(self) -> str:
-            """
-            The name of this time directory.
-            """
+            """The name of this time directory."""
             return self.path.name
 
         def __getitem__(self, key: str) -> FoamFieldFile:
             try:
                 return FoamFieldFile(self.path / key)
             except FileNotFoundError as e:
                 raise KeyError(key) from e
@@ -168,31 +163,27 @@
         def ignore(path: Union[Path, str], names: Collection[str]) -> Collection[str]:
             paths = {Path(path) / name for name in names}
             return {p.name for p in paths.intersection(clean_paths)}
 
         return ignore
 
     def _clean_script(self) -> Optional[Path]:
-        """
-        Return the path to the (All)clean script, or None if no clean script is found.
-        """
+        """Return the path to the (All)clean script, or None if no clean script is found."""
         clean = self.path / "clean"
         all_clean = self.path / "Allclean"
 
         if clean.is_file():
             return clean
         elif all_clean.is_file():
             return all_clean
         else:
             return None
 
     def _run_script(self, *, parallel: Optional[bool]) -> Optional[Path]:
-        """
-        Return the path to the (All)run script, or None if no run script is found.
-        """
+        """Return the path to the (All)run script, or None if no run script is found."""
         run = self.path / "run"
         run_parallel = self.path / "run-parallel"
         all_run = self.path / "Allrun"
         all_run_parallel = self.path / "Allrun-parallel"
 
         if run.is_file() or all_run.is_file():
             if run_parallel.is_file() or all_run_parallel.is_file():
@@ -209,17 +200,15 @@
             run_parallel.is_file() or all_run_parallel.is_file()
         ):
             return run_parallel if run_parallel.is_file() else all_run_parallel
         else:
             return None
 
     def _env(self) -> Mapping[str, str]:
-        """
-        Return the environment variables for this case.
-        """
+        """Return the environment variables for this case."""
         env = os.environ.copy()
         env["PWD"] = str(self.path)
         return env
 
     def _parallel_cmd(
         self, cmd: Union[Sequence[Union[str, Path]], str, Path]
     ) -> Union[Sequence[Union[str, Path]], str]:
@@ -233,104 +222,80 @@
                 cmd[0],
                 "-parallel",
                 *cmd[1:],
             ]
 
     @property
     def name(self) -> str:
-        """
-        The name of the case.
-        """
+        """The name of the case."""
         return self.path.name
 
     def file(self, path: Union[Path, str]) -> FoamFile:
-        """
-        Return a FoamFile object for the given path in the case.
-        """
+        """Return a FoamFile object for the given path in the case."""
         return FoamFile(self.path / path)
 
     @property
     def _nsubdomains(self) -> Optional[int]:
-        """
-        Return the number of subdomains as set in the decomposeParDict, or None if no decomposeParDict is found.
-        """
+        """Return the number of subdomains as set in the decomposeParDict, or None if no decomposeParDict is found."""
         try:
             nsubdomains = self.decompose_par_dict["numberOfSubdomains"]
             if not isinstance(nsubdomains, int):
                 raise TypeError(
                     f"numberOfSubdomains in {self.decompose_par_dict} is not an integer"
                 )
             return nsubdomains
         except FileNotFoundError:
             return None
 
     @property
     def _nprocessors(self) -> int:
-        """
-        Return the number of processor directories in the case.
-        """
+        """Return the number of processor directories in the case."""
         return len(list(self.path.glob("processor*")))
 
     @property
     def application(self) -> str:
-        """
-        The application name as set in the controlDict.
-        """
+        """The application name as set in the controlDict."""
         application = self.control_dict["application"]
         if not isinstance(application, str):
             raise TypeError(f"application in {self.control_dict} is not a string")
         return application
 
     @property
     def control_dict(self) -> FoamFile:
-        """
-        The controlDict file.
-        """
+        """The controlDict file."""
         return self.file("system/controlDict")
 
     @property
     def fv_schemes(self) -> FoamFile:
-        """
-        The fvSchemes file.
-        """
+        """The fvSchemes file."""
         return self.file("system/fvSchemes")
 
     @property
     def fv_solution(self) -> FoamFile:
-        """
-        The fvSolution file.
-        """
+        """The fvSolution file."""
         return self.file("system/fvSolution")
 
     @property
     def decompose_par_dict(self) -> FoamFile:
-        """
-        The decomposeParDict file.
-        """
+        """The decomposeParDict file."""
         return self.file("system/decomposeParDict")
 
     @property
     def block_mesh_dict(self) -> FoamFile:
-        """
-        The blockMeshDict file.
-        """
+        """The blockMeshDict file."""
         return self.file("system/blockMeshDict")
 
     @property
     def transport_properties(self) -> FoamFile:
-        """
-        The transportProperties file.
-        """
+        """The transportProperties file."""
         return self.file("constant/transportProperties")
 
     @property
     def turbulence_properties(self) -> FoamFile:
-        """
-        The turbulenceProperties file.
-        """
+        """The turbulenceProperties file."""
         return self.file("constant/turbulenceProperties")
 
     def __fspath__(self) -> str:
         return str(self.path)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.path})"
@@ -395,15 +360,15 @@
                     cmd,
                     check=check,
                     cwd=self.path,
                     env=self._env(),
                 )
             except CalledProcessError as e:
                 raise RuntimeError(
-                    f"{e.cmd} failed with return code {e.returncode}\n{e.stderr.decode()}"
+                    f"{e.cmd} failed with return code {e.returncode}\n{e.stderr}"
                 ) from None
 
         else:
             script_path = self._run_script(parallel=parallel) if script else None
 
             if script_path is not None:
                 return self.run([script_path], check=check)
@@ -428,29 +393,23 @@
                 self.run(
                     [self.application],
                     parallel=parallel,
                     check=check,
                 )
 
     def block_mesh(self, *, check: bool = True) -> None:
-        """
-        Run blockMesh on this case.
-        """
+        """Run blockMesh on this case."""
         self.run(["blockMesh"], check=check)
 
     def decompose_par(self, *, check: bool = True) -> None:
-        """
-        Decompose this case for parallel running.
-        """
+        """Decompose this case for parallel running."""
         self.run(["decomposePar"], check=check)
 
     def reconstruct_par(self, *, check: bool = True) -> None:
-        """
-        Reconstruct this case after parallel running.
-        """
+        """Reconstruct this case after parallel running."""
         self.run(["reconstructPar"], check=check)
 
     def copy(self, dest: Union[Path, str]) -> "FoamCase":
         """
         Make a copy of this case.
 
         :param dest: The destination path.
@@ -570,15 +529,15 @@
                         cmd,
                         check=check,
                         cwd=self.path,
                         env=self._env(),
                     )
             except CalledProcessError as e:
                 raise RuntimeError(
-                    f"{e.cmd} failed with return code {e.returncode}\n{e.stderr.decode()}"
+                    f"{e.cmd} failed with return code {e.returncode}\n{e.stderr}"
                 ) from None
 
         else:
             script_path = self._run_script(parallel=parallel) if script else None
 
             if script_path is not None:
                 if cpus is None:
@@ -620,29 +579,23 @@
                     [self.application],
                     parallel=parallel,
                     check=check,
                     cpus=cpus,
                 )
 
     async def block_mesh(self, *, check: bool = True) -> None:
-        """
-        Run blockMesh on this case.
-        """
+        """Run blockMesh on this case."""
         await self.run(["blockMesh"], check=check)
 
     async def decompose_par(self, *, check: bool = True) -> None:
-        """
-        Decompose this case for parallel running.
-        """
+        """Decompose this case for parallel running."""
         await self.run(["decomposePar"], check=check)
 
     async def reconstruct_par(self, *, check: bool = True) -> None:
-        """
-        Reconstruct this case after parallel running.
-        """
+        """Reconstruct this case after parallel running."""
         await self.run(["reconstructPar"], check=check)
 
     async def copy(self, dest: Union[Path, str]) -> "AsyncFoamCase":
         """
         Make a copy of this case.
 
         :param dest: The destination path.
```

### Comparing `foamlib-0.2.5/foamlib/_dictionaries/_base.py` & `foamlib-0.2.6/foamlib/_dictionaries/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-
 from abc import abstractmethod
 from dataclasses import dataclass
 from typing import Dict, NamedTuple, Optional, Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Sequence
 else:
@@ -40,11 +39,9 @@
     A value that can be stored in an OpenFOAM dictionary.
     """
 
     _Dict = Dict[str, Union["FoamDictionaryBase.Value", "_Dict"]]
 
     @abstractmethod
     def as_dict(self) -> _Dict:
-        """
-        Return a nested dict representation of the dictionary.
-        """
+        """Return a nested dict representation of the dictionary."""
         raise NotImplementedError
```

### Comparing `foamlib-0.2.5/foamlib/_dictionaries/_files.py` & `foamlib-0.2.6/foamlib/_dictionaries/_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-
 from pathlib import Path
 from typing import (
     Any,
     Optional,
     Tuple,
     Union,
     cast,
@@ -95,17 +94,15 @@
     Use as a context manager to make multiple changes to the file while saving all changes only once at the end.
     """
 
     class Dictionary(
         FoamDictionaryBase,
         MutableMapping[str, Union["FoamFile.Value", "FoamFile.Dictionary"]],
     ):
-        """
-        An OpenFOAM dictionary within a file as a mutable mapping.
-        """
+        """An OpenFOAM dictionary within a file as a mutable mapping."""
 
         def __init__(self, _file: "FoamFile", _keywords: Sequence[str]) -> None:
             self._file = _file
             self._keywords = _keywords
 
         def __getitem__(
             self, keyword: str
@@ -150,17 +147,15 @@
             with self._file:
                 super().clear()
 
         def __repr__(self) -> str:
             return f"{type(self).__qualname__}({self._file}, {self._keywords})"
 
         def as_dict(self) -> FoamDictionaryBase._Dict:
-            """
-            Return a nested dict representation of the dictionary.
-            """
+            """Return a nested dict representation of the dictionary."""
             ret = self._file.as_dict()
 
             for k in self._keywords:
                 assert isinstance(ret, dict)
                 v = ret[k]
                 assert isinstance(v, dict)
                 ret = v
@@ -260,17 +255,15 @@
     def __fspath__(self) -> str:
         return str(self.path)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.path})"
 
     def as_dict(self) -> FoamDictionaryBase._Dict:
-        """
-        Return a nested dict representation of the file.
-        """
+        """Return a nested dict representation of the file."""
         _, parsed = self._read()
         return as_dict(parsed)
 
 
 class FoamFieldFile(FoamFile):
     """An OpenFOAM dictionary file representing a field as a mutable mapping."""
 
@@ -285,17 +278,15 @@
             if key == "value":
                 self._setitem(key, value, assume_field=True)
             else:
                 self._setitem(key, value)
 
         @property
         def type(self) -> str:
-            """
-            Alias of `self["type"]`.
-            """
+            """Alias of `self["type"]`."""
             ret = self["type"]
             if not isinstance(ret, str):
                 raise TypeError("type is not a string")
             return ret
 
         @type.setter
         def type(self, value: str) -> None:
@@ -306,17 +297,15 @@
             self,
         ) -> Union[
             int,
             float,
             Sequence[Union[int, float, Sequence[Union[int, float]]]],
             "NDArray[np.generic]",
         ]:
-            """
-            Alias of `self["value"]`.
-            """
+            """Alias of `self["value"]`."""
             ret = self["value"]
             if not isinstance(ret, (int, float, Sequence)):
                 raise TypeError("value is not a field")
             return cast(Union[int, float, Sequence[Union[int, float]]], ret)
 
         @value.setter
         def value(
@@ -357,17 +346,15 @@
         elif keywords == ("dimensions",):
             self._setitem(keywords, value, assume_dimensions=True)
         else:
             self._setitem(keywords, value)
 
     @property
     def dimensions(self) -> FoamFile.DimensionSet:
-        """
-        Alias of `self["dimensions"]`.
-        """
+        """Alias of `self["dimensions"]`."""
         ret = self["dimensions"]
         if not isinstance(ret, FoamFile.DimensionSet):
             raise TypeError("dimensions is not a DimensionSet")
         return ret
 
     @dimensions.setter
     def dimensions(
@@ -380,17 +367,15 @@
         self,
     ) -> Union[
         int,
         float,
         Sequence[Union[int, float, Sequence[Union[int, float]]]],
         "NDArray[np.generic]",
     ]:
-        """
-        Alias of `self["internalField"]`.
-        """
+        """Alias of `self["internalField"]`."""
         ret = self["internalField"]
         if not isinstance(ret, (int, float, Sequence)):
             raise TypeError("internalField is not a field")
         return cast(Union[int, float, Sequence[Union[int, float]]], ret)
 
     @internal_field.setter
     def internal_field(
@@ -402,15 +387,13 @@
             "NDArray[np.generic]",
         ],
     ) -> None:
         self["internalField"] = value
 
     @property
     def boundary_field(self) -> "FoamFieldFile.BoundariesDictionary":
-        """
-        Alias of `self["boundaryField"]`.
-        """
+        """Alias of `self["boundaryField"]`."""
         ret = self["boundaryField"]
         if not isinstance(ret, FoamFieldFile.BoundariesDictionary):
             assert not isinstance(ret, FoamFile.Dictionary)
             raise TypeError("boundaryField is not a dictionary")
         return ret
```

### Comparing `foamlib-0.2.5/foamlib/_dictionaries/_parsing.py` & `foamlib-0.2.6/foamlib/_dictionaries/_parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-
 from typing import Optional, Tuple
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping, MutableMapping, Sequence
 else:
     from typing import Mapping, MutableMapping, Sequence
 
@@ -12,29 +11,32 @@
     Forward,
     Group,
     Keyword,
     LineEnd,
     Literal,
     Located,
     Opt,
-    ParseResults,
     ParserElement,
+    ParseResults,
     QuotedString,
     Word,
     c_style_comment,
     common,
     cpp_style_comment,
     identbodychars,
     printables,
 )
 
 from ._base import FoamDictionaryBase
 
-_YES = Keyword("yes").set_parse_action(lambda: True)
-_NO = Keyword("no").set_parse_action(lambda: False)
+_SWITCH = (
+    Keyword("yes") | Keyword("true") | Keyword("on") | Keyword("y") | Keyword("t")
+).set_parse_action(lambda: True) | (
+    Keyword("no") | Keyword("false") | Keyword("off") | Keyword("n") | Keyword("f")
+).set_parse_action(lambda: False)
 _DIMENSIONS = (
     Literal("[").suppress() + common.number * 7 + Literal("]").suppress()
 ).set_parse_action(lambda tks: FoamDictionaryBase.DimensionSet(*tks))
 
 
 def _list_of(elem: ParserElement) -> ParserElement:
     return Opt(
@@ -61,17 +63,15 @@
 )
 _FIELD = (Keyword("uniform").suppress() + _TENSOR) | (
     Keyword("nonuniform").suppress() + _list_of(_TENSOR)
 )
 _TOKEN = QuotedString('"', unquote_results=False) | _IDENTIFIER
 _ITEM = Forward()
 _LIST = _list_of(_ITEM)
-_ITEM <<= (
-    _FIELD | _LIST | _DIMENSIONED | _DIMENSIONS | common.number | _YES | _NO | _TOKEN
-)
+_ITEM <<= _FIELD | _LIST | _DIMENSIONED | _DIMENSIONS | common.number | _SWITCH | _TOKEN
 _TOKENS = (
     QuotedString('"', unquote_results=False) | Word(printables.replace(";", ""))
 )[2, ...].set_parse_action(lambda tks: " ".join(tks))
 
 _VALUE = _ITEM ^ _TOKENS
 
 _ENTRY = Forward()
@@ -127,30 +127,26 @@
     return ret
 
 
 def get_value(
     parsed: Parsed,
     keywords: Tuple[str, ...],
 ) -> Optional[FoamDictionaryBase.Value]:
-    """
-    Value of an entry.
-    """
+    """Value of an entry."""
     _, value, _ = parsed[keywords]
     return value
 
 
 def get_entry_locn(
     parsed: Parsed,
     keywords: Tuple[str, ...],
     *,
     missing_ok: bool = False,
 ) -> Tuple[int, int]:
-    """
-    Location of an entry or where it should be inserted.
-    """
+    """Location of an entry or where it should be inserted."""
     try:
         start, _, end = parsed[keywords]
     except KeyError:
         if missing_ok:
             if len(keywords) > 1:
                 _, _, end = parsed[keywords[:-1]]
                 end -= 1
@@ -161,17 +157,15 @@
         else:
             raise
 
     return start, end
 
 
 def as_dict(parsed: Parsed) -> FoamDictionaryBase._Dict:
-    """
-    Return a nested dict representation of the file.
-    """
+    """Return a nested dict representation of the file."""
     ret: FoamDictionaryBase._Dict = {}
     for keywords, (_, value, _) in parsed.items():
         r = ret
         for k in keywords[:-1]:
             assert isinstance(r, dict)
             v = r[k]
             assert isinstance(v, dict)
```

### Comparing `foamlib-0.2.5/foamlib/_dictionaries/_serialization.py` & `foamlib-0.2.6/foamlib/_dictionaries/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sys
-
 from contextlib import suppress
 from typing import Any
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping
 else:
     from typing import Mapping
 
-from ._base import FoamDictionaryBase
 from .._util import is_sequence
+from ._base import FoamDictionaryBase
 
 
-def _serialize_bool(value: Any) -> str:
+def _serialize_switch(value: Any) -> str:
     if value is True:
         return "yes"
     elif value is False:
         return "no"
     else:
         raise TypeError(f"Not a bool: {type(value)}")
 
@@ -31,18 +30,18 @@
 def _serialize_field(value: Any) -> str:
     if is_sequence(value):
         try:
             s = _serialize_list(value)
         except TypeError:
             raise TypeError(f"Not a valid field: {type(value)}") from None
         else:
-            if len(value) < 10:
+            if not is_sequence(value[0]) and len(value) < 10:
                 return f"uniform {s}"
             else:
-                if isinstance(value[0], (int, float)):
+                if not is_sequence(value[0]):
                     kind = "scalar"
                 elif len(value[0]) == 3:
                     kind = "vector"
                 elif len(value[0]) == 6:
                     kind = "symmTensor"
                 elif len(value[0]) == 9:
                     kind = "tensor"
@@ -86,15 +85,15 @@
     with suppress(TypeError):
         return _serialize_dimensioned(value)
 
     with suppress(TypeError):
         return _serialize_list(value)
 
     with suppress(TypeError):
-        return _serialize_bool(value)
+        return _serialize_switch(value)
 
     return str(value)
 
 
 def _serialize_dictionary(value: Any) -> str:
     if isinstance(value, Mapping):
         return "\n".join(serialize_entry(k, v) for k, v in value.items())
```

### Comparing `foamlib-0.2.5/foamlib/_util.py` & `foamlib-0.2.6/foamlib/_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
-import sys
 import subprocess
-
+import sys
 from pathlib import Path
 from typing import Any, Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping, Sequence
 else:
     from typing import Mapping, Sequence
@@ -32,72 +31,80 @@
         or numpy
         and isinstance(value, np.ndarray)
     )
 
 
 CalledProcessError = subprocess.CalledProcessError
 
+if sys.version_info >= (3, 9):
+    CompletedProcess = subprocess.CompletedProcess[str]
+else:
+    CompletedProcess = subprocess.CompletedProcess
+
 
 def run_process(
     cmd: Union[Sequence[Union[str, Path]], str, Path],
     *,
     check: bool = True,
     cwd: Union[None, str, Path] = None,
     env: Union[None, Mapping[str, str]] = None,
-) -> "subprocess.CompletedProcess[bytes]":
+) -> CompletedProcess:
     shell = not is_sequence(cmd)
 
     if sys.version_info < (3, 8):
         if shell:
             cmd = str(cmd)
         else:
             cmd = (str(arg) for arg in cmd)
 
     proc = subprocess.run(
         cmd,
         cwd=cwd,
         env=env,
-        capture_output=True,
+        stdout=asyncio.subprocess.DEVNULL,
+        stderr=asyncio.subprocess.PIPE,
+        text=True,
         shell=shell,
         check=check,
     )
 
     return proc
 
 
 async def run_process_async(
     cmd: Union[Sequence[Union[str, Path]], str, Path],
     *,
     check: bool = True,
     cwd: Union[None, str, Path] = None,
     env: Union[None, Mapping[str, str]] = None,
-) -> "subprocess.CompletedProcess[bytes]":
+) -> CompletedProcess:
     if not is_sequence(cmd):
         proc = await asyncio.create_subprocess_shell(
             str(cmd),
             cwd=cwd,
             env=env,
-            stdout=asyncio.subprocess.PIPE,
+            stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.PIPE,
         )
 
     else:
         if sys.version_info < (3, 8):
             cmd = (str(arg) for arg in cmd)
         proc = await asyncio.create_subprocess_exec(
             *cmd,
             cwd=cwd,
             env=env,
-            stdout=asyncio.subprocess.PIPE,
+            stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.PIPE,
         )
 
     stdout, stderr = await proc.communicate()
 
+    assert stdout is None
     assert proc.returncode is not None
 
-    ret = subprocess.CompletedProcess(cmd, proc.returncode, stdout, stderr)
+    ret = CompletedProcess(cmd, proc.returncode, None, stderr.decode())
 
     if check:
         ret.check_returncode()
 
     return ret
```

### Comparing `foamlib-0.2.5/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.6/foamlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.5/pyproject.toml` & `foamlib-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,13 @@
 
 [tool.mypy]
 packages = [
     "foamlib",
     "tests",
 ]
 strict = true
+
+[tool.ruff.lint]
+extend-select = ["D", "I", "RUF", "UP"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "pep257"
```

