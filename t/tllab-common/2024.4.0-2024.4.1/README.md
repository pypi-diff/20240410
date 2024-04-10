# Comparing `tmp/tllab_common-2024.4.0.tar.gz` & `tmp/tllab_common-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2024.4.0.tar", max compression
+gzip compressed data, was "tllab_common-2024.4.1.tar", max compression
```

## Comparing `tllab_common-2024.4.0.tar` & `tllab_common-2024.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.0/LICENSE
--rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.0/README.md
--rw-r--r--   0        0        0      953 2024-04-05 09:50:18.499420 tllab_common-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.0/tllab_common/__init__.py
--rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.0/tllab_common/findcells.py
--rw-r--r--   0        0        0    10664 2024-04-05 09:44:33.967664 tllab_common-2024.4.0/tllab_common/fit.py
--rw-r--r--   0        0        0    13331 2024-04-05 09:50:19.667419 tllab_common-2024.4.0/tllab_common/io.py
--rw-r--r--   0        0        0    15988 2024-04-05 09:48:59.307476 tllab_common-2024.4.0/tllab_common/misc.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 tllab_common-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.1/LICENSE
+-rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.1/README.md
+-rw-r--r--   0        0        0      963 2024-04-10 14:31:27.762533 tllab_common-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.1/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.1/tllab_common/findcells.py
+-rw-r--r--   0        0        0    11610 2024-04-10 11:07:13.403168 tllab_common-2024.4.1/tllab_common/fit.py
+-rw-r--r--   0        0        0     7924 2024-04-09 12:21:00.201925 tllab_common-2024.4.1/tllab_common/io.py
+-rw-r--r--   0        0        0    19679 2024-04-10 12:13:00.480242 tllab_common-2024.4.1/tllab_common/misc.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 tllab_common-2024.4.1/PKG-INFO
```

### Comparing `tllab_common-2024.4.0/LICENSE` & `tllab_common-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.0/README.md` & `tllab_common-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.0/pyproject.toml` & `tllab_common-2024.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2024.4.0"
+version = "2024.4.1"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
@@ -14,23 +14,24 @@
 untangle = "*"
 pandas  = "*"
 psutil = "*"
 numpy = "*"
 tqdm = "*"
 tifffile = "*"
 czifile = "*"
-"ruamel.yaml" = "^0.17"
+"ruamel.yaml" = "*"
 dill = "*"
 colorcet = "*"
 scipy = "*"
 tiffwrite = "*"
 roifile = "*"
 ipython = "*"
 regex = "*"
 bidict = "*"
+makefun = "*"
 pytest-xdist = { version = "*", optional = true }
 
 [tool.poetry.extras]
 test = ["pytest"]
 transforms = ["SimpleITK-SimpleElastix"]
 bioformats = ["python-javabridge", "python-bioformats"]
```

### Comparing `tllab_common-2024.4.0/tllab_common/findcells.py` & `tllab_common-2024.4.1/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.0/tllab_common/fit.py` & `tllab_common-2024.4.1/tllab_common/fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
 class Exponential2(Fit):
     n_p = 4
     bounds = ((0, None), (0, 1), (0, None), (0, None))
 
     @property
     def p0(self) -> ArrayLike:
-        """ y = A(a*exp(-t/tau_0) + (1-a)*exp(-t/tau_1)
+        """ y = A(a*exp(-t/tau_0) + (1-a)*exp(-t/tau_1))
             return A, a, tau_0, tau_1
         """
         n = len(self.x) // 2
         y0 = np.nanmax(self.y)
         q = Exponential1(self.x[n:], self.y[n:] / y0).p0
         return [np.clip(value, *bound)
                 for value, bound in zip((y0, 1 - q[0], q[1] / 3, q[1]), self.bounds)]
@@ -195,14 +195,35 @@
     # def dfun(self, p, x, diffstep=None):
     #     e0 = np.exp(-x / p[2])
     #     e1 = np.exp(-x / p[3])
     #     return np.vstack((p[1] * e0 + (1 - p[1]) * e1, p[0] * (e0 - e1),
     #                       p[0] * p[1] * e0 / p[2] ** 2, p[0] * (1 - p[1]) * e1 / p[3] ** 2))
 
 
+class Exponential3(Fit):
+    n_p = 6
+    bounds = ((0, None), (0, 1), (0, 1), (0, None), (0, None), (0, None))
+
+    @property
+    def p0(self) -> ArrayLike:
+        """ y = A(a*exp(-t/tau_0) + b*exp(-t/tau_1) + (1-a-b)*exp(-t/tau-2))
+            return A, a, b, tau_0, tau_1, tau_2
+        """
+        n = len(self.x) // 2
+        y0 = np.nanmax(self.y)
+        q = Exponential2(self.x[n:], self.y[n:] / y0).p0
+        return [np.clip(value, *bound)
+                for value, bound in zip((y0, 0.3, 0.3, q[2] / 3, q[3] / 3, q[3]), self.bounds)]
+
+    @staticmethod
+    def fun(p: ArrayLike, x: Number | ArrayLike) -> ArrayLike:
+        return p[0] * (p[1] * np.exp(-x / p[3]) + p[2] * np.exp(-x / p[4]) +
+                       (1 - p[1] - p[2]) * np.exp(-x / p[5]))
+
+
 class Powerlaw(Fit):
     n_p = 2
 
     @property
     def p0(self) -> ArrayLike:
         """ y = (x/tau)^alpha
             return alpha, tau
@@ -271,35 +292,38 @@
     """
     eps = np.spacing(1)
     a = np.array(a).flatten()
     y = np.array(y).flatten()
     w = np.ones_like(y) if w is None else np.asarray(w).flatten()
     s = np.ones_like(y) if s is None else np.asarray(s).flatten()
 
-    n_data = np.size(y)
-    n_par = np.size(a)
-    f0 = np.array(fun(a, *args)).flatten()
-    chisq = np.sum(((f0 - y) * w / s) ** 2) / (n_data - n_par)
-
-    # calculate R^2
-    sstot = np.sum((y - np.nanmean(y)) ** 2)
-    ssres = np.sum((y - f0) ** 2)
-    r_squared = 1 - ssres / sstot
-
-    # calculate derivatives
-    deriv = np.zeros((n_data, n_par), dtype='complex')
-    for i in range(n_par):
-        ah = a.copy()
-        ah[i] = a[i] * (1 + diffstep) + eps
-        f = np.array(fun(ah, *args)).flatten()
-        deriv[:, i] = (f - f0) / (ah[i] - a[i]) * w / s
-
-    hesse = np.matmul(deriv.T, deriv)
-
-    try:
-        if np.linalg.matrix_rank(hesse) == np.shape(hesse)[0]:
-            da = np.sqrt(chisq * np.diag(np.linalg.inv(hesse)))
-        else:
-            da = np.sqrt(chisq * np.diag(np.linalg.pinv(hesse)))
-    except (Exception,):
-        da = np.full_like(a, np.nan)
-    return chisq.real, 1.96 * da.real, r_squared.real
+    if len(y):
+        n_data = np.size(y)
+        n_par = np.size(a)
+        f0 = np.array(fun(a, *args)).flatten()
+        chisq = np.sum(((f0 - y) * w / s) ** 2) / (n_data - n_par)
+
+        # calculate R^2
+        sstot = np.sum((y - np.nanmean(y)) ** 2)
+        ssres = np.sum((y - f0) ** 2)
+        r_squared = 1 - ssres / sstot
+
+        # calculate derivatives
+        deriv = np.zeros((n_data, n_par), dtype='complex')
+        for i in range(n_par):
+            ah = a.copy()
+            ah[i] = a[i] * (1 + diffstep) + eps
+            f = np.array(fun(ah, *args)).flatten()
+            deriv[:, i] = (f - f0) / (ah[i] - a[i]) * w / s
+
+        hesse = np.matmul(deriv.T, deriv)
+
+        try:
+            if np.linalg.matrix_rank(hesse) == np.shape(hesse)[0]:
+                da = np.sqrt(chisq * np.diag(np.linalg.inv(hesse)))
+            else:
+                da = np.sqrt(chisq * np.diag(np.linalg.pinv(hesse)))
+        except (Exception,):
+            da = np.full_like(a, np.nan)
+        return chisq.real, 1.96 * da.real, r_squared.real
+    else:
+        return np.nan, np.full_like(a, np.nan), np.nan
```

### Comparing `tllab_common-2024.4.0/tllab_common/misc.py` & `tllab_common-2024.4.1/tllab_common/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import re
 import sys
 from abc import ABCMeta
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from glob import glob
+from inspect import signature, Parameter
 from pathlib import Path
 from traceback import format_exc, print_exception
-from typing import Any, Hashable, Sequence
+from typing import Any, Callable, Hashable, Sequence, TypeVar
 
 import numpy as np
 import pandas
 import regex
 from IPython import embed
+from makefun import wraps
 from ruamel import yaml
 
 from .io import get_params, pickle_dump, yaml_load
 
 Number = int | float | complex
 
 
@@ -73,16 +75,15 @@
             else:
                 for key, value in arg:
                     self[key] = value
         for key, value in kwargs.items():
             self[key] = value
 
 
-dumper = yaml.SafeDumper
-dumper.add_representer(Struct, dumper.represent_dict)
+yaml.RoundTripRepresenter.add_representer(Struct, yaml.RoundTripRepresenter.represent_dict)
 
 
 @dataclass
 class ErrorValue:
     """ format a value and its error with equal significance
         example f"value = {ErrorValue(1.23234, 0.34463):.2g}"
     """
@@ -457,12 +458,92 @@
     for key, value in extra_parameters.items():
         if isinstance(value, dict):
             add_extra_parameters(parameters[key], value)
         else:
             parameters[key] = value
 
 
+R = TypeVar('R')
+
+
+def wraps_combine(wrapper: Callable[[Any, ...], Any]) -> Callable[[Any, ...], R]:
+    """ decorator to combine arguments and doc strings of wrapped and wrapper functions,
+        *args and/or **kwargs in wrapped will be replaced by the arguments from wrapper,
+        duplicate arguments will be left in place in wrapped
+
+        example:
+
+        def wrapper(a, b, c, **kwargs):
+            return a + b + c
+
+        @wraps_combine(wrapper)
+        def wrapped(a, d, e=45, *args, f=5, **kwargs):
+            return d * e * wrapper(*args, **kwargs)
+
+        signature: wrapped(a, d, e, b, c, *, f=5, **kwargs)
+    """
+
+    def wrap(wrapped: Callable[[Any, ...], R]) -> Callable[[Any, ...], R]:
+        if isinstance(wrapper, type):
+            sig_wrapper = signature(wrapper.__init__)
+        else:
+            sig_wrapper = signature(wrapper)
+        sig_wrapped = signature(wrapped)
+        p1, n1, k1 = zip(*[(p, p.name, p.kind) for p in sig_wrapped.parameters.values()])
+        p0, n0, k0 = zip(*[(p, p.name, p.kind) for p in sig_wrapper.parameters.values()
+                           if p.kind in (Parameter.VAR_POSITIONAL, Parameter.VAR_KEYWORD) or p.name not in n1])
+
+        idx0a = k0.index(Parameter.VAR_POSITIONAL) if Parameter.VAR_POSITIONAL in k0 else None
+        idx0k = k0.index(Parameter.VAR_KEYWORD) if Parameter.VAR_KEYWORD in k0 else None
+        idx1a = k1.index(Parameter.VAR_POSITIONAL) if Parameter.VAR_POSITIONAL in k1 else None
+        idx1k = k1.index(Parameter.VAR_KEYWORD) if Parameter.VAR_KEYWORD in k1 else None
+
+        if idx1a is not None:
+            if idx0a:
+                new_parameters = [Parameter(p.name, p.kind, annotation=p.annotation) for p in p1[:idx1a]]
+            else:
+                new_parameters = list(p1[:idx1a])
+            if new_parameters[-1].default == Parameter.empty:
+                new_parameters.extend(p0[:idx0k])
+            else:
+                new_parameters.extend([Parameter(p.name, p.kind,
+                                                 default='empty' if p.default == Parameter.empty else p.default,
+                                                 annotation=p.annotation)
+                                       for p in p0[:idx0k]])
+            new_parameters.extend(p1[idx1a + 1:idx1k])
+        elif idx1k is not None:
+            if idx0a is not None:
+                new_parameters = list(p1[:idx1k])
+            else:
+                new_parameters = [Parameter(p.name, p.kind, annotation=p.annotation) for p in p1[:idx1k]]
+            new_parameters.extend([Parameter(p.name, Parameter.KEYWORD_ONLY,
+                                             default='empty' if p.default == Parameter.empty else p.default,
+                                             annotation=p.annotation)
+                                  for p in p0[:(idx0k if idx0a is None else idx0a)]])
+        else:
+            raise ValueError(f'No *args or **kwargs in {wrapped.__name__}{sig_wrapped}')
+        if idx0k is not None:
+            new_parameters.append(p0[idx0k])
+
+        if wrapped.__doc__ and wrapper.__doc__:
+            doc = f"{wrapped.__doc__}\n\ninherited from:\n\n{wrapper.__doc__.lstrip(' ')}"
+        elif wrapped.__doc__:
+            doc = wrapped.__doc__
+        elif wrapper.__doc__:
+            doc = wrapper.__doc__
+        else:
+            doc = None
+
+        @wraps(wrapped, new_sig=sig_wrapper.replace(parameters=new_parameters), doc=doc)
+        def fun(*args: Any, **kwargs: Any) -> R:
+            return wrapped(*args, **kwargs)
+
+        return fun
+
+    return wrap  # type: ignore
+
+
 color = Color()
 get_config = yaml_load
 getConfig = get_config
 getParams = get_params
 objFromDict = Struct
```

### Comparing `tllab_common-2024.4.0/PKG-INFO` & `tllab_common-2024.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab_common
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.10,<4.0
@@ -17,21 +17,22 @@
 Provides-Extra: test
 Provides-Extra: transforms
 Requires-Dist: bidict
 Requires-Dist: colorcet
 Requires-Dist: czifile
 Requires-Dist: dill
 Requires-Dist: ipython
+Requires-Dist: makefun
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pytest-xdist
 Requires-Dist: regex
 Requires-Dist: roifile
-Requires-Dist: ruamel.yaml (>=0.17,<0.18)
+Requires-Dist: ruamel.yaml
 Requires-Dist: scipy
 Requires-Dist: tifffile
 Requires-Dist: tiffwrite
 Requires-Dist: tqdm
 Requires-Dist: untangle
 Project-URL: Repository, https://github.com/Lenstralab/tllab_common
 Description-Content-Type: text/markdown
```

