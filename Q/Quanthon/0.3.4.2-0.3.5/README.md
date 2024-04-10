# Comparing `tmp/Quanthon-0.3.4.2.tar.gz` & `tmp/Quanthon-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.4.2.tar", last modified: Wed Apr  3 18:39:45 2024, max compression
+gzip compressed data, was "Quanthon-0.3.5.tar", last modified: Wed Apr 10 00:22:10 2024, max compression
```

## Comparing `Quanthon-0.3.4.2.tar` & `Quanthon-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678838 Quanthon-0.3.4.2/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4.2/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 18:39:45.678639 Quanthon-0.3.4.2/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.677352 Quanthon-0.3.4.2/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4.2/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4.2/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4.2/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     6270 2024-04-03 18:01:53.000000 Quanthon-0.3.4.2/Quanthon/algorithms_new.py
--rw-r--r--   0 bukser     (501) staff       (20)     4403 2024-04-03 18:20:37.000000 Quanthon-0.3.4.2/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4.2/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.4.2/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4.2/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)    12029 2024-04-03 18:33:51.000000 Quanthon-0.3.4.2/Quanthon/new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4.2/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4.2/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4.2/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4.2/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-03 18:16:14.000000 Quanthon-0.3.4.2/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678425 Quanthon-0.3.4.2/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      540 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4.2/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 18:39:45.678887 Quanthon-0.3.4.2/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-03 18:39:16.000000 Quanthon-0.3.4.2/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678258 Quanthon-0.3.4.2/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     5905 2024-04-03 18:39:02.000000 Quanthon-0.3.4.2/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.484564 Quanthon-0.3.5/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-10 00:22:10.484357 Quanthon-0.3.5/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.482572 Quanthon-0.3.5/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.5/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.5/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6801 2024-04-10 00:12:04.000000 Quanthon-0.3.5/Quanthon/algorithms_new.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4696 2024-04-09 17:44:34.000000 Quanthon-0.3.5/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.5/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-09 17:39:50.000000 Quanthon-0.3.5/Quanthon/new_base.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.484136 Quanthon-0.3.5/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      581 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.5/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:22:10.484609 Quanthon-0.3.5/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-10 00:21:18.000000 Quanthon-0.3.5/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.483914 Quanthon-0.3.5/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)      286 2024-04-10 00:10:36.000000 Quanthon-0.3.5/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3785 2024-04-10 00:22:08.000000 Quanthon-0.3.5/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.4.2/PKG-INFO` & `Quanthon-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4.2
+Version: 0.3.5
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4.2/Quanthon/Models.py` & `Quanthon-0.3.5/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/algorithms.py` & `Quanthon-0.3.5/Quanthon/algorithms.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/algorithms_new.py` & `Quanthon-0.3.5/Quanthon/algorithms_new.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''Doc:
     Normal VQE, Adapt-VQE
 '''
 
-from scipy.optimize import minimize
+from scipy.optimize import minimize, Bounds
 import numpy as np
 import warnings
 from .expectation import cal_expectation
 from .utils import pauli_sum
 from .new_base import Qubits
 
 class VQE():
@@ -21,36 +21,51 @@
             self.expectation = cal_expectation
             try:
                 ansatz.create_circuit(init_points)
             except ValueError:
                 raise ValueError(f'The initial points ({init_points}) do not match the dimension of the ansatz.')
 
             self.minimise = optimiser
-            
                 
+
         def _objective(self, params):
+
+            # print(params)
+            params = np.real(params)
             self.ansatz.create_circuit(params)
             qc = self.ansatz.qubits
             qc.run()
-
+            
             energy = self.expectation(qc, self.H, self.num_shots)
+
+            # self.H_mat = pauli_sum(self.H)
+            # energy = self.ansatz.qubits.state.conj().T @ self.H_mat @ self.ansatz.qubits.state
             return energy
 
         def minimise_eigenvalue(self, H_pauli_str, num_shots=10000):
             '''
             Rotates the parametrised circuit to find the minimised energy using classical 
             minimisation algorithms.
             Inputs:
             H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
             num_shots: (int) number of shots,
             return: (float) minimised energy eigenvalues.'''
             self.H = H_pauli_str
 
             self.num_shots = num_shots
-            result = self.minimise(self._objective, self.params, method='Powell', options= {"maxiter": 10000})
+
+            lb = -np.pi * np.ones(len(self.params))
+            ub = np.pi * np.ones(len(self.params))
+            bounds = Bounds(lb, ub)
+            
+            result = self.minimise(self._objective, 
+                                   self.params, 
+                                   method='Powell', 
+                                #    bounds=bounds, 
+                                   options= {"maxiter": 10000})
             min_params = result.x
             min_energy = result.fun
             
             return min_params, min_energy
```

### Comparing `Quanthon-0.3.4.2/Quanthon/ansatzs.py` & `Quanthon-0.3.5/Quanthon/ansatzs.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,21 +41,26 @@
         if len(init_params) != self.n_params:
             raise ValueError(f'Initial parameters do not match the number of parameters required for the ansatz: {len(init_params)} != {self.n_params}')
         
         reshaped_params = init_params.reshape(self.reps, 2*self.n_qubits)
         
         for r in range(self.reps):
             for i in range(self.n_qubits):
+                # check if the parameters are real
+                if reshaped_params[r, i] != reshaped_params[r, i].real:
+                    raise ValueError(f'Parameter {[r,i]} is not real.')
                 self.qubits.Rx(reshaped_params[r, i], i)
                 self.qubits.Ry(reshaped_params[r, i + self.n_qubits], i)
+        
+        for r in range(self.reps):
+            for i in range(self.n_qubits):
                 if i != self.n_qubits - 1:
                     self.qubits.CNOT(i, i+1)
-        
 
-        
+        # self.qubits.draw()
 
     def run(self):
         self.qubits.run()
     
 
 
 class QubitAdaptAnsatz:
```

### Comparing `Quanthon-0.3.4.2/Quanthon/base.py` & `Quanthon-0.3.5/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/expectation.py` & `Quanthon-0.3.5/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/mappers.py` & `Quanthon-0.3.5/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/new_base.py` & `Quanthon-0.3.5/Quanthon/new_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,16 @@
         else:
             gate_map = {
                 'H': '\\gate{H}',
                 'I': '\\qw',
                 'X': '\\gate{X}',
                 'Y': '\\gate{Y}',
                 'Z': '\\gate{Z}',
-                'Rx': lambda angle: '\\gate{R_x(' + f"{angle}" + ')}',
-                'Ry': lambda angle: '\\gate{R_y(' + f"{angle}" + ')}',
+                'Rx': lambda angle: '\\gate{R_x(' + f"{float(angle).real:.3f}" + ')}',
+                'Ry': lambda angle: '\\gate{R_y(' + f"{float(angle).real:.3f}" + ')}',
                 'Sdag': '\\gate{S^\\dagger}',
                 'CNOTctrl': lambda dist: "\\ctrl{" + f"{dist}" + '}',
                 'CNOTtrgt': '\\targ{}',
                 'SWAP1': lambda dist: "\\swap{" + f"{dist}" + '}',
                 'SWAP2': '\\targX{}',
                 # 'exp': lambda axis, theta: f'\\gate{R_{axis}}'
             }
@@ -328,28 +328,27 @@
             
             quantikz_str += "\\end{quantikz}"
             
             print(quantikz_str)
 
 
 if __name__ == "__main__":
-    qc = Qubits(4)
-    qc.H(1)
-    qc.H(0)
+    qc = Qubits(6)
+    # qc.H(1)
+    # qc.H(0)
 
-    qc.CNOT(0,1)
-    qc.CNOT(1,2)
-    qc.CNOT(2,3)
+    # qc.CNOT(0,1)
+    # qc.CNOT(1,2)
+    # qc.CNOT(2,3)
 
 
-    qc.run()
+    # qc.run()
     # print(qc)
 
     # qc.X(1)
     # qc.Y(0)
     # qc.rx(0.4, 1)
-    
-    # qc.rx(-1.2080928149562626, 1)
+
     # print(qc.gate_history)
     # qc.draw(True)
 
     print(qc)
```

### Comparing `Quanthon-0.3.4.2/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.5/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.5/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/ut_test_jw.py` & `Quanthon-0.3.5/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/Quanthon/utils.py` & `Quanthon-0.3.5/Quanthon/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -131,16 +131,38 @@
     return val
 
 
 
     
 if __name__ == "__main__":
     # Test Pauli operators
-    pauli_ops = [('IZZZ', 3), ('ZXYI', 2)]
-    a = pauli_sum(pauli_ops)
+    # pauli_ops = [('IZZZ', 3), ('ZXYI', 2)]
+    qubit_op = [('IIIIII', 0.1875), ('IIIIIZ', -0.5625), 
+                    ('IIIIZI', -0.0625), ('IIIZII', 0.4375), 
+                    ('IIZIII', -0.5625), ('IIZIIZ', 0.0625), 
+                    ('IXXIII', 0.0625), ('IXXIIZ', -0.03125), 
+                    ('IXXIZI', -0.03125), ('IXYIIZ', 0.03125j), 
+                    ('IXYIZI', -0.03125j), ('IYXIIZ', -0.03125j), 
+                    ('IYXIZI', 0.03125j), ('IYYIII', (0.0625+0j)), 
+                    ('IYYIIZ', (-0.03125+0j)), ('IYYIZI', (-0.03125+0j)), 
+                    ('IZIIII', -0.0625), ('IZIIZI', 0.0625), 
+                    ('XXIIII', 0.0625), ('XXIIZI', -0.03125), 
+                    ('XXIZII', -0.03125), ('XYIIZI', 0.03125j), 
+                    ('XYIZII', -0.03125j), ('XZXIII', 0.0625), 
+                    ('XZXIIZ', -0.03125), ('XZXZII', -0.03125), 
+                    ('XZYIIZ', 0.03125j), ('XZYZII', -0.03125j), 
+                    ('YXIIZI', -0.03125j), ('YXIZII', 0.03125j), 
+                    ('YYIIII', (0.0625+0j)), ('YYIIZI', (-0.03125+0j)), 
+                    ('YYIZII', (-0.03125+0j)), ('YZXIIZ', -0.03125j), 
+                    ('YZXZII', 0.03125j), ('YZYIII', (0.0625+0j)), 
+                    ('YZYIIZ', (-0.03125+0j)), ('YZYZII', (-0.03125+0j)), 
+                    ('ZIIIII', 0.4375), ('ZIIZII', 0.0625)]
+    h = pauli_sum(qubit_op)
+    # a = pauli_sum(pauli_ops)
+    
     
     n = 78
     t = 0
     # fn = flip_bit(n, t)
     # sn = swap_bits(4, 0, 1)
     # print(f'Flipping the {t}th bit of {n} gives {fn}')
     # print(f'Swapping the {0}th bit and the {1} bit of {4} gives {sn}')
```

### Comparing `Quanthon-0.3.4.2/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.5/Quanthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4.2
+Version: 0.3.5
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4.2/README.md` & `Quanthon-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.2/setup.py` & `Quanthon-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.4.2" #####
+version = "0.3.5" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.4.2/tests/test_vqes.py` & `Quanthon-0.3.5/tests/test_cmp_qk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import unittest
-import numpy as np
-
 from qiskit_nature.second_q.mappers import JordanWignerMapper
 from qiskit_nature.second_q.operators import FermionicOp
 from qiskit_nature.second_q.algorithms import GroundStateEigensolver
 
 from qiskit.quantum_info import SparsePauliOp
 from qiskit.primitives import Estimator
 from qiskit.circuit.library import TwoLocal
 
-from qiskit_algorithms import VQE as qk_VQE
-from qiskit_algorithms import AdaptVQE as qk_AdaptVQE
+from qiskit_algorithms import VQE
+from qiskit_algorithms import AdaptVQE
 
 from qiskit_algorithms.optimizers import COBYLA, L_BFGS_B, SLSQP
 from qiskit_algorithms.utils import algorithm_globals
 
 import warnings
 
-from Quanthon import VQE, AdaptVQE, jordan_wigner, Hamiltonian, QubitAdaptAnsatz, HardwareEfficietnAnsatz, pauli_sum
-
-
-class AlgorithmTest(unittest.TestCase):
+import numpy as np
 
-    def _qiskit_hardware(self, op):
+def qiskit_hardware(op):
         
         warnings.filterwarnings("ignore")
 
         estimator = Estimator()
         qubit_op = SparsePauliOp.from_list(op)
 
         # we will iterate over these different optimizers
@@ -42,104 +36,50 @@
             counts = []
             values = []
 
             def store_intermediate_result(eval_count, parameters, mean, std):
                 counts.append(eval_count)
                 values.append(mean)
 
-            vqe = qk_VQE(estimator, ansatz, optimizer, callback=store_intermediate_result)
+            vqe = VQE(estimator, ansatz, optimizer, callback=store_intermediate_result)
             result = vqe.compute_minimum_eigenvalue(operator=qubit_op)
             converge_counts[i] = np.asarray(counts)
             converge_vals[i] = np.asarray(values)
         
         return result
-    
-    def _qiskit_adapt(self):
-        
-        pass
-        warnings.filterwarnings("ignore")
-
-        estimator = Estimator()
-        qubit_op = SparsePauliOp.from_list(
-        [
-            ("II", -1.052373245772859),
-            ("IZ", 0.39793742484318045),
-            ("ZI", -0.39793742484318045),
-            ("ZZ", -0.01128010425623538),
-            ("XX", 0.18093119978423156),
-        ]
-        )
-
-        # we will iterate over these different optimizers
-        optimizer = SLSQP(maxiter=60)
-
-        print("\rOptimizer: {}        ".format(type(optimizer).__name__), end="")
-        algorithm_globals.random_seed = 50
-        ansatz = TwoLocal(rotation_blocks="ry", entanglement_blocks="cz")
-
-        vqe = VQE(estimator, ansatz, optimizer)
-        adapt_vqe = AdaptVQE(vqe)
-        eigenvalue, _ = adapt_vqe.compute_minimum_eigenvalue(qubit_op)
-        print(eigenvalue)
-
-        return eigenvalue
 
+def _qiskit_adapt(self):
     
-    def test_vqe(self):
+    pass
+    warnings.filterwarnings("ignore")
 
-        op_str =[("II", -1.052373245772859),
-                    ("IZ", 0.39793742484318045),
-                    ("ZI", -0.39793742484318045),
-                    ("ZZ", -0.01128010425623538),
-                    ("XX", 0.18093119978423156),
-                ]
-        
-        ansatz = HardwareEfficietnAnsatz(2, reps=2)
-
-        rng = np.random.default_rng(826)
-        n_params = ansatz.n_params
-
-        init_points = rng.random(n_params) * 2 * np.pi - np.pi 
-        vqe = VQE(ansatz, init_points)
-        min_params, min_energy = vqe.minimise_eigenvalue(op_str, 1000)
-        print(min_energy)
-
-        # with qiskit
-
-        result = self._qiskit_hardware(op_str)
-        # print("diff from qiskit")
-        print(result.eigenvalue)
-    
-    def _test_adapt_vqe(self):
-
-        qubit_op =[("II", -1.052373245772859),
-                    ("IZ", 0.39793742484318045),
-                    ("ZI", -0.39793742484318045),
-                    ("ZZ", -0.01128010425623538),
-                    ("XX", 0.18093119978423156),
-                ]
-        h_mat = pauli_sum(qubit_op)
-        # print(f"h_mat: {h_mat}")
+    estimator = Estimator()
+    qubit_op = SparsePauliOp.from_list(
+    [
+        ("II", -1.052373245772859),
+        ("IZ", 0.39793742484318045),
+        ("ZI", -0.39793742484318045),
+        ("ZZ", -0.01128010425623538),
+        ("XX", 0.18093119978423156),
+    ]
+    )
+
+    # we will iterate over these different optimizers
+    optimizer = SLSQP(maxiter=60)
+
+    print("\rOptimizer: {}        ".format(type(optimizer).__name__), end="")
+    algorithm_globals.random_seed = 50
+    ansatz = TwoLocal(rotation_blocks="ry", entanglement_blocks="cz")
+
+    vqe = VQE(estimator, ansatz, optimizer)
+    adapt_vqe = AdaptVQE(vqe)
+    eigenvalue, _ = adapt_vqe.compute_minimum_eigenvalue(qubit_op)
+    print(eigenvalue)
 
-        ansatz = QubitAdaptAnsatz(2)
-        print(ansatz.qubits)
-
-        print(ansatz)
-        
-
-        vqe = AdaptVQE(ansatz)
-        ansatz, min_energy = vqe.run_adapt_circuit(qubit_op, 10000, max_iter=10)
-        print(min_energy)
-
-        # with qiskit
-
-        result = self._qiskit_hardware(qubit_op)
-        print(result.eigenvalue)
-
- 
+    return eigenvalue
 
 def matrix_to_fermionic_op(one_body_matrix, two_body_matrix):
     # Get the size of the one-body matrix
     n = one_body_matrix.shape[0]
 
     # Initialize an empty FermionicOp dictionary
     op_dict = {}
@@ -176,11 +116,8 @@
     two_body = two_body + two_body.conj().T
 
     op = matrix_to_fermionic_op(one_body,two_body)
 
     h = Hamiltonian(np.flip(one_body), np.flip(two_body))
 
     # h: Hamiltonian, op: FermionicOp for qiskit stuff
-    return h, op
-
-if __name__ == '__main__':
-    unittest.main()
+    return h, op
```

