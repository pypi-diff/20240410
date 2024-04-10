# Comparing `tmp/fakefarsi-0.0.1.tar.gz` & `tmp/fakefarsi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakefarsi-0.0.1.tar", last modified: Thu Mar 21 20:43:15 2024, max compression
+gzip compressed data, was "fakefarsi-0.0.2.tar", last modified: Wed Apr 10 19:52:01 2024, max compression
```

## Comparing `fakefarsi-0.0.1.tar` & `fakefarsi-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 20:43:15.065944 fakefarsi-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-03-21 20:43:15.065944 fakefarsi-0.0.1/FakeFarsi/
--rw-rw-rw-   0        0        0        0 2024-03-20 13:03:24.000000 fakefarsi-0.0.1/FakeFarsi/__init__.py
--rw-rw-rw-   0        0        0     2725 2024-03-20 13:04:49.000000 fakefarsi-0.0.1/FakeFarsi/fakefarsi.py
--rw-rw-rw-   0        0        0     1091 2024-03-15 11:57:21.000000 fakefarsi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1011 2024-03-21 20:43:15.065944 fakefarsi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-03-21 15:19:48.000000 fakefarsi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 20:43:15.065944 fakefarsi-0.0.1/fakefarsi.egg-info/
--rw-rw-rw-   0        0        0     1011 2024-03-21 20:43:15.000000 fakefarsi-0.0.1/fakefarsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-03-21 20:43:15.000000 fakefarsi-0.0.1/fakefarsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 20:43:15.000000 fakefarsi-0.0.1/fakefarsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 20:43:15.000000 fakefarsi-0.0.1/fakefarsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      535 2024-03-21 20:40:26.000000 fakefarsi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-21 20:43:15.065944 fakefarsi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      621 2024-03-21 20:40:19.000000 fakefarsi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:52:01.782291 fakefarsi-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-15 11:57:21.000000 fakefarsi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       18 2024-04-10 19:45:16.000000 fakefarsi-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1011 2024-04-10 19:52:01.781246 fakefarsi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-03-21 15:19:48.000000 fakefarsi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 19:52:01.767427 fakefarsi-0.0.2/data/
+-rw-rw-rw-   0        0        0    69171 2024-03-15 12:53:13.000000 fakefarsi-0.0.2/data/first_name.txt
+-rw-rw-rw-   0        0        0     6733 2024-03-15 12:18:35.000000 fakefarsi-0.0.2/data/last_name.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 19:52:01.769575 fakefarsi-0.0.2/fakefarsi/
+-rw-rw-rw-   0        0        0        0 2024-03-20 13:03:24.000000 fakefarsi-0.0.2/fakefarsi/__init__.py
+-rw-rw-rw-   0        0        0     2745 2024-04-10 19:49:57.000000 fakefarsi-0.0.2/fakefarsi/fakefarsi.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:52:01.780207 fakefarsi-0.0.2/fakefarsi.egg-info/
+-rw-rw-rw-   0        0        0     1011 2024-04-10 19:52:01.000000 fakefarsi-0.0.2/fakefarsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-10 19:52:01.000000 fakefarsi-0.0.2/fakefarsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 19:52:01.000000 fakefarsi-0.0.2/fakefarsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 19:52:01.000000 fakefarsi-0.0.2/fakefarsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      535 2024-04-10 19:31:27.000000 fakefarsi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 19:52:01.782291 fakefarsi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-10 19:28:51.000000 fakefarsi-0.0.2/setup.py
```

### Comparing `fakefarsi-0.0.1/FakeFarsi/fakefarsi.py` & `fakefarsi-0.0.2/fakefarsi/fakefarsi.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,12 +106,13 @@
 # Function to generate a fake email
 def fake_email(name, lastname):
     email = translator(name) + translator(lastname) + str(random.randint(1, 999)) + "@gmail.com"
     return email.replace(" ", "")
 
 
 # Read names from file
-names = read_names('اسامی.txt')
+names = read_names('../data/first_name.txt')
 
 
 # Read last names from file
-last_names = read_last_names('نام خانوادگی.txt')
+last_names = read_last_names('../data/last_name.txt')
+print(fake_name())
```

### Comparing `fakefarsi-0.0.1/LICENSE` & `fakefarsi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fakefarsi-0.0.1/PKG-INFO` & `fakefarsi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakefarsi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for generate a fake iranian person information
 Home-page: https://github.com/mhnrhmni/FakeFarsi/
 Author: Mahan Rahmani
 Author-email: Mahan Rahmani <mahanrahmani777@gmail.com>
 Project-URL: Homepage, https://github.com/mhnrhmni/FakeFarsi
 Project-URL: Issues, https://github.com/mhnrhmni/FakeFarsi/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fakefarsi-0.0.1/fakefarsi.egg-info/PKG-INFO` & `fakefarsi-0.0.2/fakefarsi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakefarsi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for generate a fake iranian person information
 Home-page: https://github.com/mhnrhmni/FakeFarsi/
 Author: Mahan Rahmani
 Author-email: Mahan Rahmani <mahanrahmani777@gmail.com>
 Project-URL: Homepage, https://github.com/mhnrhmni/FakeFarsi
 Project-URL: Issues, https://github.com/mhnrhmni/FakeFarsi/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fakefarsi-0.0.1/pyproject.toml` & `fakefarsi-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fakefarsi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mahan Rahmani", email="mahanrahmani777@gmail.com" },
 ]
 description = "A package for generate a fake iranian person information"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fakefarsi-0.0.1/setup.py` & `fakefarsi-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="fakefarsi",
-    version="0.0.1",
+    version="0.0.2",
     author="Mahan Rahmani",
     author_email="mahanrahmani777@gmail.com",
     description="A package for generate a fake iranian person information",
     long_description=readme,
     url="https://github.com/mhnrhmni/FakeFarsi/",
     packages=find_packages(),
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: Mit License",
         "Operating System :: OS Independent",
     ],
 )
```

