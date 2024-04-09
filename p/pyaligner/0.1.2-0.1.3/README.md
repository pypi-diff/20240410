# Comparing `tmp/pyaligner-0.1.2.tar.gz` & `tmp/pyaligner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaligner-0.1.2.tar", last modified: Tue Mar 19 19:08:26 2024, max compression
+gzip compressed data, was "pyaligner-0.1.3.tar", last modified: Tue Apr  9 22:23:55 2024, max compression
```

## Comparing `pyaligner-0.1.2.tar` & `pyaligner-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.879934 pyaligner-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.867934 pyaligner-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.871934 pyaligner-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-19 19:08:14.000000 pyaligner-0.1.2/.github/workflows/add_assets.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-19 19:08:14.000000 pyaligner-0.1.2/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-19 19:08:14.000000 pyaligner-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-19 19:08:14.000000 pyaligner-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-19 19:08:14.000000 pyaligner-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-19 19:08:26.879934 pyaligner-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-19 19:08:14.000000 pyaligner-0.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-03-19 19:08:14.000000 pyaligner-0.1.2/dist_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.871934 pyaligner-0.1.2/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/create_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.871934 pyaligner-0.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/images/favicon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/images/gui_example.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.871934 pyaligner-0.1.2/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/scripts/pre_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs/source/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-19 19:08:14.000000 pyaligner-0.1.2/docs_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-19 19:08:14.000000 pyaligner-0.1.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/install/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 19:08:14.000000 pyaligner-0.1.2/install/PyAligner-Linux-x86_64.sh
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-19 19:08:14.000000 pyaligner-0.1.2/install/PyAligner-MacOSX-x86_64.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/pyaligner/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/pyaligner/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/notebooks/first.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/pyaligner/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/scripts/aligner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/scripts/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/pyaligner/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyaligner/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:08:26.875934 pyaligner-0.1.2/pyaligner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 19:08:26.000000 pyaligner-0.1.2/pyaligner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-19 19:08:14.000000 pyaligner-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-19 19:08:14.000000 pyaligner-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:08:26.879934 pyaligner-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.676100 pyaligner-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.664100 pyaligner-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.668100 pyaligner-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 22:23:51.000000 pyaligner-0.1.3/.github/workflows/add_assets.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-09 22:23:51.000000 pyaligner-0.1.3/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-09 22:23:51.000000 pyaligner-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 22:23:51.000000 pyaligner-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 22:23:51.000000 pyaligner-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 22:23:55.676100 pyaligner-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 22:23:51.000000 pyaligner-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-09 22:23:51.000000 pyaligner-0.1.3/README.private.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-04-09 22:23:51.000000 pyaligner-0.1.3/dist_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.668100 pyaligner-0.1.3/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/create_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.668100 pyaligner-0.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/images/favicon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/images/gui_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.668100 pyaligner-0.1.3/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/scripts/pre_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.668100 pyaligner-0.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs/source/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 22:23:51.000000 pyaligner-0.1.3/docs_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 22:23:51.000000 pyaligner-0.1.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 22:23:51.000000 pyaligner-0.1.3/install/PyAligner-Linux-x86_64.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 22:23:51.000000 pyaligner-0.1.3/install/PyAligner-MacOSX-x86_64.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/pyaligner/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/pyaligner/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/notebooks/first.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/pyaligner/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/scripts/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/scripts/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/pyaligner/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyaligner/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:23:55.672100 pyaligner-0.1.3/pyaligner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 22:23:55.000000 pyaligner-0.1.3/pyaligner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 22:23:51.000000 pyaligner-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 22:23:51.000000 pyaligner-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:23:55.676100 pyaligner-0.1.3/setup.cfg
```

### Comparing `pyaligner-0.1.2/.github/workflows/python_publish.yml` & `pyaligner-0.1.3/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/.gitignore` & `pyaligner-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/.readthedocs.yaml` & `pyaligner-0.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/LICENSE` & `pyaligner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/docs/images/favicon-192x192.png` & `pyaligner-0.1.3/docs/images/favicon-192x192.png`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/docs/images/favicon.ico` & `pyaligner-0.1.3/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/docs/images/gui_example.png` & `pyaligner-0.1.3/docs/images/gui_example.png`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/docs/source/conf.py` & `pyaligner-0.1.3/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # -- Project information
 
 project = 'pyaligner'
 project_slug = project.lower()
 # project_slug = 'uc3m-pic'
 author = metadata(project.lower())['Author-email'].split('<')[0][:-1]
 # author = 'Álvaro Ramajo'
-version = metadata(project.lower())['Version']
-# version = '0.1.5'
+# version = metadata(project.lower())['Version']
+version = '0.1.3'
 release = version
 copyright = f'{datetime.now().year}, {author}'
 # release = '0.1'
 # version = '0.1.0'
 
 # -- General configuration
```

### Comparing `pyaligner-0.1.2/docs/source/install.rst` & `pyaligner-0.1.3/docs/source/install.rst`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,29 @@
          wget "https://github.com/ramajoballester/pyaligner/releases/latest/download/PyAligner-$(uname)-$(uname -m).sh"
          bash PyAligner-$(uname)-$(uname -m).sh
 
    .. group-tab:: Windows
          
          Not available yet.
          
+You can now close the terminal and open a new one to install PyAligner.
+
+PyAligner
+---------
+
+Finally, install the PyAligner package:
+
+.. code-block:: bash
+
+   mamba activate pyaligner_env
+   pip install pyaligner
+
+
+PyAligner is now installed and ready to use. Check the :ref:`user guide` 
+chapter for more information.
 
 
 Manual installation
 +++++++++++++++++++
 
 Run each command at a time.
```

### Comparing `pyaligner-0.1.2/docs/source/user_guide.rst` & `pyaligner-0.1.3/docs/source/user_guide.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 User guide
 ==========
 
-Before using PyAligner, do not forget to install the software as 
+Before using PyAligner, do not forget to install it as 
 explained in the :ref:`installation` section.
 
 .. warning::
    Do not forget to activate the virtual environment before running any 
-   command
+   command:
+
+   .. code-block:: bash
+
+      mamba activate pyaligner_env
 
 
 Graphical User Interface
 ++++++++++++++++++++++++
 
 The graphical user interface (GUI) is the main way to interact with the
 software.
@@ -22,15 +26,15 @@
 .. figure:: ../images/gui_example.png
    :width: 10em
    :align: center
    :alt: GUI
 
 |
 
-All the commands will perform the tasks to all the files in the specified 
+All the commands will perform the specified tasks to all the files in the specified 
 folder and its subfolders. 
 
 
 Command Line Interface
 ++++++++++++++++++++++
 
 Pyaligner offers three main features: transcription, alignment and both 
@@ -74,19 +78,16 @@
 The language parameter is necessary. Check available 
 `dictionaries <https://mfa-models.readthedocs.io/en/latest/dictionary/index.html#dictionary>`_ 
 and `acoustic models <https://mfa-models.readthedocs.io/en/latest/acoustic/index.html#acoustic>`_
 
 The input folder must contain audio files and their corresponding transcription 
 text files. The transcription text files must have the same name as the 
 audio files, but with a different extension.
-
 For example, if you have an audio file called ``audio.wav``, the transcription
-file must be called ``audio.txt``.
-
-You can get more information with:
+file must be called ``audio.txt``. You can get more information with:
 
 .. code-block:: bash
 
    pyaligner align --help
 
 
 Transcription and Alignment
```

### Comparing `pyaligner-0.1.2/pyaligner/notebooks/first.ipynb` & `pyaligner-0.1.3/pyaligner/notebooks/first.ipynb`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/pyaligner/scripts/aligner.py` & `pyaligner-0.1.3/pyaligner/scripts/aligner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,64 @@
 #!/usr/bin/env python
 import argparse
 import os
 import sys
 import torch
+import time
 import whisper
+import subprocess
 from tqdm import tqdm
 from pyaligner.utils import utils
 from PyQt5.QtWidgets import QApplication
 
 
 def align_action(args, progress_signal=None, error_signal=None):
     try:
         if progress_signal:
             progress_signal.emit(0)
             QApplication.processEvents()
         # Get a list of all filenames in the input folder and its subdirectories
         folder_path = utils.get_correct_path(args.input_folder)
         filenames = []
+        audio_filenames = []
         for root, dirs, files in os.walk(folder_path):
             for file in files:
                 if file.endswith('.txt'):
                     filenames.append(os.path.join(root, file))
+                elif file.endswith(tuple(utils.audio_formats)):
+                    audio_filenames.append(os.path.join(root, file))
+                
         filenames.sort()
+        audio_filenames.sort()
+
+        # Count the number of audio files whose extension is in the blacklist
+        audio_blacklist_count = sum([1 for audio_filename in audio_filenames 
+                                    if audio_filename.endswith(tuple(utils.audio_formats_blacklist))])
+        if audio_blacklist_count > 0:
+            print(f'Converting {audio_blacklist_count} audio files to mp3 format')
+            if error_signal:
+                error_signal.emit(f'Converting {audio_blacklist_count} audio files to mp3 format')
+                QApplication.processEvents()
+
+            if progress_signal:
+                progress_signal.emit(0)
+                QApplication.processEvents()
+            # If any audio_filename is in the utils.audio_formats_blacklist, convert it to mp3 with ffmpeg
+            for audio_filename in audio_filenames:
+                if os.path.splitext(audio_filename)[1][1:] in utils.audio_formats_blacklist:
+                    new_audio_filename = os.path.splitext(audio_filename)[0] + '.mp3'
+                    audio_filename_idx = audio_filenames.index(audio_filename)
+                    command = f'ffmpeg -i {audio_filename} -q:a 0 {new_audio_filename}'
+                    os.system(command)
+                    os.remove(audio_filename)
+                    audio_filenames[audio_filename_idx] = new_audio_filename
+
+                    if progress_signal:
+                        progress_signal.emit(int(audio_filename_idx / len(audio_filenames) * 100))
+                        QApplication.processEvents()
 
         print(f'Checking MFA models for {args.language}')
         if error_signal:
             error_signal.emit(f'Checking MFA models for {args.language} language')
             QApplication.processEvents()
         os.system(f'mfa models download acoustic {args.language}')
         os.system(f'mfa models download dictionary {args.language}')
@@ -37,15 +70,20 @@
             command += ' > /dev/null 2>&1'
 
         print(f'Aligning {len(filenames)} audio-transcription files')
         if error_signal:
             error_signal.emit(f'Aligning {len(filenames)} audio-transcription files')
             QApplication.processEvents()
 
-        os.system(command)
+        # os.system(command)
+        exit_state = subprocess.run(command, shell=True, check=True)
+        if exit_state.returncode != 0:
+            raise ValueError(f'Error aligning files: {exit_state.stderr}')
+
+
         print('Alignment complete')
         if progress_signal:
             progress_signal.emit(100)
             QApplication.processEvents()
         if error_signal:
             error_signal.emit('Alignment complete')
             QApplication.processEvents()
```

### Comparing `pyaligner-0.1.2/pyaligner/scripts/gui.py` & `pyaligner-0.1.3/pyaligner/scripts/gui.py`

 * *Files identical despite different names*

### Comparing `pyaligner-0.1.2/pyaligner.egg-info/SOURCES.txt` & `pyaligner-0.1.3/pyaligner.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
+README.private.md
 dist_package.sh
 docs_requirements.txt
 environment.yml
 pyproject.toml
 requirements.txt
 .github/workflows/add_assets.yml
 .github/workflows/python_publish.yml
```

### Comparing `pyaligner-0.1.2/pyproject.toml` & `pyaligner-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools', 'setuptools-scm']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'pyaligner'
-version = '0.1.2'
+version = '0.1.3'
 authors = [
     {name='Álvaro Ramajo-Ballester', email='aramajo@ing.uc3m.es'},
 ]
 description = 'Automatic audio transcriptor and audi-text aligner'
 readme = 'README.md'
 # requires-python = '>=3.8,<3.10'
 requires-python = '>=3.7'
@@ -45,14 +45,15 @@
 
 [project.optional-dependencies]
 dev = [
     'ipykernel',
     # 'pyqt',
     'twine',
     'build',
+    'bump-my-version',
 ]
 
 docs = [
     'sphinx==7.1.2',
     'sphinx_rtd_theme==1.3.0',
     'sphinx-copybutton==0.5.1',
     'sphinx-markdown-tables==0.0.17',
@@ -64,11 +65,35 @@
 
 [tool.setuptools.packages]
 find = {namespaces = false, exclude = ['docs']}
 
 [project.scripts]
 pyaligner = "pyaligner.scripts.aligner:main"
 
+[tool.bumpversion]
+current_version = "0.1.3"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
+serialize = ["{major}.{minor}.{patch}"]
+search = "{current_version}"
+replace = "{new_version}"
+regex = false
+ignore_missing_version = false
+ignore_missing_files = false
+tag = true
+sign_tags = false
+tag_name = "v{new_version}"
+tag_message = "Bump version: {current_version} → {new_version}"
+allow_dirty = false
+commit = true
+message = "Bump version: {current_version} → {new_version}"
+commit_args = ""
+
+[[tool.bumpversion.files]]
+filename = "pyproject.toml"
+
+[[tool.bumpversion.files]]
+filename = "docs/source/conf.py"
+
 
 [project.urls]
 'Homepage' = 'https://github.com/ramajoballester/pyaligner'
 'Bug Tracker' = 'https://github.com/ramajoballester/pyaligner/issues'
```

