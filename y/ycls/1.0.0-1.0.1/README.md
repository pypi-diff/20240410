# Comparing `tmp/ycls-1.0.0.tar.gz` & `tmp/ycls-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycls-1.0.0.tar", last modified: Wed Apr 10 11:03:08 2024, max compression
+gzip compressed data, was "ycls-1.0.1.tar", last modified: Wed Apr 10 11:26:13 2024, max compression
```

## Comparing `ycls-1.0.0.tar` & `ycls-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:03:08.839671 ycls-1.0.0/
--rw-rw-rw-   0        0        0     2866 2024-04-10 11:03:08.839671 ycls-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2024-04-10 10:16:00.000000 ycls-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 11:03:08.839671 ycls-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-10 11:01:51.000000 ycls-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:03:08.839671 ycls-1.0.0/ycls/
--rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.0/ycls/__init__.py
--rw-rw-rw-   0        0        0      944 2024-04-10 11:02:55.000000 ycls-1.0.0/ycls/ycls.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:03:08.839671 ycls-1.0.0/ycls.egg-info/
--rw-rw-rw-   0        0        0     2866 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 11:03:08.000000 ycls-1.0.0/ycls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 11:26:13.511210 ycls-1.0.1/
+-rw-rw-rw-   0        0        0     2976 2024-04-10 11:26:13.511210 ycls-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2666 2024-04-10 11:23:08.000000 ycls-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:26:13.511210 ycls-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-10 11:14:25.000000 ycls-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:26:13.495585 ycls-1.0.1/ycls/
+-rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.1/ycls/__init__.py
+-rw-rw-rw-   0        0        0      944 2024-04-10 11:02:55.000000 ycls-1.0.1/ycls/ycls.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:26:13.511210 ycls-1.0.1/ycls.egg-info/
+-rw-rw-rw-   0        0        0     2976 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 11:26:13.000000 ycls-1.0.1/ycls.egg-info/top_level.txt
```

### Comparing `ycls-1.0.0/PKG-INFO` & `ycls-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.0
+Version: 1.0.1
 Summary: YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
 
-YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
+YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
 
 ## Installation
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
@@ -26,51 +26,51 @@
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
 
 ## Functions
 
 ### `calculate_loudness_lufs(input_file)`
 
-This function calculates the loudness level of the input audio file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
+This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio file in LUFS.
+  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
-This function calculates the adjusted loudness suitable for YouTube content based on the input audio file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
+This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
   - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
-This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio file using the `r128gain` library.
+This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio file in dBFS.
+  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
 ```
 
-Replace `<input_file_path>` with the path to your audio file.
+Replace `<input_file_path>` with the path to your audio (or video) file.
 
 ### Example
 
 Suppose you have an audio file named `example_audio.mp3`. You can calculate its loudness metrics using the CLI:
 
 ```bash
 ycls -i example_audio.mp3
```

### Comparing `ycls-1.0.0/README.md` & `ycls-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # YCLS (YouTube Content Loudness Scanner)
 
-YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
+YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
 
 ## Installation
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
@@ -18,51 +18,51 @@
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
 
 ## Functions
 
 ### `calculate_loudness_lufs(input_file)`
 
-This function calculates the loudness level of the input audio file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
+This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio file in LUFS.
+  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
-This function calculates the adjusted loudness suitable for YouTube content based on the input audio file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
+This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
   - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
-This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio file using the `r128gain` library.
+This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio file in dBFS.
+  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
 ```
 
-Replace `<input_file_path>` with the path to your audio file.
+Replace `<input_file_path>` with the path to your audio (or video) file.
 
 ### Example
 
 Suppose you have an audio file named `example_audio.mp3`. You can calculate its loudness metrics using the CLI:
 
 ```bash
 ycls -i example_audio.mp3
```

### Comparing `ycls-1.0.0/setup.py` & `ycls-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ycls",
-    version="1.0.0",
+    version="1.0.1",
     description="YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content.",
     packages=find_packages(),
     install_requires=requirements,
     long_description=description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
```

### Comparing `ycls-1.0.0/ycls/ycls.py` & `ycls-1.0.1/ycls/ycls.py`

 * *Files identical despite different names*

### Comparing `ycls-1.0.0/ycls.egg-info/PKG-INFO` & `ycls-1.0.1/ycls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.0
+Version: 1.0.1
 Summary: YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
 
-YCLS is a Python module for calculating loudness metrics for audio files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
+YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
 
 ## Installation
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
@@ -26,51 +26,51 @@
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
 
 ## Functions
 
 ### `calculate_loudness_lufs(input_file)`
 
-This function calculates the loudness level of the input audio file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
+This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio file in LUFS.
+  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
-This function calculates the adjusted loudness suitable for YouTube content based on the input audio file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
+This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
   - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
-This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio file using the `r128gain` library.
+This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
-  - `input_file` (str): The path to the input audio file.
+  - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio file in dBFS.
+  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
 ```
 
-Replace `<input_file_path>` with the path to your audio file.
+Replace `<input_file_path>` with the path to your audio (or video) file.
 
 ### Example
 
 Suppose you have an audio file named `example_audio.mp3`. You can calculate its loudness metrics using the CLI:
 
 ```bash
 ycls -i example_audio.mp3
```

