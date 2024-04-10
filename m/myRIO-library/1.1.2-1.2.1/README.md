# Comparing `tmp/myRIO_library-1.1.2.tar.gz` & `tmp/myRIO_library-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myRIO_library-1.1.2.tar", last modified: Thu Mar 14 22:23:22 2024, max compression
+gzip compressed data, was "myRIO_library-1.2.1.tar", last modified: Wed Apr 10 08:19:36 2024, max compression
```

## Comparing `myRIO_library-1.1.2.tar` & `myRIO_library-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:22.403783 myRIO_library-1.1.2/
--rw-rw-rw-   0        0        0     3283 2024-03-14 22:23:22.393793 myRIO_library-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myRIO_library-1.1.2/README.md
--rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myRIO_library-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1273 2024-03-14 22:23:22.426883 myRIO_library-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-03-14 22:16:30.000000 myRIO_library-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.313601 myRIO_library-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.466315 myRIO_library-1.1.2/src/myRIO_API/
--rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myRIO_library-1.1.2/src/myRIO_API/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.527296 myRIO_library-1.1.2/src/myRIO_API/examples/
--rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myRIO_library-1.1.2/src/myRIO_API/examples/README_server.txt
--rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myRIO_library-1.1.2/src/myRIO_API/examples/myRIO_API
--rw-rw-rw-   0        0        0     5802 2024-03-14 20:37:51.000000 myRIO_library-1.1.2/src/myRIO_API/myRIO_API.py
--rw-rw-rw-   0        0        0      979 2024-03-14 22:16:25.000000 myRIO_library-1.1.2/src/myRIO_API/version.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.605288 myRIO_library-1.1.2/src/myRIO_API_client/
--rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myRIO_library-1.1.2/src/myRIO_API_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.701780 myRIO_library-1.1.2/src/myRIO_API_client/examples/
--rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myRIO_library-1.1.2/src/myRIO_API_client/examples/README_client.txt
--rw-rw-rw-   0        0        0     1617 2024-03-14 21:54:43.000000 myRIO_library-1.1.2/src/myRIO_API_client/examples/client_examples.py
--rw-rw-rw-   0        0        0     7676 2024-03-14 20:49:39.000000 myRIO_library-1.1.2/src/myRIO_API_client/myRIO_API_client.py
--rw-rw-rw-   0        0        0      979 2024-03-14 22:16:16.000000 myRIO_library-1.1.2/src/myRIO_API_client/version.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:21.817312 myRIO_library-1.1.2/src/myRIO_base/
--rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myRIO_library-1.1.2/src/myRIO_base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:22.002970 myRIO_library-1.1.2/src/myRIO_base/data/
--rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myRIO_library-1.1.2/src/myRIO_base/data/Default.lvbitx
--rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myRIO_library-1.1.2/src/myRIO_base/data/High-throughput.lvbitx
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:22.226647 myRIO_library-1.1.2/src/myRIO_base/examples/
--rw-rw-rw-   0        0        0     1756 2024-03-12 10:25:50.000000 myRIO_library-1.1.2/src/myRIO_base/examples/analog-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     2626 2024-03-14 22:22:02.000000 myRIO_library-1.1.2/src/myRIO_base/examples/digital-inputs-and-outputs.py
--rw-rw-rw-   0        0        0     1435 2024-03-14 21:47:14.000000 myRIO_library-1.1.2/src/myRIO_base/examples/mxp-board-tests.py
--rw-rw-rw-   0        0        0    16911 2024-03-14 20:21:33.000000 myRIO_library-1.1.2/src/myRIO_base/myRIO_base.py
--rw-rw-rw-   0        0        0      979 2024-03-14 22:16:13.000000 myRIO_library-1.1.2/src/myRIO_base/version.py
-drwxrwxrwx   0        0        0        0 2024-03-14 22:23:22.376746 myRIO_library-1.1.2/src/myRIO_library.egg-info/
--rw-rw-rw-   0        0        0     3283 2024-03-14 22:23:20.000000 myRIO_library-1.1.2/src/myRIO_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2024-03-14 22:23:21.000000 myRIO_library-1.1.2/src/myRIO_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 22:23:21.000000 myRIO_library-1.1.2/src/myRIO_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2024-03-14 22:23:21.000000 myRIO_library-1.1.2/src/myRIO_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-03-14 22:23:21.000000 myRIO_library-1.1.2/src/myRIO_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.572133 myRIO_library-1.2.1/
+-rw-rw-rw-   0        0        0     3283 2024-04-10 08:19:36.566146 myRIO_library-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2249 2024-03-14 22:01:02.000000 myRIO_library-1.2.1/README.md
+-rw-rw-rw-   0        0        0       78 2024-03-01 11:10:42.000000 myRIO_library-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1273 2024-04-10 08:19:36.576114 myRIO_library-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-04-10 08:15:09.000000 myRIO_library-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.382138 myRIO_library-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.420115 myRIO_library-1.2.1/src/myRIO_API/
+-rw-rw-rw-   0        0        0       73 2024-03-11 14:39:40.000000 myRIO_library-1.2.1/src/myRIO_API/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.431115 myRIO_library-1.2.1/src/myRIO_API/examples/
+-rw-rw-rw-   0        0        0     1067 2024-03-11 16:34:21.000000 myRIO_library-1.2.1/src/myRIO_API/examples/README_server.txt
+-rw-rw-rw-   0        0        0      602 2024-03-11 14:24:10.000000 myRIO_library-1.2.1/src/myRIO_API/examples/myRIO_API
+-rw-rw-rw-   0        0        0     5802 2024-03-14 20:37:51.000000 myRIO_library-1.2.1/src/myRIO_API/myRIO_API.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 08:15:27.000000 myRIO_library-1.2.1/src/myRIO_API/version.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.445133 myRIO_library-1.2.1/src/myRIO_API_client/
+-rw-rw-rw-   0        0        0       80 2024-03-12 05:47:26.000000 myRIO_library-1.2.1/src/myRIO_API_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.455129 myRIO_library-1.2.1/src/myRIO_API_client/examples/
+-rw-rw-rw-   0        0        0      612 2024-03-12 09:54:55.000000 myRIO_library-1.2.1/src/myRIO_API_client/examples/README_client.txt
+-rw-rw-rw-   0        0        0     1617 2024-03-14 21:54:43.000000 myRIO_library-1.2.1/src/myRIO_API_client/examples/client_examples.py
+-rw-rw-rw-   0        0        0     7676 2024-03-14 20:49:39.000000 myRIO_library-1.2.1/src/myRIO_API_client/myRIO_API_client.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 08:15:43.000000 myRIO_library-1.2.1/src/myRIO_API_client/version.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.471113 myRIO_library-1.2.1/src/myRIO_base/
+-rw-rw-rw-   0        0        0       74 2024-03-12 09:59:59.000000 myRIO_library-1.2.1/src/myRIO_base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.486114 myRIO_library-1.2.1/src/myRIO_base/data/
+-rw-rw-rw-   0        0        0  2957199 2016-12-02 19:23:24.000000 myRIO_library-1.2.1/src/myRIO_base/data/Default.lvbitx
+-rw-rw-rw-   0        0        0  2906853 2022-07-10 07:27:56.000000 myRIO_library-1.2.1/src/myRIO_base/data/High-throughput.lvbitx
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.525114 myRIO_library-1.2.1/src/myRIO_base/examples/
+-rw-rw-rw-   0        0        0  8277342 2024-04-10 07:58:35.000000 myRIO_library-1.2.1/src/myRIO_base/examples/PinkPanther.csv
+-rw-rw-rw-   0        0        0     1756 2024-03-12 10:25:50.000000 myRIO_library-1.2.1/src/myRIO_base/examples/analog-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     2626 2024-03-14 22:22:02.000000 myRIO_library-1.2.1/src/myRIO_base/examples/digital-inputs-and-outputs.py
+-rw-rw-rw-   0        0        0     1435 2024-03-14 21:47:14.000000 myRIO_library-1.2.1/src/myRIO_base/examples/mxp-board-tests.py
+-rw-rw-rw-   0        0        0      700 2024-04-10 08:09:53.000000 myRIO_library-1.2.1/src/myRIO_base/examples/waveform-test.py
+-rw-rw-rw-   0        0        0    18956 2024-04-10 08:10:08.000000 myRIO_library-1.2.1/src/myRIO_base/myRIO_base.py
+-rw-rw-rw-   0        0        0     1048 2024-04-10 08:15:02.000000 myRIO_library-1.2.1/src/myRIO_base/version.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:19:36.557114 myRIO_library-1.2.1/src/myRIO_library.egg-info/
+-rw-rw-rw-   0        0        0     3283 2024-04-10 08:19:36.000000 myRIO_library-1.2.1/src/myRIO_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2024-04-10 08:19:36.000000 myRIO_library-1.2.1/src/myRIO_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:19:36.000000 myRIO_library-1.2.1/src/myRIO_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2024-04-10 08:19:36.000000 myRIO_library-1.2.1/src/myRIO_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-10 08:19:36.000000 myRIO_library-1.2.1/src/myRIO_library.egg-info/top_level.txt
```

### Comparing `myRIO_library-1.1.2/PKG-INFO` & `myRIO_library-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.1.2
+Version: 1.2.1
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.1.2/README.md` & `myRIO_library-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/setup.cfg` & `myRIO_library-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/setup.py` & `myRIO_library-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='myRIO_library',
-version='1.1.2',
+version='1.2.1',
 author='Aitzol Ezeiza Ramos',
 author_email='aitzol.ezeiza@ehu.eus',
 description='A library to control the myRIO board from National Instruments',
 long_description=long_description,
 long_description_content_type='text/markdown',
 
 packages=find_packages('src'),
```

### Comparing `myRIO_library-1.1.2/src/myRIO_API/examples/README_server.txt` & `myRIO_library-1.2.1/src/myRIO_API/examples/README_server.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API/examples/myRIO_API` & `myRIO_library-1.2.1/src/myRIO_API/examples/myRIO_API`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API/myRIO_API.py` & `myRIO_library-1.2.1/src/myRIO_API/myRIO_API.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API/version.py` & `myRIO_library-1.2.1/src/myRIO_API/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.1.2"
+__version__ = "1.2.1"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -12,8 +12,9 @@
 1.0.0: API_client added and a name change for the myRIO_base package (2024/03/12)
 1.0.1: minor fix: format change to solve 3.5 compatibility (2024/03/12)
 1.0.2: minor change in the API client examples (2024/03/12)
 1.0.3: GitHub Actions (2024/03/14)
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
+1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 """
```

### Comparing `myRIO_library-1.1.2/src/myRIO_API_client/examples/README_client.txt` & `myRIO_library-1.2.1/src/myRIO_API_client/examples/README_client.txt`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API_client/examples/client_examples.py` & `myRIO_library-1.2.1/src/myRIO_API_client/examples/client_examples.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API_client/myRIO_API_client.py` & `myRIO_library-1.2.1/src/myRIO_API_client/myRIO_API_client.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_API_client/version.py` & `myRIO_library-1.2.1/src/myRIO_API_client/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.1.2"
+__version__ = "1.2.1"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -12,8 +12,9 @@
 1.0.0: API_client added and a name change for the myRIO_base package (2024/03/12)
 1.0.1: minor fix: format change to solve 3.5 compatibility (2024/03/12)
 1.0.2: minor change in the API client examples (2024/03/12)
 1.0.3: GitHub Actions (2024/03/14)
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
+1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 """
```

### Comparing `myRIO_library-1.1.2/src/myRIO_base/data/Default.lvbitx` & `myRIO_library-1.2.1/src/myRIO_base/data/Default.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_base/data/High-throughput.lvbitx` & `myRIO_library-1.2.1/src/myRIO_base/data/High-throughput.lvbitx`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_base/examples/analog-inputs-and-outputs.py` & `myRIO_library-1.2.1/src/myRIO_base/examples/analog-inputs-and-outputs.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_base/examples/digital-inputs-and-outputs.py` & `myRIO_library-1.2.1/src/myRIO_base/examples/digital-inputs-and-outputs.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_base/examples/mxp-board-tests.py` & `myRIO_library-1.2.1/src/myRIO_base/examples/mxp-board-tests.py`

 * *Files identical despite different names*

### Comparing `myRIO_library-1.1.2/src/myRIO_base/myRIO_base.py` & `myRIO_library-1.2.1/src/myRIO_base/myRIO_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 """
 
 from nifpga import Session
 from typing import Tuple
 import ctypes
 import pkg_resources
 
+
 # RGB constants
 
 RED = 2
 GREEN = 1
 BLUE = 4
 WHITE = 7
 RGB_OFF = 0
 
+
+# Support functions. They are not part of the class MyRIO, but they are used by it.
+# Feel free to use them in your own programs.
+
 def u8_to_bits (u8_number: int) -> [bool]:
     """ This function converts u8 values to an array of Booleans """
     mask = 1
     one_by_one = []
     for i in range(8):
         one_by_one.append(bool((u8_number & mask) != 0))
         mask = mask * 2
@@ -100,17 +105,37 @@
 
 def volts_to_luminosity (volts: float) -> float:
     """ This function converts values in Volts 
     to luminosity in percentage (0-100%)
     """
     return 100-(volts*30.3)
 
+def extract_waveform_from_csv_file(file_name: str) -> [int]:
+    """ This function extracts a stereo waveform from a .csv file
+    and returns it as a list of I16 integers.
+    The .csv format is very basic for an audio file, but
+    the myRIO has memory limitations, so the audio files
+    must be mono and quite shorts.
+    We have tried the wave library from Python, but it does not work
+    properly with the myRIO, so we have used the csv format that 
+    can be easily generated (we used a simple LabVIEW program for that).
+    """
+    # Open and read a csv file 
+    with open(file_name, 'r') as file:
+        data = file.readlines()     # Read all the lines of the file
+        waveform = []               # Create an empty list for the waveform
+        for line in data:           # Read line by line
+            waveform.append(volts_to_raw_audio(float(line))) # Append the integer value to the list
+
+    return waveform                # Return the list
+
+
 
 class MyRIO:
-    """Class MyRIO: class for accessing NI myRIO inputs and outputs using nifgpa
+    """ Class MyRIO: class for accessing NI myRIO inputs and outputs using nifgpa
 
     NI myRIO is a programmable device with digital and analog inputs and outputs.
     It is usually programmed in LabVIEW, but it can be programmed in Python too.
     """
 
     __session = None
 
@@ -372,21 +397,37 @@
         else:
             #TODO how to report the exception (port name error)
             raw_value = 0
         channel_handler.write(raw_value)
         go_handler = self.__session.registers['AO.SYS.GO']
         go_handler.write(True)
 
+    def play_waveform(self, waveform: [int]):
+        """ plays a waveform on the myRIO Audio Output channels """
+    
+        channel_string_left = 'AO.AudioOut_L.VAL'
+        channel_string_right = 'AO.AudioOut_R.VAL'
+        channel_handler_left = self.__session.registers[channel_string_left]
+        channel_handler_right = self.__session.registers[channel_string_right]
+
+        go_handler = self.__session.registers['AO.SYS.GO']
+
+        for i in range(len(waveform)):
+            channel_handler_left.write(waveform[i])
+            channel_handler_right.write(waveform[i])
+            go_handler.write(True)
+
 if __name__ == "__main__":
     print("This is a library for working with NI myRIO in Python")
     print("It is not intended to be run directly, but to be imported in other programs.")
     print("Please, see the documentation for more information.")
     from time import sleep
     myrio1 = MyRIO()
 
+    
     print("Read digital port A:")
     print(myrio1.read_digital_port(port='A'))
     print("Read temperature from MXP port A, channel 0:")
     print(myrio1.read_MXP_temperature())
     print("Read luminosity from MXP port A, channel 1:")
     print(myrio1.read_MXP_luminosity())
     print("RGB LED in MXP port A: RED")
@@ -397,14 +438,22 @@
     sleep(1)
     print("RGB LED in MXP port A: BLUE")
     myrio1.write_MXP_RGB_LED(BLUE)
     sleep(1)
     print("RGB LED in MXP port A: OFF")
     myrio1.write_MXP_RGB_LED(RGB_OFF)
 
+    
+    # Play a simple waveform (2024/04/10)
+    print("Playing a simple waveform")
+    csv_file = pkg_resources.resource_filename('myRIO_base', 'examples/PinkPanther.csv')
+    my_waveform = extract_waveform_from_csv_file(csv_file)
+    myrio1.play_waveform(my_waveform)
+
+
 
         
 """ TODO
 
 There are some extra features that we do not cover.
 They are interesting, but are not so commonly used, and given
 their complexity, we leave them for future development.
```

### Comparing `myRIO_library-1.1.2/src/myRIO_base/version.py` & `myRIO_library-1.2.1/src/myRIO_base/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # version.py
-__version__ = "1.1.2"
+__version__ = "1.2.1"
 
 """ version notes
 0.2.0: added __del__ method to myRio class to close the connection
        to the myRIO (2024/03/05)
 0.2.3: fixed the Default.lvbitx error: now the file is distributed 
        with the package. We use the relative folder of __file__ (2024/3/6)
 0.3.0: Added examples. Fixed a bug in the digital write function. (2024/3/7)
@@ -12,8 +12,9 @@
 1.0.0: API_client added and a name change for the myRIO_base package (2024/03/12)
 1.0.1: minor fix: format change to solve 3.5 compatibility (2024/03/12)
 1.0.2: minor change in the API client examples (2024/03/12)
 1.0.3: GitHub Actions (2024/03/14)
 1.1.0: MXP functions added to base, API and API client(2024/03/15)
 1.1.1: MXP function testing bugs fixed (2024/03/15)
 1.1.2: Bug fix: examples folder was not being copied to the site-packages (2024/03/15)
+1.2.1: Added play_waveform function to the myRIO class (2024/04/10)
 """
```

### Comparing `myRIO_library-1.1.2/src/myRIO_library.egg-info/PKG-INFO` & `myRIO_library-1.2.1/src/myRIO_library.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myRIO_library
-Version: 1.1.2
+Version: 1.2.1
 Summary: A library to control the myRIO board from National Instruments
 Home-page: https://github.com/AitzolEzeizaUPVEHU/myRIO_library
 Download-URL: https://github.com/AitzolEzeizaUPVEHU/myRIO_library/archive/refs/heads/main.zip
 Author: Aitzol Ezeiza Ramos
 Author-email: aitzol.ezeiza@ehu.eus
 License: MIT
 Keywords: myRIO,NI,National Instruments,LabVIEW,Python,FPGA,Real-Time,Embedded Systems
```

### Comparing `myRIO_library-1.1.2/src/myRIO_library.egg-info/SOURCES.txt` & `myRIO_library-1.2.1/src/myRIO_library.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 src/myRIO_API_client/examples/README_client.txt
 src/myRIO_API_client/examples/client_examples.py
 src/myRIO_base/__init__.py
 src/myRIO_base/myRIO_base.py
 src/myRIO_base/version.py
 src/myRIO_base/data/Default.lvbitx
 src/myRIO_base/data/High-throughput.lvbitx
+src/myRIO_base/examples/PinkPanther.csv
 src/myRIO_base/examples/analog-inputs-and-outputs.py
 src/myRIO_base/examples/digital-inputs-and-outputs.py
 src/myRIO_base/examples/mxp-board-tests.py
+src/myRIO_base/examples/waveform-test.py
 src/myRIO_library.egg-info/PKG-INFO
 src/myRIO_library.egg-info/SOURCES.txt
 src/myRIO_library.egg-info/dependency_links.txt
 src/myRIO_library.egg-info/requires.txt
 src/myRIO_library.egg-info/top_level.txt
```

