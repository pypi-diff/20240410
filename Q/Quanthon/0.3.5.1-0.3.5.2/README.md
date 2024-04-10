# Comparing `tmp/Quanthon-0.3.5.1.tar.gz` & `tmp/Quanthon-0.3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.5.1.tar", last modified: Wed Apr 10 00:29:27 2024, max compression
+gzip compressed data, was "Quanthon-0.3.5.2.tar", last modified: Wed Apr 10 00:51:57 2024, max compression
```

## Comparing `Quanthon-0.3.5.1.tar` & `Quanthon-0.3.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886935 Quanthon-0.3.5.1/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5.1/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:29:27.886706 Quanthon-0.3.5.1/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.884158 Quanthon-0.3.5.1/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5.1/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      319 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     6797 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     4692 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-09 17:39:50.000000 Quanthon-0.3.5.1/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5.1/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5.1/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5.1/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5.1/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5.1/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5.1/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5.1/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886438 Quanthon-0.3.5.1/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      533 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1506 2024-04-10 00:23:56.000000 Quanthon-0.3.5.1/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:29:27.886987 Quanthon-0.3.5.1/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-10 00:29:25.000000 Quanthon-0.3.5.1/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886068 Quanthon-0.3.5.1/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5.1/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)      331 2024-04-10 00:24:57.000000 Quanthon-0.3.5.1/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.5.1/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:51:57.650202 Quanthon-0.3.5.2/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5.2/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:51:57.650007 Quanthon-0.3.5.2/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:51:57.647894 Quanthon-0.3.5.2/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5.2/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      319 2024-04-10 00:27:46.000000 Quanthon-0.3.5.2/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6849 2024-04-10 00:41:48.000000 Quanthon-0.3.5.2/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4727 2024-04-10 00:49:28.000000 Quanthon-0.3.5.2/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-10 00:38:34.000000 Quanthon-0.3.5.2/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5.2/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5.2/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5.2/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5.2/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5.2/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5.2/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5.2/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:51:57.649817 Quanthon-0.3.5.2/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:51:57.000000 Quanthon-0.3.5.2/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      533 2024-04-10 00:51:57.000000 Quanthon-0.3.5.2/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:51:57.000000 Quanthon-0.3.5.2/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:51:57.000000 Quanthon-0.3.5.2/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:51:57.000000 Quanthon-0.3.5.2/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1506 2024-04-10 00:23:56.000000 Quanthon-0.3.5.2/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:51:57.650248 Quanthon-0.3.5.2/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-10 00:45:16.000000 Quanthon-0.3.5.2/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:51:57.649454 Quanthon-0.3.5.2/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5.2/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)      331 2024-04-10 00:24:57.000000 Quanthon-0.3.5.2/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.5.2/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.5.1/PKG-INFO` & `Quanthon-0.3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5.1
+Version: 0.3.5.2
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.5.1/Quanthon/Models.py` & `Quanthon-0.3.5.2/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/algorithms.py` & `Quanthon-0.3.5.2/Quanthon/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,16 @@
             the adapted ansatz and the energy eigenvalues.
         '''
         self.H_mat = pauli_sum(H)
         self.H_str = H
         self.params = np.array([])
         for i in range(max_iter): 
             # need to update the state too
-            print(self.ansatz.qubits)
-
+            # print(self.ansatz.qubits)
+            # self.ansatz.run(self.params) # ??????
             old_params, energy = self.minimise_eigenvalue(num_shots) # state is not updated here
             self.params = old_params
             print(f"i: {i}, min_energy = {energy}")
             
 
             if not self._append_operator(): # new parameter is added here 
                 break
@@ -188,8 +188,8 @@
         # print(self.params)
         result = self.minimise(self._objective, self.params, method='Powell', options= {"maxiter": 100000})
         min_params = result.x
         min_energy = result.fun
 
         # self.ansatz.run(min_params) # update the state using only the optimal parameters
          
-        return min_params, min_energy
+        return min_params, min_energy
```

### Comparing `Quanthon-0.3.5.1/Quanthon/ansatzs.py` & `Quanthon-0.3.5.2/Quanthon/ansatzs.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         '''Ansatz for the Adapt-VQE calculation.'''
 
         self.qubits = Qubits(n_qubits)
 
         if init_state is None:
             # initial state not sepcified, initialise randomly
-            init_state = np.random.rand(2**n_qubits)
+            init_state = np.random.rand(2**n_qubits) + 1j * np.random.rand(2**n_qubits)
             init_state = init_state / np.linalg.norm(init_state) 
         
         self.init_state = init_state
         self.qubits.set_state(init_state)
 
         if pool == 'V':
             self.pool = self.create_complete_V_pool(n_qubits)
```

### Comparing `Quanthon-0.3.5.1/Quanthon/base.py` & `Quanthon-0.3.5.2/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/expectation.py` & `Quanthon-0.3.5.2/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/mappers.py` & `Quanthon-0.3.5.2/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.5.2/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.5.2/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/ut_test_jw.py` & `Quanthon-0.3.5.2/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon/utils.py` & `Quanthon-0.3.5.2/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.5.2/Quanthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5.1
+Version: 0.3.5.2
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.5.1/Quanthon.egg-info/SOURCES.txt` & `Quanthon-0.3.5.2/Quanthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/README.md` & `Quanthon-0.3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/setup.py` & `Quanthon-0.3.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.5.1" #####
+version = "0.3.5.2" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.5.1/tests/test_cmp_qk.py` & `Quanthon-0.3.5.2/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5.1/tests/test_vqes.py` & `Quanthon-0.3.5.2/tests/test_vqes.py`

 * *Files identical despite different names*

