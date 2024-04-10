# Comparing `tmp/aiondata-0.4.1.tar.gz` & `tmp/aiondata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.4.1.tar", max compression
+gzip compressed data, was "aiondata-0.4.2.tar", max compression
```

## Comparing `aiondata-0.4.1.tar` & `aiondata-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-03-12 13:04:24.124179 aiondata-0.4.1/LICENSE
--rw-r--r--   0        0        0     4606 2024-03-12 13:04:24.124179 aiondata-0.4.1/README.md
--rw-r--r--   0        0        0      419 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/__init__.py
--rw-r--r--   0        0        0     5155 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2118 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/protein_structure.py
--rw-r--r--   0        0        0     3645 2024-03-12 13:04:24.124179 aiondata-0.4.1/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1478 2024-03-12 13:04:24.128179 aiondata-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-04-10 08:39:27.092199 aiondata-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4606 2024-04-10 08:39:27.092199 aiondata-0.4.2/README.md
+-rw-r--r--   0        0        0      419 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2118 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-04-10 08:39:27.096199 aiondata-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.2/PKG-INFO
```

### Comparing `aiondata-0.4.1/LICENSE` & `aiondata-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.1/README.md` & `aiondata-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.1/aiondata/bindingdb.py` & `aiondata-0.4.2/aiondata/bindingdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import io
-from typing import Optional
+from typing import Optional, Generator, Union
 import urllib.request
 from rdkit import Chem
 from rdkit import RDLogger
 from tqdm.auto import tqdm
 import zipfile
 
 from .datasets import GeneratedDataset
@@ -31,19 +31,25 @@
         """
         Initializes a BindingDB instance.
 
         Args:
             fd (Optional[io.BytesIO]): The file-like object containing the dataset content.
                 If `fd` is not provided, the dataset content will be fetched from the default source.
         """
-        if fd is not None:
+        if fd is None:
+            cached_sdf = self.get_cache_path().parent / "BindingDB.sdf.zip"
+            if cached_sdf.exists():
+                self.fd = self.from_compressed_file(cached_sdf)
+            else:
+                self.fd = self.from_url(self.SOURCE)
+        else:
             self.fd = fd
 
     @staticmethod
-    def _convert_to_numeric(prop_name: str, value: str):
+    def _convert_to_numeric(prop_name: str, value: str) -> Union[int, float, str, None]:
         """
         Converts a property value to numeric type.
 
         Args:
             prop_name (str): The name of the property.
             value (str): The value of the property.
 
@@ -111,34 +117,26 @@
         Returns:
             A BindingDB instance.
         """
         with open(file_path, "rb") as f:
             file_content = io.BytesIO(f.read())
         return BindingDB(file_content)
 
-    def to_generator(self, progress_bar: bool = True):
+    def to_generator(self, progress_bar: bool = True) -> Generator[dict, None, None]:
         """
         Converts the dataset to a generator.
 
         Args:
             progress_bar (bool): Whether to display a progress bar.
 
         Yields:
             dict: A dictionary representing a record in the dataset.
         """
         RDLogger.DisableLog("rdApp.*")  # Suppress RDKit warnings and errors
 
-        cached_sdf = self.get_cache_path().parent / "BindingDB.sdf.zip"
-
-        if cached_sdf.exists():
-            self.fd = self.from_compressed_file(cached_sdf)
-
-        if self.fd is None:
-            self.fd = self.from_url(self.SOURCE)
-
         sd = Chem.ForwardSDMolSupplier(self.fd, sanitize=False, removeHs=False)
 
         if progress_bar:
             pb = tqdm
         else:
 
             def pb(x, **kwargs):
```

### Comparing `aiondata-0.4.1/aiondata/datasets.py` & `aiondata-0.4.2/aiondata/datasets.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.1/aiondata/moleculenet.py` & `aiondata-0.4.2/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.1/aiondata/protein_structure.py` & `aiondata-0.4.2/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.1/aiondata/weizmann_ccca.py` & `aiondata-0.4.2/aiondata/weizmann_ccca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import urllib.request
 import zipfile
 import io
 from typing import Tuple
 import warnings
 import polars as pl
 from scipy.io import mmread
+from scipy.sparse import issparse, coo_matrix
+import numpy as np
 
 from .datasets import ParquetDataset
 
 
 class Weizmann3CA(ParquetDataset):
     """Curated Cancer Cell Atlas of collected, annotated and analyzed cancer scRNA-seq datasets from the Weizmann Institute of Science."""
 
     COLLECTION = "weizmann_ccca"
     SOURCE = "https://raw.githubusercontent.com/aion-labs/aiondata/main/data/3ca_links.parquet"
 
     def __getitem__(
         self, study_name_to_find: str
-    ) -> Tuple[pl.DataFrame, list, pl.DataFrame, "NDArray[Any]"]:
+    ) -> Tuple[pl.DataFrame, list, pl.DataFrame, coo_matrix]:
         """
         Retrieve data for a specific study name.
 
         Args:
             study_name_to_find (str): The study name to search for.
 
         Returns:
@@ -57,14 +59,58 @@
                 matrix_file_name = [
                     f for f in zip_file.namelist() if f.endswith(".mtx")
                 ][0]
                 exp_data = self._load_mtx_from_zip(zip_file, matrix_file_name)
 
         return cells, genes, metadata, exp_data
 
+    def get_gene_expression_by_cell(self, study_name: str) -> list:
+        """
+        Retrieves the gene expression data for each cell in a given study.
+
+        Args:
+            study_name (str): The name of the study.
+
+        Returns:
+            list: A list of dictionaries, where each dictionary represents the gene expression data for a cell.
+                  Each dictionary contains the cell name as well as the gene expression values for that cell.
+        """
+        cells, genes, _, exp_data = self[study_name]
+
+        cell_gene_expression_dicts = []
+
+        if issparse(exp_data):
+            exp_data_csc = exp_data.tocsc()  # Ensure it's in a column-suitable format
+        else:
+            raise ValueError("exp_data must be a scipy sparse matrix.")
+
+        cell_names = cells["cell_name"].to_list()
+        cell_types = cells["cell_type"].to_list()
+
+        for col_idx, (cell_name, cell_type) in enumerate(zip(cell_names, cell_types)):
+            cell_data = (
+                exp_data_csc[:, col_idx].toarray().ravel()
+            )  # Get expression values for the current cell
+            gene_expression_dict = {
+                genes[row_idx]: cell_data[row_idx]
+                for row_idx in range(len(genes))
+                if cell_data[row_idx] != 0
+            }
+
+            if gene_expression_dict:
+                # Prepend the cell name to the dictionary
+                cell_gene_expression = {
+                    "_cell_name": cell_name,
+                    "_cell_type": cell_type,
+                    **gene_expression_dict,
+                }
+                cell_gene_expression_dicts.append(cell_gene_expression)
+
+        return cell_gene_expression_dicts
+
     def _download_or_cache(self, study_name: str, data_url: str) -> "os.PathLike":
         filename = study_name.replace(" ", "_") + ".zip"
         cache = self.get_cache_path().parent / filename
         if not cache.exists():
             response = urllib.request.urlopen(data_url)
             with open(cache, "wb") as fd:
                 fd.write(response.read())
```

### Comparing `aiondata-0.4.1/pyproject.toml` & `aiondata-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.4.1"
+version = "0.4.2"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -34,16 +34,18 @@
 numpy = [
     {version = "^1.26.0", python = "^3.12"},
     {version = "^1.25.2", python = "^3.11"},
     {version = "^1.25.2", python = "^3.10"}
 ]
 
 [tool.poetry.group.dev.dependencies]
-ipykernel = "^6.29.2"
-iprogress = "^0.4"
+ipykernel = "*"
+iprogress = "*"
+ipywidgets = "*"
+scikit-learn = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.0.1"
```

### Comparing `aiondata-0.4.1/PKG-INFO` & `aiondata-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.4.1
+Version: 0.4.2
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```

