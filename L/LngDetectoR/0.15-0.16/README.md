# Comparing `tmp/LngDetectoR-0.15.tar.gz` & `tmp/LngDetectoR-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LngDetectoR-0.15.tar", last modified: Mon Dec 11 09:35:57 2023, max compression
+gzip compressed data, was "LngDetectoR-0.16.tar", last modified: Wed Apr 10 13:06:47 2024, max compression
```

## Comparing `LngDetectoR-0.15.tar` & `LngDetectoR-0.16.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-12-11 09:35:57.813877 LngDetectoR-0.15/
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-12-11 09:35:57.812263 LngDetectoR-0.15/LngDetectoR.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2715 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      274 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       54 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       25 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       12 2023-12-11 09:35:57.000000 LngDetectoR-0.15/LngDetectoR.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2715 2023-12-11 09:35:57.813543 LngDetectoR-0.15/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2344 2023-12-11 09:35:09.000000 LngDetectoR-0.15/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-12-11 09:35:57.812518 LngDetectoR-0.15/lngdetector/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-12-10 12:53:44.000000 LngDetectoR-0.15/lngdetector/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6915 2023-12-10 13:37:21.000000 LngDetectoR-0.15/lngdetector/main.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-12-11 09:35:57.813937 LngDetectoR-0.15/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      741 2023-12-11 09:35:09.000000 LngDetectoR-0.15/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 13:06:47.147178 LngDetectoR-0.16/
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 13:06:47.144848 LngDetectoR-0.16/LngDetectoR.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3386 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      413 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       56 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       25 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       18 2024-04-10 13:06:47.000000 LngDetectoR-0.16/LngDetectoR.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3386 2024-04-10 13:06:47.147040 LngDetectoR-0.16/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2503 2024-04-10 13:05:55.000000 LngDetectoR-0.16/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 13:06:47.146114 LngDetectoR-0.16/lngdetector/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 08:46:44.000000 LngDetectoR-0.16/lngdetector/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2470 2024-04-10 10:05:45.000000 LngDetectoR-0.16/lngdetector/detect.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1554 2024-04-10 09:12:01.000000 LngDetectoR-0.16/lngdetector/extension_lang.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1835 2024-04-10 09:12:01.000000 LngDetectoR-0.16/lngdetector/mime_lang.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1631 2024-04-10 10:05:26.000000 LngDetectoR-0.16/lngdetector/report.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-10 13:06:47.147217 LngDetectoR-0.16/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1270 2024-04-10 13:05:55.000000 LngDetectoR-0.16/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 13:06:47.146782 LngDetectoR-0.16/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 11:03:32.000000 LngDetectoR-0.16/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      201 2024-04-10 13:01:50.000000 LngDetectoR-0.16/tests/test_detect.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      454 2024-04-10 13:00:03.000000 LngDetectoR-0.16/tests/test_report.py
```

### Comparing `LngDetectoR-0.15/LngDetectoR.egg-info/PKG-INFO` & `LngDetectoR-0.16/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,58 @@
-Metadata-Version: 2.1
-Name: LngDetectoR
-Version: 0.15
-Summary: A tool to detect programming languages in a directory.
-Home-page: https://github.com/chigwell/langdetector
-Author: Evgenii Evstafev
-Author-email: chigwel@gmail.com
-Keywords: language detection programming report
-Description-Content-Type: text/markdown
-Requires-Dist: prettytable
-Requires-Dist: python-magic
-
 [![PyPI version](https://badge.fury.io/py/LngDetectoR.svg)](https://badge.fury.io/py/LngDetectoR)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/lngdetector)](https://pepy.tech/project/lngdetector)
 
 # LngDetectoR
 
-LngDetectoR is a Python tool designed to analyze directories and detect the programming languages used in the files. It provides a comprehensive report including the count of files, lines of code, and the percentage of each language present.
+LngDetectoR is a Python tool designed to analyze directories and detect the programming languages used within files. It generates a comprehensive report detailing the count of files, lines of code, and the percentage of each language present.
 
 ## Installation
 
 To install LngDetectoR, you can use pip:
 
 ```bash
 pip install LngDetectoR
 ```
 
 ## Usage
 
 ### As a Command Line Tool
 
-You can use LngDetectoR directly from the command line. The basic usage is as follows:
+LngDetectoR can be utilized directly from the command line. Basic usage is as follows:
 
 ```bash
 lngdetector --directory <path-to-directory>
 ```
 
-- `--directory`: Specify the directory you want to analyze. If not specified, it uses the current working directory.
+- `--directory`: Specifies the directory to analyze. If not specified, it defaults to the current working directory.
 
 ### As a Python Module
 
-LngDetectoR can also be used as a Python module in your scripts.
+LngDetectoR can also be used within your Python scripts.
 
 Example:
 
 ```python
-from lngdetector.main import generate_report
+from lngdetector.detect import generate_report
 
-# Generate a report for the current directory
+# Generate a report for the specified directory
 report = generate_report('/path/to/your/project')
 
-# Print the pretty table
+# Display the report in a pretty table format
 report.print_pretty_table()
 
-# Get data for a specific language
+# Retrieve data for a specific language
 python_data = report.get_language_data('Python')
 print(f"Python files: {python_data['count']}, lines of code: {python_data['lines']}")
 ```
 
 ## Output Example
 
-When you run LngDetectoR, it outputs a table with the detected languages, the count of files, lines of code, and the percentage. Here is an example output:
+When you run LngDetectoR, it generates a table with the detected languages, file counts, lines of code, and their percentage contributions. Here's an example of what the output might look like:
 
 ```
 Total files: 50
 Total lines of code: 1200
 +------------+------------+---------------+------------+
 |  Language  | File Count | Lines of Code | Percentage |
 +------------+------------+---------------+------------+
@@ -73,13 +61,12 @@
 | HTML       |     10     |      200      |   16.67%   |
 | CSS        |      5     |      150      |   12.50%   |
 +------------+------------+---------------+------------+
 ```
 
 ## Contributing
 
-Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/chigwell/langdetector/issues).
+Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/chigwell/langdetector/issues) for a list of proposed features (and known issues).
 
 ## License
 
-[MIT](https://choosealicense.com/licenses/mit/)
-
+This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
```

### Comparing `LngDetectoR-0.15/PKG-INFO` & `LngDetectoR-0.16/LngDetectoR.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 Metadata-Version: 2.1
 Name: LngDetectoR
-Version: 0.15
+Version: 0.16
 Summary: A tool to detect programming languages in a directory.
 Home-page: https://github.com/chigwell/langdetector
-Author: Evgenii Evstafev
+Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
-Keywords: language detection programming report
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: prettytable
-Requires-Dist: python-magic
 
 [![PyPI version](https://badge.fury.io/py/LngDetectoR.svg)](https://badge.fury.io/py/LngDetectoR)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/lngdetector)](https://pepy.tech/project/lngdetector)
 
 # LngDetectoR
 
-LngDetectoR is a Python tool designed to analyze directories and detect the programming languages used in the files. It provides a comprehensive report including the count of files, lines of code, and the percentage of each language present.
+LngDetectoR is a Python tool designed to analyze directories and detect the programming languages used within files. It generates a comprehensive report detailing the count of files, lines of code, and the percentage of each language present.
 
 ## Installation
 
 To install LngDetectoR, you can use pip:
 
 ```bash
 pip install LngDetectoR
 ```
 
 ## Usage
 
 ### As a Command Line Tool
 
-You can use LngDetectoR directly from the command line. The basic usage is as follows:
+LngDetectoR can be utilized directly from the command line. Basic usage is as follows:
 
 ```bash
 lngdetector --directory <path-to-directory>
 ```
 
-- `--directory`: Specify the directory you want to analyze. If not specified, it uses the current working directory.
+- `--directory`: Specifies the directory to analyze. If not specified, it defaults to the current working directory.
 
 ### As a Python Module
 
-LngDetectoR can also be used as a Python module in your scripts.
+LngDetectoR can also be used within your Python scripts.
 
 Example:
 
 ```python
-from lngdetector.main import generate_report
+from lngdetector.detect import generate_report
 
-# Generate a report for the current directory
+# Generate a report for the specified directory
 report = generate_report('/path/to/your/project')
 
-# Print the pretty table
+# Display the report in a pretty table format
 report.print_pretty_table()
 
-# Get data for a specific language
+# Retrieve data for a specific language
 python_data = report.get_language_data('Python')
 print(f"Python files: {python_data['count']}, lines of code: {python_data['lines']}")
 ```
 
 ## Output Example
 
-When you run LngDetectoR, it outputs a table with the detected languages, the count of files, lines of code, and the percentage. Here is an example output:
+When you run LngDetectoR, it generates a table with the detected languages, file counts, lines of code, and their percentage contributions. Here's an example of what the output might look like:
 
 ```
 Total files: 50
 Total lines of code: 1200
 +------------+------------+---------------+------------+
 |  Language  | File Count | Lines of Code | Percentage |
 +------------+------------+---------------+------------+
@@ -73,13 +83,12 @@
 | HTML       |     10     |      200      |   16.67%   |
 | CSS        |      5     |      150      |   12.50%   |
 +------------+------------+---------------+------------+
 ```
 
 ## Contributing
 
-Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/chigwell/langdetector/issues).
+Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/chigwell/langdetector/issues) for a list of proposed features (and known issues).
 
 ## License
 
-[MIT](https://choosealicense.com/licenses/mit/)
-
+This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
```

