# Comparing `tmp/pyPCR-0.0.1.tar.gz` & `tmp/pyPCR-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPCR-0.0.1.tar", last modified: Wed Apr 10 11:18:01 2024, max compression
+gzip compressed data, was "pyPCR-0.0.2.tar", last modified: Wed Apr 10 11:32:14 2024, max compression
```

## Comparing `pyPCR-0.0.1.tar` & `pyPCR-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:18:01.002202 pyPCR-0.0.1/
--rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 pyPCR-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0    10732 2024-04-10 11:18:01.002202 pyPCR-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9769 2024-04-10 10:44:48.000000 pyPCR-0.0.1/README.md
--rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 pyPCR-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      710 2024-04-10 11:18:01.008186 pyPCR-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1330 2024-04-10 11:17:44.000000 pyPCR-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:18:00.916433 pyPCR-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 11:18:01.000208 pyPCR-0.0.1/src/PyPCR.egg-info/
--rw-rw-rw-   0        0        0    10732 2024-04-10 11:18:00.000000 pyPCR-0.0.1/src/PyPCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-04-10 11:18:00.000000 pyPCR-0.0.1/src/PyPCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:18:00.000000 pyPCR-0.0.1/src/PyPCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2024-04-10 11:18:00.000000 pyPCR-0.0.1/src/PyPCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 11:18:00.000000 pyPCR-0.0.1/src/PyPCR.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 11:18:00.967296 pyPCR-0.0.1/src/pyPCR/
--rw-rw-rw-   0        0        0    24915 2024-04-10 08:04:25.000000 pyPCR-0.0.1/src/pyPCR/Mep_panel.py
--rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 pyPCR-0.0.1/src/pyPCR/Rextractor.py
--rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 pyPCR-0.0.1/src/pyPCR/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:32:14.430903 pyPCR-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-04-09 08:47:53.000000 pyPCR-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0    10453 2024-04-10 11:32:14.423921 pyPCR-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9769 2024-04-10 10:44:48.000000 pyPCR-0.0.2/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-10 09:37:56.000000 pyPCR-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:32:14.430903 pyPCR-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2024-04-10 11:32:01.000000 pyPCR-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:32:14.363085 pyPCR-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 11:32:14.379045 pyPCR-0.0.2/src/pyPCR/
+-rw-rw-rw-   0        0        0    24915 2024-04-10 08:04:25.000000 pyPCR-0.0.2/src/pyPCR/Mep_panel.py
+-rw-rw-rw-   0        0        0    11738 2024-04-09 07:05:50.000000 pyPCR-0.0.2/src/pyPCR/Rextractor.py
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:36:13.000000 pyPCR-0.0.2/src/pyPCR/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:32:14.421929 pyPCR-0.0.2/src/pyPCR.egg-info/
+-rw-rw-rw-   0        0        0    10453 2024-04-10 11:32:14.000000 pyPCR-0.0.2/src/pyPCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-10 11:32:14.000000 pyPCR-0.0.2/src/pyPCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:32:14.000000 pyPCR-0.0.2/src/pyPCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-04-10 11:32:14.000000 pyPCR-0.0.2/src/pyPCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 11:32:14.000000 pyPCR-0.0.2/src/pyPCR.egg-info/top_level.txt
```

### Comparing `pyPCR-0.0.1/LICENCE.txt` & `pyPCR-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pyPCR-0.0.1/PKG-INFO` & `pyPCR-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: pyPCR
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
 Home-page: https://github.com/PyPCR/PyPCR
-Author: ChandruGaneshan VikramSekar
-Author-email: chandruganeshan24@gmail.com vikramsekar2305@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: fpdf==1.7.2
 Requires-Dist: matplotlib==3.6.3
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
```

#### html2text {}

```diff
@@ -1,16 +1,12 @@
-Metadata-Version: 2.1 Name: pyPCR Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: pyPCR Version: 0.0.2 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
 for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyPCR
-Author: ChandruGaneshan VikramSekar Author-email: chandruganeshan24@gmail.com
-vikramsekar2305@gmail.com License: MIT Keywords: High Resolution
-Melt,Amplification Curve,Cycle threshold,PCR,rt-
-PCR,Meningoencephalitis,MEP,Pathogens Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+License: MIT Keywords: High Resolution Melt,Amplification Curve,Cycle
+threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens Description-Content-
 Type: text/markdown License-File: LICENCE.txt Requires-Dist: fpdf==1.7.2
 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5 Requires-Dist:
 pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist: scipy==1.13.0
 
 
                               ************ PPyyPPCCRR ************
```

### Comparing `pyPCR-0.0.1/README.md` & `pyPCR-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPCR-0.0.1/setup.py` & `pyPCR-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 rd_file = os.path.join(dir_path, 'README.md')
 
 with io.open(rd_file, encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyPCR',
-    version='0.0.1',
+    version='0.0.2',
     description='A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/PyPCR/PyPCR',
     authors=["ChandruGaneshan", "VikramSekar"],
     authors_email=['chandruganeshan24@gmail.com', 'vikramsekar2305@gmail.com'],
     license='MIT',
     keywords=['High Resolution Melt', 'Amplification Curve', "Cycle threshold",
               'PCR', 'rt-PCR', 'Meningoencephalitis', "MEP", 'Pathogens'],
     packages=find_packages(where='src'),
     package_dir={"": "src"},
-    package_data={"PyPCR": ["*.py", "*.pkl", "*.md", "*.xlsx", "*.cfg"]},
+    package_data={"PyPCR": ["*.py", "*.pkl", "*.md", "*.xlsx"]},
     include_package_data=True,
     install_requires=[
         'fpdf==1.7.2',
         'matplotlib==3.6.3',
         'numpy==1.23.5',
         'pandas==1.5.3',
         'Pillow==9.4.0',
```

### Comparing `pyPCR-0.0.1/src/PyPCR.egg-info/PKG-INFO` & `pyPCR-0.0.2/src/pyPCR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 Metadata-Version: 2.1
 Name: pyPCR
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for processing and interpreting DNA high-resolution melt and amplification curves for the meningoencephalitis panel.
 Home-page: https://github.com/PyPCR/PyPCR
-Author: ChandruGaneshan VikramSekar
-Author-email: chandruganeshan24@gmail.com vikramsekar2305@gmail.com
 License: MIT
 Keywords: High Resolution Melt,Amplification Curve,Cycle threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: fpdf==1.7.2
 Requires-Dist: matplotlib==3.6.3
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: Pillow==9.4.0
```

#### html2text {}

```diff
@@ -1,16 +1,12 @@
-Metadata-Version: 2.1 Name: pyPCR Version: 0.0.1 Summary: A library for
+Metadata-Version: 2.1 Name: pyPCR Version: 0.0.2 Summary: A library for
 processing and interpreting DNA high-resolution melt and amplification curves
 for the meningoencephalitis panel. Home-page: https://github.com/PyPCR/PyPCR
-Author: ChandruGaneshan VikramSekar Author-email: chandruganeshan24@gmail.com
-vikramsekar2305@gmail.com License: MIT Keywords: High Resolution
-Melt,Amplification Curve,Cycle threshold,PCR,rt-
-PCR,Meningoencephalitis,MEP,Pathogens Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+License: MIT Keywords: High Resolution Melt,Amplification Curve,Cycle
+threshold,PCR,rt-PCR,Meningoencephalitis,MEP,Pathogens Description-Content-
 Type: text/markdown License-File: LICENCE.txt Requires-Dist: fpdf==1.7.2
 Requires-Dist: matplotlib==3.6.3 Requires-Dist: numpy==1.23.5 Requires-Dist:
 pandas==1.5.3 Requires-Dist: Pillow==9.4.0 Requires-Dist: plotly==5.13.1
 Requires-Dist: scikit_learn==1.4.1.post1 Requires-Dist: scipy==1.13.0
 
 
                               ************ PPyyPPCCRR ************
```

### Comparing `pyPCR-0.0.1/src/pyPCR/Mep_panel.py` & `pyPCR-0.0.2/src/pyPCR/Mep_panel.py`

 * *Files identical despite different names*

### Comparing `pyPCR-0.0.1/src/pyPCR/Rextractor.py` & `pyPCR-0.0.2/src/pyPCR/Rextractor.py`

 * *Files identical despite different names*

