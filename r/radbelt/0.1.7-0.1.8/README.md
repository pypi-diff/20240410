# Comparing `tmp/radbelt-0.1.7.tar.gz` & `tmp/radbelt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radbelt-0.1.7.tar", last modified: Thu Feb  1 03:46:51 2024, max compression
+gzip compressed data, was "radbelt-0.1.8.tar", last modified: Wed Apr 10 15:43:21 2024, max compression
```

## Comparing `radbelt-0.1.7.tar` & `radbelt-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      116 2024-02-01 03:41:31.000000 radbelt-0.1.7/.github/dependabot.yml
--rw-r--r--   0        0        0     1921 2024-02-01 03:41:31.000000 radbelt-0.1.7/.github/workflows/cibuildwheel.yml
--rw-r--r--   0        0        0       75 2024-02-01 03:41:31.000000 radbelt-0.1.7/.gitignore
--rw-r--r--   0        0        0    12693 2024-02-01 03:41:31.000000 radbelt-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     2633 2024-02-01 03:41:31.000000 radbelt-0.1.7/README.md
--rw-r--r--   0        0        0     2672 2024-02-01 03:41:31.000000 radbelt-0.1.7/meson.build
--rw-r--r--   0        0        0     1463 2024-02-01 03:41:31.000000 radbelt-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2568 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/__init__.py
--rw-r--r--   0        0        0     1850 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/core.f
--rw-r--r--   0        0        0      855 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/core.pyf
--rw-r--r--   0        0        0      224 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/README.md
--rw-r--r--   0        0        0    83596 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/ae8max.asc
--rw-r--r--   0        0        0    81254 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/ae8min.asc
--rw-r--r--   0        0        0   100542 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/ap8max.asc
--rw-r--r--   0        0        0   102318 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/ap8min.asc
--rw-r--r--   0        0        0    14732 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/aep8/trmfun.f
--rw-r--r--   0        0        0      500 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/README.md
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1945.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1950.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1955.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1960.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1965.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1970.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1975.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1980.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1985.dat
--rw-r--r--   0        0        0     1591 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1990.dat
--rw-r--r--   0        0        0     1590 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1655 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1785 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1785 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1785 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1785 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/igrf2020.dat
--rw-r--r--   0        0        0     1786 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/igrf2020s.dat
--rw-r--r--   0        0        0    43035 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/extern/igrf/shellig.f
--rw-r--r--   0        0        0      473 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/paths.py
--rw-r--r--   0        0        0      493 2024-02-01 03:41:31.000000 radbelt-0.1.7/radbelt/util.py
--rw-r--r--   0        0        0     3718 2024-02-01 03:46:51.863679 radbelt-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      116 2024-04-08 15:48:50.000000 radbelt-0.1.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1921 2024-04-08 15:48:50.000000 radbelt-0.1.8/.github/workflows/cibuildwheel.yml
+-rw-r--r--   0        0        0       75 2024-04-08 15:48:50.000000 radbelt-0.1.8/.gitignore
+-rw-r--r--   0        0        0    12693 2024-04-08 15:48:50.000000 radbelt-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     2633 2024-04-08 15:48:50.000000 radbelt-0.1.8/README.md
+-rw-r--r--   0        0        0     2672 2024-04-08 15:48:50.000000 radbelt-0.1.8/meson.build
+-rw-r--r--   0        0        0     1467 2024-04-08 15:48:50.000000 radbelt-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2568 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/__init__.py
+-rw-r--r--   0        0        0     1880 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/core.f
+-rw-r--r--   0        0        0      855 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/core.pyf
+-rw-r--r--   0        0        0      224 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/README.md
+-rw-r--r--   0        0        0    83596 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/ae8max.asc
+-rw-r--r--   0        0        0    81254 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/ae8min.asc
+-rw-r--r--   0        0        0   100542 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/ap8max.asc
+-rw-r--r--   0        0        0   102318 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/ap8min.asc
+-rw-r--r--   0        0        0    14732 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/aep8/trmfun.f
+-rw-r--r--   0        0        0      500 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/README.md
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1945.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1950.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1955.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1960.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1965.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1970.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1975.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1980.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1985.dat
+-rw-r--r--   0        0        0     1591 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1990.dat
+-rw-r--r--   0        0        0     1590 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf1995.dat
+-rw-r--r--   0        0        0     1655 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf2000.dat
+-rw-r--r--   0        0        0     1785 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf2005.dat
+-rw-r--r--   0        0        0     1785 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf2010.dat
+-rw-r--r--   0        0        0     1785 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/dgrf2015.dat
+-rw-r--r--   0        0        0     1785 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/igrf2020.dat
+-rw-r--r--   0        0        0     1786 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/igrf2020s.dat
+-rw-r--r--   0        0        0    43035 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/extern/igrf/shellig.f
+-rw-r--r--   0        0        0      473 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/paths.py
+-rw-r--r--   0        0        0      493 2024-04-08 15:48:50.000000 radbelt-0.1.8/radbelt/util.py
+-rw-r--r--   0        0        0     3718 2024-04-10 15:43:21.327736 radbelt-0.1.8/PKG-INFO
```

### Comparing `radbelt-0.1.7/.github/workflows/cibuildwheel.yml` & `radbelt-0.1.8/.github/workflows/cibuildwheel.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       - name: Install MinGW
         if: runner.os == 'Windows'
         run: |
           choco install rtools -y --no-progress --force --version=4.0.0.20220206
           echo "c:\rtools40\ucrt64\bin;" >> $env:GITHUB_PATH
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16
+        uses: pypa/cibuildwheel@v2.17
         env:
           CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_WINDOWS: AMD64
           CIBW_ENVIRONMENT_MACOS: FC=gfortran-11
           # Skip musllinux wheels, which take a long time to build because Numpy must be built from source
           # Skip PyPy wheels
           # Skip 32-bit Intel wheels
```

### Comparing `radbelt-0.1.7/LICENSE.txt` & `radbelt-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/README.md` & `radbelt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/meson.build` & `radbelt-0.1.8/meson.build`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/pyproject.toml` & `radbelt-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = 'mesonpy'
 requires = ["meson>=0.63.0",
             "meson-python",
             "setuptools_scm>=6.2",
             "wheel",
-            "numpy>=1.25"]
+            "numpy>=2.0.0rc1"]
 
 [project]
 name = "radbelt"
 description = "Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model"
 readme = "README.md"
 authors = [ { name = "Leo Singer", email = "leo.p.singer@nasa.gov" } ]
 classifiers = [
```

### Comparing `radbelt-0.1.7/radbelt/__init__.py` & `radbelt-0.1.8/radbelt/__init__.py`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/core.f` & `radbelt-0.1.8/radbelt/core.f`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             BBX = BABS / BEQU
         END
 
 C Adapted from
 C https://ccmc.gsfc.nasa.gov/pub/modelweb/radiation_belt/radbelt/fortran_code/radbelt.for
 
         SUBROUTINE AEP8(E, L, BB0, IMNAME, FLUX)
+            INTEGER     IERR
             REAL        L, BB0
             DIMENSION   MAP(20000), IHEAD(8), EE(1)
             CHARACTER*10  	NAME, MNAME(4)
             DATA MNAME  /'ae8min.asc','ae8max.asc','ap8min.asc',
      &                   'ap8max.asc'/
 
             IUAEAP = 15
@@ -43,13 +44,13 @@
      &           FORM='FORMATTED')
             READ(IUAEAP,1301) IHEAD
             NMAP=IHEAD(8)
             READ(IUAEAP,1301) (MAP(I),I=1,NMAP)
 1301	    FORMAT(1X,12I6)
         
 1822        CLOSE(IUAEAP)
-            IF (IER .NE. 0) STOP
+            IF (IERR .NE. 0) STOP
 
             EE(1) = E
             CALL TRARA1(IHEAD,MAP,L,BB0,E,FLUX,1)
             IF(FLUX.GT.0.0) FLUX=10.**FLUX
         END
```

### Comparing `radbelt-0.1.7/radbelt/core.pyf` & `radbelt-0.1.8/radbelt/core.pyf`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/aep8/ae8max.asc` & `radbelt-0.1.8/radbelt/extern/aep8/ae8max.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/aep8/ae8min.asc` & `radbelt-0.1.8/radbelt/extern/aep8/ae8min.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/aep8/ap8max.asc` & `radbelt-0.1.8/radbelt/extern/aep8/ap8max.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/aep8/ap8min.asc` & `radbelt-0.1.8/radbelt/extern/aep8/ap8min.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/aep8/trmfun.f` & `radbelt-0.1.8/radbelt/extern/aep8/trmfun.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1945.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1945.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1950.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1950.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1955.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1955.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1960.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1960.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1965.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1965.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1970.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1970.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1975.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1975.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1980.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1980.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1985.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1985.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1990.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1990.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf1995.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf1995.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf2000.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf2005.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf2010.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/dgrf2015.dat` & `radbelt-0.1.8/radbelt/extern/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/igrf2020.dat` & `radbelt-0.1.8/radbelt/extern/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/igrf2020s.dat` & `radbelt-0.1.8/radbelt/extern/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/radbelt/extern/igrf/shellig.f` & `radbelt-0.1.8/radbelt/extern/igrf/shellig.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.7/PKG-INFO` & `radbelt-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radbelt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 Author-Email: Leo Singer <leo.p.singer@nasa.gov>
 License: NOSA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
 Classifier: Operating System :: MacOS
```

