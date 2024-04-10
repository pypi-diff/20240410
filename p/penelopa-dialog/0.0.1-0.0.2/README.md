# Comparing `tmp/penelopa-dialog-0.0.1.tar.gz` & `tmp/penelopa-dialog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/penelopa-dialog-0.0.1.tar", last modified: Sat Jan  6 13:36:33 2024, max compression
+gzip compressed data, was "penelopa-dialog-0.0.2.tar", last modified: Wed Apr 10 14:04:45 2024, max compression
```

## Comparing `penelopa-dialog-0.0.1.tar` & `penelopa-dialog-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 evgenijevstafev   (501) staff       (20)        0 2024-01-06 13:36:33.770485 penelopa-dialog-0.0.1/
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)     2965 2024-01-06 13:36:33.770135 penelopa-dialog-0.0.1/PKG-INFO
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)     1963 2024-01-06 13:36:29.000000 penelopa-dialog-0.0.1/README.md
-drwxr-xr-x   0 evgenijevstafev   (501) staff       (20)        0 2024-01-06 13:36:33.767952 penelopa-dialog-0.0.1/penelopa_dialog/
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)       39 2024-01-06 13:27:06.000000 penelopa-dialog-0.0.1/penelopa_dialog/__init__.py
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)      534 2024-01-06 13:33:14.000000 penelopa-dialog-0.0.1/penelopa_dialog/main_logic.py
-drwxr-xr-x   0 evgenijevstafev   (501) staff       (20)        0 2024-01-06 13:36:33.769594 penelopa-dialog-0.0.1/penelopa_dialog.egg-info/
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)     2965 2024-01-06 13:36:33.000000 penelopa-dialog-0.0.1/penelopa_dialog.egg-info/PKG-INFO
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)      232 2024-01-06 13:36:33.000000 penelopa-dialog-0.0.1/penelopa_dialog.egg-info/SOURCES.txt
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)        1 2024-01-06 13:36:33.000000 penelopa-dialog-0.0.1/penelopa_dialog.egg-info/dependency_links.txt
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)       16 2024-01-06 13:36:33.000000 penelopa-dialog-0.0.1/penelopa_dialog.egg-info/top_level.txt
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)       38 2024-01-06 13:36:33.770616 penelopa-dialog-0.0.1/setup.cfg
--rw-r--r--   0 evgenijevstafev   (501) staff       (20)      703 2024-01-06 13:28:07.000000 penelopa-dialog-0.0.1/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 14:04:45.041851 penelopa-dialog-0.0.2/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-10 14:01:38.000000 penelopa-dialog-0.0.2/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2469 2024-04-10 14:04:45.041709 penelopa-dialog-0.0.2/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1965 2024-04-10 14:02:50.000000 penelopa-dialog-0.0.2/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 14:04:45.040512 penelopa-dialog-0.0.2/penelopa_dialog/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       39 2024-04-10 14:01:38.000000 penelopa-dialog-0.0.2/penelopa_dialog/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      192 2024-04-10 14:02:50.000000 penelopa-dialog-0.0.2/penelopa_dialog/main_logic.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 14:04:45.041397 penelopa-dialog-0.0.2/penelopa_dialog.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2469 2024-04-10 14:04:44.000000 penelopa-dialog-0.0.2/penelopa_dialog.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      270 2024-04-10 14:04:45.000000 penelopa-dialog-0.0.2/penelopa_dialog.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-10 14:04:44.000000 penelopa-dialog-0.0.2/penelopa_dialog.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       16 2024-04-10 14:04:44.000000 penelopa-dialog-0.0.2/penelopa_dialog.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-10 14:04:45.041893 penelopa-dialog-0.0.2/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      693 2024-04-10 14:02:50.000000 penelopa-dialog-0.0.2/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-10 14:04:45.041525 penelopa-dialog-0.0.2/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      796 2024-04-10 14:04:34.000000 penelopa-dialog-0.0.2/tests/test_penelopa_dialog.py
```

### Comparing `penelopa-dialog-0.0.1/PKG-INFO` & `penelopa-dialog-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: penelopa-dialog
-Version: 0.0.1
+Version: 0.0.2
 Summary: Penelopa Dialog for managing and coordinating tasks
 Home-page: https://github.com/chigwell/penelopa-dialog
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
-License: UNKNOWN
-Description: [![PyPI version](https://badge.fury.io/py/penelopa-dialog.svg)](https://badge.fury.io/py/penelopa-dialog)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-        [![Downloads](https://static.pepy.tech/badge/penelopadialog)](https://pepy.tech/project/penelopadialog)
-        
-        # Penelopa Dialog
-        
-        `Penelopa Dialog` is a Python module for creating interactive console applications. It simplifies the process of dialogues in the console, waiting for user inputs, and handling responses, making it easier to create interactive command-line tools.
-        
-        ## Installation
-        
-        To install `Penelopa Dialog`, you can use pip:
-        
-        ```bash
-        pip install penelopa-dialog
-        ```
-        
-        ## Usage
-        
-        ### As a Python Module
-        
-        You can use `Penelopa Dialog` as a module in your Python scripts.
-        
-        Example:
-        
-        ```python
-        from penelopa_dialog import PenelopaDialog
-        
-        # Initialize the dialog with a prompt message
-        dialog = PenelopaDialog("Hello, please tell me your task.")
-        
-        # Run the dialog and capture the user's input
-        user_response = dialog.run()
-        
-        print("You responded with:", user_response)
-        ```
-        
-        This example demonstrates initializing the `Penelopa Dialog` with a specific message, running the dialogue to wait for the user's input, and then printing out the response.
-        
-        ### Customizing Your Dialogue
-        
-        You can customize your dialogue by adjusting the prompt message or by extending the `PenelopaDialog` class to include more complex logic or additional interactive features.
-        
-        ## Output Example
-        
-        When you run the `Penelopa Dialog`, it displays the prompt message and waits for the user's input. Here is an example interaction:
-        
-        ```
-        Hello, please tell me your task:
-        > Refactor the database schema.
-        You responded with: Refactor the database schema.
-        ```
-        
-        ## Contributing
-        
-        Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/chigwell/penelopa-dialog/issues).
-        
-        ## License
-        
-        [MIT](https://choosealicense.com/licenses/mit/)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/penelopa-dialog.svg)](https://badge.fury.io/py/penelopa-dialog)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
+[![Downloads](https://static.pepy.tech/badge/penelopa-dialog)](https://pepy.tech/project/penelopa-dialog)
+
+# Penelopa Dialog
+
+`Penelopa Dialog` is a Python module for creating interactive console applications. It simplifies the process of dialogues in the console, waiting for user inputs, and handling responses, making it easier to create interactive command-line tools.
+
+## Installation
+
+To install `Penelopa Dialog`, you can use pip:
+
+```bash
+pip install penelopa-dialog
+```
+
+## Usage
+
+### As a Python Module
+
+You can use `Penelopa Dialog` as a module in your Python scripts.
+
+Example:
+
+```python
+from penelopa_dialog import PenelopaDialog
+
+# Initialize the dialog with a prompt message
+dialog = PenelopaDialog("Hello, please tell me your task.")
+
+# Run the dialog and capture the user's input
+user_response = dialog.run()
+
+print("You responded with:", user_response)
+```
+
+This example demonstrates initializing the `Penelopa Dialog` with a specific message, running the dialogue to wait for the user's input, and then printing out the response.
+
+### Customizing Your Dialogue
+
+You can customize your dialogue by adjusting the prompt message or by extending the `PenelopaDialog` class to include more complex logic or additional interactive features.
+
+## Output Example
+
+When you run the `Penelopa Dialog`, it displays the prompt message and waits for the user's input. Here is an example interaction:
+
+```
+Hello, please tell me your task:
+> Refactor the database schema.
+You responded with: Refactor the database schema.
+```
+
+## Contributing
+
+Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/chigwell/penelopa-dialog/issues).
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `penelopa-dialog-0.0.1/README.md` & `penelopa-dialog-0.0.2/penelopa_dialog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,25 @@
+Metadata-Version: 2.1
+Name: penelopa-dialog
+Version: 0.0.2
+Summary: Penelopa Dialog for managing and coordinating tasks
+Home-page: https://github.com/chigwell/penelopa-dialog
+Author: Eugene Evstafev
+Author-email: chigwel@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI version](https://badge.fury.io/py/penelopa-dialog.svg)](https://badge.fury.io/py/penelopa-dialog)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Downloads](https://static.pepy.tech/badge/penelopadialog)](https://pepy.tech/project/penelopadialog)
+[![Downloads](https://static.pepy.tech/badge/penelopa-dialog)](https://pepy.tech/project/penelopa-dialog)
 
 # Penelopa Dialog
 
 `Penelopa Dialog` is a Python module for creating interactive console applications. It simplifies the process of dialogues in the console, waiting for user inputs, and handling responses, making it easier to create interactive command-line tools.
 
 ## Installation
```

### Comparing `penelopa-dialog-0.0.1/setup.py` & `penelopa-dialog-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# setup.py
 from setuptools import setup, find_packages
 
+
 setup(
     name='penelopa-dialog',
-    version='0.0.1',
+    version='0.0.2',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='Penelopa Dialog for managing and coordinating tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/penelopa-dialog',
     packages=find_packages(),
```

