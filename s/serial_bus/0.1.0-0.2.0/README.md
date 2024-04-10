# Comparing `tmp/serial_bus-0.1.0.tar.gz` & `tmp/serial_bus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial_bus-0.1.0.tar", max compression
+gzip compressed data, was "serial_bus-0.2.0.tar", max compression
```

## Comparing `serial_bus-0.1.0.tar` & `serial_bus-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-03-11 13:26:43.919858 serial_bus-0.1.0/LICENSE
--rw-r--r--   0        0        0     2530 2024-03-11 20:27:54.450008 serial_bus-0.1.0/README.md
--rw-r--r--   0        0        0      830 2024-03-11 20:36:14.269669 serial_bus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      391 2024-03-11 20:27:54.450008 serial_bus-0.1.0/serial_bus/__init__.py
--rw-r--r--   0        0        0     5316 2024-03-11 20:27:54.450008 serial_bus-0.1.0/serial_bus/config.py
--rw-r--r--   0        0        0     1512 2024-03-11 20:27:54.450008 serial_bus-0.1.0/serial_bus/custom_collections.py
--rw-r--r--   0        0        0     8332 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/datastore.py
--rw-r--r--   0        0        0     3432 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/dumpers.py
--rw-r--r--   0        0        0     1617 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/exceptions.py
--rw-r--r--   0        0        0     4702 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/loaders.py
--rw-r--r--   0        0        0    13645 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/models.py
--rw-r--r--   0        0        0        0 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/__init__.py
--rw-r--r--   0        0        0      508 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/converting.py
--rw-r--r--   0        0        0      589 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/customers.json
--rw-r--r--   0        0        0      397 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/customers.toml
--rw-r--r--   0        0        0      362 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/customers.yaml
--rw-r--r--   0        0        0      362 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/customers.yml
--rw-r--r--   0        0        0      524 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/products.yaml
--rw-r--r--   0        0        0     1020 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/rendered_customers.txt
--rw-r--r--   0        0        0      362 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/mocked_data/yml_customers.yaml
--rw-r--r--   0        0        0     1183 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/models.py
--rw-r--r--   0        0        0      388 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/templates/customer.j2
--rw-r--r--   0        0        0     1459 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/test_data_conversion.py
--rw-r--r--   0        0        0     3318 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/test_models.py
--rw-r--r--   0        0        0      727 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/tests/utils.py
--rw-r--r--   0        0        0     7581 2024-03-11 20:27:54.460008 serial_bus-0.1.0/serial_bus/utils.py
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 serial_bus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-10 13:54:41.481333 serial_bus-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3111 2024-04-10 20:51:05.531879 serial_bus-0.2.0/README.md
+-rw-r--r--   0        0        0      830 2024-04-10 20:51:36.310991 serial_bus-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      391 2024-03-12 10:35:53.459485 serial_bus-0.2.0/serial_bus/__init__.py
+-rw-r--r--   0        0        0     5316 2024-03-12 10:35:53.459632 serial_bus-0.2.0/serial_bus/config.py
+-rw-r--r--   0        0        0     1500 2024-04-10 16:34:19.012043 serial_bus-0.2.0/serial_bus/custom_collections.py
+-rw-r--r--   0        0        0     8221 2024-04-10 20:38:08.754509 serial_bus-0.2.0/serial_bus/datastore.py
+-rw-r--r--   0        0        0     3432 2024-03-12 10:35:53.460022 serial_bus-0.2.0/serial_bus/dumpers.py
+-rw-r--r--   0        0        0     1617 2024-03-12 10:35:53.460133 serial_bus-0.2.0/serial_bus/exceptions.py
+-rw-r--r--   0        0        0     4702 2024-03-12 10:35:53.460262 serial_bus-0.2.0/serial_bus/loaders.py
+-rw-r--r--   0        0        0    13645 2024-03-12 10:35:53.460420 serial_bus-0.2.0/serial_bus/models.py
+-rw-r--r--   0        0        0     7764 2024-04-10 18:01:39.390015 serial_bus-0.2.0/serial_bus/utils.py
+-rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 serial_bus-0.2.0/PKG-INFO
```

### Comparing `serial_bus-0.1.0/LICENSE` & `serial_bus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/README.md` & `serial_bus-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 
 
 - **Extensibility**: The code was thought to allow for ease of extensibility. For more information and examples, refer
 to the documentation below.
 
 
 <p align="center">
-  <img src="/docs/images/serial_bus.png" alt="SerialBus" width="300"/>
+  <img src="https://github.com/theandrelima/serial_bus/blob/main/docs/images/serial_bus.png" alt="SerialBus" width="300"/>
 </p>
 
 
 ## Quick Start
-  - [Usage examples](/docs/getting_started.md#usage):
-    - [Example 1: Instantiating models from serialized data](/docs/getting_started.md#example-1-instantiating-models-from-serialized-data)
-    - [Example 2: Data Relationship & Model Rendering](/docs/getting_started.md#example-2-data-relationship--model-rendering)
-    - [Example 3: Converting data between supported formats](/docs/getting_started.md#example-3-converting-data-between-supported-formats)
-  - [Configuration & Extensibility](docs/configuration-and-extensibility.md)
-- [SerialBus Base Models](/docs/base_models.md)
-- [The GLOBAL_DATA_STORE](/docs/the_global_data_store.md)
-- [Loaders](/docs/loaders.md)
-- [Dumpers](/docs/dumpers.md)
-- [Contributing](#contributing)
+  - [Usage examples](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#usage):
+    - [Example 1: Instantiating models from serialized data](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-1-instantiating-models-from-serialized-data)
+    - [Example 2: Data Relationship & Model Rendering](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-2-data-relationship--model-rendering)
+    - [Example 3: Converting data between supported formats](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-3-converting-data-between-supported-formats)
+  - [Configuration & Extensibility](https://github.com/theandrelima/serial_bus/blob/main/docs/configuration-and-extensibility.md)
+- [SerialBus Base Models](https://github.com/theandrelima/serial_bus/blob/main/docs/base_models.md)
+- [The GLOBAL_DATA_STORE](https://github.com/theandrelima/serial_bus/blob/main/docs/the_global_data_store.md)
+- [Loaders](https://github.com/theandrelima/serial_bus/blob/main/docs/loaders.md)
+- [Dumpers](https://github.com/theandrelima/serial_bus/blob/main/docs/dumpers.md)
+- [Contributing](https://github.com/theandrelima/serial_bus/blob/main/docs/contributing.md)
```

### Comparing `serial_bus-0.1.0/pyproject.toml` & `serial_bus-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "serial_bus"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python package that standardizes data parsing from multiple serialized formats into pydantic models."
 authors = ["André Lima"]
 documentation= "https://github.com/theandrelima/serial_bus"
 keywords=["serialization", "deserialization", "parsing", "pydantic-models", "serial-to-pydantic", "pydantic-to-serial"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "serial_bus"}]
```

### Comparing `serial_bus-0.1.0/serial_bus/config.py` & `serial_bus-0.2.0/serial_bus/config.py`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/serial_bus/custom_collections.py` & `serial_bus-0.2.0/serial_bus/custom_collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
     All fields in a SerialBus model must be hashable so that the model
     instance itself can be hashable as well. Because Python's native dict
     is not hashable, this class might come in handy for SerialBus model
     fields that have to be dicts.
 
     Optionally, a code using SerialBus may use its own implementation of a
-    hashable dictionary through 'HASHABLE_DICT_MODULE' and 'HASHABLE_DICT_CLASS'
-    environment variables. See serial_bus.config.SerialBusConfig
+    hashable dictionary by informing it using the 'HASHABLE_DICT_CLS'
+    environment variable. See serial_bus.config.SerialBusConfig
     class for more details.
 
     NOTE: The requirement for a hashable dictionary is due to the fact that each
     model instance will be stored in a set data structure, implemented by the
     SerialBusSortedSet class.
     """
```

### Comparing `serial_bus-0.1.0/serial_bus/datastore.py` & `serial_bus-0.2.0/serial_bus/datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,31 +116,29 @@
     ) -> SerialBusSortedSet:
         """
         Searches the records of a given model class based on the search_params.
         Currently, only one k:v pair is supported in the search_params.
 
         Args:
             model_class (Type["SerialBusBaseModel"]): the class of the model to
-            be searched. 
-            search_params (Optional[Dict[Any, Any]], optional): a single k:v pair
-            dictionary with the key being the attribute of the model and the value
-            being the value to be searched for. If None, returns the entire
-            SerialBusSortedSet associated with model_class key. Defaults to None.
+            be searched.
+            search_params (Optional[Dict[Any, Any]], optional): a dictionary with
+            keys being the attributes of the model and the values being the values
+            to be searched for. If `None`, returns the entire SerialBusSortedSet
+            associated with `model_class` key. Defaults to None.
 
         Returns:
             SerialBusSortedSet: the SerialBusSortedSet containing the records
             that match the search_params.
         """
         cls_name = self._get_cls_name(model_class)
 
         if search_params:
-            # we only take the first k,v pair from search_params
-            search_k, value = list(search_params.items())[0]
             return SerialBusSortedSet(
-                [x for x in self.records[cls_name] if getattr(x, search_k) == value]
+                [x for x in self.records[cls_name] if all(getattr(x, k) == v for k, v in search_params.items())]
             )
 
         return self.records[cls_name]
 
     def filter(
         self,
         model_class: Type["SerialBusBaseModel"],
```

### Comparing `serial_bus-0.1.0/serial_bus/dumpers.py` & `serial_bus-0.2.0/serial_bus/dumpers.py`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/serial_bus/exceptions.py` & `serial_bus-0.2.0/serial_bus/exceptions.py`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/serial_bus/loaders.py` & `serial_bus-0.2.0/serial_bus/loaders.py`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/serial_bus/models.py` & `serial_bus-0.2.0/serial_bus/models.py`

 * *Files identical despite different names*

### Comparing `serial_bus-0.1.0/serial_bus/utils.py` & `serial_bus-0.2.0/serial_bus/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import importlib
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Type, TypeVar, Union
-
-# This module is where the 'HashableDict' will be used the most.
-# Hence, we import it here and in serial_bus.__init__.py we import
-# it from here. Other modules, including client code, should always do
-# 'from serial_bus import HashableDict'.
 from serial_bus.config import get_config
 from serial_bus.exceptions import (
     SerialBusImportError,
     SerialBusTypeError,
     UnsupportedFileFormatError,
 )
 
 GLOBAL_CONFIGS = get_config()
+
+# This module is where the 'HashableDict' will be used the most.
+# Hence, we import it here and in serial_bus.__init__.py we import
+# it from here. Other modules, including client code, should always do
+# 'from serial_bus import HashableDict'.
 _module, _, _cls = GLOBAL_CONFIGS.hashable_dict_cls.rpartition(".")
 try:
     hashable_dict_module = importlib.import_module(_module)
     HashableDict = getattr(hashable_dict_module, _cls)
 except AttributeError:
     raise SerialBusImportError(
         f"Could not import class {_cls} from module {_module}"
@@ -89,39 +89,41 @@
         )
     return loader_function(file_path)
 
 
 def convert_src_file_to(
     src_file: Union[str, Path],
     dst_format: str,
+    save_to_file: Optional[bool] = True,
     dst_file: Optional[Union[str, Path]] = None,
     *args,
     **kwargs,
 ) -> None:
     """
-    TODO: change this function behavior to OPTIONALLY save the converted data to a file.
     Converts a serialized file to another format. Saves the content of
     converted data to a file and also returns the converted data as a string.
 
-
     Args:
         src_file (str, Path): the path to the file to be converted. Can be either
         a string or a Path object.
         dst_format (str): the format to which the file will be converted.
-        dst_file (Optional[Path], optional): the path to the output file. If not
+        save_to_file (Optional[bool]): If True, the converted data will be
+        saved to a file. Defaults to True to keep compatibility with the original
+        implementation of this method.
+        dst_file (Optional[str, Path]): the path to the output file. If not
         provided, the output will be written to a file with the same name as the input
         file, but with the new extension. Defaults to None.
 
-        additional arguments and keyword arguments will be passed to the dumper
+        Any additional arguments and keyword arguments will be passed to the dumper
         function.
 
     Raises:
         UnsupportedFileFormatError: If the src_file format is not supported.
-        SerialBusImportError: If either a loader of dumper function
-        can't be found for the src_file format or dst_format respectively.
+        SerialBusImportError: If a loader of dumper function can't be found
+        for the dst_format respectively.
     """
     if isinstance(src_file, str):
         src_file = Path(src_file)
 
     if isinstance(dst_file, str):
         dst_file = Path(dst_file)
 
@@ -130,15 +132,18 @@
     try:
         dumper_function = getattr(GLOBAL_CONFIGS.dumpers_module, f"{dst_format}_dumper")
     except AttributeError:
         raise SerialBusImportError(
             f"Could not find a dumper function with name {dst_format}_dumper"
         )
 
-    dst_file = dst_file or src_file.with_suffix(f".{dst_format}")
+    if not save_to_file:
+        dst_file = None
+    else:
+        dst_file = dst_file or src_file.with_suffix(f".{dst_format}")
 
     return dumper_function(loaded_dict, dst_file, *args, **kwargs)
 
 
 def convert_flat_dict_to_hashabledict(dict_obj: dict) -> Type[HashableDictType]:
     """
     Converts a flat dictionary to a HashableDict.
```

### Comparing `serial_bus-0.1.0/PKG-INFO` & `serial_bus-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_bus
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package that standardizes data parsing from multiple serialized formats into pydantic models.
 License: MIT
 Keywords: serialization,deserialization,parsing,pydantic-models,serial-to-pydantic,pydantic-to-serial
 Author: André Lima
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -59,23 +59,23 @@
 
 
 - **Extensibility**: The code was thought to allow for ease of extensibility. For more information and examples, refer
 to the documentation below.
 
 
 <p align="center">
-  <img src="/docs/images/serial_bus.png" alt="SerialBus" width="300"/>
+  <img src="https://github.com/theandrelima/serial_bus/blob/main/docs/images/serial_bus.png" alt="SerialBus" width="300"/>
 </p>
 
 
 ## Quick Start
-  - [Usage examples](/docs/getting_started.md#usage):
-    - [Example 1: Instantiating models from serialized data](/docs/getting_started.md#example-1-instantiating-models-from-serialized-data)
-    - [Example 2: Data Relationship & Model Rendering](/docs/getting_started.md#example-2-data-relationship--model-rendering)
-    - [Example 3: Converting data between supported formats](/docs/getting_started.md#example-3-converting-data-between-supported-formats)
-  - [Configuration & Extensibility](docs/configuration-and-extensibility.md)
-- [SerialBus Base Models](/docs/base_models.md)
-- [The GLOBAL_DATA_STORE](/docs/the_global_data_store.md)
-- [Loaders](/docs/loaders.md)
-- [Dumpers](/docs/dumpers.md)
-- [Contributing](#contributing)
+  - [Usage examples](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#usage):
+    - [Example 1: Instantiating models from serialized data](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-1-instantiating-models-from-serialized-data)
+    - [Example 2: Data Relationship & Model Rendering](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-2-data-relationship--model-rendering)
+    - [Example 3: Converting data between supported formats](https://github.com/theandrelima/serial_bus/blob/main/docs/getting_started.md#example-3-converting-data-between-supported-formats)
+  - [Configuration & Extensibility](https://github.com/theandrelima/serial_bus/blob/main/docs/configuration-and-extensibility.md)
+- [SerialBus Base Models](https://github.com/theandrelima/serial_bus/blob/main/docs/base_models.md)
+- [The GLOBAL_DATA_STORE](https://github.com/theandrelima/serial_bus/blob/main/docs/the_global_data_store.md)
+- [Loaders](https://github.com/theandrelima/serial_bus/blob/main/docs/loaders.md)
+- [Dumpers](https://github.com/theandrelima/serial_bus/blob/main/docs/dumpers.md)
+- [Contributing](https://github.com/theandrelima/serial_bus/blob/main/docs/contributing.md)
```

