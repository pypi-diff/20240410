# Comparing `tmp/cleverslice-0.0.1.tar.gz` & `tmp/cleverslice-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleverslice-0.0.1.tar", last modified: Wed Apr 10 02:50:47 2024, max compression
+gzip compressed data, was "cleverslice-1.0.0.tar", last modified: Wed Apr 10 03:14:04 2024, max compression
```

## Comparing `cleverslice-0.0.1.tar` & `cleverslice-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.130021 cleverslice-0.0.1/
--rw-rw-rw-   0        0        0     1087 2024-04-10 01:57:40.000000 cleverslice-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2125 2024-04-10 02:50:47.127022 cleverslice-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1510 2024-04-10 02:50:32.000000 cleverslice-0.0.1/README.md
--rw-rw-rw-   0        0        0      623 2024-04-10 02:50:20.000000 cleverslice-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 02:50:47.130021 cleverslice-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.079020 cleverslice-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.094021 cleverslice-0.0.1/src/cleverslice/
--rw-rw-rw-   0        0        0       29 2024-04-10 02:50:25.000000 cleverslice-0.0.1/src/cleverslice/__init__.py
--rw-rw-rw-   0        0        0     2576 2024-04-10 01:57:40.000000 cleverslice-0.0.1/src/cleverslice/sdict.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.124021 cleverslice-0.0.1/src/cleverslice.egg-info/
--rw-rw-rw-   0        0        0     2125 2024-04-10 02:50:47.000000 cleverslice-0.0.1/src/cleverslice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-10 02:50:47.000000 cleverslice-0.0.1/src/cleverslice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:50:47.000000 cleverslice-0.0.1/src/cleverslice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-10 02:50:47.000000 cleverslice-0.0.1/src/cleverslice.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.080019 cleverslice-0.0.1/src/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 02:50:47.121020 cleverslice-0.0.1/src/src/slicedict/
--rw-rw-rw-   0        0        0       29 2024-04-10 02:50:29.000000 cleverslice-0.0.1/src/src/slicedict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.448827 cleverslice-1.0.0/
+-rw-rw-rw-   0        0        0     1087 2024-04-10 01:57:40.000000 cleverslice-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2620 2024-04-10 03:14:04.445829 cleverslice-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2024-04-10 03:13:44.000000 cleverslice-1.0.0/README.md
+-rw-rw-rw-   0        0        0      623 2024-04-10 03:12:56.000000 cleverslice-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:14:04.448827 cleverslice-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.407827 cleverslice-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.418827 cleverslice-1.0.0/src/cleverslice/
+-rw-rw-rw-   0        0        0       29 2024-04-10 02:50:25.000000 cleverslice-1.0.0/src/cleverslice/__init__.py
+-rw-rw-rw-   0        0        0     2576 2024-04-10 01:57:40.000000 cleverslice-1.0.0/src/cleverslice/sdict.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.443829 cleverslice-1.0.0/src/cleverslice.egg-info/
+-rw-rw-rw-   0        0        0     2620 2024-04-10 03:14:04.000000 cleverslice-1.0.0/src/cleverslice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-10 03:14:04.000000 cleverslice-1.0.0/src/cleverslice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:14:04.000000 cleverslice-1.0.0/src/cleverslice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-10 03:14:04.000000 cleverslice-1.0.0/src/cleverslice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.407827 cleverslice-1.0.0/src/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:14:04.439828 cleverslice-1.0.0/src/src/slicedict/
+-rw-rw-rw-   0        0        0       29 2024-04-10 02:50:29.000000 cleverslice-1.0.0/src/src/slicedict/__init__.py
```

### Comparing `cleverslice-0.0.1/LICENSE` & `cleverslice-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleverslice-0.0.1/PKG-INFO` & `cleverslice-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleverslice
-Version: 0.0.1
+Version: 1.0.0
 Summary: Slice dictionaries just like tuples and lists
 Author-email: Gu waakzi <guwaakzi@gmail.com>
 Project-URL: url, https://github.com/Guwaakzi/cleverslice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,23 +34,45 @@
 ```
 
 ## Usage
 
 Here is a quick example to get you started with `cleverslice`:
 
 ```python
+
 from cleverslice import sdict
 
 my_dict = sdict({'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5})
 
+# First 3 items as a dict
+f3d = my_dict[:3]
+
+# Last 2 items as a dict
+l2d = my_dict[-2:]
+
+# Middle items as a dict, from index 1 to 3
+md = my_dict[1:3]
+
+# Every other item as a dict
+e2d = my_dict[::2]
+
+# 4th item's value
+v4 = my_dict[3]
+
+# 4th item as a dict
+d4 = my_dict[3:4]
 
 ```
 
 In this example, we first create a `cleverslice` object from a standard dictionary. We then perform a slicing operation to obtain a subset of the dictionary. The `cleverslice` object still supports all standard dictionary operations.
 
 ## Documentation
 
 For more detailed documentation, please visit our [official documentation](#).
 
 ## Contributing
 
 Contributions to `cleverslice` are welcome! If you have ideas for improvement or have found a bug, feel free to open an issue or submit a pull request. Please see our [contributing guide](CONTRIBUTING.md) for more details.
+
+
+## Acknowledgments
+A special thank you to Miss Jyu for the continuous support and encouragement throughout the development of this project. Your insight and contributions have been invaluable.
```

### Comparing `cleverslice-0.0.1/README.md` & `cleverslice-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,23 +18,45 @@
 ```
 
 ## Usage
 
 Here is a quick example to get you started with `cleverslice`:
 
 ```python
+
 from cleverslice import sdict
 
 my_dict = sdict({'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5})
 
+# First 3 items as a dict
+f3d = my_dict[:3]
+
+# Last 2 items as a dict
+l2d = my_dict[-2:]
+
+# Middle items as a dict, from index 1 to 3
+md = my_dict[1:3]
+
+# Every other item as a dict
+e2d = my_dict[::2]
+
+# 4th item's value
+v4 = my_dict[3]
+
+# 4th item as a dict
+d4 = my_dict[3:4]
 
 ```
 
 In this example, we first create a `cleverslice` object from a standard dictionary. We then perform a slicing operation to obtain a subset of the dictionary. The `cleverslice` object still supports all standard dictionary operations.
 
 ## Documentation
 
 For more detailed documentation, please visit our [official documentation](#).
 
 ## Contributing
 
 Contributions to `cleverslice` are welcome! If you have ideas for improvement or have found a bug, feel free to open an issue or submit a pull request. Please see our [contributing guide](CONTRIBUTING.md) for more details.
+
+
+## Acknowledgments
+A special thank you to Miss Jyu for the continuous support and encouragement throughout the development of this project. Your insight and contributions have been invaluable.
```

### Comparing `cleverslice-0.0.1/pyproject.toml` & `cleverslice-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cleverslice"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name = "Gu waakzi", email = "guwaakzi@gmail.com" },
 ]
 dependencies = []
 description = "Slice dictionaries just like tuples and lists"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cleverslice-0.0.1/src/cleverslice/sdict.py` & `cleverslice-1.0.0/src/cleverslice/sdict.py`

 * *Files identical despite different names*

### Comparing `cleverslice-0.0.1/src/cleverslice.egg-info/PKG-INFO` & `cleverslice-1.0.0/src/cleverslice.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleverslice
-Version: 0.0.1
+Version: 1.0.0
 Summary: Slice dictionaries just like tuples and lists
 Author-email: Gu waakzi <guwaakzi@gmail.com>
 Project-URL: url, https://github.com/Guwaakzi/cleverslice
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,23 +34,45 @@
 ```
 
 ## Usage
 
 Here is a quick example to get you started with `cleverslice`:
 
 ```python
+
 from cleverslice import sdict
 
 my_dict = sdict({'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5})
 
+# First 3 items as a dict
+f3d = my_dict[:3]
+
+# Last 2 items as a dict
+l2d = my_dict[-2:]
+
+# Middle items as a dict, from index 1 to 3
+md = my_dict[1:3]
+
+# Every other item as a dict
+e2d = my_dict[::2]
+
+# 4th item's value
+v4 = my_dict[3]
+
+# 4th item as a dict
+d4 = my_dict[3:4]
 
 ```
 
 In this example, we first create a `cleverslice` object from a standard dictionary. We then perform a slicing operation to obtain a subset of the dictionary. The `cleverslice` object still supports all standard dictionary operations.
 
 ## Documentation
 
 For more detailed documentation, please visit our [official documentation](#).
 
 ## Contributing
 
 Contributions to `cleverslice` are welcome! If you have ideas for improvement or have found a bug, feel free to open an issue or submit a pull request. Please see our [contributing guide](CONTRIBUTING.md) for more details.
+
+
+## Acknowledgments
+A special thank you to Miss Jyu for the continuous support and encouragement throughout the development of this project. Your insight and contributions have been invaluable.
```

