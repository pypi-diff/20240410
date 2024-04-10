# Comparing `tmp/ycls-1.0.3.tar.gz` & `tmp/ycls-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycls-1.0.3.tar", last modified: Wed Apr 10 11:45:22 2024, max compression
+gzip compressed data, was "ycls-1.0.4.tar", last modified: Wed Apr 10 12:43:21 2024, max compression
```

## Comparing `ycls-1.0.3.tar` & `ycls-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:45:22.382733 ycls-1.0.3/
--rw-rw-rw-   0        0        0     2987 2024-04-10 11:45:22.382733 ycls-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2666 2024-04-10 11:33:23.000000 ycls-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 11:45:22.382733 ycls-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-04-10 11:44:25.000000 ycls-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:45:22.367007 ycls-1.0.3/ycls/
--rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.3/ycls/__init__.py
--rw-rw-rw-   0        0        0      957 2024-04-10 11:35:51.000000 ycls-1.0.3/ycls/ycls.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:45:22.382733 ycls-1.0.3/ycls.egg-info/
--rw-rw-rw-   0        0        0     2987 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 11:45:22.000000 ycls-1.0.3/ycls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.860084 ycls-1.0.4/
+-rw-rw-rw-   0        0        0     3127 2024-04-10 12:43:21.860084 ycls-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2806 2024-04-10 12:38:30.000000 ycls-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:43:21.860084 ycls-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      688 2024-04-10 12:24:32.000000 ycls-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.844453 ycls-1.0.4/ycls/
+-rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.4/ycls/__init__.py
+-rw-rw-rw-   0        0        0      957 2024-04-10 11:35:51.000000 ycls-1.0.4/ycls/ycls.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:43:21.860084 ycls-1.0.4/ycls.egg-info/
+-rw-rw-rw-   0        0        0     3127 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 12:43:21.000000 ycls-1.0.4/ycls.egg-info/top_level.txt
```

### Comparing `ycls-1.0.3/PKG-INFO` & `ycls-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.3
+Version: 1.0.4
 Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
 
@@ -14,14 +14,21 @@
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
 ```
 
+Make sure you have `ffmpeg` installed on your system.
+
+**For Windows:**
+```bash
+winget install Gyan.FFmpeg.Essentials
+```
+
 ## Usage
 
 You can import functions from the `ycls` module using the following syntax:
 
 ```python
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
@@ -84,7 +91,8 @@
 ```
 
 ## Requirements
 
 - Python 3.6+
 - r128gain library
 - typer library
+- ffmpeg
```

### Comparing `ycls-1.0.3/README.md` & `ycls-1.0.4/ycls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+Metadata-Version: 2.1
+Name: ycls
+Version: 1.0.4
+Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
+Description-Content-Type: text/markdown
+Requires-Dist: r128gain
+Requires-Dist: typer
+
 # YCLS (YouTube Content Loudness Scanner)
 
 YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
 
 ## Installation
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
 ```
 
+Make sure you have `ffmpeg` installed on your system.
+
+**For Windows:**
+```bash
+winget install Gyan.FFmpeg.Essentials
+```
+
 ## Usage
 
 You can import functions from the `ycls` module using the following syntax:
 
 ```python
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
@@ -75,8 +90,9 @@
 Youtube Content Loudness: -9.6 dB
 ```
 
 ## Requirements
 
 - Python 3.6+
 - r128gain library
-- typer library
+- typer library
+- ffmpeg
```

### Comparing `ycls-1.0.3/setup.py` & `ycls-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ycls",
-    version="1.0.3",
+    version="1.0.4",
     description="YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.",
     packages=find_packages(),
     install_requires=requirements,
     long_description=description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
```

### Comparing `ycls-1.0.3/ycls/ycls.py` & `ycls-1.0.4/ycls/ycls.py`

 * *Files identical despite different names*

### Comparing `ycls-1.0.3/ycls.egg-info/PKG-INFO` & `ycls-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1
-Name: ycls
-Version: 1.0.3
-Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
-Description-Content-Type: text/markdown
-Requires-Dist: r128gain
-Requires-Dist: typer
-
 # YCLS (YouTube Content Loudness Scanner)
 
 YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content. It provides functions to calculate various loudness metrics such as LUFS (Loudness Units Full Scale), peak loudness in dBFS (decibels relative to full scale), and adjusted loudness suitable for YouTube.
 
 ## Installation
 
 You can install the `ycls` module using pip:
 
 ```bash
 pip install ycls
 ```
 
+Make sure you have `ffmpeg` installed on your system.
+
+**For Windows:**
+```bash
+winget install Gyan.FFmpeg.Essentials
+```
+
 ## Usage
 
 You can import functions from the `ycls` module using the following syntax:
 
 ```python
 from ycls import calculate_loudness_lufs, calculate_youtube_content_loudness, calculate_peak_dbfs
 ```
@@ -84,7 +83,8 @@
 ```
 
 ## Requirements
 
 - Python 3.6+
 - r128gain library
 - typer library
+- ffmpeg
```

