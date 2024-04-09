# Comparing `tmp/gaussianutility-0.1.2.tar.gz` & `tmp/gaussianutility-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussianutility-0.1.2.tar", last modified: Fri Jul 14 16:55:37 2023, max compression
+gzip compressed data, was "gaussianutility-0.1.4.tar", last modified: Tue Apr  9 22:03:55 2024, max compression
```

## Comparing `gaussianutility-0.1.2.tar` & `gaussianutility-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/.gitignore
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/LICENSE
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5750 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5282 2023-07-13 14:06:36.000000 gaussianutility-0.1.2/README.md
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.165971 gaussianutility-0.1.2/gaussianutility/
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/gaussianutility/__init__.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2595 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/com2vasp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/com2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/freezeLayer.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     6161 2023-07-03 20:31:32.000000 gaussianutility-0.1.2/gaussianutility/gibbsTemp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1494 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/out2com.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1578 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/out2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/printE.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/sortInput.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)    10666 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/spectrum.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/utilities.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2794 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/vasp2com.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1713 2023-07-14 16:47:10.000000 gaussianutility-0.1.2/gaussianutility/xyz2com.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.165971 gaussianutility-0.1.2/gaussianutility.egg-info/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5750 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1022 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/SOURCES.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/dependency_links.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      467 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/entry_points.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      103 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/requires.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/top_level.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      472 2023-07-13 21:38:45.000000 gaussianutility-0.1.2/pyproject.toml
--rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/setup.cfg
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1682 2023-07-13 21:38:37.000000 gaussianutility-0.1.2/setup.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.215970 gaussianutility-0.1.2/test/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/3trimerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/3trimerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/4tetramerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/4tetramerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/5pentamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/5pentamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/6hexamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/6hexamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/7heptamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/7heptamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/8octamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/8octamerPrism.SiAl.out
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2024-04-09 22:03:55.443343 gaussianutility-0.1.4/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2024-04-01 19:21:28.000000 gaussianutility-0.1.4/.gitignore
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2024-04-01 19:21:28.000000 gaussianutility-0.1.4/LICENSE
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6686 2024-04-09 22:03:55.441341 gaussianutility-0.1.4/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6217 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/README.md
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2024-04-09 22:03:55.340790 gaussianutility-0.1.4/gaussianutility/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2024-04-01 19:21:28.000000 gaussianutility-0.1.4/gaussianutility/__init__.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2636 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/com2vasp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/com2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/freezeLayer.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6161 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/gibbsTemp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1496 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/out2com.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1578 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/out2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/printE.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/sortInput.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)    11536 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/spectrum.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/utilities.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2576 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/vasp2com.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1713 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/gaussianutility/xyz2com.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2024-04-09 22:03:55.439344 gaussianutility-0.1.4/gaussianutility.egg-info/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6686 2024-04-09 22:03:55.000000 gaussianutility-0.1.4/gaussianutility.egg-info/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      989 2024-04-09 22:03:55.000000 gaussianutility-0.1.4/gaussianutility.egg-info/SOURCES.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2024-04-09 22:03:55.000000 gaussianutility-0.1.4/gaussianutility.egg-info/dependency_links.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2024-04-09 22:03:55.000000 gaussianutility-0.1.4/gaussianutility.egg-info/top_level.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      473 2024-04-09 22:01:54.000000 gaussianutility-0.1.4/pyproject.toml
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2024-04-09 22:03:55.444341 gaussianutility-0.1.4/setup.cfg
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1682 2024-04-09 22:01:31.000000 gaussianutility-0.1.4/setup.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2024-04-09 22:03:55.438340 gaussianutility-0.1.4/test/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/3trimerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/3trimerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/4tetramerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/4tetramerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/5pentamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/5pentamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/6hexamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/6hexamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/7heptamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/7heptamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/8octamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2024-04-09 22:00:58.000000 gaussianutility-0.1.4/test/8octamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)    17217 2024-04-02 21:02:24.000000 gaussianutility-0.1.4/test/com2vasp_ZSM5.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)    10011 2024-04-01 19:46:21.000000 gaussianutility-0.1.4/test/vasp2com_ZSM5.vasp
```

### Comparing `gaussianutility-0.1.2/.gitignore` & `gaussianutility-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/LICENSE` & `gaussianutility-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/PKG-INFO` & `gaussianutility-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gaussianutility
-Version: 0.1.2
-Summary: Useful utilities to use Gaussian09/16 software
-Home-page: https://github.com/Sungil-Hong/gaussianutility
-Author: Sungil Hong
-Author-email: Sungil Hong <suh33@pitt.edu>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Gaussian Utility
 
 [![License Badge](https://img.shields.io/github/license/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
 [![Issues Badge](https://img.shields.io/github/issues/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
@@ -29,24 +15,25 @@
 
 Most of the scripts that work on a Gaussian output file are written based Density Functional Theory calculations.
 Hence, the compatibility with different types of calculations, e.g., coupled cluster, Hartree-Fock, semi-empirical, and Møller–Plesset perturbation methodes has not been confirmed yet.
 
 The package includes the following scripts:
 
 1. Convert input structure file type:
-   - `com2vasp`: Converts Gaussian input files (.com) to VASP input files (.vasp).
-   - `com2xyz`: Converts Gaussian input files (.com) to XYZ coordinate files (.xyz).
-   - `vasp2com`: Converts VASP input files (.vasp) to Gaussian input files (.com).
+   - `com2vasp`: Converts Gaussian input file (.com) to VASP input file (.vasp).
+   - `com2xyz`: Converts Gaussian input file (.com) to XYZ coordinate file (.xyz).
+   - `vasp2com`: Converts VASP input file (.vasp) to Gaussian input file (.com).
+   - `xyz2com`: Converts XYZ coordinate file (.xyz) to Gaussian input file (.com).
    
 2. Extract structure from output file:
-   - `out2com`: Generate Gaussian input files (.com) from Gaussian output files (.out).
-   - `out2xyz`: Generate XYZ coordinate files (.xyz) from Gaussian output files (.out).
+   - `out2com`: Generate Gaussian input file (.com) from Gaussian output file (.out).
+   - `out2xyz`: Generate XYZ coordinate file (.xyz) from Gaussian output file (.out).
 
 3. Spectrum utilities:
-   - `spectrum`: Produces Normal-IR, Raman, or UV-Vis spectra from Gaussian output files (.out).
+   - `spectrum`: Produces Normal-IR, Raman, or UV-Vis spectra from Gaussian output file (.out).
 
 4. Other utilities:
    - `gibbsTemp`: Calculates the Gibbs free energies at given temperatures from a Gaussian output file with frequency calculation.
    - `printE`: Prints the energy from a Gaussian output file.
    - `freezeLayer`: Freezes a specific ONIOM layer of atoms in a Gaussian input file with ONIOM formulation.
    - `sortInput`: Sorts the atoms in a Gaussian input file based on their atomic numbers, x, y, or z coordiate, or ONIOM layer.
 
@@ -79,78 +66,88 @@
 The Gaussian Utility package has the following dependencies:
 
 - numpy>=1.17.2
 - pandas>=1.1.0
 - periodictable>=1.6.1
 - ase
 - argparse>=1.1
-- matplotlib>=3.5.3
-- mendeleev>=0.12.0
+- matplotlib>=3.5.1
+- mendeleev>=0.9.0
 
 These dependencies will be automatically installed when you install the package using `setuptools`.
 
 ## Usage
 
 The Gaussian Utility package provides command-line utilities that can be accessed by running the corresponding command.
 Here are some examples of how to use the utilities:
 
-1. Convert a Gaussian input file to a VASP input file:
-   ```
-   com2vasp input.com
-   ```
-
-2. Convert a Gaussian input file to an XYZ coordinate file:
-   ```
-   com2xyz input.com
-   ```
-
-3. Convert a VASP input file to a Gaussian input file:
+1. Convert a structure file format:
    ```
-   vasp2com output.vasp
+   com2vasp structure.com
+   com2xyz structure.com
+   vasp2com structure.vasp
+   xyz2com structure.xyz
    ```
 
-4. Extract optimized geometry to a Gaussian input file from a Gaussian output file:
+2. Extract optimized geometry from a Gaussian output file:
    ```
    out2com output.out
-   ```
-
-5. Extract optimized geometry to an XYZ coordinate file:
-   ```
    out2xyz output.out
    ```
 
-6. Produce a spectrum from a Gaussian output file:
+3. Produce a spectrum from a Gaussian output file:
    ```
    spectrum type file_name1 [ratio1 [file_name2 ratio2 ...]]
    ```
 
-7. Freeze a specific ONIOM layer of atoms in a Gaussian input file:
+4. Freeze a specific ONIOM layer of atoms in a Gaussian input file:
    ```
    freezeLayer [-i [layer index]] file_name
    ```
 
-8. Calculate the Gibbs free energy at a given temperature:
+5. Calculate the Gibbs free energy at a given temperature:
    ```
    gibbsTemp file_name temp1 [temp2 [step_number]]
    ```
 
-9. Print the energy of a Gaussian output file:
+6. Print the energy of a Gaussian output file:
    ```
    printE file_name
    ```
 
-10. Sort the atoms in a Gaussian input file based on their atomic numbers:
+7. Sort the atoms in a Gaussian input file based on their atomic numbers:
     ```
     sortInput [-s [sort index]] [-o [order index]] file_name
     ```
+## Test
+In the test folder, you'll find files for testing each command with the naming convention "command_structure.extension". For example, to test the "com2vasp" command, follow these steps:
+1. Navigate to the test directory:
+
+```
+cd test
+```
+
+2. Run the desired command with the corresponding test file. For example, to test the "com2vasp" command with the file "com2vasp_ZSM5.com", use the following command:
+```
+com2vasp com2vasp_ZSM5.com
+```
+
+3. Verify that the command executes as expected and produces the correct output.
 
 ## Authors
 
-The Gaussian Utility package was developed by Sungil Hong. For any inquiries or issues, you can contact Sungil Hong via email at suh33@pitt.edu.
+The Gaussian Utility package was developed by Sungil Hong. For any inquiries or issues, you can contact Sungil Hong via email at s.hong@pitt.edu.
 
 ## License
 
 The Gaussian Utility package is distributed under the MIT License. Please refer to the [LICENSE](LICENSE) file for more information.
 
 ## Additional Information
 
 For more information about the Gaussian Utility package, you can visit the [GitHub repository](https://github.com/Sungil-Hong/gaussianutility). The repository contains the source code, documentation, and examples of usage for the package.
+
+## Acknowledgment
+
+The Gaussian Utility package has developed over multiple computational chemistry research projects conducted in the Computer-Aided Nano and Energy Lab (CANELa), led by Prof. Mpourmpakis at the University of Pittsburgh.
+The projects have been financially supported by U.S. Department of Energy Nuclear Energy University Program (DOE-NEUP) (18-15496), and National Science Foundation (NSF) (1920623),
+and computationally supported by the Center for Research Computing (CRC) at the University of Pittsburgh for performing DFT calculations.
+
```

### Comparing `gaussianutility-0.1.2/gaussianutility/com2vasp.py` & `gaussianutility-0.1.4/gaussianutility/com2vasp.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,45 +6,37 @@
 import argparse
 from argparse import RawTextHelpFormatter
 from gaussianutility.utilities import readinput
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description= "Convert Gaussian input file to .vasp file\n\n"
-                     "Return file_name.vasp: VASP geometry file (POSCAR)"
-                     , formatter_class=RawTextHelpFormatter)
+                     "Return file_name.vasp: VASP geometry file (POSCAR)",
+        formatter_class=RawTextHelpFormatter)
 
     parser.add_argument("file_name", help='Gaussian input file (.com or .gjf)')
-    args = parser.parse_args()
-    return args
-
-def main():
-    args = parse_args()
-    file_name = args.file_name
+    return parser.parse_args()
 
+def com_2_vasp():
     # Read geometry from a Gaussian input file
     _, _, _, df_geom, _ = readinput(file_name)
     df_geom = df_geom[['Atom', 'x', 'y', 'z']]
     df_geom['Atom'] = np.array([i.rsplit("-",1)[0] for i in list(df_geom['Atom'])])
     if not 'Tv' in df_geom['Atom'].values:
         raise ValueError('The Gaussian input file does not contain lattice information')
 
     # Convert Gaussian input to VASP input
-    elem = []
-    for el in elements:
-        elem.append(el.symbol)
-     
+    elem = [el.symbol for el in elements]
     df_atom_sort = pd.DataFrame(elem[1:], columns = ['symbol'])
     atom_sort_mapping = df_atom_sort.reset_index().set_index('symbol')
     df_geom['Atomic_num'] = df_geom['Atom'].map(atom_sort_mapping['index'])
 
     df_geom = df_geom.sort_values(by=['Atomic_num'], ascending = 0)
     df_geom = df_geom.drop(columns=['Atomic_num'])
 
-
     # Read lattice information
     lattice = df_geom[-3:].drop(['Atom'], axis=1) 
 
     df_geom = df_geom.drop(df_geom[df_geom['Atom'] == 'Tv'].index)
     df_geom = df_geom.drop(df_geom[df_geom['Atom'] == '?s'].index)
 
     atomlist = np.array(df_geom['Atom'])
@@ -60,19 +52,26 @@
 
     uniqatomlist = np.array(uniqatomlist)
     uniqatomcount= np.array(uniqatomcount, dtype=str)
 
     # Write VASP input file
     name = ".".join(file_name.rsplit(".",1)[0:-1])
     out_file = name + ".vasp"
-    output = open(out_file, 'w')
-    output.write(name+'\n')
-    output.write('1.0\n')
-    output.write(lattice.to_csv(index=False, header=False, sep='\t'))
-    output.write('   '+' '.join(uniqatomlist)+'\n')
-    output.write('   '+' '.join(uniqatomcount)+'\n')
-    output.write('Cartesian\n')
-    output.write(coord.to_csv(index=False, header=False, sep='\t'))
-    output.write('\n')
-    output.close()
+    with open(out_file, 'w') as output:
+        output.write(name + '\n')
+        output.write('1.0\n')
+        output.write(lattice.to_csv(index=False, header=False, sep='\t'))
+        output.write('   '+' '.join(uniqatomlist)+'\n')
+        output.write('   '+' '.join(uniqatomcount)+'\n')
+        output.write('Cartesian\n')
+        output.write(coord.to_csv(index=False, header=False, sep='\t'))
+        output.write('\n')
+
+def main():
+    args = parse_args()
+    file_name = args.file_name
+    com_2_vasp(file_name)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `gaussianutility-0.1.2/gaussianutility/com2xyz.py` & `gaussianutility-0.1.4/gaussianutility/com2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/freezeLayer.py` & `gaussianutility-0.1.4/gaussianutility/freezeLayer.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/gibbsTemp.py` & `gaussianutility-0.1.4/gaussianutility/gibbsTemp.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/out2com.py` & `gaussianutility-0.1.4/gaussianutility/out2com.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,11 +34,11 @@
     name = ".".join(file_name.rsplit(".",1)[0:-1])
     out_file = name + "_geom.com"
     output = open(out_file, 'w')
     output.write(routeStr + '\n\n')
     output.write(out_file + '\n\n')
     output.write(charge_mult + '\n')
     output.write(df_geom.to_string(index=False, header=False))
-    output.write('\n')
+    output.write('\n\n')
     output.close()
```

### Comparing `gaussianutility-0.1.2/gaussianutility/out2xyz.py` & `gaussianutility-0.1.4/gaussianutility/out2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/printE.py` & `gaussianutility-0.1.4/gaussianutility/printE.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/sortInput.py` & `gaussianutility-0.1.4/gaussianutility/sortInput.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/spectrum.py` & `gaussianutility-0.1.4/gaussianutility/spectrum.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,37 +2,50 @@
 
 import sys
 import math as m
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
+##### Change these lines to modify X range or make corrections #####
+
+UV_wl_range = np.linspace(100,500,801) # nm
+UV_alpha = 1 #UV-Vis wavelength scaling factor; default
+#UV_alpha = 1.12 #for M062X; ref: https://doi.org/10.26434/chemrxiv-2022-pfvhc-v3
+UV_delta = 0.4/m.sqrt(2) #UV-Vis bandwith parameter, eV; default
+#UV_delta = 0.21  #for M062X; ref: https://doi.org/10.26434/chemrxiv-2022-pfvhc-v3
+
+IR_wv_range = np.linspace(0,4000,8001) # cm-1
+IR_wn_factor = 1 # default
+#IR_wn_factor = 0.947 #For M062X; ref: J. Phys. Chem. A, 121(11), 2265 (2017)#
+IR_HWHM = 4 # IR peak half-width at half-max, cm-1 # default
+
+
 # Define functions to extract spectrum data from output file(s)
 def uv_vis(file_name):
     readfile = open(file_name).readlines()
     wavelengths = []
     strengths = []
     
     for idx, line in enumerate(reversed(readfile)):
         if "Excitation energies and oscillator strengths" in line:
             break
             
     ex_idx = len(readfile)-idx-1
             
     for line in readfile[ex_idx:]:
         if 'Excited State' in line:
-            wavelengths.append(line.split()[6])
-            strengths.append(line.split()[8].split('=')[1])
+            wavelengths.append(float(line.split()[6]))
+            strengths.append(float(line.split()[8].split('=')[1]))
             
     if len(wavelengths) == 0:
         raise TypeError('The Gaussian job does not look like excited state calculations')
 
-    wavelengths = np.array(wavelengths, dtype='float')
-    wavelengths = np.rint(wavelengths)
-    strengths = np.array(strengths, dtype='float')
+    wavelengths = np.array(wavelengths)
+    strengths = np.array(strengths)
     
     return wavelengths, strengths
 
 
 def ir(file_name):
     readfile = open(file_name, 'r')
     frequencies = []
@@ -43,17 +56,16 @@
             frequencies.append(line.split()[2:])
         if 'IR Inten' in line:
             intensities.append(line.split()[3:])
             
     if len(intensities) == 0:
         raise TypeError('The Gaussian job does not look like conntaining normal IR information')
             
-    frequencies = np.array(frequencies, dtype='float').flatten()
-    frequencies = np.rint(frequencies)
-    intensities = np.array(intensities, dtype='float').flatten()
+    frequencies = np.array(frequencies, dtype='float').flatten() #cm-1
+    intensities = np.array(intensities, dtype='float').flatten() #km/mole
 
     return frequencies, intensities
 
 def raman(file_name):
     readfile = open(file_name, 'r')
     frequencies = []
     intensities = []
@@ -63,29 +75,41 @@
             frequencies.append(line.split()[2:])
         if 'Raman Activ' in line:
             intensities.append(line.split()[3:])
             
     if len(intensities) == 0:
         raise TypeError('The Gaussian job does not look like conntaining normal IR information')
             
-    frequencies = np.array(frequencies, dtype='float').flatten()
-    frequencies = np.rint(frequencies)
-    intensities = np.array(intensities, dtype='float').flatten()
+    frequencies = np.array(frequencies, dtype='float').flatten() #cm-1
+    intensities = np.array(intensities, dtype='float').flatten() 
 
     return frequencies, intensities
 
+h = 6.6261e-34 # J/s
+c = 299792458  # m/s
+J2eV = 6.02214076e23/96.48530749925793/1000
+
+def wvl2E(wvl): # wvl in nm
+    E = h*c/(wvl/1e9)*J2eV
+    return E # E in eV
+
+def E2wvl(E): #E in eV
+    wvl = h*c*1e9/(E/J2eV)
+    return wvl # wvl in nm
+
 def uvGauss(x, f, wv):
     #Gaussian distribution for UV-Vis
     #Reference: https://gaussian.com/uvvisplot/
-    return 13.062973*f*3099.6*m.exp(-((1/x-1/wv)/0.00032262)**2)
+#    return 13.062973*f*3099.6*m.exp(-((1/x-1/wv)/0.00032262)**2)
+    return 13.062973*f*E2wvl(m.sqrt(2)*UV_delta)*m.exp(-((wvl2E(x)-wvl2E(wv)/UV_alpha)/UV_delta/m.sqrt(2))**2)
 
-def cauchy(x, i, mu):
+def cauchy(x, mu):
     # Cauchy distribution for normal and raman IR
-    gamma = 3
-    return i/m.pi/gamma/(1+((x-mu)/gamma)**2)
+    gamma = IR_HWHM
+    return 1/m.pi/gamma/(1+((x-mu)/gamma)**2)
 
 def main():
     # Print error/help messages that looks like argparse functionality
     argvLen = len(sys.argv)
     if argvLen == 1:
         print("usage: spectrum [-h] type file_name1 [ratio1 [file_name2 ratio2 ...]]")
         print("spectrum: error: the following arguments are required: type file_name1")
@@ -161,15 +185,15 @@
         blue = 0.8
         alpha = 0.6
 
         f = plt.figure()
         f.set_figwidth(12)
         f.set_figheight(8)
         
-        xrange = np.linspace(100,500,401)
+        xrange = UV_wl_range
         curve_per_file = []
         
         for fn in file_name:
             wavelengths, strengths = uv_vis(fn)
             
             curve_per_x = []
             for idx, wv in enumerate(wavelengths):
@@ -227,29 +251,29 @@
         blue = 0.8
         alpha = 0.6
 
         f = plt.figure()
         f.set_figwidth(12)
         f.set_figheight(8)
         
-        xrange = np.linspace(0,3900,3901)
+        xrange = IR_wv_range
         curve_per_file = []
         
         for fn in file_name:
             if type_name == 'ir':
                 frequencies, intensities = ir(fn)
+                frequencies *= IR_wn_factor # Correction factor
+                intensities *= 1e5/2.24e3
             elif type_name == 'raman':
                 frequencies, intensities = raman(fn)
                 
             curve_per_x = []
             for idx, mu in enumerate(frequencies):
                 mu_array = np.ones(len(xrange))*mu
-                it_array = np.ones(len(xrange)) * intensities[idx]
-                
-                curve = np.array(list(map(cauchy,xrange,it_array,mu_array)))
+                curve = np.array(list(map(cauchy,xrange,mu_array))) * intensities[idx]
                 curve_per_x.append(curve)
             
             final_curve = np.sum(curve_per_x, axis=0)
             curve_per_file.append(final_curve)
             
             if argvLen == 3:
                 plt.plot(xrange, final_curve, 'b')
```

### Comparing `gaussianutility-0.1.2/gaussianutility/utilities.py` & `gaussianutility-0.1.4/gaussianutility/utilities.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/gaussianutility/vasp2com.py` & `gaussianutility-0.1.4/gaussianutility/xyz2com.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,63 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import numpy as np
-import itertools
-import mendeleev as md
-import pandas as pd
 import argparse
 from argparse import RawTextHelpFormatter
+import mendeleev as md
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description= "Convert vasp input file to Gaussian input file (.com)\n"
-                     "The computational method in the Gaussian calculation must be modified manually if needed\n\n"
+        description= "Convert xyz file to Gaussian input file (.com)\n\n"
                      "Return file_name.com: Gaussian input file"
                      , formatter_class=RawTextHelpFormatter)
 
-    parser.add_argument("file_name", help='VASP input file (.vasp)')
+    parser.add_argument("file_name", help='XYZ structure file (.xyz)')
     args = parser.parse_args()
     return args
 
 def main():
     args = parse_args()
     file_name = args.file_name
-        
-    # Check input file
-    name, input_format = file_name.rsplit(".",1)[0], file_name.rsplit(".",1)[-1]
-    if input_format != "vasp":
-        raise ValueError('The input structure must be .vasp file')
 
-    # Read geometry information and make Pandas dataframe
+    # Read geometry from a Gaussian input file
     lines = open(file_name).readlines()
+    
+    for idx, line in enumerate(lines[:]):
+        if len(line.split()) == 4:
+            isxyz = True
+            for val in line.split()[1:]:
+                 isxyz *= val.replace('.', '', 1).isdigit()
+
+            if isxyz: break
+
+    # Decide multiplicity assuming overall neutral charge
+    elemts = []
+    for line in lines[idx:]:
+        elemts.append(line.split()[0])
+        
+    elemts, counts = np.unique(elemts, return_counts=True)
+        
+    elem_elect = []
 
-    elem_type = lines[5].split()
-    elem_num = np.array(list(map(int, lines[6].split())))
-    elect_num = []
+    for elem in elemts:
+        elem_elect.append(md.element(elem).electrons)
 
-    for e in elem_type:
-        elect_num.append(md.element(e).electrons)
-        
-    elect_num = np.array(elect_num)
+    total_elect = sum(np.array(elem_elect) * counts)
 
-    if sum(elect_num * elem_num)%2 == 0:
+    if total_elect%2 == 0:
         multiplicity = 1
     else: multiplicity = 2
 
-    elem_list = []
-    for i in range(len(elem_type)):
-        elem_list.append((elem_type[i],)*elem_num[i])
-        
-    elem_list = np.array(list(itertools.chain(*elem_list)))
-
-    geom = []
-    for line in lines[8:]:
-        if len(line) < 2: break
-        geom.append(line.split())
-
-    geom = np.array(geom, dtype='float_')
-
-    lattice_scailing_factor = float(lines[1].split()[0])
-    lattice_vector = [line.split() for line in lines[2:5]]
-    lattice_vector = np.array(lattice_vector, dtype = float)
-
-    geomMod = lines[7].split()[0]
-    if geomMod == 'Cartesian' or geomMod == 'cartesian':
-        geom = geom*lattice_scailing_factor
-    elif geomMod == 'Direct' or geomMod == 'direct':
-        geom = np.dot(lattice_vector, geom.T).T
-        geom = geom*lattice_scailing_factor
-        
-    df_geom = pd.DataFrame(geom, columns = ['x','y','z'])
-    df_geom.insert(loc=0, column='element', value=elem_list)
-
-    # Write .com file
-    out_file = file_name.rsplit(".",1)[0] + ".com"
+    # Write Gaussian input file
+    name = ".".join(file_name.rsplit(".",1)[0:-1])
+    out_file = name + ".com"
     output = open(out_file, 'w')
-    output.write('# pbepbe/3-21g/auto\n')
-    output.write('\n')
-    output.write(name)
-    output.write('\n\n')
-    output.write('0 '+str(multiplicity))
-    output.write('\n')
-    output.write(df_geom.to_string(index=False, header=False))
-    output.write('\n')
-    output.write('Tv ' + lines[2])
-    output.write('Tv ' + lines[3])
-    output.write('Tv ' + lines[4])
+    output.write('# hf/3-21g\n\n')
+    output.write(out_file + '\n\n')
+    output.write('0 ' + str(multiplicity) + '\n')
+    for line in lines[idx:]:
+        output.write(line)
     output.write('\n')
     output.close()
```

### Comparing `gaussianutility-0.1.2/gaussianutility.egg-info/PKG-INFO` & `gaussianutility-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gaussianutility
-Version: 0.1.2
+Version: 0.1.4
 Summary: Useful utilities to use Gaussian09/16 software
 Home-page: https://github.com/Sungil-Hong/gaussianutility
 Author: Sungil Hong
-Author-email: Sungil Hong <suh33@pitt.edu>
+Author-email: Sungil Hong <s.hong@pitt.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -29,24 +29,25 @@
 
 Most of the scripts that work on a Gaussian output file are written based Density Functional Theory calculations.
 Hence, the compatibility with different types of calculations, e.g., coupled cluster, Hartree-Fock, semi-empirical, and Møller–Plesset perturbation methodes has not been confirmed yet.
 
 The package includes the following scripts:
 
 1. Convert input structure file type:
-   - `com2vasp`: Converts Gaussian input files (.com) to VASP input files (.vasp).
-   - `com2xyz`: Converts Gaussian input files (.com) to XYZ coordinate files (.xyz).
-   - `vasp2com`: Converts VASP input files (.vasp) to Gaussian input files (.com).
+   - `com2vasp`: Converts Gaussian input file (.com) to VASP input file (.vasp).
+   - `com2xyz`: Converts Gaussian input file (.com) to XYZ coordinate file (.xyz).
+   - `vasp2com`: Converts VASP input file (.vasp) to Gaussian input file (.com).
+   - `xyz2com`: Converts XYZ coordinate file (.xyz) to Gaussian input file (.com).
    
 2. Extract structure from output file:
-   - `out2com`: Generate Gaussian input files (.com) from Gaussian output files (.out).
-   - `out2xyz`: Generate XYZ coordinate files (.xyz) from Gaussian output files (.out).
+   - `out2com`: Generate Gaussian input file (.com) from Gaussian output file (.out).
+   - `out2xyz`: Generate XYZ coordinate file (.xyz) from Gaussian output file (.out).
 
 3. Spectrum utilities:
-   - `spectrum`: Produces Normal-IR, Raman, or UV-Vis spectra from Gaussian output files (.out).
+   - `spectrum`: Produces Normal-IR, Raman, or UV-Vis spectra from Gaussian output file (.out).
 
 4. Other utilities:
    - `gibbsTemp`: Calculates the Gibbs free energies at given temperatures from a Gaussian output file with frequency calculation.
    - `printE`: Prints the energy from a Gaussian output file.
    - `freezeLayer`: Freezes a specific ONIOM layer of atoms in a Gaussian input file with ONIOM formulation.
    - `sortInput`: Sorts the atoms in a Gaussian input file based on their atomic numbers, x, y, or z coordiate, or ONIOM layer.
 
@@ -79,78 +80,88 @@
 The Gaussian Utility package has the following dependencies:
 
 - numpy>=1.17.2
 - pandas>=1.1.0
 - periodictable>=1.6.1
 - ase
 - argparse>=1.1
-- matplotlib>=3.5.3
-- mendeleev>=0.12.0
+- matplotlib>=3.5.1
+- mendeleev>=0.9.0
 
 These dependencies will be automatically installed when you install the package using `setuptools`.
 
 ## Usage
 
 The Gaussian Utility package provides command-line utilities that can be accessed by running the corresponding command.
 Here are some examples of how to use the utilities:
 
-1. Convert a Gaussian input file to a VASP input file:
+1. Convert a structure file format:
    ```
-   com2vasp input.com
+   com2vasp structure.com
+   com2xyz structure.com
+   vasp2com structure.vasp
+   xyz2com structure.xyz
    ```
 
-2. Convert a Gaussian input file to an XYZ coordinate file:
-   ```
-   com2xyz input.com
-   ```
-
-3. Convert a VASP input file to a Gaussian input file:
-   ```
-   vasp2com output.vasp
-   ```
-
-4. Extract optimized geometry to a Gaussian input file from a Gaussian output file:
+2. Extract optimized geometry from a Gaussian output file:
    ```
    out2com output.out
-   ```
-
-5. Extract optimized geometry to an XYZ coordinate file:
-   ```
    out2xyz output.out
    ```
 
-6. Produce a spectrum from a Gaussian output file:
+3. Produce a spectrum from a Gaussian output file:
    ```
    spectrum type file_name1 [ratio1 [file_name2 ratio2 ...]]
    ```
 
-7. Freeze a specific ONIOM layer of atoms in a Gaussian input file:
+4. Freeze a specific ONIOM layer of atoms in a Gaussian input file:
    ```
    freezeLayer [-i [layer index]] file_name
    ```
 
-8. Calculate the Gibbs free energy at a given temperature:
+5. Calculate the Gibbs free energy at a given temperature:
    ```
    gibbsTemp file_name temp1 [temp2 [step_number]]
    ```
 
-9. Print the energy of a Gaussian output file:
+6. Print the energy of a Gaussian output file:
    ```
    printE file_name
    ```
 
-10. Sort the atoms in a Gaussian input file based on their atomic numbers:
+7. Sort the atoms in a Gaussian input file based on their atomic numbers:
     ```
     sortInput [-s [sort index]] [-o [order index]] file_name
     ```
+## Test
+In the test folder, you'll find files for testing each command with the naming convention "command_structure.extension". For example, to test the "com2vasp" command, follow these steps:
+1. Navigate to the test directory:
+
+```
+cd test
+```
+
+2. Run the desired command with the corresponding test file. For example, to test the "com2vasp" command with the file "com2vasp_ZSM5.com", use the following command:
+```
+com2vasp com2vasp_ZSM5.com
+```
+
+3. Verify that the command executes as expected and produces the correct output.
 
 ## Authors
 
-The Gaussian Utility package was developed by Sungil Hong. For any inquiries or issues, you can contact Sungil Hong via email at suh33@pitt.edu.
+The Gaussian Utility package was developed by Sungil Hong. For any inquiries or issues, you can contact Sungil Hong via email at s.hong@pitt.edu.
 
 ## License
 
 The Gaussian Utility package is distributed under the MIT License. Please refer to the [LICENSE](LICENSE) file for more information.
 
 ## Additional Information
 
 For more information about the Gaussian Utility package, you can visit the [GitHub repository](https://github.com/Sungil-Hong/gaussianutility). The repository contains the source code, documentation, and examples of usage for the package.
+
+## Acknowledgment
+
+The Gaussian Utility package has developed over multiple computational chemistry research projects conducted in the Computer-Aided Nano and Energy Lab (CANELa), led by Prof. Mpourmpakis at the University of Pittsburgh.
+The projects have been financially supported by U.S. Department of Energy Nuclear Energy University Program (DOE-NEUP) (18-15496), and National Science Foundation (NSF) (1920623),
+and computationally supported by the Center for Research Computing (CRC) at the University of Pittsburgh for performing DFT calculations.
+
```

### Comparing `gaussianutility-0.1.2/gaussianutility.egg-info/SOURCES.txt` & `gaussianutility-0.1.4/gaussianutility.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 gaussianutility/spectrum.py
 gaussianutility/utilities.py
 gaussianutility/vasp2com.py
 gaussianutility/xyz2com.py
 gaussianutility.egg-info/PKG-INFO
 gaussianutility.egg-info/SOURCES.txt
 gaussianutility.egg-info/dependency_links.txt
-gaussianutility.egg-info/entry_points.txt
-gaussianutility.egg-info/requires.txt
 gaussianutility.egg-info/top_level.txt
 test/3trimerPrism.SiAl.geom.com
 test/3trimerPrism.SiAl.out
 test/4tetramerPrism.SiAl.geom.com
 test/4tetramerPrism.SiAl.out
 test/5pentamerPrism.SiAl.geom.com
 test/5pentamerPrism.SiAl.out
 test/6hexamerPrism.SiAl.geom.com
 test/6hexamerPrism.SiAl.out
 test/7heptamerPrism.SiAl.geom.com
 test/7heptamerPrism.SiAl.out
 test/8octamerPrism.SiAl.geom.com
-test/8octamerPrism.SiAl.out
+test/8octamerPrism.SiAl.out
+test/com2vasp_ZSM5.com
+test/vasp2com_ZSM5.vasp
```

### Comparing `gaussianutility-0.1.2/setup.py` & `gaussianutility-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gaussianutility",
-    version="0.1.2",
+    version="0.1.4",
     author="Sungil Hong",
-    author_email="suh33@pitt.edu",
+    author_email="s.hong@pitt.edu",
     description="Useful utilities to use Gaussian09/16 software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': [
                   'com2vasp = gaussianutility.com2vasp:main',
                   'com2xyz = gaussianutility.com2xyz:main',
                   'xyz2com = gaussianutility.xyz2com:main',
@@ -32,10 +32,10 @@
         "Operating System :: OS Independent"],
     python_requires='>=3.6',
     install_requires=['numpy>=1.17.2',
                       'pandas>=1.1.0',
                       'periodictable>=1.6.1',
                       'ase',
                       'argparse>=1.1',
-                      'matplotlib>=3.5.3',
-                      'mendeleev>=0.12.0']
+                      'matplotlib>=3.5.1',
+                      'mendeleev>=0.9.0']
 )
```

### Comparing `gaussianutility-0.1.2/test/3trimerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/3trimerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/3trimerPrism.SiAl.out` & `gaussianutility-0.1.4/test/3trimerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/4tetramerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/4tetramerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/4tetramerPrism.SiAl.out` & `gaussianutility-0.1.4/test/4tetramerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/5pentamerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/5pentamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/5pentamerPrism.SiAl.out` & `gaussianutility-0.1.4/test/5pentamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/6hexamerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/6hexamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/6hexamerPrism.SiAl.out` & `gaussianutility-0.1.4/test/6hexamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/7heptamerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/7heptamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/7heptamerPrism.SiAl.out` & `gaussianutility-0.1.4/test/7heptamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/8octamerPrism.SiAl.geom.com` & `gaussianutility-0.1.4/test/8octamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.2/test/8octamerPrism.SiAl.out` & `gaussianutility-0.1.4/test/8octamerPrism.SiAl.out`

 * *Files identical despite different names*

