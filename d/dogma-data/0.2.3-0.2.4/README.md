# Comparing `tmp/dogma-data-0.2.3.tar.gz` & `tmp/dogma-data-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogma-data-0.2.3.tar", last modified: Tue Apr  9 06:17:29 2024, max compression
+gzip compressed data, was "dogma-data-0.2.4.tar", last modified: Wed Apr 10 08:57:15 2024, max compression
```

## Comparing `dogma-data-0.2.3.tar` & `dogma-data-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.084868 dogma-data-0.2.3/
--rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-09 06:17:29.084868 dogma-data-0.2.3/PKG-INFO
--rw-r--r--   0 roed     (23269) users      (100)        0 2024-03-30 18:11:44.000000 dogma-data-0.2.3/README.md
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.080868 dogma-data-0.2.3/dogma_data/
--rw-r--r--   0 roed     (23269) users      (100)      235 2024-04-08 20:03:17.000000 dogma-data-0.2.3/dogma_data/__init__.py
--rw-r--r--   0 roed     (23269) users      (100)    10688 2024-04-09 06:15:25.000000 dogma-data-0.2.3/dogma_data/_dogma_data.py
--rw-r--r--   0 roed     (23269) users      (100)      450 2024-04-02 00:00:59.000000 dogma-data-0.2.3/dogma_data/dogma_torch.py
--rw-r--r--   0 roed     (23269) users      (100)     7035 2024-04-08 23:40:28.000000 dogma-data-0.2.3/dogma_data/fasta.py
--rw-r--r--   0 roed     (23269) users      (100)      762 2024-03-31 04:28:41.000000 dogma-data-0.2.3/dogma_data/utils.py
-drwxr-xr-x   0 roed     (23269) users      (100)        0 2024-04-09 06:17:29.084868 dogma-data-0.2.3/dogma_data.egg-info/
--rw-r--r--   0 roed     (23269) users      (100)      648 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/PKG-INFO
--rw-r--r--   0 roed     (23269) users      (100)      308 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/SOURCES.txt
--rw-r--r--   0 roed     (23269) users      (100)        1 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/dependency_links.txt
--rw-r--r--   0 roed     (23269) users      (100)       98 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/requires.txt
--rw-r--r--   0 roed     (23269) users      (100)       11 2024-04-09 06:17:29.000000 dogma-data-0.2.3/dogma_data.egg-info/top_level.txt
--rw-r--r--   0 roed     (23269) users      (100)     1078 2024-04-09 06:17:20.000000 dogma-data-0.2.3/pyproject.toml
--rw-r--r--   0 roed     (23269) users      (100)       38 2024-04-09 06:17:29.084868 dogma-data-0.2.3/setup.cfg
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/
+-rw-r--r--   0 roed     (23269) root         (0)      648 2024-04-10 08:57:15.204752 dogma-data-0.2.4/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)        0 2024-04-10 03:45:24.000000 dogma-data-0.2.4/README.md
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/dogma_data/
+-rw-r--r--   0 roed     (23269) root         (0)      235 2024-04-10 03:46:52.000000 dogma-data-0.2.4/dogma_data/__init__.py
+-rw-r--r--   0 roed     (23269) root         (0)    11007 2024-04-10 05:57:55.000000 dogma-data-0.2.4/dogma_data/_dogma_data.py
+-rw-r--r--   0 roed     (23269) root         (0)      450 2024-04-10 03:45:24.000000 dogma-data-0.2.4/dogma_data/dogma_torch.py
+-rw-r--r--   0 roed     (23269) root         (0)     7292 2024-04-10 07:59:30.000000 dogma-data-0.2.4/dogma_data/fasta.py
+-rw-r--r--   0 roed     (23269) root         (0)      762 2024-04-10 03:45:24.000000 dogma-data-0.2.4/dogma_data/utils.py
+drwxr-sr-x   0 roed     (23269) root         (0)        0 2024-04-10 08:57:15.204752 dogma-data-0.2.4/dogma_data.egg-info/
+-rw-r--r--   0 roed     (23269) root         (0)      648 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/PKG-INFO
+-rw-r--r--   0 roed     (23269) root         (0)      308 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/SOURCES.txt
+-rw-r--r--   0 roed     (23269) root         (0)        1 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/dependency_links.txt
+-rw-r--r--   0 roed     (23269) root         (0)       98 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/requires.txt
+-rw-r--r--   0 roed     (23269) root         (0)       11 2024-04-10 08:57:15.000000 dogma-data-0.2.4/dogma_data.egg-info/top_level.txt
+-rw-r--r--   0 roed     (23269) root         (0)     1078 2024-04-10 08:55:46.000000 dogma-data-0.2.4/pyproject.toml
+-rw-r--r--   0 roed     (23269) root         (0)       38 2024-04-10 08:57:15.204752 dogma-data-0.2.4/setup.cfg
```

### Comparing `dogma-data-0.2.3/PKG-INFO` & `dogma-data-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.3
+Version: 0.2.4
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dogma-data-0.2.3/dogma_data/_dogma_data.py` & `dogma-data-0.2.4/dogma_data/_dogma_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import awkward as ak
 
 from numba import njit, prange
 
 from dogma_data.utils import check_equality, timer, ceildiv
 from smart_open import open as smart_open
 
-from dogma_rust import awkward_from_list_of_numpy
+from dogma_rust import awkward_from_list_of_numpy, concatenate_awkward as rust_concatenate_awkward
 
 # import os
 # os.environ['EXTRA_CLING_ARGS'] = '-O3'
 
 # import cppyy
 
 # cppyy.add_include_path(np.get_include())
@@ -33,15 +33,14 @@
         ref_point = current[-1] 
         next_adjusted = next + ref_point
         ready_to_merge.append(next_adjusted)
         i += 1
 
     return np.concatenate(ready_to_merge)
 
-
 def find_chunk_size(total_size):
     assert total_size >= 0
     # Each chunk needs to be at most 2**32 - 1, so keep dividing by 2 until we get a valid chunk size 
     current = total_size
     while current > 2**32 - 1:
         current //= 2
     return current
@@ -141,14 +140,22 @@
             new_field = field.layout.data[permutation]
             new_fields[field_name] = ak.contents.NumpyArray(new_field)
         else:
             raise NotImplementedError(f'Cannot handle layout {field.layout}')
     return ak.Array(ak.contents.RecordArray(new_fields.values(), new_fields.keys()))
     # return ak.Array(ak.layout.ListOffsetArray64(ak.layout.Index64(new_cu_seqlens), new_content))
     
+# def concatenate_awkward(awkward_arrays: list[ak.Array]) -> ak.Array:
+#     """
+#     Concatenate a list of awkward arrays into a single awkward array.
+#     """
+#     new_fields = {}
+#     arr0 = awkward_arrays[0]
+
+#     return rust_concatenate_awkward(awkward_arrays)
 
 def awkward_from_flat(all_tokens: np.ndarray, cu_seqlens: np.ndarray) -> ak.Array:
     assert all_tokens.shape[0] == cu_seqlens[-1], 'Mismatched cu_seqlens and all_tokens shapes'
     assert cu_seqlens.dtype == np.int64
     if all_tokens.dtype != np.uint8:
         warnings.warn('The input tokens are not of type np.uint8. This can mean massive amounts of wasted space. Make sure this was intentional.', RuntimeWarning)
     offsets = ak.index.Index64(cu_seqlens)
```

### Comparing `dogma-data-0.2.3/dogma_data/fasta.py` & `dogma-data-0.2.4/dogma_data/fasta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Literal
 
 import numba as nb
 from numba.typed import List
 import awkward as ak
 import numpy as np
 from dogma_data.utils import ceildiv
 import dogma_rust
@@ -111,27 +111,30 @@
 #     buffer, cu_seqlens = _parse_fasta(complete_file_text, mappings)
 
 #     offsets = ak.index.Index64(cu_seqlens)
 #     tokens = ak.contents.NumpyArray(buffer)
 #     return ak.Array(ak.contents.ListOffsetArray(offsets, tokens))
     
 
-def parse_fasta(path: str, vocab: Any) -> ak.Array:
+def parse_fasta(path: str, vocab: Any, fasta_type: Literal['protein', 'rna']) -> ak.Array:
     """
     complete_file_text: The entire contents of a fasta file as a string, including newlines
     vocab: The vocabulary to use for parsing the fasta file, must contain the tokens 'a', 't', 'c', 'g', and '<unk>'
     """
+    assert fasta_type in ['protein', 'rna'], 'fasta_type must be one of "protein" or "rna"'
     # Only parsing ATCG, which are lowercase in the vocab
     mapping_values = [*[vocab[token] for token in ['a', 't', 'c', 'g']], vocab['<unk>']]
 
-    buffer, cu_seqlens,  = dogma_rust.parse_fasta(path, np.array(mapping_values, dtype=np.uint8))
+    buffer, cu_seqlens, taxon_ids = dogma_rust.parse_fasta(path, mapping=np.array(mapping_values, dtype=np.uint8), is_rna=fasta_type == 'rna')
 
     offsets = ak.index.Index64(cu_seqlens)
     tokens = ak.contents.NumpyArray(buffer)
-    return ak.Array(ak.contents.ListOffsetArray(offsets, tokens))
+    tokens_ak = ak.Array(ak.contents.ListOffsetArray(offsets, tokens))
+
+    return ak.Array({'tokens': tokens_ak, 'taxon_id': taxon_ids})
     
 
 
 if __name__ == '__main__':
     from torchtext import vocab
     from collections import OrderedDict
     AA_VOCAB = vocab.vocab(
```

### Comparing `dogma-data-0.2.3/dogma_data/utils.py` & `dogma-data-0.2.4/dogma_data/utils.py`

 * *Files identical despite different names*

### Comparing `dogma-data-0.2.3/dogma_data.egg-info/PKG-INFO` & `dogma-data-0.2.4/dogma_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogma-data
-Version: 0.2.3
+Version: 0.2.4
 Summary: Data processing for Dogma
 Author-email: Marcel Rød <roed@stanford.edu>
 Project-URL: Homepage, https://github.com/marcelroed/dogma-data
 Project-URL: Repository, https://github.com/marcelroed/dogma-data.git
 Keywords: single-cell,RNA-seq,embedding,pytorch,uce
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dogma-data-0.2.3/pyproject.toml` & `dogma-data-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dogma-data"
 description = "Data processing for Dogma"
-version = "0.2.3"
+version = "0.2.4"
 requires-python = ">=3.11"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["single-cell", "RNA-seq", "embedding", "pytorch", "uce"]
 dependencies = [
     "lightning",
     "numpy",
```

