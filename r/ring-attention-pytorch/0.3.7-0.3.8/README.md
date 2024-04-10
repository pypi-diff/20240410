# Comparing `tmp/ring-attention-pytorch-0.3.7.tar.gz` & `tmp/ring-attention-pytorch-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.7.tar", last modified: Mon Apr  8 03:47:07 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.8.tar", last modified: Tue Apr  9 15:28:21 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.7.tar` & `ring-attention-pytorch-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:47:07.307486 ring-attention-pytorch-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 03:47:07.307486 ring-attention-pytorch-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:47:07.303486 ring-attention-pytorch-0.3.7/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:47:07.307486 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 03:47:07.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 03:47:07.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:47:07.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 03:47:07.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 03:47:07.000000 ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:47:07.307486 ring-attention-pytorch-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 03:47:03.000000 ring-attention-pytorch-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 15:28:21.000000 ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:28:21.311985 ring-attention-pytorch-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-09 15:28:17.000000 ring-attention-pytorch-0.3.8/setup.py
```

### Comparing `ring-attention-pytorch-0.3.7/LICENSE` & `ring-attention-pytorch-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.7/PKG-INFO` & `ring-attention-pytorch-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.7
+Version: 0.3.8
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.7/README.md` & `ring-attention-pytorch-0.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     - [x] cuda backwards pass must have same dq, dk, dv as naive
 - [x] fix naive flash attention backwards
 - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise flash attention is ineffective
 - [x] for cuda striped attention, for backwards hack, pad the extra token once and index out when passing into Tri's cuda kernel
 - [x] find a machine with 8 GPUs and test with a quarter million tokens first
 
+- [ ] see for cuda version whether softmax_D can be computed once and cached over the ring reduce. go for modified triton backwards if notattn)
 - [ ] think about how to craft a special `Dataset` that shards across sequence length (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some cuda ring reduce impl
 - [ ] figure out how to pytest distributed pytorch
 - [ ] use sdp context manager to validate when it is possible to use `ring_flash_attn_cuda`, otherwise assert out
 
 ## Citations
```

#### html2text {}

```diff
@@ -54,33 +54,35 @@
 float16 - [x] prevent an unnecessary `tl.load` on the first ring pass - [x]
 cuda backwards pass must have same dq, dk, dv as naive - [x] fix naive flash
 attention backwards - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise
 flash attention is ineffective - [x] for cuda striped attention, for backwards
 hack, pad the extra token once and index out when passing into Tri's cuda
 kernel - [x] find a machine with 8 GPUs and test with a quarter million tokens
-first - [ ] think about how to craft a special `Dataset` that shards across
-sequence length (take into account labels for cross entropy loss) for ring
-transformer training - [ ] add ring attention to Tri's flash attention
-implementation. find some cuda ring reduce impl - [ ] figure out how to pytest
-distributed pytorch - [ ] use sdp context manager to validate when it is
-possible to use `ring_flash_attn_cuda`, otherwise assert out ## Citations
-```bibtex @article{Liu2023RingAW, title = {Ring Attention with Blockwise
-Transformers for Near-Infinite Context}, author = {Hao Liu and Matei Zaharia
-and Pieter Abbeel}, journal = {ArXiv}, year = {2023}, volume = {abs/
-2310.01889}, url = {https://api.semanticscholar.org/CorpusID:263608461} } ```
-```bibtex @article{Brandon2023StripedAF, title = {Striped Attention: Faster
-Ring Attention for Causal Transformers}, author = {William Brandon and
-Aniruddha Nrusimha and Kevin Qian and Zachary Ankner and Tian Jin and Zhiye
-Song and Jonathan Ragan-Kelley}, journal = {ArXiv}, year = {2023}, volume =
-{abs/2311.09431}, url = {https://api.semanticscholar.org/CorpusID:265220849} }
-``` ```bibtex @article{Dao2022FlashAttentionFA, title = {FlashAttention: Fast
-and Memory-Efficient Exact Attention with IO-Awareness}, author = {Tri Dao and
-Daniel Y. Fu and Stefano Ermon and Atri Rudra and Christopher R'e}, journal =
-{ArXiv}, year = {2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
+first - [ ] see for cuda version whether softmax_D can be computed once and
+cached over the ring reduce. go for modified triton backwards if notattn) - [ ]
+think about how to craft a special `Dataset` that shards across sequence length
+(take into account labels for cross entropy loss) for ring transformer training
+- [ ] add ring attention to Tri's flash attention implementation. find some
+cuda ring reduce impl - [ ] figure out how to pytest distributed pytorch - [ ]
+use sdp context manager to validate when it is possible to use
+`ring_flash_attn_cuda`, otherwise assert out ## Citations ```bibtex @article
+{Liu2023RingAW, title = {Ring Attention with Blockwise Transformers for Near-
+Infinite Context}, author = {Hao Liu and Matei Zaharia and Pieter Abbeel},
+journal = {ArXiv}, year = {2023}, volume = {abs/2310.01889}, url = {https://
+api.semanticscholar.org/CorpusID:263608461} } ``` ```bibtex @article
+{Brandon2023StripedAF, title = {Striped Attention: Faster Ring Attention for
+Causal Transformers}, author = {William Brandon and Aniruddha Nrusimha and
+Kevin Qian and Zachary Ankner and Tian Jin and Zhiye Song and Jonathan Ragan-
+Kelley}, journal = {ArXiv}, year = {2023}, volume = {abs/2311.09431}, url =
+{https://api.semanticscholar.org/CorpusID:265220849} } ``` ```bibtex @article
+{Dao2022FlashAttentionFA, title = {FlashAttention: Fast and Memory-Efficient
+Exact Attention with IO-Awareness}, author = {Tri Dao and Daniel Y. Fu and
+Stefano Ermon and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year =
+{2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
 {dao2023flashattention2, title = {Flash{A}ttention-2: Faster Attention with
 Better Parallelism and Work Partitioning, author = {Dao, Tri}, year = {2023} }
 ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
 language and compiler for tiled neural network computations}, author =
 {Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
 SIGPLAN International Workshop on Machine Learning and Programming Languages},
 year = {2019} } ```
```

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,21 @@
         kv_and_dkv = torch.stack((k, v, dk, dv))
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv_and_dkv = None
         receive_mask = None
 
+        # precompute the softmax D
+
+        D = (do * o).sum(dim = -1, keepdims = True)
+        D = rearrange(D, 'b n h 1 -> b h n 1')
+
+        # ring reduce key / values
+
         for (ring_rank, _), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
             k_ring_rank = ring_rank % ring_size
 
             k, v, dk, dv = kv_and_dkv
 
             col_splits = zip(
                 k.split(bucket_size, dim = 1),
@@ -270,21 +277,21 @@
             )
 
             for k_ind, (kc, vc, dkc, dvc, col_mask) in enumerate(col_splits):
                 col_bucket_index = k_ring_rank * per_machine_buckets + k_ind
 
                 row_splits = zip(
                     q.split(bucket_size, dim = 1),
-                    o.split(bucket_size, dim = 1),
                     do.split(bucket_size, dim = 1),
+                    D.split(bucket_size, dim = -2),
                     lse.split(bucket_size, dim = -2),
                     dq.split(bucket_size, dim = 1)
                 )
 
-                for ind, (qc, oc, doc, lsec, dqc) in enumerate(row_splits):
+                for ind, (qc, doc, Dc, lsec, dqc) in enumerate(row_splits):
                     row_bucket_index = row_ring_rank * per_machine_buckets + ind
 
                     attn_weights = einsum('b i h d, b j h d -> b h i j', qc, kc) * scale
 
                     if causal:
                         if (row_bucket_index - col_bucket_index) > num_lookback_buckets:
                             continue
@@ -307,17 +314,15 @@
                     if exists(col_mask):
                         col_mask_unsqueezed = rearrange(col_mask, 'b j -> b 1 1 j')
                         p = p.masked_fill(~col_mask_unsqueezed, 0.)
 
                     dv_chunk = einsum('b h i j, b i h d -> b j h d', p, doc)
                     dp = einsum('b i h d, b j h d -> b h i j', doc, vc)
 
-                    D = (doc * oc).sum(dim = -1, keepdims = True)
-                    D = rearrange(D, 'b n h 1 -> b h n 1')
-                    ds = p * scale * (dp - D)
+                    ds = p * scale * (dp - Dc)
 
                     dq_chunk = einsum('b h i j, b j h d -> b i h d', ds, kc)
                     dk_chunk = einsum('b h i j, b i h d -> b j h d', ds, qc)
 
                     dqc.add_(dq_chunk)
                     dkc.add_(dk_chunk)
                     dvc.add_(dv_chunk)
```

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.7/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.8/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.7
+Version: 0.3.8
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.7/setup.py` & `ring-attention-pytorch-0.3.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

