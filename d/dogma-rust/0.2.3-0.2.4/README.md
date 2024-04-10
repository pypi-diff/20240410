# Comparing `tmp/dogma_rust-0.2.3.tar.gz` & `tmp/dogma_rust-0.2.4.tar.gz`

## Comparing `dogma_rust-0.2.3.tar` & `dogma_rust-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.3/Cargo.toml
--rw-r--r--   0    23269      100     3526 2024-04-03 16:48:42.000000 dogma_rust-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0    23269      100      686 2024-04-07 01:43:02.000000 dogma_rust-0.2.3/.gitignore
--rw-r--r--   0    23269      100      377 2024-04-07 01:19:19.000000 dogma_rust-0.2.3/README.md
--rw-r--r--   0    23269      100     2140 2024-04-08 22:43:21.000000 dogma_rust-0.2.3/src/data.rs
--rw-r--r--   0    23269      100     4431 2024-04-08 23:00:26.000000 dogma_rust-0.2.3/src/fasta.rs
--rw-r--r--   0    23269      100     5871 2024-04-09 06:13:57.000000 dogma_rust-0.2.3/src/lib.rs
--rw-r--r--   0    23269      100     2708 2024-04-07 02:48:08.000000 dogma_rust-0.2.3/src/parallel.rs
--rw-r--r--   0    23269      100    19296 2024-04-08 23:03:02.000000 dogma_rust-0.2.3/Cargo.lock
--rw-r--r--   0    23269      100      538 2024-04-07 01:24:54.000000 dogma_rust-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.4/Cargo.toml
+-rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/.gitignore
+-rw-r--r--   0    23269        0      377 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/README.md
+-rw-r--r--   0    23269        0     2305 2024-04-10 04:14:26.000000 dogma_rust-0.2.4/src/data.rs
+-rw-r--r--   0    23269        0     5185 2024-04-10 08:10:45.000000 dogma_rust-0.2.4/src/fasta.rs
+-rw-r--r--   0    23269        0     5893 2024-04-10 08:04:45.000000 dogma_rust-0.2.4/src/lib.rs
+-rw-r--r--   0    23269        0     2708 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/src/parallel.rs
+-rw-r--r--   0    23269        0    19296 2024-04-10 04:02:22.000000 dogma_rust-0.2.4/Cargo.lock
+-rw-r--r--   0    23269        0      538 2024-04-10 03:45:24.000000 dogma_rust-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.4/PKG-INFO
```

### Comparing `dogma_rust-0.2.3/.github/workflows/CI.yml` & `dogma_rust-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.3/.gitignore` & `dogma_rust-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.3/src/data.rs` & `dogma_rust-0.2.4/src/data.rs`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,28 @@
         let cu_seqlen_offsets = arrs.iter().copied().scan(0, |acc, arr| {
             let start = *acc;
             *acc += arr.cu_seqlens.last().copied().unwrap_or(0);
             Some(start)
         }).collect::<Vec<_>>();
 
         let shifted_cu_seqlens = arrs.par_iter().zip(cu_seqlen_offsets).map(|(arr, offset)| {
-            let mut shifted = arr.cu_seqlens.clone().into_owned();
-            shifted.iter_mut().for_each(|cu_seqlen| *cu_seqlen += offset);
-            shifted
+            if offset == 0 {
+                arr.cu_seqlens.to_vec()
+            } else {
+                let mut shifted = (&arr.cu_seqlens[1..]).to_vec(); // Skip the first element
+                shifted.iter_mut().for_each(|cu_seqlen| *cu_seqlen += offset);
+                shifted
+            }
         }).collect::<Vec<_>>();
-        let shifted_cu_seqlens_bufs = shifted_cu_seqlens.iter().map(|cu_seqlens| cu_seqlens.borrow()).collect::<Vec<_>>();
 
-        let (out_cu_seqlens, _) = parallel_concatenate_buffers(&shifted_cu_seqlens_bufs);
+        let shifted_cu_seqlens_refs = shifted_cu_seqlens.iter().map(|cu_seqlens| {
+            cu_seqlens.as_slice()
+        }).collect::<Vec<_>>();
+
+        let (out_cu_seqlens, _) = parallel_concatenate_buffers(&shifted_cu_seqlens_refs);
 
 
         AwkwardArray::new(cat_content, out_cu_seqlens)
     }
 }
```

### Comparing `dogma_rust-0.2.3/src/fasta.rs` & `dogma_rust-0.2.4/src/fasta.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 use std::fs::read;
+use std::ops::Index;
 use rayon::prelude::*;
 use crate::data::AwkwardArray;
 use crate::parallel::parallel_concatenate_buffers;
 
+// struct CharMapping {
+//     a: u8,
+//     t: u8,
+//     c: u8,
+//     g: u8,
+//     all_other: u8,
+// }
 
+// Any fasta mapping can be stored in a vector of 256 elements
 struct CharMapping {
-    a: u8,
-    t: u8,
-    c: u8,
-    g: u8,
-    all_other: u8,
+    mappings: [u8; 256],
 }
 
 impl CharMapping {
-    pub fn from_mapping_vector(vec: &[u8]) -> Self {
-        assert!(vec.len() == 5);
+    fn from_pairs(mapping_pairs: &[(u8, u8)], default_value: u8) -> Self {
+        let mut mappings = [default_value; 256];
+        for (k, v) in mapping_pairs {
+            mappings[*k as usize] = *v;
+        }
         CharMapping {
-            a: vec[0],
-            t: vec[1],
-            c: vec[2],
-            g: vec[3],
-            all_other: vec[4],
+            mappings,
         }
     }
 }
 
+impl Index<u8> for CharMapping {
+    type Output = u8;
+
+    fn index(&self, index: u8) -> &Self::Output {
+        &self.mappings[index as usize]
+    }
+}
+
 pub struct ParsedFasta {
     pub sequences: AwkwardArray<'static, u8>,
     pub taxon_ids: Vec<u64>,
 }
 
 fn parse_fasta_chunk(text: &[u8], start_i: usize, end_i: usize, mapping: &CharMapping) -> ParsedFasta {
     let mut out_content = vec![];
@@ -38,22 +50,16 @@
 
     let text_length = text.len();
     while i < text_length && unsafe { *text.get_unchecked(i) } != b'>' {
         // Move to first header
         i += 1;
     }
 
-    let parse_char = |c: u8| {
-        match c {
-            b'A' => mapping.a,
-            b'T' | b'U' => mapping.t,
-            b'C' => mapping.c,
-            b'G' => mapping.g,
-            _ => mapping.all_other,
-        }
+    let parse_char = |c| {
+        mapping[c]
     };
 
     let mut current_taxon_id: Option<u64> = None;
 
     while i < text.len() {
         let c = unsafe { *text.get_unchecked(i) };
 
@@ -69,18 +75,18 @@
             let taxon_id_end = i;
             let taxon_str = std::str::from_utf8(&text[taxon_id_start..taxon_id_end]).unwrap();
             current_taxon_id = Some(taxon_str.parse::<u64>().unwrap());
             i += 1; // Move to next line
             continue;
         } else { // Parse one line
             while i < text_length && unsafe { *text.get_unchecked(i) } != b'\n' {
-                i += 1;
                 unsafe {
                     out_content.push(parse_char(*text.get_unchecked(i)));
                 }
+                i += 1;
             } // Ends if newline or end of file
             i += 1;
             out_cu_seqlens.push(out_content.len() as isize);
             out_taxon_ids.push(current_taxon_id.unwrap());
         }
     }
 
@@ -88,15 +94,15 @@
         sequences: AwkwardArray::new(out_content, out_cu_seqlens),
         taxon_ids: out_taxon_ids,
     }
     
 }
 
 
-pub(crate) fn parse_fasta(path: &str, mapping: &[u8]) -> ParsedFasta{
+pub(crate) fn parse_fasta(path: &str, mapping: &[u8], is_rna: bool) -> ParsedFasta{
     assert!(mapping.len() == 5);
 
     // Read file
     println!("Reading file");
     let data = read(path).unwrap();
 
     let mut n_threads = rayon::current_num_threads();
@@ -105,15 +111,44 @@
 
     if total_length < 100_000 {
         n_threads = 1;
     }
 
     let chunk_size = total_length.div_ceil(n_threads);
 
-    let char_mapping = CharMapping::from_mapping_vector(mapping);
+    let mapping_pairs = if is_rna {vec![
+        (b'A', 4),
+        (b'G', 5),
+        (b'C', 6),
+        (b'T', 7),
+        (b'U', 7),
+    ]} else { vec![
+        (b'A', 8 ),
+        (b'C', 9 ),
+        (b'D', 10),
+        (b'E', 11),
+        (b'F', 12),
+        (b'G', 13),
+        (b'H', 14),
+        (b'I', 15),
+        (b'K', 16),
+        (b'L', 17),
+        (b'M', 18),
+        (b'N', 19),
+        (b'P', 20),
+        (b'Q', 21),
+        (b'R', 22),
+        (b'S', 23),
+        (b'T', 24),
+        (b'V', 25),
+        (b'W', 26),
+        (b'Y', 27),
+    ]};
+
+    let char_mapping = CharMapping::from_pairs(&mapping_pairs, if is_rna {3} else {29});
 
     println!("Parsing file {path} in chunks");
 
     let chunk_results: Vec<ParsedFasta> = (0..n_threads).par_bridge().map(|i| {
         let start_i = i * chunk_size;
         let end_i = std::cmp::min((i + 1) * chunk_size, total_length);
         let chunk_result = parse_fasta_chunk(&data, start_i, end_i, &char_mapping);
```

### Comparing `dogma_rust-0.2.3/src/lib.rs` & `dogma_rust-0.2.4/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         // AwkwardArray {
 
         // }
     }
 }
 
 #[pyfunction]
-fn parse_fasta<'py>(py: Python<'py>, path: &str, mapping: PyReadonlyArray1<'py, u8>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>, Bound<'py, PyArray1<u64>>)> {
+fn parse_fasta<'py>(py: Python<'py>, path: &str, mapping: PyReadonlyArray1<'py, u8>, is_rna: bool) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>, Bound<'py, PyArray1<u64>>)> {
     let mapping = mapping.as_slice()?;
 
-    let ParsedFasta{sequences: AwkwardArray {content, cu_seqlens}, taxon_ids} = fasta::parse_fasta(path, mapping);
+    let ParsedFasta{sequences: AwkwardArray {content, cu_seqlens}, taxon_ids} = fasta::parse_fasta(path, mapping, is_rna);
 
     let content = content.into_owned().into_pyarray_bound(py);
     let cu_seqlens = cu_seqlens.into_owned().into_pyarray_bound(py);
     let taxon_ids = taxon_ids.into_pyarray_bound(py);
     Ok((content, cu_seqlens, taxon_ids))
 }
```

### Comparing `dogma_rust-0.2.3/src/parallel.rs` & `dogma_rust-0.2.4/src/parallel.rs`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.3/Cargo.lock` & `dogma_rust-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dogma-rust"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "anyhow",
  "chrono",
  "eyre",
  "num-bigint",
  "numpy",
  "pyo3",
```

### Comparing `dogma_rust-0.2.3/pyproject.toml` & `dogma_rust-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.3/PKG-INFO` & `dogma_rust-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dogma_rust
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/marcelroed/dogma-data
 Project-URL: repository, https://github.com/marcelroed/dogma-data
```

