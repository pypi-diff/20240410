# Comparing `tmp/pyquickbench-0.2.0.tar.gz` & `tmp/pyquickbench-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquickbench-0.2.0.tar", last modified: Wed Mar 13 17:34:44 2024, max compression
+gzip compressed data, was "pyquickbench-0.2.1.tar", last modified: Wed Apr 10 21:01:32 2024, max compression
```

## Comparing `pyquickbench-0.2.0.tar` & `pyquickbench-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-03-13 17:34:44.394492 pyquickbench-0.2.0/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1326 2023-02-10 09:29:15.000000 pyquickbench-0.2.0/LICENSE
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-03-13 17:34:44.390367 pyquickbench-0.2.0/PKG-INFO
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2785 2024-02-08 13:53:18.000000 pyquickbench-0.2.0/README.md
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1860 2024-03-13 17:34:22.000000 pyquickbench-0.2.0/pyproject.toml
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-03-13 17:34:44.312999 pyquickbench-0.2.0/pyquickbench/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3170 2024-03-12 21:59:12.000000 pyquickbench-0.2.0/pyquickbench/__init__.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)    50179 2024-03-12 21:59:12.000000 pyquickbench-0.2.0/pyquickbench/_benchmark.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3894 2024-03-12 21:59:12.000000 pyquickbench-0.2.0/pyquickbench/_defaults.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     8407 2024-03-13 17:05:56.000000 pyquickbench-0.2.0/pyquickbench/_time_train.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)    16795 2024-03-12 21:59:12.000000 pyquickbench-0.2.0/pyquickbench/_utils.py
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-03-13 17:34:44.376307 pyquickbench-0.2.0/pyquickbench.egg-info/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-03-13 17:34:44.000000 pyquickbench-0.2.0/pyquickbench.egg-info/PKG-INFO
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      444 2024-03-13 17:34:44.000000 pyquickbench-0.2.0/pyquickbench.egg-info/SOURCES.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)        1 2024-03-13 17:34:44.000000 pyquickbench-0.2.0/pyquickbench.egg-info/dependency_links.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      260 2024-03-13 17:34:44.000000 pyquickbench-0.2.0/pyquickbench.egg-info/requires.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       13 2024-03-13 17:34:44.000000 pyquickbench-0.2.0/pyquickbench.egg-info/top_level.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)      183 2024-01-18 10:03:43.000000 pyquickbench-0.2.0/requirements-docs.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       25 2024-01-04 08:26:02.000000 pyquickbench-0.2.0/requirements-tests.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       32 2024-01-10 08:42:41.000000 pyquickbench-0.2.0/requirements.txt
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)       38 2024-03-13 17:34:44.394492 pyquickbench-0.2.0/setup.cfg
-drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-03-13 17:34:44.369278 pyquickbench-0.2.0/tests/
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2886 2024-01-30 15:39:33.000000 pyquickbench-0.2.0/tests/test_config.py
--rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3400 2024-03-12 21:59:12.000000 pyquickbench-0.2.0/tests/test_simple.py
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.699876 pyquickbench-0.2.1/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1326 2023-02-10 09:29:15.000000 pyquickbench-0.2.1/LICENSE
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-04-10 21:01:32.694675 pyquickbench-0.2.1/PKG-INFO
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2785 2024-02-08 13:53:18.000000 pyquickbench-0.2.1/README.md
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     1860 2024-04-10 20:39:14.000000 pyquickbench-0.2.1/pyproject.toml
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.590066 pyquickbench-0.2.1/pyquickbench/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3866 2024-04-10 20:59:03.000000 pyquickbench-0.2.1/pyquickbench/__init__.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)    50575 2024-04-10 20:45:31.000000 pyquickbench-0.2.1/pyquickbench/_benchmark.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3966 2024-04-10 20:41:22.000000 pyquickbench-0.2.1/pyquickbench/_defaults.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     8514 2024-04-10 17:43:44.000000 pyquickbench-0.2.1/pyquickbench/_time_train.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)    17042 2024-04-10 17:43:11.000000 pyquickbench-0.2.1/pyquickbench/_utils.py
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.687987 pyquickbench-0.2.1/pyquickbench.egg-info/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     6278 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/PKG-INFO
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      444 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)        1 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      260 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/requires.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       13 2024-04-10 21:01:32.000000 pyquickbench-0.2.1/pyquickbench.egg-info/top_level.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)      183 2024-01-18 10:03:43.000000 pyquickbench-0.2.1/requirements-docs.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       25 2024-01-04 08:26:02.000000 pyquickbench-0.2.1/requirements-tests.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       32 2024-01-10 08:42:41.000000 pyquickbench-0.2.1/requirements.txt
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)       38 2024-04-10 21:01:32.700391 pyquickbench-0.2.1/setup.cfg
+drwxrwxrwx   0 gfo       (1000) gfo       (1000)        0 2024-04-10 21:01:32.673478 pyquickbench-0.2.1/tests/
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     2886 2024-01-30 15:39:33.000000 pyquickbench-0.2.1/tests/test_config.py
+-rwxrwxrwx   0 gfo       (1000) gfo       (1000)     3400 2024-03-12 21:59:12.000000 pyquickbench-0.2.1/tests/test_simple.py
```

### Comparing `pyquickbench-0.2.0/LICENSE` & `pyquickbench-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.0/PKG-INFO` & `pyquickbench-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquickbench
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pure Pyton tool to perform time and accuracy benchmarks
 Author-email: Gabriel Fougeron <gabriel.fougeron@hotmail.fr>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Gabriel Fougeron
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.0 Summary: A pure Pyton
+Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.1 Summary: A pure Pyton
 tool to perform time and accuracy benchmarks Author-email: Gabriel Fougeron
 hotmail.fr> License: BSD 2-Clause License Copyright (c) 2021, Gabriel Fougeron
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `pyquickbench-0.2.0/README.md` & `pyquickbench-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.0/pyproject.toml` & `pyquickbench-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "build",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyquickbench"
-version = "0.2.0"
+version = "0.2.1"
 description = "A pure Pyton tool to perform time and accuracy benchmarks"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["Python", "benchmark"]
 authors = [
   {name = "Gabriel Fougeron", email = "gabriel.fougeron@hotmail.fr"},
 ]
```

### Comparing `pyquickbench-0.2.0/pyquickbench/__init__.py` & `pyquickbench-0.2.1/pyquickbench/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,21 +41,22 @@
    
    default_ax_name
    fun_ax_name
    repeat_ax_name
    out_ax_name
    all_reductions
    all_plot_intents
+   all_transforms
    
 """
 
 from ._benchmark  import run_benchmark, plot_benchmark
 
 from ._defaults   import default_ax_name, fun_ax_name, repeat_ax_name, out_ax_name
-from ._defaults   import all_reductions, all_plot_intents
+from ._defaults   import all_reductions, all_plot_intents, all_transforms
 from ._time_train import TimeTrain
 
 
 # Ugly hack to define Sphinx docstrings for variables
 default_ax_name = default_ax_name
 """The default value for benchmarked functions arguments."""
 
@@ -107,7 +108,23 @@
 
    .. rubric:: See Also
 
    * :func:`pyquickbench.plot_benchmark` : Plot benchmarks
    * :data:`pyquickbench.all_reductions` : List of available data reductions
 
 """
+
+all_transforms = all_transforms
+"""Available data transformations.
+
+   List of all available data transformations to be used in :func:`pyquickbench.plot_benchmark`.
+
+   * "pol_growth_order"  : Plots an estimate of :math:`\\alpha` based on consecutive measured values if the data scales as :math:`\\approx n^\\alpha`.
+   * "pol_cvgence_order" :  Plots an estimate of :math:`\\alpha` based on consecutive measured values if the data scales as :math:`\\approx n^{-\\alpha}`.
+
+   See :ref:`sphx_glr__build_auto_examples_tutorial_06-Transforming_values.py` for usage example.
+
+   .. rubric:: See Also
+
+   * :func:`pyquickbench.plot_benchmark` : Plot benchmarks
+
+"""
```

### Comparing `pyquickbench-0.2.0/pyquickbench/_benchmark.py` & `pyquickbench-0.2.1/pyquickbench/_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,17 @@
     else:    
         all_funs_list = [fun for fun in all_funs]
 
     if mode in ["timings", "scalar_output"]:
         n_out = 1
     elif mode == "vector_output":
         n_out, all_out_names = _build_out_names(all_args, setup, all_funs_list)
-            
+    else:
+        raise ValueError(f'Invalid mode: {mode}')
+
     args_shape, res_shape = _build_args_shapes(all_args, all_funs, n_repeat, n_out)
 
     MonotonicAxes_idx = _arg_names_list_to_idx(MonotonicAxes, all_args)
 
     if Load_timings_file:
         
         try:
@@ -477,18 +479,22 @@
     for loaded_axis_len, (axis_name, expected_axis_len) in zip(all_vals.shape, res_shape.items()):
         if not(loaded_axis_len == expected_axis_len):
             raise ValueError(f'Axis {axis_name} of the benchmark results has a length of {loaded_axis_len} instead of the expected {expected_axis_len}.')
             
     n_funs = res_shape[fun_ax_name]
     n_repeat = res_shape[repeat_ax_name]
     n_out = res_shape[out_ax_name]
-     
-    if all_out_names is None:
+    
+    if (all_out_names is None):
         
-        if all_funs is None:
+        if (mode != 'vector_output'):
+            
+            all_out_names_list = [str(idx) for idx in range(n_out)]
+
+        elif all_funs is None:
 
             all_out_names_list = [str(idx) for idx in range(n_out)]
 
         else:
             
             if setup is None:
                 all_out_names_list = [str(idx) for idx in range(n_out)]
@@ -513,14 +519,18 @@
         linestyle_list = [linestyle_list]    
     if not(isinstance(pointstyle_list, list)):
         pointstyle_list = [pointstyle_list]
     
     n_colors = len(color_list)
     n_linestyle = len(linestyle_list)
     n_pointstyle = len(pointstyle_list)
+    
+    if not(transform is None):
+        if not(transform in all_transforms):
+            raise ValueError((f'Unknown transform {transform}. Possible values are: {all_transforms}'))
 
     if plot_intent is None:
         
         plot_intent = {name: 'points' if (i==0) else 'curve_color' for i, name in enumerate(all_args)}
         plot_intent[fun_ax_name] = 'curve_color'
         plot_intent[repeat_ax_name] = 'reduction_min'
         plot_intent[out_ax_name] = 'curve_linestyle'
@@ -632,15 +642,15 @@
             n_points += 1
             idx_points = i
             name_points = name
         elif value == 'same':
             idx_all_same.append(i)
         elif value == 'single_value':
 
-            fixed_idx = _choose_idx_val(name, single_values_idx, single_values_val, all_args, all_fun_names_list)
+            fixed_idx = _choose_idx_val(name, single_values_idx, single_values_val, all_args, all_fun_names_list, all_out_names_list)
             
             if fixed_idx is None:
                 warnings.warn("Arguments single_values_idx / single_values_val were not properly set. A sensible default was provided, but please beware.")
                 fixed_idx = 0
                 
             assert isinstance(fixed_idx, int)
             
@@ -670,15 +680,15 @@
         elif value.startswith("reduction_"):
             n_reductions += 1
             name = value[10:]
             idx_all_reduction[name].append(i)
         else:
             raise ValueError("This error should never be raised")
             
-        relative_idx = _choose_idx_val(name, relative_to_idx, relative_to_val, all_args, all_fun_names_list)
+        relative_idx = _choose_idx_val(name, relative_to_idx, relative_to_val, all_args, all_fun_names_list, all_out_names_list)
         if isinstance(relative_idx, int):
             idx_all_relative.append(i)
             idx_relative.append(relative_idx)   
             
     if (n_points != 1):
         raise ValueError(f"There should be exactly one plot_intent named 'points'. There are currently {n_points}.")
```

### Comparing `pyquickbench-0.2.0/pyquickbench/_defaults.py` & `pyquickbench-0.2.1/pyquickbench/_defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,7 +126,11 @@
     'curve_pointstyle'  ,
     'subplot_grid_x'    ,
     'subplot_grid_y'    ,
 ]
 
 all_plot_intents.extend([f'reduction_{name}' for name in all_reductions])
 
+all_transforms = [
+    'pol_growth_order'  ,
+    'pol_cvgence_order' ,
+]
```

### Comparing `pyquickbench-0.2.0/pyquickbench/_time_train.py` & `pyquickbench-0.2.1/pyquickbench/_time_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import warnings
 import typing
 import numpy.typing
 
 from pyquickbench._defaults import *
 
 class TimeTrain():
-    """ Records elapsed time between interest points in code"""
+    """ Records elapsed time between interest points in code
+    
+    See :ref:`sphx_glr__build_auto_examples_tutorial_10-TimeTrains.py` for usage example.\n
+    
+    """
     
     def __init__(
         self                                                    ,
         path_prefix         : typing.Union[str , None] = None   ,
         include_locs        : typing.Union[bool, None] = None   ,
         include_filename    : bool = True                       ,
         include_lineno      : bool = True                       ,
```

### Comparing `pyquickbench-0.2.0/pyquickbench/_utils.py` & `pyquickbench-0.2.1/pyquickbench/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,28 +215,32 @@
             break
     
     if not(FoundValidRes):
         raise ValueError("Could not find a single valid result in the whole benchmark !")
 
     if isinstance(res, TimeTrain):
         if res.names_reduction is None:
-            res = res.to_dict()
-        else:
             res = res.to_dict(names_reduction=all_reductions['sum'])
+        else:
+            res = res.to_dict()
 
     if isinstance(res, float):
         n_out = 1
         all_out_names = ["0"]
     elif isinstance(res, dict):
         n_out = len(res)
         all_out_names = list(res.keys())
     else:
-        n_out = len(res)
-        n_fig = 1 + math.floor(math.log(n_out) / math.log(10))
-        all_out_names = [str(i).zfill(n_fig) for i in range(n_out)]
+        try:
+            n_out = len(res)
+        except TypeError:
+            raise ValueError("Could not determine size of output")            
+            
+        n_fill = 1 + math.floor(math.log(n_out) / math.log(10))
+        all_out_names = [str(i).zfill(n_fill) for i in range(n_out)]
             
     return n_out, all_out_names
 
 class FakeProgressBar(object):
     def __init__(self, *args, **kwargs):
         pass
      
@@ -265,17 +269,17 @@
                 except TypeError: 
                     setup_vars_dict_cp = copy.copy(setup_vars_dict)
                     
                 res = fun(**setup_vars_dict_cp)
                 
                 if isinstance(res, TimeTrain):
                     if res.names_reduction is None:
-                        res = res.to_dict()
-                    else:
                         res = res.to_dict(names_reduction=all_reductions['sum'])
+                    else:
+                        res = res.to_dict()
                 
                 if isinstance(res, float):
                     assert n_out == 1
                     vals[i_fun, i_repeat, :] = res
                     
                 elif isinstance(res, np.ndarray):
                     assert res.ndim == 1
@@ -443,29 +447,31 @@
             if KeyValLegend:
                 label += f'{cat_name} : {val_name}, '
             else:
                 label += f'{val_name}, '
             
     return label
 
-def _choose_idx_val(name, all_idx, all_val, all_args, all_fun_names_list):
+def _choose_idx_val(name, all_idx, all_val, all_args, all_fun_names_list, all_out_names_list):
     
     if isinstance(all_idx, dict):
         idx = all_idx.get(name)
     elif isinstance(all_val, dict):
         val = all_val.get(name)
         
         if val is None:
             idx = None
         else:
         
             if name == fun_ax_name:
                 idx = all_fun_names_list.index(val)
             elif name == repeat_ax_name:
                 idx = int(val)
+            elif name == out_ax_name:
+                idx = all_out_names_list.index(val)
             else:
                 search_in = all_args[name]
                 if isinstance(search_in, list):
                     idx = search_in.index(val)
                 elif isinstance(search_in, np.ndarray):
                     idx = np.nonzero(search_in == val)[0]
                 else:
```

### Comparing `pyquickbench-0.2.0/pyquickbench.egg-info/PKG-INFO` & `pyquickbench-0.2.1/pyquickbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquickbench
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pure Pyton tool to perform time and accuracy benchmarks
 Author-email: Gabriel Fougeron <gabriel.fougeron@hotmail.fr>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Gabriel Fougeron
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.0 Summary: A pure Pyton
+Metadata-Version: 2.1 Name: pyquickbench Version: 0.2.1 Summary: A pure Pyton
 tool to perform time and accuracy benchmarks Author-email: Gabriel Fougeron
 hotmail.fr> License: BSD 2-Clause License Copyright (c) 2021, Gabriel Fougeron
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
```

### Comparing `pyquickbench-0.2.0/tests/test_config.py` & `pyquickbench-0.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyquickbench-0.2.0/tests/test_simple.py` & `pyquickbench-0.2.1/tests/test_simple.py`

 * *Files identical despite different names*

