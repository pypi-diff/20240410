# Comparing `tmp/ycls-1.0.4.tar.gz` & `tmp/ycls-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycls-1.0.4.tar", last modified: Wed Apr 10 12:43:21 2024, max compression
+gzip compressed data, was "ycls-1.0.5.tar", last modified: Wed Apr 10 14:38:42 2024, max compression
```

## Comparing `ycls-1.0.4.tar` & `ycls-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.860084 ycls-1.0.4/
--rw-rw-rw-   0        0        0     3127 2024-04-10 12:43:21.860084 ycls-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2806 2024-04-10 12:38:30.000000 ycls-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 12:43:21.860084 ycls-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-04-10 12:24:32.000000 ycls-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.844453 ycls-1.0.4/ycls/
--rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.4/ycls/__init__.py
--rw-rw-rw-   0        0        0      957 2024-04-10 11:35:51.000000 ycls-1.0.4/ycls/ycls.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.860084 ycls-1.0.4/ycls.egg-info/
--rw-rw-rw-   0        0        0     3127 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:38:42.318450 ycls-1.0.5/
+-rw-rw-rw-   0        0        0     3059 2024-04-10 14:38:42.318450 ycls-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2738 2024-04-10 14:30:08.000000 ycls-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:38:42.318450 ycls-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      688 2024-04-10 14:37:11.000000 ycls-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:38:42.302826 ycls-1.0.5/ycls/
+-rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.5/ycls/__init__.py
+-rw-rw-rw-   0        0        0     1432 2024-04-10 14:34:06.000000 ycls-1.0.5/ycls/ycls.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:38:42.318450 ycls-1.0.5/ycls.egg-info/
+-rw-rw-rw-   0        0        0     3059 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 14:38:42.000000 ycls-1.0.5/ycls.egg-info/top_level.txt
```

### Comparing `ycls-1.0.4/PKG-INFO` & `ycls-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.4
+Version: 1.0.5
 Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
 
@@ -39,35 +39,35 @@
 
 This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
+  - The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
 This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
+  - The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
 This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
+  - The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
```

### Comparing `ycls-1.0.4/README.md` & `ycls-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,35 +31,35 @@
 
 This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
+  - The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
 This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
+  - The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
 This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
+  - The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
```

### Comparing `ycls-1.0.4/setup.py` & `ycls-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ycls",
-    version="1.0.4",
+    version="1.0.5",
     description="YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.",
     packages=find_packages(),
     install_requires=requirements,
     long_description=description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
```

### Comparing `ycls-1.0.4/ycls.egg-info/PKG-INFO` & `ycls-1.0.5/ycls.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.4
+Version: 1.0.5
 Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
 
@@ -39,35 +39,35 @@
 
 This function calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `lufs` (float): The loudness level of the input audio (or video) file in LUFS.
+  - The loudness level of the input audio (or video) file in LUFS.
 
 ### `calculate_youtube_content_loudness(input_file)`
 
 This function calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by `calculate_loudness_lufs`.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `youtube_content_loudness` (float): The adjusted loudness suitable for YouTube content in dB.
+  - The adjusted loudness suitable for YouTube content in dB.
 
 ### `calculate_peak_dbfs(input_file)`
 
 This function calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the `r128gain` library.
 
 - **Parameters:**
   - `input_file` (str): The path to the input audio (or video) file.
 
 - **Returns:**
-  - `peak` (float): The peak loudness of the input audio (or video) file in dBFS.
+  - The peak loudness of the input audio (or video) file in dBFS.
 
 ## Running the Module via CLI
 
 You can also run `ycls` from the command line interface (CLI). After installing the module, you can use it as follows:
 
 ```bash
 ycls -i <input_file_path>
```

