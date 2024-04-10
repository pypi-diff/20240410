# Comparing `tmp/diverge-flow-0.6.0.tar.gz` & `tmp/diverge-flow-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diverge-flow-0.6.0.tar", last modified: Mon Apr  1 05:33:58 2024, max compression
+gzip compressed data, was "diverge-flow-0.6.1.tar", last modified: Wed Apr 10 08:09:18 2024, max compression
```

## Comparing `diverge-flow-0.6.0.tar` & `diverge-flow-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-01 05:33:58.347899 diverge-flow-0.6.0/
--rw-r--r--   0 lennart   (1000) users      (100)    34893 2023-09-01 10:58:44.000000 diverge-flow-0.6.0/LICENSE.md
--rw-r--r--   0 lennart   (1000) users      (100)     3358 2024-04-01 05:33:58.347899 diverge-flow-0.6.0/PKG-INFO
--rw-r--r--   0 lennart   (1000) users      (100)     2725 2024-04-01 05:18:33.000000 diverge-flow-0.6.0/README.md
-drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-01 05:33:58.347899 diverge-flow-0.6.0/diverge_flow.egg-info/
--rw-r--r--   0 lennart   (1000) users      (100)     3358 2024-04-01 05:33:58.000000 diverge-flow-0.6.0/diverge_flow.egg-info/PKG-INFO
--rw-r--r--   0 lennart   (1000) users      (100)      285 2024-04-01 05:33:58.000000 diverge-flow-0.6.0/diverge_flow.egg-info/SOURCES.txt
--rw-r--r--   0 lennart   (1000) users      (100)        1 2024-04-01 05:33:58.000000 diverge-flow-0.6.0/diverge_flow.egg-info/dependency_links.txt
--rw-r--r--   0 lennart   (1000) users      (100)       31 2024-04-01 05:33:58.000000 diverge-flow-0.6.0/diverge_flow.egg-info/requires.txt
--rw-r--r--   0 lennart   (1000) users      (100)        8 2024-04-01 05:33:58.000000 diverge-flow-0.6.0/diverge_flow.egg-info/top_level.txt
--rw-r--r--   0 lennart   (1000) users      (100)      505 2024-04-01 05:33:58.347899 diverge-flow-0.6.0/setup.cfg
--rw-r--r--   0 lennart   (1000) users      (100)      362 2024-04-01 05:18:33.000000 diverge-flow-0.6.0/setup.py
-drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-01 05:33:58.347899 diverge-flow-0.6.0/util/
--rw-r--r--   0 lennart   (1000) users      (100)    58878 2024-04-01 05:18:33.000000 diverge-flow-0.6.0/util/__init__.py
--rw-rw-r--   0 lennart   (1000) users      (100)    26899 2023-09-05 10:03:55.000000 diverge-flow-0.6.0/util/helpers.py
--rwxrwxr-x   0 lennart   (1000) users      (100)  6230480 2024-04-01 05:27:26.000000 diverge-flow-0.6.0/util/libdivERGe.so
--rw-r--r--   0 lennart   (1000) users      (100)    36478 2024-04-01 05:18:33.000000 diverge-flow-0.6.0/util/output.py
+drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-10 08:09:18.636418 diverge-flow-0.6.1/
+-rw-r--r--   0 lennart   (1000) users      (100)    34893 2023-09-01 10:58:44.000000 diverge-flow-0.6.1/LICENSE.md
+-rw-r--r--   0 lennart   (1000) users      (100)     3358 2024-04-10 08:09:18.636418 diverge-flow-0.6.1/PKG-INFO
+-rw-r--r--   0 lennart   (1000) users      (100)     2725 2024-04-01 05:18:33.000000 diverge-flow-0.6.1/README.md
+drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-10 08:09:18.636418 diverge-flow-0.6.1/diverge_flow.egg-info/
+-rw-r--r--   0 lennart   (1000) users      (100)     3358 2024-04-10 08:09:18.000000 diverge-flow-0.6.1/diverge_flow.egg-info/PKG-INFO
+-rw-r--r--   0 lennart   (1000) users      (100)      285 2024-04-10 08:09:18.000000 diverge-flow-0.6.1/diverge_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 lennart   (1000) users      (100)        1 2024-04-10 08:09:18.000000 diverge-flow-0.6.1/diverge_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 lennart   (1000) users      (100)       31 2024-04-10 08:09:18.000000 diverge-flow-0.6.1/diverge_flow.egg-info/requires.txt
+-rw-r--r--   0 lennart   (1000) users      (100)        8 2024-04-10 08:09:18.000000 diverge-flow-0.6.1/diverge_flow.egg-info/top_level.txt
+-rw-r--r--   0 lennart   (1000) users      (100)      505 2024-04-10 08:09:18.636418 diverge-flow-0.6.1/setup.cfg
+-rw-r--r--   0 lennart   (1000) users      (100)      362 2024-04-10 08:08:21.000000 diverge-flow-0.6.1/setup.py
+drwxr-xr-x   0 lennart   (1000) users      (100)        0 2024-04-10 08:09:18.636418 diverge-flow-0.6.1/util/
+-rw-r--r--   0 lennart   (1000) users      (100)    55598 2024-04-10 08:08:21.000000 diverge-flow-0.6.1/util/__init__.py
+-rw-rw-r--   0 lennart   (1000) users      (100)    26899 2023-09-05 10:03:55.000000 diverge-flow-0.6.1/util/helpers.py
+-rwxrwxr-x   0 lennart   (1000) users      (100)  6230480 2024-04-10 08:09:06.000000 diverge-flow-0.6.1/util/libdivERGe.so
+-rw-r--r--   0 lennart   (1000) users      (100)    39152 2024-04-10 08:08:21.000000 diverge-flow-0.6.1/util/output.py
```

### Comparing `diverge-flow-0.6.0/LICENSE.md` & `diverge-flow-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `diverge-flow-0.6.0/PKG-INFO` & `diverge-flow-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diverge-flow
-Version: 0.6.0
+Version: 0.6.1
 Summary: divERGe implements various ERG examples
 Author: Jonas B. Profe, Lennart Klebl
 Author-email: jonas.hauck@rwth-aachen.de, lennart.klebl@rwth-aachen.de
 License: GPLv3
 Keywords: frg,hpc
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: C
```

### Comparing `diverge-flow-0.6.0/README.md` & `diverge-flow-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `diverge-flow-0.6.0/diverge_flow.egg-info/PKG-INFO` & `diverge-flow-0.6.1/diverge_flow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diverge-flow
-Version: 0.6.0
+Version: 0.6.1
 Summary: divERGe implements various ERG examples
 Author: Jonas B. Profe, Lennart Klebl
 Author-email: jonas.hauck@rwth-aachen.de, lennart.klebl@rwth-aachen.de
 License: GPLv3
 Keywords: frg,hpc
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: C
```

### Comparing `diverge-flow-0.6.0/util/__init__.py` & `diverge-flow-0.6.1/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,15 @@
-# Namespace: dvg
-# import diverge::
-# Wrapper for diverge.h, generated with some help of ctypesgen. It is heavily
-# based on wrapping C arrays as numpy structured arrays. Therefore, some
-# documentation for these (and how to use them from <dvg>) is included <below at
-# Structured Arrays>.
-#
-# The documentation only includes those functions that exist *on top* of the <C
-# library at libdivERGe.so>. Everything else is documented <there at
-# libdivERGe.so>. For usage examples, see the python examples shipped with
-# <diverge.tar.gz at
-# https://git.rwth-aachen.de/frg/diverge/-/raw/master/public/releases/v0.2/divERGe.tar.gz>
-# (or found in the <examples/ directory of the repo at
-# https://git.rwth-aachen.de/frg/diverge/-/tree/master/examples>).
-#
-# Note::
-# on linux, the python library will search for libdivERGe.so in your
-# LD_LIBRARY_PATH _with precedence_ over the shipped version (located somewhere
-# in your PYTHONPATH). This makes it easy to swap out the backend by pointing
-# LD_LIBRARY_PATH to a location with the desired libdivERGe.so:
-# === Code ===
-# LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/path/to/gpu/version/ python script.py
-# ============
-
 from diverge.helpers import *
 from diverge.helpers import String, ReturnString, _libs
 from ctypes import *
 
-# Function: info
-# print information on the shared library
 def info():
+    r"""
+    print information on the shared library
+    """
     try:
         info_str = str(_libs["divERGe"].access['cdecl'])
     except:
         info_str = "libdivERGe.so not found, or unable to use it."
     try:
         mpi_py_eprint( info_str )
     except:
@@ -303,26 +280,26 @@
         ('yaxis', c_double * int(3*MAX_ORBS_PER_SITE)),
     ]
 
     generate_symm_trafo_ = _libs["divERGe"].get("diverge_generate_symm_trafo", "cdecl")
     generate_symm_trafo_.argtypes = [ index_t, c_voidp, index_t, c_voidp, index_t, c_voidp, c_voidp ]
     generate_symm_trafo_.restype = None
 
-    # Function: generate_symm_trafo
-    # python version of the symmetry transformation
-    #
-    # Parameters:
-    # n_spin - number of spins
-    # orbs - np.array( ..., dtype=site_descr_t )
-    # syms - np.array( ..., dtype=sym_op_t )
-    #
-    # Returns:
-    # rs_trafo - (3,3) double array
-    # orb_trafo - (n_spin*orbs.size, n_spin*orbs.size) complex128_t array
     def generate_symm_trafo( n_spin, orbs, syms ):
+        r"""
+        python version of the symmetry transformation
+
+        :param n_spin: number of spins
+        :param orbs: np.array( ..., dtype=site_descr_t )
+        :param syms: np.array( ..., dtype=sym_op_t )
+
+        :returns:
+            * rs_trafo; (3,3) double array
+            * orb_trafo; (n_spin*orbs.size, n_spin*orbs.size) :c:type:`complex128_t` array
+        """
         rs_trafo = np.zeros( (3,3), dtype=np.float64 )
         orb_trafo = np.zeros( (n_spin*orbs.size, n_spin*orbs.size), dtype=np.complex128 )
 
         generate_symm_trafo_( n_spin, orbs.ctypes.data, orbs.size,
                              syms.ctypes.data, syms.size, rs_trafo.ctypes.data,
                              orb_trafo.ctypes.data )
         return rs_trafo, orb_trafo
@@ -497,15 +474,15 @@
         ('vert', c_voidp),
         ('tu_ff', c_voidp),
         ('n_tu_ff', index_t),
         ('n_vert_chan', index_t * int(3)),
         ('vfill', channel_vertex_generator_t),
         ('ffill', full_vertex_generator_t),
         ('gfill', greensfunc_generator_t),
-        ('grpoj', greensfunc_generator_t),
+        ('gproj', greensfunc_generator_t),
         ('data', String),
         ('nbytes_data', index_t),
         ('data_destructor', CFUNCTYPE(UNCHECKED(None), POINTER(c_char))),
         ('internals', POINTER(internals_t)),
     ]
 
     # function definitions
@@ -532,25 +509,27 @@
     read_fplo = _libs["divERGe"].get("diverge_read_fplo", "cdecl")
     read_fplo.argtypes = [String]
     read_fplo.restype = POINTER(model_t)
 
     read_W90 = _libs["divERGe"].get("diverge_read_W90_C", "cdecl")
     read_W90.argtypes = [c_char_p,index_t,POINTER(index_t),POINTER(index_t)]
     read_W90.restype = c_void_p
-    # Function: read_W90_PY
-    # returns a numpy array of <rs_hopping_t> with the hoppings from W90 file
-    # and its length
-    #
-    # Parameters:
-    # fname - filename to read W90 data from (usually ..._hr.dat)
-    # nspin - default value 0 amounts to SU(2) symmetric model. if nspin != 0,
-    #         abs(nspin) = (S+1/2)*2 with S the physical spin (i.e., for S=1/2 we
-    #         have abs(nspin)=2). the sign determines whether the spin index is the
-    #         one which increases memory slowly (negative) for fast (positive)
+
     def read_W90_PY( fname, nspin ):
+        """
+        returns a numpy array of :c:struct:`rs_hopping_t` with the hoppings from
+        W90 file. Wraps :c:func:`diverge_read_W90_C` s.t. no messy pointer stuff
+        must be done manually from within python.
+
+        :param fname: filename to read W90 data from (usually ..._hr.dat)
+        :param nspin: default value 0 amounts to SU(2) symmetric model. if nspin != 0,
+                abs(nspin) = (S+1/2)*2 with S the physical spin (i.e., for S=1/2 we
+                have abs(nspin)=2). the sign determines whether the spin index is the
+                one which increases memory slowly (negative) for fast (positive)
+        """
         length = index_t()
         n_orb = index_t(0)
         ptr = POINTER(rs_hopping_t)
         ptr = read_W90( fname.encode('utf-8'), nspin, byref(length), byref(n_orb) )
         pts_ary = view_array( ptr, dtype=rs_hopping_t, shape=(np.array(length),) )
         pts_cpy = np.copy( pts_ary )
         mem_free( ptr )
@@ -632,18 +611,19 @@
 
     class ArgUnion(Union):
         _fields_ = [("np_ibz", index_t),
                     ("max_dist", c_double)]
     model_internals_any_ = _libs["divERGe"].get("diverge_model_internals_any", "cdecl")
     model_internals_any_.argtypes = [POINTER(model_t), String, ArgUnion]
     model_internals_any_.restype = None
-    # Function: model_internals_any_PY
-    # wraps <diverge_model_internals_any> with varargs substituted by kwargs
-    # np_ibz or max_dist.
     def model_internals_any_PY( model, mode, np_ibz=None, max_dist=None ):
+        """
+        wraps :c:func:`diverge_model_internals_any` with varargs substituted by
+        kwargs; np_ibz or max_dist.
+        """
         arg = ArgUnion()
         if not np_ibz is None:
             arg.np_ibz = np_ibz
         if not max_dist is None:
             arg.max_dist = max_dist
         model_internals_any_( model, mode, arg )
 
@@ -888,27 +868,25 @@
     postprocess_and_write.argtypes = [POINTER(flow_step_t), String]
     postprocess_and_write.restype = None
 
     postprocess_and_write_finegrained = _libs["divERGe"].get("diverge_postprocess_and_write_finegrained", "cdecl")
     postprocess_and_write_finegrained.argtypes = [POINTER(flow_step_t), String, POINTER(postprocess_conf_t)]
     postprocess_and_write_finegrained.restype = None
 
-    # Function: postprocess_and_write_PY
-    # wraps <diverge_postprocess_and_write_finegrained at
-    # diverge_postprocess_conf_t.diverge_postprocess_and_write_finegrained> in a
-    # convenient pythonic way.
-    #
-    # Parameters:
-    # step - <diverge_flow_step_t> pointer
-    # filename - string: where to save the postprocessing results
-    # **kwargs - each member of <diverge_postprocess_conf_t> can be passed as
-    #            kwarg (key1 = val1, key2 = val2, …). The defaults are those
-    #            returned by <diverge_postprocess_conf_defaults_CPP at
-    #            diverge_postprocess_conf_t.diverge_postprocess_conf_defaults_CPP>.
     def postprocess_and_write_PY( step, filename, **kwargs ):
+        r"""
+        wraps :c:func:`diverge_postprocess_and_write_finegrained` in a
+        convenient pythonic way.
+
+        :param step: :c:type:`diverge_flow_step_t` pointer
+        :param filename: string where to save the postprocessing results
+        :param \*\*kwargs: each member of :c:struct:`diverge_postprocess_conf_t`
+            can be passed as kwarg (key1 = val1, key2 = val2, …). The defaults
+            are those returned by :c:func:`diverge_postprocess_conf_defaults_CPP`.
+        """
         cfg = postprocess_conf_defaults_CPP()
         for s in struct_postprocess_conf_t.__slots__:
             try:
                 v = kwargs.pop(s)
                 cfg.__setattr__( s, v )
             except KeyError:
                 pass
@@ -956,29 +934,26 @@
     model_to_file_finegrained.argtypes = [POINTER(model_t), String, POINTER(model_output_conf_t)]
     if sizeof(c_int) == sizeof(c_void_p):
         model_to_file_finegrained.restype = ReturnString
     else:
         model_to_file_finegrained.restype = String
         model_to_file_finegrained.errcheck = ReturnString
 
-    # Function: model_to_file_PY
-    # writes a <diverge_model_t> to file using the
-    # <diverge_model_to_file_finegrained at
-    # diverge_model_output_conf_t.diverge_model_to_file_finegrained> backend
-    # wrapped in a convenient pythonic way. Returns the md5sum of the model file
-    # as string.
-    #
-    # Parameters:
-    # model - <diverge_model_t> pointer
-    # filename - string: where to save the model
-    # **kwargs - each member of <diverge_model_output_conf_t> can be passed as
-    #            kwarg (key1 = val1, key2 = val2, …). The defaults are those
-    #            returned by <diverge_model_output_conf_defaults_CPP at
-    #            diverge_model_output_conf_t.diverge_model_output_conf_defaults_CPP>.
     def model_to_file_PY( model, filename, **kwargs ):
+        """
+        function that wraps :c:func:`diverge_model_to_file_finegrained` in a
+        pythonic way.
+
+        :param model: diverge model
+        :param filename: output file name
+        :param \*\*kwargs: keyword arguments, where each member of
+            :c:struct:`diverge_model_output_conf_t` can be passed as kwarg in
+            the form ``key=val``. Defaults are those returned by
+            :c:func:`diverge_model_output_conf_defaults_CPP`.
+        """
         cfg = model_output_conf_defaults_CPP()
         for s in struct_model_output_conf_t.__slots__:
             try:
                 v = kwargs.pop(s)
                 cfg.__setattr__( s, v )
             except KeyError:
                 pass
@@ -995,27 +970,28 @@
     model_generate_mom_basis.argtypes = [(c_double * int(3)) * int(3), (c_double * int(3)) * int(3)]
     model_generate_mom_basis.restype = None
 
     # Patching
     patching_find_fs_pts_C_ = _libs["divERGe"].get("diverge_patching_find_fs_pts_C", "cdecl")
     patching_find_fs_pts_C_.argtypes = [POINTER(model_t), POINTER(c_double), index_t, index_t, index_t, POINTER(POINTER(index_t)), POINTER(index_t)]
     patching_find_fs_pts_C_.restype = None
-    # Function: patching_find_fs_pts_PY
-    # returns a numpy array of <index_t> with the indices of the found patches
-    #
-    # Parameters:
-    # model - <diverge_model_t> pointer
-    # energies - either None or pointer to a double (64bit) floating point array
-    #            that holds energies for nbands bands on the mesh defined in the
-    #            model, i.e. an (nk, nb) array
-    # nbands - number of bands to use. if energies is None, must coincide with the
-    #          number of bands defined in the model
-    # np_ibz - number of patches that should be found in the IBZ
-    # np_ibz_search - number of points that are considered for the patch search
     def patching_find_fs_pts_PY( model, energies, nbands, np_ibz, np_ibz_search ):
+        r"""
+        returns a numpy array of :c:type:`index_t` with the indices of the found
+        patches. wraps :c:func:`diverge_patching_find_fs_pts_C` in a pythonic way.
+
+        :param model: :c:struct:`diverge_model_t` pointer
+        :param energies: either None or pointer to a double (64bit) floating point array
+            that holds energies for nbands bands on the mesh defined in the
+            model, i.e. an (nk, nb) array
+        :param nbands: number of bands to use. if energies is None, must coincide with the
+            number of bands defined in the model
+        :param np_ibz: number of patches that should be found in the IBZ
+        :param np_ibz_search: number of points that are considered for the patch search
+        """
         if energies is None:
             e_ptr = None
         else:
             e_ptr = energies.ctypes.data
         pts = (POINTER(index_t))()
         npts = index_t()
         patching_find_fs_pts_C_( model, e_ptr, nbands, np_ibz,
@@ -1067,22 +1043,27 @@
     merge_rs_orb.argtypes = [POINTER(model_t)]
     merge_rs_orb.restype = None
 
     # Testing
     run_tests_ = _libs["divERGe"].get("diverge_run_tests", "cdecl")
     run_tests_.argtypes = [c_int, POINTER(POINTER(c_char))]
     run_tests_.restype = c_int
-    # Function: run_tests
-    # run all unit tests shipped with divERGe to check health.
-    #
-    # Parameters:
-    # args - list of strings to pass as an argument to CATCH (the testing
-    #        framework). To enable a specific test filter, set args=['[filter]'].
-    #        For example, the BHK tests can be run with args=['[BHK]'].
     def run_tests( args=[] ):
+        r"""
+        run all unit tests shipped with divERGe to check health, wraps
+        :c:func:`diverge_run_tests` without pointer stuff for the argc/argv
+        parameters.
+
+        *Note*: You must initialize the library before calling this function!
+
+        :param args: list of strings to pass as an argument to CATCH (the testing
+               framework). To enable a specific test filter, set
+               args=['[filter]']. For example, the BHK tests can be run with
+               args=['[BHK]'].
+        """
         try:
             arr = (c_char_p * (len(args) + 1))()
             arr[1:] = [ a.encode('utf8') for a in args ]
             arr[0] = b"diverge.py"
             return run_tests_( len(arr), POINTER(POINTER(c_char))(arr) )
         except:
             mpi_py_eprint("could not find test function")
@@ -1129,118 +1110,121 @@
     mom_patching_t = struct_mom_patching_t
     model_t = struct_model_t
     internals_t = struct_internals_t
     tu_formfactor_t = struct_tu_formfactor_t
     flow_step_t = struct_flow_step_t
     euler_t = struct_euler_t
 
-    # Var: numpy
-    # imports numpy in standard fashion (as np)
     import numpy as np
-    # Var: zeros
-    # additionally import zeros from numpy for less namespace pollution
     zeros = np.zeros
 
-    # Function: view_array
-    # give an array view on existing memory
-    #
-    # Parameters:
-    #   dtype - data type that the view is using
-    #   shape - all dimensions (in C ordering) that the view is using
     def view_array( mem, dtype=np.complex128, shape=(1,) ):
+        r"""
+        give an array view on existing memory
+
+        :param dtype: data type that the view is using
+        :param shape: all dimensions (in C ordering) that the view is using
+        """
         dtype = np.dtype(dtype)
         return np.ctypeslib.as_array( cast(mem, POINTER(c_char)), shape=(*shape,dtype.itemsize) ).view( dtype=dtype ).reshape( shape )
 
-    # Function: alloc_array
-    # allocate an array of given data type and shape such that it is not cleared by
-    # the python garbage collector
-    #
-    # Parameters:
-    #   shape - all dimensions (in C ordering)
-    #   dtype - data type. can be <complex128_t>, <rs_hopping_t>, <rs_vertex_t>, or
-    #           <tu_formfactor_t>. data type name must be passed as python string.
     def alloc_array( shape, dtype = "complex128_t" ):
+        r"""
+        allocate an array of given data type and shape such that it is not cleared by
+        the python garbage collector
+
+        :param shape: all dimensions (in C ordering)
+        :param dtype: data type. can be ``"complex128_t"``, ``"rs_hopping_t"``,
+            ``"rs_vertex_t"``, or ``"tu_formfactor_t"``. data type name must be
+            passed *as python string*.
+        """
         if dtype == "complex128_t":
             return view_array( mem_alloc_complex128_t(np.prod(shape)), dtype=np.complex128, shape=shape )
         elif dtype == "rs_hopping_t":
             return view_array( mem_alloc_rs_hopping_t(np.prod(shape)), dtype=struct_rs_hopping_t, shape=shape )
         elif dtype == "rs_vertex_t":
             return view_array( mem_alloc_rs_vertex_t(np.prod(shape)), dtype=struct_rs_vertex_t, shape=shape )
         elif dtype == "tu_formfactor_t":
             return view_array( mem_alloc_tu_formfactor_t(np.prod(shape)), dtype=struct_tu_formfactor_t, shape=shape )
         else:
             mpi_py_eprint("cannot allocate array of type '%s'" % dtype)
             return None
 
     print_ = print
-    # Function: print
-    # wraps the python print function to work with MPI
+
     def print( *args, **kwargs ):
+        """
+        wraps the python print function to work with MPI
+        """
         if mpi_comm_rank() == 0:
             print_( *args, **kwargs )
 
-    # Function: autoflow
-    # simplest possible FRG flow
-    #
-    # Parameters:
-    #   hoppings - numpy array of dtype <rs_hopping_t>, *required*.
-    #   vertex - numpy array of dtype <rs_vertex_t>, *required*.
-    #   nk - number of coarse k points in all three dimensions, *required*.
-    #        Dimensionality of the model is inferred from the nk list by inspecting
-    #        how many nonzero entries exist.
-    #   nkf - number of fine k points in all three dimensions, defaults to 15 in
-    #         each dimension for mode=="grid" or mode=="tu", and to 1 for
-    #         mode=="patch".
-    #   lattice - 3×3 matrix in C order that holds the lattice vectors lattice[0],
-    #             lattice[1], and lattice[2]
-    #   no - number of orbitals and sites
-    #   SU2 - SU2 symmetry setting. If SU2>0, model is assumed to be SU2 symmetric.
-    #         If SU2==0, model is not SU2 symmetric and exchange symmetry in the
-    #         vertex is *not* enforced. for SU2<0, model is not SU2 symmetric, but
-    #         exchange symmetry in the vertex *is* enforced.
-    #   nspin - number of spin indices. For SU2>0, nspin=1 is required. For SU2<=0,
-    #           nspin must be set from physical grounds.
-    #   sites - positions of the orbital centers in real space as array of shape
-    #           (no, 3).
-    #   model_output - output file for the model.
-    #   post_output - output file for postprocessing info.
-    #   flow_output - output file for flow data.
-    #   rs_symmetries - realspace symmetry list as array of shape (nsym, 3, 3). If
-    #                   None, no symmetries are used.
-    #   orb_symmetries - orbital symmetry list as array of shape (nsym, no, no). If
-    #                    None, no symmetries are used.
-    #   mode - backend selection. valid choices are "grid", "patch", and "tu".
-    #   npatches_ibz - number of FS patches in the IBZ used with the "patch"
-    #                  backend.
-    #   formfactor_maxdist - maximal distance up to which formfactors should be
-    #                        included in the "tu" backend.
-    #   channels - selection of channels to be included in the FRG flow. The library
-    #              looks for the characters 'P', 'C', 'D', 'S' in the string that
-    #              stand for the particle particle channel ('P'), the crossed
-    #              particle hole channel ('C'), the direct particle hole channel
-    #              ('D'), and self-energies ('S'), respectively.
-    #   ibz_path - Brillouin zone path in reciprocal crystal coordinates. if empty,
-    #              do not compute band structure
-    #   maxvert - value after which the vertex is considered 'diverged'
-    #   mu - chemical potential. use if mu is not None
-    #   nu - filling value. use if nu is not None. nu has precedence over mu, i.e.
-    #        if both nu and mu are not None, the filling value is used.
-    #
-    # Create the (numpy) arrays with
-    # === Python ===
-    # import diverge as dvg
-    # hoppings = dvg.zeros(shape_h, dtype=dvg.rs_hopping_t)
-    # vertex = dvg.zeros(shape_v, dtype=dvg.rs_vertex_t)
-    # ==============
     def autoflow( hoppings=None, vertex=None, nk=None, nkf=None, lattice=np.eye(3),
                  no=1, SU2=1, nspin=1, sites=[[0,0,0]], model_output="model.dvg",
                  post_output="post.dvg", flow_output="flow.dat", rs_symmetries=None,
                  orb_symmetries=None, mode="tu", npatches_ibz=6,
                  formfactor_maxdist=2.01, channels="PCD", ibz_path=[], maxvert=50.0,
                  mu=None, nu=None ):
+        r"""
+        Function for the simplest possible FRG flow.
+
+        Can be used to get familiar with the library, or to do some extremely
+        rapid coding for a 'standard' FRG run. Outputs to three files by default
+        and has some drastic simplifications built in, with no control left to
+        the user. You are strongly advised to (a) build on top of this function
+        or (b) use the actual API for actual (serious) projects.
+
+        :param hoppings: :c:struct:`rs_hopping_t` array with the hopping
+            elements. Created by ``diverge.zeros((n_hop,),
+            dtype=diverge.rs_hopping_t)``. **required**.
+        :param vertex: :c:struct:`rs_vertex_t` array with the interaction
+            elements. Created by ``diverge.zeros((n_vert,),
+            dtype=diverge.rs_vertex_t)``. **required**.
+        :param nk: length 3 integer tuple for the momentum mesh. **required**.
+        :param nkf: length 3 integer tuple for the refined momentum mesh,
+            default: refinement factor 15
+        :param lattice: (3,3) float64 array for the lattice vectors in C
+            ordering, default: ``np.eye(3)``
+        :param no: number of orbitals, default: 1
+        :param SU2: use :math:`SU(2)` symmetry, default: 1
+        :param nspin: number of spin degrees of freedom
+            (:math:`n_\mathrm{spin}`), default: 1 (since SU(2) is active)
+        :param sites: (n_orb, 3) float64 array for the positions in C ordering
+            (see :c:member:`diverge_model_t.positions`), default: ``[[0,0,0]]``
+        :param model_output: string for the model output file
+            (see :c:func:`diverge_model_to_file`), default: ``"model.dvg"``
+        :param post_output: string for the postprocessing output file
+            (see :c:func:`diverge_postprocess_and_write`), default:
+            ``"post.dvg"``
+        :param flow_output: string for the flow output file (see :ref:`Flow`),
+            default: ``"flow.dat"``
+        :param rs_symmetries: (n_sym, 3, 3) array or None. use these matrices as
+            real-space symmetries (see :ref:`Symmetries`), default: None
+        :param orb_symmetries: (n_sym, n_orb, n_orb) array or None. use these
+            matrices as orbital symmetries, default: None
+        :param mode: string for backend selection, default: ``"tu"``
+        :param npatches_ibz: in case ``mode == "patch"``, the number of patches
+            to look for in the IBZ
+            (see :c:func:`diverge_model_internals_patch`), default: 6
+        :param formfactor_maxdist: in case ``mode == "tu"``, the formfactor
+            cutoff distance (see :c:func:`diverge_model_internals_tu`), default
+            2.01
+        :param channels: string that holds the diagrammatic channels that should
+            be included in the FRG flow (see :c:func:`diverge_flow_step_init`),
+            default: ``"PCD"``
+        :param ibz_path: array that holds the crystalc coordinates of the high
+            symmetry path for band structures
+            (see :c:member:`diverge_model_t.ibz_path`), default: []
+        :param maxvert: value of maximum vertex element that is considered
+            'diverged' (see :c:struct:`diverge_euler_t`).
+        :param mu: chemical potential :math:`\mu`
+            (see :c:func:`diverge_model_set_chempot`), default: None
+        :param nu: filling value :math:`\nu` between zero and one
+            (see :c:func:`diverge_model_set_filling`), default: None
+        """
 
         errors = 0
         init(None, None)
         compilation_status()
 
         if (hoppings is None) or (vertex is None) or (nk is None):
             mpi_py_eprint("must provide hoppings, vertex, and nk")
@@ -1379,23 +1363,25 @@
         mpi_py_eprint( "postprocessing output to %s…" % post_output )
         postprocess_and_write( step, post_output )
 
         flow_step_free( step )
         model_free( model )
         finalize()
 
-    # Class: mpi_stdout_logger
-    # direct output to stdout and a file at the same time. usage:
-    # === Python ===
-    # stdout_ = sys.stdout
-    # sys.stdout = mpi_stdout_logger(filename)
-    # # some code with print() statements
-    # sys.stdout = stdout_
-    # ==============
     class mpi_stdout_logger(object):
+        r"""
+        direct output to stdout and a file at the same time. usage:
+
+        .. sourcecode:: python
+
+            stdout_ = sys.stdout
+            sys.stdout = mpi_stdout_logger(filename)
+            # some code with print() statements
+            sys.stdout = stdout_
+        """
         def __init__(self, fname, mode="w"):
             if mpi_comm_rank() == 0:
                 self.terminal = sys.stdout
                 self.log = open(fname, mode)
         def write(self, message):
             if mpi_comm_rank() == 0:
                 self.terminal.write(message)
@@ -1404,68 +1390,7 @@
             if mpi_comm_rank() == 0:
                 self.terminal.flush()
                 self.log.flush()
 
 else: # _libs["divERGe"] is None
     print( info() )
 
-# Namespace: Structured Arrays
-# DivERGe defines several primitive datatypes (structures) that can be
-# interfaced to from this python library:
-#
-# - <complex128_t>
-# - <rs_hopping_t>
-# - <rs_vertex_t>
-# - <tu_formfactor_t>
-# - <sym_op_t>
-# - <site_descr_t>
-#
-# Allocation:
-# To allocate an array that is *not* garbage collected from python (and can thus
-# be free'd from within divERGe or via <diverge.mem_free at diverge_mem_free>),
-# call <diverge.alloc_array at dvg.alloc_array>. The datatype is passed as
-# *string* to this function, in contrast to what one may be used to from numpy.
-# For standard, garbage-collected allocation, use <diverge.zeros at dvg.zeros>
-# (or just np.zeros):
-# === Python ===
-# hopping_gc = diverge.zeros( (128,), dtype=diverge.rs_hopping_t )
-# hopping_non_gc = diverge.alloc_array( (128,), dtype="rs_hopping_t" )
-# ==============
-#
-# View:
-# A numpy structured array can be used just as any other numpy array (shapes,
-# views, etc). To conveniently use memory owned by divERGe in a pythonic way, we
-# added <diverge.view_array at dvg.view_array>:
-# === Python ===
-# positions = diverge.view_array( model.contents.positions, dtype=np.float64, shape=(12,3) )
-# positions[:] += 1 # now positions are updated!
-# ==============
-#
-# Access:
-# Now to the usage of structured arrays (or array views). If one or more full
-# element(s) is (are) to be set, a (list of) tuple(s) can be passed as so:
-# === Python ===
-# hopping = diverge.alloc_array( (128,), dtype="rs_hopping_t" )
-# hopping[0] = ( [0,0,0], 0,0, 0,0, (1.0,0.0) )
-# hopping[1:3] = [ ( [0,0,0], 1,1, 0,0, (0.2,0.0) ),
-#                  ( [0,0,0], 2,2, 0,0, (0.2,0.0) ) ]
-# ==============
-# This works because the inserted tuples are understood as compatible with the
-# <rs_hopping_t> data type:
-# ---- C/C++ ----
-# // C declaration
-# struct rs_hopping_t {
-#   index_t R[3];
-#   index_t o1,o2, s1,s2;
-#   complex128_t t;
-# };
-# ---------------
-# If only a single member of the structure should be modified or accessed, a
-# dictionary-like syntax is supported:
-# === Python ===
-# vertex = diverge.alloc_array( (128,), dtype="rs_vertex_t" )
-# vertex[0]['chan'] = 'D'
-# vertex[0]['V'] = (3.0,0.0)
-# ==============
-# The keys of this dictionary-like access resemble the names of the members in
-# the respective C declaration.
-
```

### Comparing `diverge-flow-0.6.0/util/helpers.py` & `diverge-flow-0.6.1/util/helpers.py`

 * *Files identical despite different names*

### Comparing `diverge-flow-0.6.0/util/libdivERGe.so` & `diverge-flow-0.6.1/util/libdivERGe.so`

 * *Files identical despite different names*

### Comparing `diverge-flow-0.6.0/util/output.py` & `diverge-flow-0.6.1/util/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import numpy as np
 import math
 
-# Namespace: dvg-output
-# python library to read diverge output files
-
 DIVERGE_MODEL_MAGIC_NUMBER = ord('D') + ord('M')
 DIVERGE_POST_GRID_MAGIC_NUMBER = ord('P')
 DIVERGE_POST_PATCH_MAGIC_NUMBER = ord('V')
 DIVERGE_POST_TU_MAGIC_NUMBER = ord('T')
 
 # return 1 if A>B, -1 if A<B, and 0 if A=B
 def version_compare( A, B ):
@@ -95,79 +92,20 @@
         n_segments = byte_ary_slice[:i8].view(dtype=i64)[0]
         n_per_segment = byte_ary_slice[i8*1 : i8*(1+n_segments)].view(dtype=i64)
         n_path = byte_ary_slice[i8*(1+n_segments):i8*(2+n_segments)].view(dtype=i64)[0]
         path = byte_ary_slice[i8*(2+n_segments):i8*(2+n_segments+n_path)].view(dtype=i64)
         rest = byte_ary_slice[i8*(2+n_segments+n_path):].view(dtype=np.float64)
         return (n_per_segment, path, rest.reshape((-1,3)))
 
-# Class: diverge_model
-# documentation found in docstring, i.e., do the following from within python
-# === Python ===
-# help(diverge_model)
-# ==============
 class diverge_model:
-    """class to read diverge model files
+    """
+    class to read diverge model files (.dvg, "magic number" = 145)
 
-    name: model name
-    version: diverge tag version (serves as file format version)
-    dim: dimension
-    nk[3]: #kpts
-    nkf[3]: #fine kpts
-
-    n_patches: #patches for npatch
-    patches: patch indices wrt coarse kmesh
-    weights: weight of each patch in BZ integral
-    p_count: #refined points per patch
-    p_displ: displacement of refined point array for each patch
-    p_map: refined indices, indexed by p_count/p_displ
-    p_weights: weights of refined indices, indexed by p_count/p_displ
-
-    kc_ibz_path: IBZ path on the coarse momentum mesh as tuple (n_per_segment, path_indices, path_vectors)
-    kf_ibz_path: IBZ path on the fine momentum mesh as tuple (n_per_segment, path_indices, path_vectors)
-
-    ibz_path: IBZ path in crystal coordinates
-
-    n_orb: #orbitals
-    n_spin: #spins
-    SU2: SU2 symmetry?
-    lattice: lattice vectors (3,3)
-    rlattice: reciprocal lattice vectors (3,3)
-    positions: atom positions (n_orb, 3)
-
-    n_sym: #symmetries
-    orb_symmetries: orbital symmetries (n_sym, n_orb*n_spin, n_orb*n_spin)
-    rs_symmetries: realspace symmetries (n_sym, 3, 3)
-
-    n_hop: #hoppings
-    hop: hopping elements (n_hop, custom struct)
-
-    n_vert: #vertex elements
-    vert: vertex elements (n_vert, custom struct)
-
-    len_ff_struct: #formfactors
-    tu_ff: formfactors (len_ff_struct, custom struct)
-
-    n_vert_chan: #vertex elements in each channel (3)
-    data: additional data (bytes)
-
-    kmesh: coarse kmesh (nk[0]*nk[1]*nk[2], 3)
-    kfmesh: fine kmesh (nk[0]*nk[1]*nk[2]*nkf[0]*nkf[1]*nkf[2], 3)
-    ham: hamiltonain on fine kmesh (kfmesh.shape[0], n_spin*n_orb, n_spin*n_orb)
-    U: eigenvectors on fine kmesh (kfmesh.shape[0], n_spin*n_orb, n_spin*n_orb)
-    E: eigenvalues on fine kmesh (kfmesh.shape[0], n_spin*n_orb)
-
-    npath: configuration for bandstructure (nonzero after v0.4.x) if -1, used
-           kf_ibz_path indices. otherwise, bandstructure array is shaped as
-           below
-    bandstructure: banstructure along irreducible path, with irreducible path
-                   in last three indices. shape usually given as
-                   ((ibz_path.size-1)*300+1, n_spin*n_orb + 3) if not specified
-                   differently in model output call.
-    fatbands: if supplied (using npath == -1), contains array of shape
-              (#kf_ibz_path, no_ns, nb) fatbands (nonzero after v0.5.x_dev)
+    :param fname: file name of a divERGe model file that should be read, usually
+                  ``XXX.dvg``.
     """
 
     def _displ_count( self, i_d ):
         return self._f_bytes[self._f_header[i_d]:self._f_header[i_d]+self._f_header[i_d+1]]
     def _head( self, i ):
         return self._f_header[i]
     def _head_displ_count( self, d, c ):
@@ -211,291 +149,359 @@
             names=['R', 'ofrom', 'oto', 'd', 'ffidx'],
             formats=['3i8', 'i8', 'i8', 'f8', 'i8'],
             offsets=self._head_displ_count(119, 5),
             itemsize=self._head(124)))
 
         self._f_bytes = numpy_fromfile(fname, dtype=np.byte)
 
+        #: name given to the model by the user through :c:member:`diverge_model_t.name`
         self.name = self._displ_count( 1 ).tobytes().decode().rstrip('\x00')
+
+        #: diverge tag version (serves as file format version)
         self.version = self._displ_count( 125 ).tobytes().decode()
+        #: dimension
         self.dim = self._head(3)
+        #: number of kpts as (3,) array of :c:type:`index_t`
         self.nk = self._head_displ_count(4,3)
+        #: number of fine kpts as (3,) array of :c:type:`index_t`
         self.nkf = self._head_displ_count(7,3)
 
+        #: number of patches (in case npatch backend was initalized)
         self.n_patches = self._head(10)
+        #: indices of the coarse mesh that are patch centers (n_patches,)
         self.patches = self._displ_count( 11 ).view( dtype=np.int64 )
+        #: weights for each of the patches (n_patches,)
         self.weights = self._displ_count( 13 ).view( dtype=np.float64 )
+        #: descriptor for the ``p_map`` and ``p_weights`` arrays, such that
+        #: ``p_map[p_displ[p]:p_displ[p]+p_count[p]]`` is the slice in the array
+        #: ``p_map`` (in python notation) that makes the refinement for patch ``p``
         self.p_count = self._displ_count( 15 ).view( dtype=np.int64 )
+        #: descriptor for the ``p_map`` and ``p_weights`` arrays, same as above
         self.p_displ = self._displ_count( 17 ).view( dtype=np.int64 )
+
+        #: refinement indices for patches; *relative convention*. Let ``p`` be a
+        #: patch index, ``i`` a refinement index for ``p`` (i.e. between zero and
+        #: ``p_count[p]``). Then, the refinement index ``kfi = p_map[p_displ[p]+i]``
+        #: is the relative shift from the patch center ``patches[p]`` to the
+        #: actual refinement point, i.e., ``kf = k1p2(kfi, patches[p])``.
         self.p_map = self._displ_count( 19 ).view( dtype=np.int64 )
+        #: refinement weights for patches, same indexing convention as ``p_map``.
         self.p_weights = self._displ_count( 21 ).view( dtype=np.float64 )
 
+        #: IBZ path in crystal coordinates
         self.ibz_path = self._displ_count( 23 ).view( dtype=np.float64 ).reshape((-1,3))
 
+        #: number of orbitals
         self.n_orb = self._head(25)
+        #: number of spins :math:`n_\mathrm{spin} = 2S+1`.
         self.n_spin = self._head(46)
+        #: :math:`SU(2)` symmetry?
         self.SU2 = self._head(45)
+        #: lattice vectors as (3,3) array
         self.lattice = self._head_displ_count(26, 9).view( dtype=np.float64 ).reshape((3,3))
+        #: reciprocal lattice vectors as (3,3) array
         self.rlattice = self._head_displ_count(58, 9).view( dtype=np.float64 ).reshape((3,3))
+        #: positions as (n_orb,3) array
         self.positions = self._displ_count( 35 ).view( dtype=np.float64 ).reshape((-1,3))
 
+        #: number of symmetries
         self.n_sym = self._head(37)
+        #: orbital symmetries (n_sym, n_orb*n_spin, n_orb*n_spin)
         self.orb_symmetries = self._displ_count( 38 ).view( dtype=np.complex128 ).reshape(
                 (-1, self.n_orb*self.n_spin, self.n_orb*self.n_spin))
+        #: realspace symmetries (n_sym, 3, 3)
         self.rs_symmetries = self._displ_count( 40 ).view( dtype=np.float64 ).reshape((-1,3,3))
 
+        #: number of hoppings
         self.n_hop = self._head(42)
+        #: hopping elements (n_hop, custom struct)
         self.hop = self._displ_count( 43 ).view( self.rs_hopping_t )
 
+        #: number of vertex elements
         self.n_vert = self._head(47)
+        #: vertex elements (n_vert, custom struct)
         self.vert = self._displ_count( 48 ).view( self.rs_vertex_t )
 
+        #: number of TU formfactors
         self.len_ff_struct = self._head( 50 )
+        #: formfactors (len_ff_struct, custom struct). *Note: usually not
+        #: present without TU internals*.
         self.tu_ff = self._displ_count( 51 ).view( self.tu_formfactor_t )
 
+        #: number of vertex elements in each channel (3)
         self.n_vert_chan = self._head_displ_count( 53, 3 )
+        #: additional data (byte array)
         self.data = self._displ_count( 56 )
 
+        #: coarse kmesh (nk[0]*nk[1]*nk[2], 3).
+        #: *Note: only present if (i) common internals were set at the time of
+        #: saving and (ii) the output config key was set to a non-default, non-zero
+        #: value.*
         self.kmesh = self._displ_count( 80 ).view( np.float64 ).reshape((-1,3))
+        #: fine kmesh (nk[0]*nk[1]*nk[2]*nkf[0]*nkf[1]*nkf[2], 3)
+        #: *Note: only present if (i) common internals were set at the time of
+        #: saving and (ii) the output config key was set to a non-default, non-zero
+        #: value.*
         self.kfmesh = self._displ_count( 82 ).view( np.float64 ).reshape((-1,3))
+        #: hamiltonain on fine kmesh (kfmesh.shape[0], n_spin*n_orb, n_spin*n_orb)
+        #: *Note: only present if (i) common internals were set at the time of
+        #: saving and (ii) the output config key was set to a non-default, non-zero
+        #: value.*
         self.ham = self._displ_count( 84 ).view( np.complex128 ).reshape(
                 (-1,self.n_spin*self.n_orb,self.n_spin*self.n_orb))
+        #: eigenvectors on fine kmesh (kfmesh.shape[0], n_spin*n_orb, n_spin*n_orb)
+        #: *Note: only present if (i) common internals were set at the time of
+        #: saving and (ii) the output config key was set to a non-default, non-zero
+        #: value.*
         self.U = self._displ_count( 86 ).view( np.complex128 ).reshape(
                 (-1,self.n_spin*self.n_orb,self.n_spin*self.n_orb))
+        #: eigenvalues on fine kmesh (kfmesh.shape[0], n_spin*n_orb)
+        #: *Note: only present if (i) common internals were set at the time of
+        #: saving and (ii) the output config key was set to a non-default, non-zero
+        #: value.*
         self.E = self._displ_count( 88 ).view( np.float64 ).reshape((-1,self.n_spin*self.n_orb))
 
+        #: IBZ path on the coarse momentum mesh as tuple (n_per_segment, path_indices, path_vectors)
         self.kc_ibz_path = k_ibz_path( self._displ_count( 90 ) )
+        #: IBZ path on the fine momentum mesh as tuple (n_per_segment, path_indices, path_vectors)
         self.kf_ibz_path = k_ibz_path( self._displ_count( 92 ) )
 
+        #: Configuration for bandstructure (nonzero after v0.4.x). If -1, used
+        #: kf_ibz_path indices. Otherwise, bandstructure array is shaped as below.
         self.npath = self._head(94) # to see what the config actually is
+
+        #: banstructure along irreducible path, with irreducible path
+        #: in last three indices. shape usually given as
+        #: ((ibz_path.size-1)*300+1, n_spin*n_orb + 3) if not specified
+        #: differently in model output call.
         self.bandstructure = self._displ_count( 100 ).view(
                 np.float64 ).reshape((-1,self.n_spin*self.n_orb + 3))
 
+        #: If supplied (using npath == -1 and the corresponding config key),
+        #: contains array of shape (#kf_ibz_path, no_ns, nb) fatbands (nonzero
+        #: after v0.6)
         fatbands = self._displ_count( 98 ).view( np.float64 )
         if fatbands.size == 0:
             self.fatbands = None
         else:
             self.fatbands = fatbands.reshape( (-1, self.n_spin*self.n_orb, self.n_spin*self.n_orb) )
 
-# Class: diverge_post_patch
-# documentation found in docstring, i.e., do the following from within python
-# === Python ===
-# help(diverge_post_patch)
-# ==============
 class diverge_post_patch:
-    '''class to read diverge postprocessing files for $N$-patch FRG
-
-    version: diverge tag version (serves as file format version)
+    r'''
+    class to read diverge postprocessing files for :math:`N`-patch FRG
 
     vertices and loops may be None if not explicitly asked for in the
     postprocessing routines. They all are of shape (np, np, np, nb, nb, nb, nb),
     i.e. refer to the patch indices.
 
-    V: full vertex
-    Lp: particle particle loop
-    Lm: particle hole loop
-    dV: increment of the last step
-
-    for each interaction channel X (X \in \{P,C,D\}), there are the following
+    for each interaction channel X (X :math:`\in \{P,C,D\}`), there are the following
     variables:
 
-    X_chan: boolean that tracks whether this channel is included in the output
-    X_dV: boolean that tracks whether the increment was used (True) or whether
-          the vertex at scale was used (False)
-    X_nq: the number of momentum transfer points
-    X_qV: the vertx in 'q representation'. A list of length X_nq with each
-          element of the list a tuple (q, k_kp_descr, values, vectors).
-          q: transfer momentum
-          k_kp_descr: array of indices of secondary momenta. Refers to the
-                      coarse kmesh. May differ for different q.
-          values: eigenvalues (shape: (nv,) with nv the number of eigenvalues
-                  requested) may be None if no eigendecomposition was done
-          vectors: eigenvectors (shape: (nv, len(k_kp_descr), nb, nb)). if
-                   values is None, nv == len(k_kp_descr)*nb*nb and the array
-                   should represents the vertex at the specified q as matrix
-                   with shape: (len(k_kp_descr), nb, nb, len(k_kp_descr), nb, nb).
+    :X_chan: boolean that tracks whether this channel is included in the output
+    :X_dV: boolean that tracks whether the increment was used (True) or whether
+           the vertex at scale was used (False)
+    :X_nq: the number of momentum transfer points
+    :X_qV: the vertx in 'q representation'. A list of length X_nq with each
+           element of the list a tuple (q, k_kp_descr, values, vectors).
+
+            :q: transfer momentum
+            :k_kp_descr: array of indices of secondary momenta. Refers to the
+                         coarse kmesh. May differ for different q.
+            :values: eigenvalues (shape: (nv,) with nv the number of eigenvalues
+                     requested) may be None if no eigendecomposition was done
+            :vectors: eigenvectors (shape: (nv, len(k_kp_descr), nb, nb)). if
+                      values is None, nv == len(k_kp_descr)*nb*nb and the array
+                      should represents the vertex at the specified q as matrix
+                      with shape: (len(k_kp_descr), nb, nb, len(k_kp_descr), nb, nb).
     '''
     def __init__(self, fname):
         d_header = numpy_fromfile(fname, dtype=np.longlong, count=128)
 
         if d_header[0] == DIVERGE_POST_PATCH_MAGIC_NUMBER:
             self.valid = True
         else:
             self.valid = False
             return
 
         d_data = numpy_fromfile(fname)
         d_data_l = numpy_fromfile(fname, dtype=np.longlong)
 
         if d_header[2] != 0:
+            #: full vertex
             self.V = d_data[ 0+d_header[1] : d_header[1]+d_header[2] : 2 ] \
                + 1j* d_data[ 1+d_header[1] : d_header[1]+d_header[2] : 2 ]
         else:
             self.V = None
         if d_header[4] != 0:
+            #: particle particle loop
             self.Lp = d_data[ 0+d_header[3] : d_header[3]+d_header[4] : 2 ] \
                 + 1j* d_data[ 1+d_header[3] : d_header[3]+d_header[4] : 2 ]
         else:
             self.Lp = None
         if d_header[6] != 0:
+            #: particle hole loop
             self.Lm = d_data[ 0+d_header[5] : d_header[5]+d_header[6] : 2 ] \
                 + 1j* d_data[ 1+d_header[5] : d_header[5]+d_header[6] : 2 ]
         else:
             self.Lm = None
         if d_header[8] != 0:
+            #: increment of the last step
             self.dV = d_data[ 0+d_header[7] : d_header[7]+d_header[8] : 2 ] \
                 + 1j* d_data[ 1+d_header[7] : d_header[7]+d_header[8] : 2 ]
         else:
             self.dV = None
 
         idx = 9
+        #: X = P
         self.P_chan = chr(d_header[idx]); idx = idx+1
+        #: X = P
         self.P_dV = bool(d_header[idx]); idx = idx+1
+        #: X = P
         self.P_nq = d_header[idx]; idx = idx+1
         if d_header[idx+1] > 0:
+            #: X = P
             self.P_qV = qmatrices( d_data, d_header[idx], d_header[idx+1], self.P_nq ); idx = idx+2
         else:
             self.P_qV = None
 
         idx = 14
+        #: X = C
         self.C_chan = chr(d_header[idx]); idx = idx+1
+        #: X = C
         self.C_dV = bool(d_header[idx]); idx = idx+1
+        #: X = C
         self.C_nq = d_header[idx]; idx = idx+1
         if d_header[idx+1] > 0:
+            #: X = C
             self.C_qV = qmatrices( d_data, d_header[idx], d_header[idx+1], self.C_nq ); idx = idx+2
         else:
             self.C_qV = None
 
         idx = 19
+        #: X = D
         self.D_chan = chr(d_header[idx]); idx = idx+1
+        #: X = D
         self.D_dV = bool(d_header[idx]); idx = idx+1
+        #: X = D
         self.D_nq = d_header[idx]; idx = idx+1
         if d_header[idx+1] > 0:
+            #: X = D
             self.D_qV = qmatrices( d_data, d_header[idx], d_header[idx+1], self.D_nq ); idx = idx+2
         else:
             self.D_qV = None
 
+        #: diverge tag version (serves as file format version)
         self.version = d_data[ d_header[125] : d_header[125]+d_header[126] ].view(
                 dtype=np.byte ).tobytes().decode().rstrip('\x00')
 
-# Class: diverge_post_grid
-# documentation found in docstring, i.e., do the following from within python
-# === Python ===
-# help(diverge_post_grid)
-# ==============
 class diverge_post_grid:
-    '''class to read diverge postprocessing files for grid FRG
-
-    version: diverge tag version (serves as file format version)
-
-    nk: number of k points
-    nb: number of bands
-    nff: number of formfactors
-    SU2: SU2 symmetry
-    lingap_num_ev: linearized gap equation number of singular values
-    lingap_matrix_size: linearized gap equation matrix size
-
-    formfac: formfactors (nff,nk)
-
-    P_susc: P susceptibility (nk,nff,nb,nb,nb,nb)
-    P_mf_U: P lingap U matrix (lingap_num_ev,lingap_matrix_size)
-    P_mf_V: P lingap V matrix (lingap_num_ev,lingap_matrix_size)
-    P_mf_S: P lingap singular values (lingap_num_ev)
-    P_mf_EU: P lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
-    P_mf_EV: P lingap vertex eigenvalues (lingap_num_ev)
-    C_susc: C susceptibility (nk,nff,nb,nb,nb,nb)
-    C_mf_U: C lingap U matrix (lingap_num_ev,lingap_matrix_size)
-    C_mf_V: C lingap V matrix (lingap_num_ev,lingap_matrix_size)
-    C_mf_S: C lingap singular values (lingap_num_ev)
-    C_mf_EU: C lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
-    C_mf_EV: C lingap vertex eigenvalues (lingap_num_ev)
-    D_susc: D susceptibility (nk,nff,nb,nb,nb,nb)
-    D_mf_U: D lingap U matrix (lingap_num_ev,lingap_matrix_size)
-    D_mf_V: D lingap V matrix (lingap_num_ev,lingap_matrix_size)
-    D_mf_S: D lingap singular values (lingap_num_ev)
-    D_mf_EU: D lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
-    D_mf_EV: D lingap vertex eigenvalues (lingap_num_ev)
-
-    any of the above can be 'None' if it was not contained in simulation
+    '''
+    class to read diverge postprocessing files for grid FRG
     '''
     def __init__(self, fname):
         d_header = numpy_fromfile(fname, dtype=np.longlong, count=64)
 
         if d_header[0] == DIVERGE_POST_GRID_MAGIC_NUMBER:
             self.valid = True
         else:
             self.valid = False
             return
 
         d_data = numpy_fromfile(fname)
 
+        #: diverge tag version (serves as file format version)
         self.version = d_data[d_header[60]:d_header[60]+d_header[61]].view(
                 dtype=np.byte ).tobytes().decode().rstrip('\x00')
 
+        #: number of kpoints, nk[0]*nk[1]*nk[2] in terms of :c:struct:`diverge_model_t`
         self.nk = d_header[1]
+        #: number of bands, n_orb*n_spin in terms of :c:struct:`diverge_model_t`
         self.nb = d_header[2]
+        #: number of 'formfactors', some heuristic value
         self.nff = d_header[3]
+        #: :math:`SU(2)`?
         self.SU2 = d_header[4]
 
+        #: linearized gap equation number of singular values
         self.lingap_num_ev = d_header[19]
+        #: linearized gap equation matrix size
         self.lingap_matrix_size = d_header[20]
 
         self.file_size = d_header[63]
 
+        #: formfactors (nff,nk)
         formfac = d_data[d_header[5]:d_header[5]+d_header[6]].reshape((self.nff,self.nk,2))
         self.formfac = formfac[:,:,0] + 1j * formfac[:,:,1]
 
         susc_shape = (self.nk,self.nff,self.nb,self.nb,self.nb,self.nb,2)
 
         _P_susc = d_data[d_header[7]:d_header[7]+d_header[8]]
         if _P_susc.size != 0:
+            #: P susceptibility (nk,nff,nb,nb,nb,nb)
             self.P_susc = _P_susc.reshape(susc_shape)
             self.P_susc = self.P_susc[:,:, :,:,:,:, 0] + 1j * self.P_susc[:,:, :,:,:,:, 1]
         else:
             self.P_susc = None
         _P_mf = d_data[d_header[9]:d_header[9]+d_header[10]]
         if _P_mf.size != 0:
             self.P_mf_U, self.P_mf_V, self.P_mf_S, self.P_mf_EU, self.P_mf_EV = self.unroll_mf_solution( _P_mf )
         else:
+            #: P lingap U matrix (lingap_num_ev,lingap_matrix_size)
             self.P_mf_U = None
+            #: P lingap V matrix (lingap_num_ev,lingap_matrix_size)
             self.P_mf_V = None
+            #: P lingap singular values (lingap_num_ev)
             self.P_mf_S = None
+            #: P lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
             self.P_mf_EU = None
+            #: P lingap vertex eigenvalues (lingap_num_ev)
             self.P_mf_EV = None
 
         _C_susc = d_data[d_header[11]:d_header[11]+d_header[12]]
         if _C_susc.size != 0:
             self.C_susc = _C_susc.reshape(susc_shape)
             self.C_susc = self.C_susc[:,:, :,:,:,:, 0] + 1j * self.C_susc[:,:, :,:,:,:, 1]
         else:
+            #: C susceptibility (nk,nff,nb,nb,nb,nb)
             self.C_susc = None
         _C_mf = d_data[d_header[13]:d_header[13]+d_header[14]]
         if _C_mf.size != 0:
             self.C_mf_U, self.C_mf_V, self.C_mf_S, self.C_mf_EU, self.C_mf_EV = self.unroll_mf_solution( _C_mf )
         else:
+            #: C lingap U matrix (lingap_num_ev,lingap_matrix_size)
             self.C_mf_U = None
+            #: C lingap V matrix (lingap_num_ev,lingap_matrix_size)
             self.C_mf_V = None
+            #: C lingap singular values (lingap_num_ev)
             self.C_mf_S = None
+            #: C lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
             self.C_mf_EU = None
+            #: C lingap vertex eigenvalues (lingap_num_ev)
             self.C_mf_EV = None
 
         _D_susc = d_data[d_header[15]:d_header[15]+d_header[16]]
         if _D_susc.size != 0:
+            #: D susceptibility (nk,nff,nb,nb,nb,nb)
             self.D_susc = _D_susc.reshape(susc_shape)
             self.D_susc = self.D_susc[:,:, :,:,:,:, 0] + 1j * self.D_susc[:,:, :,:,:,:, 1]
         else:
             self.D_susc = None
         _D_mf = d_data[d_header[17]:d_header[17]+d_header[18]]
         if _D_mf.size != 0:
             self.D_mf_U, self.D_mf_V, self.D_mf_S, self.D_mf_EU, self.D_mf_EV = self.unroll_mf_solution( _D_mf )
         else:
+            #: D lingap U matrix (lingap_num_ev,lingap_matrix_size)
             self.D_mf_U = None
+            #: D lingap V matrix (lingap_num_ev,lingap_matrix_size)
             self.D_mf_V = None
+            #: D lingap singular values (lingap_num_ev)
             self.D_mf_S = None
+            #: D lingap vertex eigenvectors (lingap_num_ev,lingap_matrix_size)
             self.D_mf_EU = None
+            #: D lingap vertex eigenvalues (lingap_num_ev)
             self.D_mf_EV = None
 
     def unroll_mf_solution( self, mf_solution ):
         U = mf_solution[:self.lingap_matrix_size * self.lingap_num_ev * 2]
         V = mf_solution[self.lingap_matrix_size * self.lingap_num_ev * 2:self.lingap_matrix_size * self.lingap_num_ev * 4]
         S = mf_solution[self.lingap_matrix_size * self.lingap_num_ev * 4:self.lingap_matrix_size * self.lingap_num_ev * 4 + self.lingap_num_ev]
 
@@ -514,120 +520,68 @@
 
         if not (EU is None or EV is None):
             EU = EU.reshape((self.lingap_num_ev,self.lingap_matrix_size,2))
             EU = EU[:,:,0] + 1j * EU[:,:,1]
             EV = EV.reshape((self.lingap_num_ev,))
         return UU[:,:,0] + 1j * UU[:,:,1], VV[:,:,0] + 1j * VV[:,:,1], S, EU, EV
 
-# Class: diverge_post_tu
-# documentation found in docstring, i.e., do the following from within python
-# === Python ===
-# help(diverge_post_tu)
-# ==============
 class diverge_post_tu:
-    '''class to read diverge postprocessing files for tu FRG
+    '''
+    class to read diverge postprocessing files for tu FRG
+
+    Vertex diagonalisation: For each channel :math:`X \in \{P,C,D\}`, we include
+
+        :Xlen: for each q point the number of stored elements (nkibz)
+        :Xoff: for each q point the offset in the array (nkibz)
+        :Xtype: for each q point the used diagonalization algorithm (nkibz)
+        :Xval: stored Eigenvalues (sum(Xlen))
+        :Xvec: stored Eigenvectors (sum(Xlen), n_orb*n_bonds*n_spin**2)
 
-    version: diverge tag version (serves as file format version)
+    Lineraized gap solution: For each physical channel Y (sc, mag, charge), we include
 
-    n_orb: number of orbitals (not spin)
-    n_spin: number of spin degrees of freedom
-    nk: number of momentum points
-    nktot: number of momentum for Hamiltonian
-    nkibz: number of momentum points in the irreducible BZ wedge
-    SU2: Exploit SU2 symmetry
-    n_orbff: number of orbital+bond combinations
-    n_bonds: maximal number of bonds of a single site, not necessarily the same 
-            for every site
-    mi_to_ofrom: map from n_orbff to (o,b) notation, stores o (n_orbff)
-    mi_to_oto: map from n_orbff to (o,b) notation, stores o+bo (n_orbff)
-    mi_to_R: map from n_orbff to (o,b) notation, stores the beyond unit cell
-            contributiom (n_orbff,3)
-    bond_sizes: number of bonds per site o, needed for correct iteration over
-            tu_ff stored in model (n_orb)
-    bond_offsets: offset to the bonds belonging to site o (n_orb)
-    idx_ibz_in_full_mesh: gives the index of the IBZ point in the full PZ (nkibz)
-
-    kmaps_to: symmetry mapping of full BZ to IBZ (nk)
-    mi_to_tuffidx: multiindex to tu_ff index mapping; useful for analysis with model.tu_ff (n_orbff)
-
-    VERTEX DIAGONALISATION
-    Plen: for each q point the number of stored elements (nkibz)
-    Poff: for each q point the offset in the array (nkibz)
-    Ptype: for each q point the used diagonalization algorithm (nkibz)
-    Pval: stored Eigenvalues (sum(Plen))
-    Pvec: stored Eigenvectors (sum(Plen), n_orb*n_bonds*n_spin**2)
-
-    Clen: for each q point the number of stored elements (nkibz)
-    Coff: for each q point the offset in the array (nkibz)
-    Ctype: for each q point the used diagonalization algorithm (nkibz)
-    Cval: stored Eigenvalues (sum(Clen))
-    Cvec: stored Eigenvectors (sum(Clen), n_orb*n_bonds*n_spin**2)
-
-    Dlen: for each q point the number of stored elements (nkibz)
-    Doff: for each q point the offset in the array (nkibz)
-    Dtype: for each q point the used diagonalization algorithm (nkibz)
-    Dval: stored Eigenvalues (sum(Dlen))
-    Dvec: stored Eigenvectors (sum(Dlen), n_orb*n_bonds*n_spin**2)
-
-    LINGAP solution
-    S_sc: singular values SC lingap (n_sing_val)
-    U_sc: U SC lingap (n_sing_val, n_orbff*n_spin**2)
-    V_sc: V SC lingap (n_sing_val, n_orbff*n_spin**2)
-
-    S_mag: singular values magnetic lingap (n_sing_val)
-    U_mag: U magnetic lingap (n_sing_val, n_orbff*n_spin**2)
-    V_mag: V magnetic lingap (n_sing_val, n_orbff*n_spin**2)
-
-    S_ch: singular values charge lingap (n_sing_val)
-    U_ch: U charge (n_sing_val, n_orbff*n_spin**2)
-    V_ch: V charge (n_sing_val, n_orbff*n_spin**2)
-
-    SUSCEPTIBILITY
-    Psusc: Pair-Pair susceptibility ([n_orb*n_spin]*4,nkibz)
-    Csusc: magnetic/crossed PH susceptibility ([n_orb*n_spin]*4,nkibz)
-    Dsusc: charge/direct PH susceptibility ([n_orb*n_spin]*4,nkibz)
-    Psuscff: formfactor resolved Pair-Pair susceptibility ([n_orbff*n_spin*n_spin]*2,nkibz)
-    Csuscff: formfactor resolved magnetic/crossed PH susceptibility ([n_orbff*n_spin*n_spin]*2,nkibz)
-    Dsuscff: formfactor resolved charge/direct PH susceptibility (n_orbff*n_spin*n_spin]*2,nkibz)
-    any of the above can be 'None' if it was not contained in simulation
-
-    SELFENERGY
-    selfenergy: Self-energy at the critical scale ([n_orb*n_spin]*2,nktot)
-
-
-    FULL channels
-    Pchannel: P channel on full PZ
-    Cchannel: C channel on full PZ
-    Dchannel: D channel on full PZ
-    pploop: non interacting PP-loop channel on full PZ
-    phloop: non interacting PH-loop channel on full PZ
-
-    SYMMETRIES
-    symm_o2m_len: length of symmetry maps
-    symm_o2m_off: offsets of symmetry maps
-    symm_o2m_idx_map: index maps
-    self.symm_o2m_Ppref: complex prefactor for P
-    self.symm_o2m_Cpref: complex prefactor for C
+        :S_Y: singular values SC lingap (n_sing_val)
+        :U_Y: U SC lingap (n_sing_val, n_orbff*n_spin**2)
+        :V_Y: V SC lingap (n_sing_val, n_orbff*n_spin**2)
+
+    Susceptibilities: For each channel X, we include the momentum space
+    (on-site) susceptibility and the formfactor susceptibilities if enabled in
+    the simulation
+
+        :Xsusc: channel momentum on-site susceptibility ([n_orb*n_spin]**4,nkibz)
+        :Xsuscff: formfactor resolved susceptibility ([n_orbff*n_spin*n_spin]**2,nkibz)
+
+    any of the above can be 'None' if it was not contained in simulation.
+
+    Full channels: For each channel X, we allow to save the TU vertex at the end
+    of the flow as Xchannel. The loops pploop and phloop can be saved as well.
     '''
     def __init__(self, fname):
         d_header = numpy_fromfile(fname, dtype=np.int64, count=128)
 
         if d_header[0] == DIVERGE_POST_TU_MAGIC_NUMBER and d_header[126] == DIVERGE_POST_TU_MAGIC_NUMBER:
             self.valid = True
         else:
             self.valid = False
             return
 
+        #: number of orbitals (not spin)
         self.n_orb = int(d_header[1])
+        #: number of spin degrees of freedom
         self.n_spin = int(d_header[2])
+        #: number of momentum points
         self.nk = int(d_header[3])
+        #: number of momentum for Hamiltonian
         self.nktot = int(d_header[4])
+        #: number of momentum points in the irreducible BZ wedge
         self.nkibz = int(d_header[5])
+        #: Exploit :math:`SU2` symmetry?
         self.SU2 = int(d_header[6])
+        #: number of orbital+bond combinations
         self.n_orbff = int(d_header[7])
+        #: maximal number of bonds of a single site, not necessarily the same for every site
         self.n_bonds = int(d_header[8])
         self.n_sym = int(d_header[9])
         n_spin = self.n_spin
         n_bonds = self.n_bonds
         n_orb = self.n_orb
         n_orbff = self.n_orbff
 
@@ -636,189 +590,250 @@
             return _f_bytes[offset_bytes:offset_bytes + count*dtype().itemsize].view( dtype=dtype )
         def get_array_header( iL, dtype ):
             res = get_array( d_header[iL[0]], d_header[iL[0]+1], dtype )
             iL[0] = iL[0] + 2
             return res
 
         iL = [10] # can't pass by reference, therefore we need a list... python is stupid after all
+
+        #: map from n_orbff to (o,b) notation, stores o (n_orbff)
         self.mi_to_ofrom = get_array_header( iL, np.int64 )
+        #: map from n_orbff to (o,b) notation, stores o+bo (n_orbff)
         self.mi_to_oto = get_array_header( iL, np.longlong )
+        #: map from n_orbff to (o,b) notation, stores the beyond unit cell contributiom (n_orbff,3)
         self.mi_to_R = get_array_header( iL, np.longlong ).reshape((-1,3))
+        #: number of bonds per site o, needed for correct iteration over tu_ff stored in model (n_orb)
         self.bond_sizes = get_array_header( iL, np.longlong )
+        #: offset to the bonds belonging to site o (n_orb)
         self.bond_offsets = get_array_header( iL, np.longlong )
+        #: gives the index of the IBZ point in the full PZ (nkibz)
         self.idx_ibz_in_bz = get_array_header( iL, np.longlong )
+
+        #: for each q point the number of stored elements (nkibz)
         self.Plen = get_array_header( iL, np.longlong )
+        #: for each q point the offset in the array (nkibz)
         self.Poff = get_array_header( iL, np.longlong )
+        #: for each q point the used diagonalization algorithm (nkibz)
         self.Ptype = get_array_header( iL, np.byte )
+        #: stored Eigenvalues (sum(Plen))
         self.Pval = get_array_header( iL, np.float64 )
+        #: stored Eigenvectors (sum(Plen), n_orbff*n_spin**2)
         self.Pvec = get_array_header( iL, np.complex128 )
 
         self.Pvec = self.Pvec.reshape((np.sum(self.Plen),n_spin,n_spin,n_orbff))
 
+        #: for each q point the number of stored elements (nkibz)
         self.Clen = get_array_header( iL, np.longlong )
+        #: for each q point the offset in the array (nkibz)
         self.Coff = get_array_header( iL, np.longlong )
+        #: for each q point the used diagonalization algorithm (nkibz)
         self.Ctype = get_array_header( iL, np.byte )
+        #: stored Eigenvalues (sum(Clen))
         self.Cval = get_array_header( iL, np.float64 )
+        #: stored Eigenvectors (sum(Clen), n_orbff*n_spin**2)
         self.Cvec = get_array_header( iL, np.complex128 )
 
         self.Cvec = self.Cvec.reshape((np.sum(self.Clen),n_spin,n_spin,n_orbff))
 
+        #: for each q point the number of stored elements (nkibz)
         self.Dlen = get_array_header( iL, np.longlong )
+        #: for each q point the offset in the array (nkibz)
         self.Doff = get_array_header( iL, np.longlong )
+        #: for each q point the used diagonalization algorithm (nkibz)
         self.Dtype = get_array_header( iL, np.byte )
+        #: stored Eigenvalues (sum(Dlen))
         self.Dval = get_array_header( iL, np.float64 )
+        #: stored Eigenvectors (sum(Dlen), n_orbff*n_spin**2)
         self.Dvec = get_array_header( iL, np.complex128 )
 
         self.Dvec = self.Dvec.reshape((np.sum(self.Dlen),n_spin,n_spin,n_orbff))
 
+        #: singular values sc lingap (n_sing_val)
         self.S_sc = get_array_header( iL, np.float64 )
         self.n_svdP = d_header[iL[0]-1]
+        #: U sc lingap (n_sing_val, n_orbff*n_spin**2)
         self.U_sc = get_array_header( iL, np.complex128 )
         self.U_sc = self.U_sc.reshape((self.n_svdP,n_spin,n_spin,n_orbff))
+        #: V sc lingap (n_sing_val, n_orbff*n_spin**2)
         self.V_sc = get_array_header( iL, np.complex128 )
         self.V_sc = self.V_sc.reshape((self.n_svdP,n_spin,n_spin,n_orbff))
 
+        #: singular values magnetic lingap (n_sing_val)
         self.S_mag = get_array_header( iL, np.float64 )
         self.n_svdC = d_header[iL[0]-1]
+        #: U magnetic lingap (n_sing_val, n_orbff*n_spin**2)
         self.U_mag = get_array_header( iL, np.complex128 )
         self.U_mag = self.U_mag.reshape((self.n_svdC,n_spin,n_spin,n_orbff))
+        #: V magnetic lingap (n_sing_val, n_orbff*n_spin**2)
         self.V_mag = get_array_header( iL, np.complex128 )
         self.V_mag = self.V_mag.reshape((self.n_svdC,n_spin,n_spin,n_orbff))
 
+        #: singular values charge lingap (n_sing_val)
         self.S_charge = get_array_header( iL, np.float64 )
         self.n_svdD = d_header[iL[0]-1]
+        #: U charge lingap (n_sing_val, n_orbff*n_spin**2)
         self.U_charge = get_array_header( iL, np.complex128 )
         self.U_charge = self.U_charge.reshape((self.n_svdD,n_spin,n_spin,n_orbff))
+        #: V charge lingap (n_sing_val, n_orbff*n_spin**2)
         self.V_charge = get_array_header( iL, np.complex128 )
         self.V_charge = self.V_charge.reshape((self.n_svdD,n_spin,n_spin,n_orbff))
 
         susc_shape = (n_spin,n_orb,n_spin,n_orb,n_spin,n_orb,n_spin,n_orb,self.nk)
+
+        #: Pair-Pair susceptibility ([n_orb*n_spin]**4,nkibz)
         self.Psusc = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Psusc = self.Psusc.reshape(susc_shape)
+        #: magnetic/crossed PH susceptibility ([n_orb*n_spin]**4,nkibz)
         self.Csusc = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Csusc = self.Csusc.reshape(susc_shape)
+        #: charge/direct PH susceptibility ([n_orb*n_spin]**4,nkibz)
         self.Dsusc = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Dsusc = self.Dsusc.reshape(susc_shape)
 
         susc_shape = (n_spin*n_spin,n_orbff,n_spin*n_spin,n_orbff,self.nk)
+        #: formfactor resolved Pair-Pair susceptibility ([n_orbff*n_spin*n_spin]**2,nkibz)
         self.Psusc_ff = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Psusc_ff = self.Psusc_ff.reshape(susc_shape)
+        #: formfactor resolved magnetic/crossed PH susceptibility ([n_orbff*n_spin*n_spin]**2,nkibz)
         self.Csusc_ff = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Csusc_ff = self.Csusc_ff.reshape(susc_shape)
+        #: formfactor resolved charge/direct PH susceptibility (n_orbff*n_spin*n_spin]**2,nkibz)
         self.Dsusc_ff = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Dsusc_ff = self.Dsusc_ff.reshape(susc_shape)
 
+        #: Self-energy at the critical scale ([n_orb*n_spin]**2,nktot)
         self.selfenergy = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.selfenergy = self.selfenergy.reshape(self.nktot,n_spin,n_orb,n_spin,n_orb)
 
+        #: P channel on full PZ
         self.Pchannel = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Pchannel = self.Pchannel.reshape(susc_shape)
+        #: C channel on full PZ
         self.Cchannel = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Cchannel = self.Cchannel.reshape(susc_shape)
+        #: D channel on full PZ
         self.Dchannel = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.Dchannel = self.Dchannel.reshape(susc_shape)
+        #: non interacting PP-loop channel on full PZ
         self.pploop = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.pploop = self.pploop.reshape(susc_shape)
+        #: non interacting PH-loop channel on full PZ
         self.phloop = get_array_header( iL, np.complex128 )
         if(d_header[iL[0]-1] > 0):
             self.phloop = self.phloop.reshape(susc_shape)
 
         symm_shape = (self.n_sym,n_spin,n_spin,n_orbff)
+        #: length of symmetry maps
         self.symm_o2m_len = get_array_header( iL, np.longlong )
         if(d_header[iL[0]-1] > 0):
             self.symm_o2m_len = self.symm_o2m_len.reshape(symm_shape)
+        #: offsets of symmetry maps
         self.symm_o2m_off = get_array_header( iL, np.longlong )
         if(d_header[iL[0]-1] > 0):
             self.symm_o2m_off = self.symm_o2m_off.reshape(symm_shape)
+        #: index maps
         self.symm_o2m_idx_map = get_array_header( iL, np.longlong )
+        #: complex prefactor for P
         self.symm_o2m_Ppref = get_array_header( iL, np.complex128 )
+        #: complex prefactor for C
         self.symm_o2m_Cpref = get_array_header( iL, np.complex128 )
 
+        #: diverge tag version (serves as file format version)
         self.version = get_array_header( iL, np.byte ).tobytes().decode()
 
+        #: symmetry mapping of full BZ to IBZ (nk)
         self.kmaps_to = get_array_header( iL, np.longlong )
+        #: multiindex to tu_ff index mapping; useful for analysis with model.tu_ff (n_orbff)
         self.mi_to_tuffidx = get_array_header( iL, np.longlong )
 
-# Function: diverge_read
-# function to read model files as well as post processing files. returns the
-# corresponding class (<diverge_model>, <diverge_post_patch>, or
-# <diverge_post_grid>). Makes use of to the file format specifications given in
-# <diverge_postprocess_and_write at
-# diverge_postprocess_conf_t.diverge_postprocess_and_write> and
-# <diverge_model_to_file>; discerning the different file types by their magic
-# numbers
-#
-# Parameters:
-# fname - file name to read from (typically ....dvg)
 def read( fname ):
+    r"""
+    function to read model files as well as post processing files. returns the
+    corresponding class (:class:`diverge_model`, :class:`diverge_post_patch`,
+    :class:`diverge_post_grid`, or :class:`diverge_post_tu`). Makes use of to
+    the file format specifications given in
+    :c:func:`diverge_postprocess_and_write` and :c:func:`diverge_model_to_file`;
+    discerning the different file types by their "magic numbers".
+
+    :param fname: file name to read from (typically ```XXX.dvg```)
+    """
     magic = numpy_fromfile( fname, dtype='i8', count=1 )[0]
     if magic == DIVERGE_MODEL_MAGIC_NUMBER:
         return diverge_model( fname )
     elif magic == DIVERGE_POST_PATCH_MAGIC_NUMBER:
         return diverge_post_patch( fname )
     elif magic == DIVERGE_POST_GRID_MAGIC_NUMBER:
         return diverge_post_grid( fname )
     elif magic == DIVERGE_POST_TU_MAGIC_NUMBER:
         return diverge_post_tu( fname )
     else:
         print(f"magic number {magic} ('{chr(magic)}') unknown")
         return None
 
-# Function: bandstructure_bands
-# return the bands array (nk,nb) from the band  structure obtained from a
-# <diverge_model>. Useful for plotting (for example see <bandstructure_xvals>).
 def bandstructure_bands( model ):
+    r"""
+    return the bands array (nk,nb) from the band  structure obtained from a
+    :class:`diverge_model`. Useful for plotting (for example see
+    :func:`bandstructure_xvals`).
+    """
     return model.bandstructure[:,:-3]
 
-# Function: bandstructure_kpts
-# return the momentum points (nk,3) from the band structure obtained from a
-# <diverge_model>. Useful for plotting and post-processing.
 def bandstructure_kpts( model ):
+    r"""
+    return the momentum points (nk,3) from the band structure obtained from a
+    :class:`diverge_model`. Useful for plotting and post-processing.
+    """
     return model.bandstructure[:,-3:]
 
-# Function: bandstructure_xvals
-# calculate the differential distance between the momentum points from the band
-# structure obtained from a <diverge_model>. Useful for plotting in conjuction
-# with <bandstructure_bands> and <bandstructure_ticks>.
-# === Python ===
-# import diverge.output as do
-# import matplotlib.pyplot as plt
-# M = do.read("model.dvg")
-# b = do.bandstructure_bands(M)
-# x = do.bandstructure_xvals(M)
-# plt.plot( x, b, color='black' )
-# plt.xticks( do.bandstructure_ticks(M) )
-# # need to set the labels manually as they are not known to the model
-# plt.show()
-# ==============
 def bandstructure_xvals( model ):
+    r"""
+    calculate the differential distance between the momentum points from the band
+    structure obtained from a :class:`diverge_model`. Useful for plotting in
+    conjuction with :func:`bandstructure_bands` and :func:`bandstructure_ticks`.
+
+    Example:
+
+    .. sourcecode:: python
+
+        import diverge.output as do
+        import matplotlib.pyplot as plt
+        M = do.read("model.dvg")
+        b = do.bandstructure_bands(M)
+        x = do.bandstructure_xvals(M)
+        plt.plot( x, b, color='black' )
+        plt.xticks( do.bandstructure_ticks(M) )
+        # need to set the labels manually as they are not known to the model
+        plt.show()
+    """
     K = bandstructure_kpts(model)
     vals = np.concatenate( [[0], np.sqrt((np.diff(K,axis=0)**2).sum(axis=1))] )
     if model.npath == -1 and not model.kf_ibz_path is None:
         n_per_segment = model.kf_ibz_path[0]
         offsets = np.cumsum( n_per_segment )
         offset_zero = offsets[n_per_segment == 0]
         vals[offset_zero] = 0.0
     return np.cumsum(vals)
 
-# Function: bandstructure_ticks
-# returns the xticks used for band structure plots from a <diverge_model>.
-# Useful in conjuction with <bandstructure_xvals>.
 def bandstructure_ticks( model ):
+    r"""
+    returns the xticks used for band structure plots from a
+    :class:`diverge_model`. Useful in conjuction with
+    :func:`bandstructure_xvals`.
+    """
     x = bandstructure_xvals( model )
     n_bandstruct = x.shape[0]
     n_ibz_path = model.ibz_path.shape[0]
 
     if n_ibz_path <= 1:
         return None
```

