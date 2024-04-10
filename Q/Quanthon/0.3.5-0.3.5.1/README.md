# Comparing `tmp/Quanthon-0.3.5.tar.gz` & `tmp/Quanthon-0.3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.5.tar", last modified: Wed Apr 10 00:22:10 2024, max compression
+gzip compressed data, was "Quanthon-0.3.5.1.tar", last modified: Wed Apr 10 00:29:27 2024, max compression
```

## Comparing `Quanthon-0.3.5.tar` & `Quanthon-0.3.5.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.484564 Quanthon-0.3.5/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-10 00:22:10.484357 Quanthon-0.3.5/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.482572 Quanthon-0.3.5/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.5/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.5/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     6801 2024-04-10 00:12:04.000000 Quanthon-0.3.5/Quanthon/algorithms_new.py
--rw-r--r--   0 bukser     (501) staff       (20)     4696 2024-04-09 17:44:34.000000 Quanthon-0.3.5/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.5/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-09 17:39:50.000000 Quanthon-0.3.5/Quanthon/new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.484136 Quanthon-0.3.5/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      581 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:22:10.000000 Quanthon-0.3.5/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.5/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:22:10.484609 Quanthon-0.3.5/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-10 00:21:18.000000 Quanthon-0.3.5/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:22:10.483914 Quanthon-0.3.5/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)      286 2024-04-10 00:10:36.000000 Quanthon-0.3.5/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3785 2024-04-10 00:22:08.000000 Quanthon-0.3.5/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886935 Quanthon-0.3.5.1/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.5.1/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:29:27.886706 Quanthon-0.3.5.1/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.884158 Quanthon-0.3.5.1/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.5.1/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      319 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6797 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4692 2024-04-10 00:27:46.000000 Quanthon-0.3.5.1/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12033 2024-04-09 17:39:50.000000 Quanthon-0.3.5.1/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.5.1/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.5.1/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.5.1/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.5.1/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.5.1/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.5.1/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6159 2024-04-10 00:03:37.000000 Quanthon-0.3.5.1/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886438 Quanthon-0.3.5.1/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2371 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      533 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-10 00:29:27.000000 Quanthon-0.3.5.1/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1506 2024-04-10 00:23:56.000000 Quanthon-0.3.5.1/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-10 00:29:27.886987 Quanthon-0.3.5.1/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-10 00:29:25.000000 Quanthon-0.3.5.1/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-10 00:29:27.886068 Quanthon-0.3.5.1/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 Quanthon-0.3.5.1/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)      331 2024-04-10 00:24:57.000000 Quanthon-0.3.5.1/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-10 00:22:16.000000 Quanthon-0.3.5.1/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.5/PKG-INFO` & `Quanthon-0.3.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5
+Version: 0.3.5.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -98,25 +98,10 @@
 # Perform a CNOT operation between the first and second qubit
 two_qubits.CONT(0, 1)
 
 two_qubits.SWAP(0, 1)
 ```
 
 
-## NEW IN VERSION 0.3:
-- You must now use Qubits.run() to execute the circuit after applying the gates.
-    
-```python
-qc = Qubits(4)
-qc.H(0)
-```
-
-- Hadamard gates are now called *Qubits.H(i)* in order to be consistent.
-Old:
-```python
-qc.Hadamard(0)
-```
-New:
-```python
-qc.H(0)
-```
+## NEW IN VERSION 0.3.5:
+- VQE now supports non-Hermitian 'Hamiltonian's, but why would you ever need it?
```

### Comparing `Quanthon-0.3.5/Quanthon/Models.py` & `Quanthon-0.3.5.1/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/algorithms_new.py` & `Quanthon-0.3.5.1/Quanthon/algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 
 from scipy.optimize import minimize, Bounds
 import numpy as np
 import warnings
 from .expectation import cal_expectation
 from .utils import pauli_sum
-from .new_base import Qubits
+from .base import Qubits
 
 class VQE():
         def __init__(self, ansatz, init_points, optimiser=minimize):
             '''
             args:
                 ansatz: a parametriced circuit that takes parmas: theta and phi
                 init_points: a list of initial points, must match the number of the parameters in the ansatz
```

### Comparing `Quanthon-0.3.5/Quanthon/ansatzs.py` & `Quanthon-0.3.5.1/Quanthon/ansatzs.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     print(msg)
 
 
 import numpy as np
 from scipy.linalg import expm
 
 
-from .new_base import Qubits, Gate
+from .base import Qubits, Gate
 from .utils import pauli_sum
 
 class Ansatz:
 
     '''Should work for any type of ansatz that are not evolving, do not use on its own.'''
     def __init__(self, n_qubits, reps=1) -> None:
```

### Comparing `Quanthon-0.3.5/Quanthon/base.py` & `Quanthon-0.3.5.1/Quanthon/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,73 @@
+'''The basic classes for quantum computing. Replaced base.py, which was discontinued after Quanthon 0.3.0'''
+
+# TODO: Add n dimension rotation 
+
 import numpy as np
 from collections import Counter
+from .utils import one_fixed_bit, flip_bit, swap_bits
 
 # Constants
 rng = np.random.default_rng()
 rangle = '\u27E9'
 
-PendingDeprecationWarning("This module is deprecated and will be removed in the next release. Please use the new_base module instead.")
-
 class Gate:
 
-    def __init__(self, name, matrix, n_qubits, params=None):
+    def __init__(self, name, matrix, n_qubits):
+        '''
+        args:
+            name: string, the name of the gate;
+            matrix: operator matrix or a function which takes params is an argument and returns the matrix of the correct size;
+            n_qubits: int, the number of qubits the gate acts on;
+            '''
         self.name = name
         self.matrix = matrix
+
         self.n_qubits = n_qubits
-        self.params = params
-    
+        # self.params = params
+
+
     def __repr__(self):
         return f"Gate: {self.name} \n Matrix: \n {self.matrix} \n"
     
-class Qubit:
+    def _check_is_unitary(self, matrix):
 
-    def __init__(self) -> None:
-        self.state = np.zeros(2, dtype=np.complex_)
+        if not np.allclose(matrix @ matrix.conj().T, np.eye(matrix.shape[0])):
+            raise ValueError(f"{self.name} is not unitary.")
+    
+    def act(self, state, param=None):
+        if param is not None:
+            self._check_is_unitary(self.matrix(param))
+            return self.matrix(param) @ state
+        self._check_is_unitary(self.matrix)
+        return self.matrix @ state
+
+    
+class Qubits:
+
+    def __init__(self,n):
+        self.state = np.zeros(2**n, dtype=np.complex_)
         self.state[0] = 1
+        self.n_qubit = n
+        self.opeartor_size = 2**n
+
         self.I = np.eye(2)
-        self.H = 1/np.sqrt(2) * np.array([[1, 1], [1, -1]])
+        self.h = 1/np.sqrt(2) * np.array([[1, 1], [1, -1]])
         self.x = np.array([[0, 1], [1, 0]])
         self.y = np.array([[0, -1j], [1j, 0]])
         self.z = np.array([[1, 0], [0, -1]])
         self.s = np.array([[1, 0], [0, 1j]])
-        self.n_qubit = 1
+
+        self.circuit = []
+
         self._get_state_dict()
         self._get_gate_history()
+        
+    def __repr__(self) -> str:
+        return f"Qubit(s) in state: \n {self._to_comp_basis()} \n"
 
     def _get_gate_history(self):
         self.gate_history = {}
         for i in range(self.n_qubit):
             self.gate_history[f'{i}'] = []
         # print(self.n_qubit)
         # print(self.gate_history)
@@ -64,27 +96,31 @@
                 if j not in i:
                     self.gate_history[f'{j}'].append('I')
             else:
                 if j != i:
                     self.gate_history[f'{j}'].append('I')
 
 
-    def __repr__(self) -> str:
-        return f"Qubit(s) in state: \n {self._to_comp_basis()} \n"
-
     def set_state(self, state):
         assert len(state) == 2**self.n_qubit, f"Invalid state: must have length {2**self.n_qubit}"
-        assert np.linalg.norm(state) == 1, "Invalid state: must be normalised"
+        assert np.isclose(np.linalg.norm(state), 1), "Invalid state: must be normalised."
         self.state = state
 
+    def reset_state(self):
+        self.state = np.zeros(2**self.n_qubit, dtype=np.complex_)
+        self.state[0] = 1
+    
+    def reset_circuit(self):
+        self.circuit = []
+
     def copy(self):
-        new_qubit = Qubit()
-        new_qubit.state = self.state.copy()
-        new_qubit.n_qubit = self.n_qubit
-        return new_qubit
+        new_qubits = Qubits(self.n_qubit)
+        new_qubits.state = self.state.copy()
+        return new_qubits
+
 
     def _get_state_dict(self):
         self.state_dict = dict()
         for i in np.arange(2 ** self.n_qubit):
             self.state_dict[format(i, f'0{self.n_qubit}b')] = self.state[i]
         
     def _to_comp_basis(self):
@@ -102,54 +138,122 @@
             computational_str += f"{amplitude:.2f}|{binary_str}⟩ + "
 
         computational_str = computational_str.rstrip("+ ")
 
         # Return the computational basis notation
         return computational_str
     
-    def operate(self, op, indx): 
+    def _make_op_mat(self, op, indx): 
         ''' Operates the qubit with the given operator and index. '''
         result = np.eye(2**indx)
         result = np.kron(result, op)
-        for _ in range(int(self.n_qubit-indx-len(op)/2)):
+        # print(op)
+        # rest_of_indices = int(self.n_qubit - indx - np.sqrt(len(op)))
+        rest_of_indices = int(self.n_qubit - indx - np.log2(len(op)))
+        for _ in range(rest_of_indices):
             result = np.kron(result, np.eye(2))
         
-        self.state = result @ self.state
-    
+        return result
+        # self.state = result @ self.state
 
-    def hadamard(self,i):
-        self.operate(self.H,i)
+    def H(self,i):
+        # self.operate(self.h,i)
+        matrix = self._make_op_mat(self.h, i)
+        self.circuit.append(Gate('H', matrix, self.n_qubit))
         self._update_gate_history('H', i)
     
     def X(self,i):
-        self.operate(self.x, i)
+        # self.operate(self.x, i)
+        matrix = self._make_op_mat(self.x, i)
+        self.circuit.append(Gate('X', matrix, self.n_qubit))
         self._update_gate_history('X', i)
 
     def Y(self,i):
-        self.operate(self.y, i)
+        # self.operate(self.y, i)
+        matrix = self._make_op_mat(self.y, i)
+        self.circuit.append(Gate('Y', matrix, self.n_qubit))
         self._update_gate_history('Y', i)
 
     def Z(self,i):
-        self.operate(self.z, i)
+        # self.operate(self.z, i)
+        matrix = self._make_op_mat(self.z, i)
+        self.circuit.append(Gate('Z', matrix, self.n_qubit))
         self._update_gate_history('Z', i)
     
-    def sdag(self,i):
-        self.operate(self.s.conj(), i)
+    def Sdag(self,i):
+        # self.operate(self.s.conj(), i)
+        matrix = self._make_op_mat(self.s.conj(), i)
+        self.circuit.append(Gate('Sdag', matrix, self.n_qubit))
         self._update_gate_history('Sdag', i)
 
-    def rx(self, theta, i):
-        Rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x 
-        self.operate(Rx, i)
+    def Rx(self, theta, i):
+
+        rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
+        # self.operate(Rx, i) 
+        matrix = self._make_op_mat(rx, i)
+        self.circuit.append(Gate('Rx', matrix, self.n_qubit))
         self._update_gate_history(f'Rx_{theta}', i)
 
-    def ry(self, phi, i):
-        Ry = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
-        self.operate(Ry, i)
+    def Ry(self, phi, i):
+        ry = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
+        # self.operate(Ry, i)
+        matrix = self._make_op_mat(ry, i)
+        self.circuit.append(Gate('Ry', matrix, self.n_qubit))
         self._update_gate_history(f'Ry_{phi}', i)
 
+    def CNOT(self, control, target):
+
+        if self.n_qubit == 1:
+            raise ValueError("The CNOT gate can not be applied to a single qubit.")
+        
+        matrix = np.eye(self.opeartor_size)
+
+        indices = one_fixed_bit(self.n_qubit, self.n_qubit - control - 1, is_decimal=True) # we do n-c cuz our 0th bit is on the left
+
+        for i in indices:
+            # print(i)
+            f = flip_bit(i, self.n_qubit - target - 1) # same reason
+            # print(f)
+            matrix[i, i] = 0
+            matrix[f, i] = 1
+            matrix[i, f] = 1
+
+        self.circuit.append(Gate('CNOT', matrix, self.n_qubit))
+        # self.state = matrix @ self.state
+        self._update_gate_history("CNOT", (control, target))
+
+
+    def SWAP(self, qubit1, qubit2):
+        if self.n_qubit == 1:
+            raise ValueError("The SWAP gate can not be applied to a single qubit.")
+        
+
+        matrix = np.zeros((self.opeartor_size, self.opeartor_size))
+        for i in range(self.opeartor_size):
+            j = swap_bits(i, self.n_qubit - qubit1 - 1, self.n_qubit - qubit2 - 1)
+            matrix[i, j] = 1
+            matrix[j, i] = 1
+
+        # self.state = matrix @ self.state
+        self.circuit.append(Gate('SWAP', matrix, self.n_qubit))
+        self._update_gate_history("SWAP", (qubit1, qubit2))
+    
+    def run(self):
+        
+        '''Execute the circuit. Return the result.'''
+        for gate in self.circuit:
+            self.state = gate.act(self.state)
+        
+    def run_and_reset(self):
+        '''Execute the circuit and reset the circuit. Return the result.'''
+        self.run()
+        state = self.state
+        self.reset_circuit()
+        return state
+
     def prob(self):
         prob = np.abs(self.state**2)
         return prob
 
     def measure(self, n_shots=1):
         ''' n: number of shots 
             indexs: the index of the qubit(s) being measured '''
@@ -183,21 +287,22 @@
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
+                # 'exp': lambda axis, theta: f'\\gate{R_{axis}}'
             }
 
             max_gate_length = max(len(gates) for gates in self.gate_history.values())
             
             quantikz_str = "\\begin{quantikz}\n"
             
             for qubit in range(self.n_qubit):
@@ -221,139 +326,29 @@
             # Fixing the positions of CNOT gates
             # quantikz_str = quantikz_str.replace('\\ctrl & \\targ', '\\targ & \\ctrl')
             
             quantikz_str += "\\end{quantikz}"
             
             print(quantikz_str)
 
-        
-
-class Qubits_2(Qubit):
-
-    def __init__(self):
-        super().__init__()
-        self.state = np.zeros(4, dtype=np.complex_)
-        self.state[0] = 1
-        self.n_qubit = 2
-        self._get_state_dict()
-        self.cnot_01 = np.array([[1, 0, 0, 0], 
-                                [0, 1, 0, 0], 
-                                [0, 0, 0, 1], 
-                                [0, 0, 1, 0]])
-        
-        self.cnot_10 = np.array([[1, 0, 0, 0], 
-                                [0, 0, 0, 1], 
-                                [0, 0, 1, 0], 
-                                [0, 1, 0, 0]])
-        
-        self.swp = np.array([[1, 0, 0, 0], 
-                              [0, 0, 1, 0], 
-                              [0, 1, 0, 0], 
-                              [0, 0, 0, 1]])
-        self._get_gate_history()
-
-    def copy(self):
-        new_qubit = Qubits_2()
-        new_qubit.state = self.state.copy()
-        new_qubit.n_qubit = self.n_qubit
-        return new_qubit
-
-    def cnot(self, i, j):
-        if i == 0 and j == 1:
-            self.state = self.cnot_01 @ self.state
-        elif i == 1 and j == 0:
-            self.state = self.cnot_10 @ self.state
-        else:
-            raise ValueError("Invalid indices")
-        
-    
-    def swap(self, qubit_i=0, qubit_j=1):
-        self.state = self.swp @ self.state 
-
-
-class Qubits(Qubits_2):
-
-    def __init__(self,n):
-        super().__init__()
-        self.state = np.zeros(2**n, dtype=np.complex_)
-        self.state[0] = 1
-        self.n_qubit = n
-        self._get_state_dict()
-        # print(self.state_dict)
-        self._get_gate_history()
-        
-    
-    def copy(self):
-        new_qubits = Qubits(self.n_qubit)
-        new_qubits.state = self.state.copy()
-        return new_qubits
-
-
-    def _find_flipped_state(self, target, state):
-        ''' 
-        input: target: int (0,n_qubit-1), index of the target qubit. 
-        Given a state, |abcd>, find the index where the target qubit is flipped. '''
-        flipped_state = list(state)
-        if state[target] == "1":
-            flipped_state[target] = '0'
-        else:
-            flipped_state[target] = '1'
-
-        return "".join(flipped_state)
-    
-    def cnot(self, control, target):
-        
-        if self.n_qubit == 1:
-            raise ValueError("The CNOT gate can not be applied to a single qubit.")
-        self._get_state_dict()
-        new_state_dict = self.state_dict.copy()
-        # print(new_state_dict)
-        for state in self.state_dict.keys():
-            if state[control] == "1":
-                flipped_state = self._find_flipped_state(target, state)
-                new_state_dict[flipped_state] = self.state_dict[state]
-
-        # print(len(new_state_dict.values()))
-        self.state = np.fromiter(new_state_dict.values(), dtype=np.complex_)
-        self._update_gate_history("CNOT", (control, target))
 
-    def _find_swapped_state(self, i, j, state):
-        swapped_state = list(state)
-
-        swapped_state[i] = state[j] 
-        swapped_state[j] = state[i]
-
-        return "".join(swapped_state)
+if __name__ == "__main__":
+    qc = Qubits(6)
+    # qc.H(1)
+    # qc.H(0)
 
-        
-    def swap(self, qubit1, qubit2):
+    # qc.CNOT(0,1)
+    # qc.CNOT(1,2)
+    # qc.CNOT(2,3)
 
-        if self.n_qubit == 1:
-            raise ValueError("The SWAP gate can not be applied to a single qubit.")
-        self._get_state_dict() 
-        new_state_dict = self.state_dict.copy()
 
-        for state in self.state_dict.keys():
-            swapped_state = self._find_swapped_state(qubit1, qubit2, state)
-            new_state_dict[swapped_state] = self.state_dict[state]
+    # qc.run()
+    # print(qc)
 
-        # print(len(new_state_dict.values()))
-        self.state = np.fromiter(new_state_dict.values(), dtype=np.complex_)
-        self._update_gate_history("SWAP", (qubit1, qubit2))
-    
+    # qc.X(1)
+    # qc.Y(0)
+    # qc.rx(0.4, 1)
 
+    # print(qc.gate_history)
+    # qc.draw(True)
 
-if __name__ == "__main__":
-    qc = Qubits(4)
-    print(qc.n_qubit)
-    print(qc)
-
-    qc.hadamard(0)
-    qc.X(1)
-    qc.cnot(1,0)
-    # qc.swap(0,1)
-    qc.Y(0)
-    # qc.rx(0.4, 1)
-    
-    qc.rx(-1.2080928149562626, 1)
-    print(qc.gate_history)
-    qc.draw(True)
+    print(qc)
```

### Comparing `Quanthon-0.3.5/Quanthon/expectation.py` & `Quanthon-0.3.5.1/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/mappers.py` & `Quanthon-0.3.5.1/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.5.1/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.5.1/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/ut_test_jw.py` & `Quanthon-0.3.5.1/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon/utils.py` & `Quanthon-0.3.5.1/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.5.1/Quanthon.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.5
+Version: 0.3.5.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -98,25 +98,10 @@
 # Perform a CNOT operation between the first and second qubit
 two_qubits.CONT(0, 1)
 
 two_qubits.SWAP(0, 1)
 ```
 
 
-## NEW IN VERSION 0.3:
-- You must now use Qubits.run() to execute the circuit after applying the gates.
-    
-```python
-qc = Qubits(4)
-qc.H(0)
-```
-
-- Hadamard gates are now called *Qubits.H(i)* in order to be consistent.
-Old:
-```python
-qc.Hadamard(0)
-```
-New:
-```python
-qc.H(0)
-```
+## NEW IN VERSION 0.3.5:
+- VQE now supports non-Hermitian 'Hamiltonian's, but why would you ever need it?
```

### Comparing `Quanthon-0.3.5/Quanthon.egg-info/SOURCES.txt` & `Quanthon-0.3.5.1/Quanthon.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 LICENSE
 README.md
 setup.py
 Quanthon/Expectation.py
 Quanthon/Models.py
 Quanthon/__init__.py
 Quanthon/algorithms.py
-Quanthon/algorithms_new.py
 Quanthon/ansatzs.py
 Quanthon/base.py
 Quanthon/expectation.py
 Quanthon/mappers.py
-Quanthon/new_base.py
 Quanthon/physics.py
 Quanthon/ut_pyscf_mel.py
 Quanthon/ut_qiskit_hamiltonian.py
 Quanthon/ut_test_jw.py
 Quanthon/utils.py
 Quanthon.egg-info/PKG-INFO
 Quanthon.egg-info/SOURCES.txt
```

### Comparing `Quanthon-0.3.5/README.md` & `Quanthon-0.3.5.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -74,25 +74,10 @@
 # Perform a CNOT operation between the first and second qubit
 two_qubits.CONT(0, 1)
 
 two_qubits.SWAP(0, 1)
 ```
 
 
-## NEW IN VERSION 0.3:
-- You must now use Qubits.run() to execute the circuit after applying the gates.
-    
-```python
-qc = Qubits(4)
-qc.H(0)
-```
-
-- Hadamard gates are now called *Qubits.H(i)* in order to be consistent.
-Old:
-```python
-qc.Hadamard(0)
-```
-New:
-```python
-qc.H(0)
-```
+## NEW IN VERSION 0.3.5:
+- VQE now supports non-Hermitian 'Hamiltonian's, but why would you ever need it?
```

### Comparing `Quanthon-0.3.5/setup.py` & `Quanthon-0.3.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.5" #####
+version = "0.3.5.1" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.5/tests/test_cmp_qk.py` & `Quanthon-0.3.5.1/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.5/tests/test_vqes.py` & `Quanthon-0.3.5.1/tests/test_vqes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .test_cmp_qk import qiskit_hardware
 from .test_utils import is_hermitian
 
 
 class AlgorithmTest(unittest.TestCase):
 
 
-    def _test_vqe(self):
+    def test_vqe(self):
 
         op_str =[("II", -1.052373245772859),
                     ("IZ", 0.39793742484318045),
                     ("ZI", -0.39793742484318045),
                     ("ZZ", -0.01128010425623538),
                     ("XX", 0.18093119978423156),
                 ]
```

