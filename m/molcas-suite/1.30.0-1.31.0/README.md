# Comparing `tmp/molcas_suite-1.30.0.tar.gz` & `tmp/molcas_suite-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.30.0.tar", last modified: Tue Feb  6 14:51:24 2024, max compression
+gzip compressed data, was "molcas_suite-1.31.0.tar", last modified: Wed Apr 10 13:50:58 2024, max compression
```

## Comparing `molcas_suite-1.30.0.tar` & `molcas_suite-1.31.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 14:51:24.267357 molcas_suite-1.30.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3803 2024-02-06 14:51:24.267357 molcas_suite-1.30.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 14:51:24.265357 molcas_suite-1.30.0/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-06 14:51:21.000000 molcas_suite-1.30.0/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    30756 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    34861 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18445 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25242 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6412 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    25980 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 14:51:24.266357 molcas_suite-1.30.0/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3803 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-06 14:51:24.000000 molcas_suite-1.30.0/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-02-06 14:51:04.000000 molcas_suite-1.30.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-06 14:51:24.267357 molcas_suite-1.30.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2024-02-06 14:51:21.000000 molcas_suite-1.30.0/setup.py
+drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.200200 molcas_suite-1.31.0/
+-rw-r--r--   0 h21027rm   (502) staff       (20)    35072 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/LICENSE
+-rw-r--r--   0 h21027rm   (502) staff       (20)     3803 2024-04-10 13:50:58.198803 molcas_suite-1.31.0/PKG-INFO
+-rwxr-xr-x   0 h21027rm   (502) staff       (20)     2952 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/README.md
+drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.191725 molcas_suite-1.31.0/molcas_suite/
+-rw-r--r--   0 h21027rm   (502) staff       (20)       31 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/__init__.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)      107 2024-04-10 13:43:53.000000 molcas_suite-1.31.0/molcas_suite/__version__.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)     6311 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/barrier.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)     1440 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/cfp.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)    31129 2024-04-10 13:21:22.000000 molcas_suite-1.31.0/molcas_suite/cli.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)    34861 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/extractor.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)    18445 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/generate_input.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)    25242 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/generate_job.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)     6412 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/h5tools.py
+-rw-r--r--   0 h21027rm   (502) staff       (20)    27067 2024-04-10 13:21:22.000000 molcas_suite-1.31.0/molcas_suite/orbs.py
+drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.197327 molcas_suite-1.31.0/molcas_suite.egg-info/
+-rw-r--r--   0 h21027rm   (502) staff       (20)     3803 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 h21027rm   (502) staff       (20)      507 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 h21027rm   (502) staff       (20)        1 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 h21027rm   (502) staff       (20)       55 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 h21027rm   (502) staff       (20)       80 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 h21027rm   (502) staff       (20)       13 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/top_level.txt
+-rw-r--r--   0 h21027rm   (502) staff       (20)     1116 2024-04-10 13:46:40.000000 molcas_suite-1.31.0/pyproject.toml
+-rw-r--r--   0 h21027rm   (502) staff       (20)       38 2024-04-10 13:50:58.200263 molcas_suite-1.31.0/setup.cfg
+-rw-r--r--   0 h21027rm   (502) staff       (20)     1458 2024-04-10 13:44:17.000000 molcas_suite-1.31.0/setup.py
```

### Comparing `molcas_suite-1.30.0/LICENSE` & `molcas_suite-1.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/PKG-INFO` & `molcas_suite-1.31.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.30.0
+Version: 1.31.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.30.0/README.md` & `molcas_suite-1.31.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/barrier.py` & `molcas_suite-1.31.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/cfp.py` & `molcas_suite-1.31.0/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/cli.py` & `molcas_suite-1.31.0/molcas_suite/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,16 @@
         wfmode=args.wf,
         outfile=args.out,
         alpha=args.alpha,
         beta=args.beta,
         root=args.root,
         ener_range=args.ener_range,
         occ_range=args.occ_range,
-        index=args.index
+        index=args.index,
+        user_total_content_choice=args.total_content
     )
 
     return
 
 
 def rotate_func(args):
     """
@@ -1049,14 +1050,24 @@
         '--index',
         type=str,
         default='i123s',
         help=('Orbital indices to include, default i123s. i: inactive, '
               '1: RAS1, 2: RAS2, 3: RAS3, s: secondary.')
     )
 
+    orbitals.add_argument(
+        '--total_content',
+        type=str,
+        default=None,
+        nargs=2,
+        help=('Print total content in each MO of given type, '
+              'e.g. C 2p would print the total C 2p % in each MO, '
+              'or C21 2s would print the total C21 2s % in each MO.')
+    )
+
     # Rotation of spaces
     rotate = subparsers.add_parser('rotate')
     rotate.set_defaults(func=rotate_func)
 
     rotate.add_argument(
         'orbfile',
         type=str,
```

### Comparing `molcas_suite-1.30.0/molcas_suite/extractor.py` & `molcas_suite-1.31.0/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/generate_input.py` & `molcas_suite-1.31.0/molcas_suite/generate_input.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/generate_job.py` & `molcas_suite-1.31.0/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/h5tools.py` & `molcas_suite-1.31.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.30.0/molcas_suite/orbs.py` & `molcas_suite-1.31.0/molcas_suite/orbs.py`

 * *Files 3% similar despite different names*

```diff
@@ -440,15 +440,15 @@
 
     return sorted_percentages, sorted_idx, group_labels
 
 
 def write_report(sorted_percentages, sorted_idx, group_labels, mo_energies,
                  mo_occ, mo_type, wfmode=False,
                  mo_coeff=None, fileobj=None, thr=1., signed_occ=False,
-                 mo_filter=None):
+                 mo_filter=None, total_content_choice=None):
     """
     Writes MO data to orbs code output file.
 
     Parameters
     ----------
     sorted_percentages : np.ndarray
         (ngroups, nbas) array of sorted AO percentage contributions
@@ -473,14 +473,18 @@
     thr : float, default 1.
         threshold for printing percentage contributions
     signed_occ : bool, default False
         if True, print singed occupation numbers
     mo_filter : np.ndarray, default None
         (bool) boolean array of MOs to be included in report. If None, all 
         orbitals printed.
+   total_content_choice : char array, default None
+        Position [0] gives atom or atom type, e.g. C or C21
+        Position [1] gives AO type, e.g. 2p
+        If None, default behaviour is maintained.
 
     Returns
     -------
     None
     """
     if fileobj is None:
         fileobj = sys.stdout
@@ -493,36 +497,47 @@
         mo_fmt = '---- MO {:4d}, occ = {:4.2f}, energy = {:+12.4E}, index = {:1} ----\n'  # noqa
 
     if wfmode:
         ao_fmt = '  {:11}  {:7.3f}    {:+13.7E}\n'
     else:
         ao_fmt = '  {:11}  {:7.3f}\n'
 
+    if total_content_choice is not None:
+        total_fmt = '  {:5}{:5}  {:11.7f}\n'
+
     for i in range(nbas):
         if mo_filter is None or mo_filter[i]:
             fileobj.write(
                     mo_fmt.format(i + 1, mo_occ[i], mo_energies[i], mo_type[i])
             )
+            component_sum = 0.0
             for j in range(ngroups):
-                if sorted_percentages[j, i] >= thr:
-                    ao_lbl = group_labels[sorted_idx[j, i]]
+                ao_lbl = group_labels[sorted_idx[j, i]]
+                if total_content_choice is not None:
+                    if total_content_choice[0] in ao_lbl and total_content_choice[1] in ao_lbl:
+                        component_sum += sorted_percentages[j, i]
+                elif sorted_percentages[j, i] >= thr:
                     if wfmode:
                         fileobj.write(
                             ao_fmt.format(
                                 ao_lbl,
                                 sorted_percentages[j, i],
                                 mo_coeff[sorted_idx[j, i], i]
                             )
                         )
                     else:
                         fileobj.write(
                             ao_fmt.format(ao_lbl, sorted_percentages[j, i])
                         )
                 else:
                     break
+            if total_content_choice is not None:
+                fileobj.write(
+                    total_fmt.format(total_content_choice[0], total_content_choice[1], component_sum)
+                )
 
 
 def average_to_root(orb_data,root):
     """
     Replaces average MO vectors and occupations with those for a specific
     root
 
@@ -563,15 +578,16 @@
     orb_data['orbtype'] = 'RasOrb (root ' + str(root) + ')'
 
     return orb_data
 
 
 def orbital_analysis(h5name, orbname=None, pattern='cnlm', thr=1.,
                      wfmode=False, outfile=None, alpha=False, beta=False,
-                     root=0, ener_range=None, occ_range=None, index='i123s'):
+                     root=0, ener_range=None, occ_range=None, index='i123s',
+                     user_total_content_choice=None):
     """
     Main method for the orbs program for orbital analysis.
 
     Parameters
     ----------
     h5name : str
         name of HDF5 file
@@ -598,15 +614,19 @@
     ener_range : list, [e_min, e_max], default None
         range of MO energies to be analysed. If None, no threshold 
         applied.
     occ_range : list, [occ_min, occ_max], default None
         range of orbital occupation numbers to be analysed. If None, no  
         threshold applied
     index : string, default 'i123s'
-        string of orbital index types (i123s) to be included. 
+        string of orbital index types (i123s) to be included.
+    user_total_content_choice : char array, default=None
+        Position [0] gives atom or atom type, e.g. C or C21
+        Position [1] gives AO type, e.g. 2p
+        If None, default behaviour is maintained.
 
     Returns
     -------
     None
     """
     if wfmode:
         pattern = 'cnlm'
@@ -721,15 +741,16 @@
             group_labels,
             orb_data['mo_energies'],
             orb_data['mo_occupations'],
             orb_data['mo_types'],
             fileobj=fout,
             thr=thr,
             signed_occ=signed_occ,
-            mo_filter=mo_filter
+            mo_filter=mo_filter,
+            total_content_choice=user_total_content_choice
         )
 
     if outfile is None:
         fout.close()
 
 
 def rotate_spaces(orbname, swap_orb, swap_space, outfile="ModOrb"):
```

### Comparing `molcas_suite-1.30.0/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.31.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.30.0
+Version: 1.31.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.30.0/setup.py` & `molcas_suite-1.31.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.30.0"
+__version__ = "1.31.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
```

