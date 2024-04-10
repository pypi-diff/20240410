# Comparing `tmp/monedadigitalf-1.6.43.post1.tar.gz` & `tmp/monedadigitalf-1.6.43.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monedadigitalf-1.6.43.post1.tar", last modified: Wed Apr 10 14:12:11 2024, max compression
+gzip compressed data, was "monedadigitalf-1.6.43.post2.tar", last modified: Wed Apr 10 17:11:52 2024, max compression
```

## Comparing `monedadigitalf-1.6.43.post1.tar` & `monedadigitalf-1.6.43.post2.tar`

### file list

```diff
@@ -1,22 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:12:11.286465 monedadigitalf-1.6.43.post1/
--rw-rw-rw-   0        0        0     2545 2024-04-10 14:12:11.286465 monedadigitalf-1.6.43.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1955 2024-04-10 13:57:11.000000 monedadigitalf-1.6.43.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 14:12:11.270841 monedadigitalf-1.6.43.post1/forexconnect/
--rw-rw-rw-   0        0        0     1652 2024-04-09 21:29:09.000000 monedadigitalf-1.6.43.post1/forexconnect/EachRowListener.py
--rw-rw-rw-   0        0        0    24872 2024-04-09 21:31:07.000000 monedadigitalf-1.6.43.post1/forexconnect/ForexConnect.py
--rw-rw-rw-   0        0        0     9928 2024-04-09 21:31:44.000000 monedadigitalf-1.6.43.post1/forexconnect/LiveHistory.py
--rw-rw-rw-   0        0        0     8006 2024-04-09 21:29:17.000000 monedadigitalf-1.6.43.post1/forexconnect/ResponseListener.py
--rw-rw-rw-   0        0        0     4786 2024-04-09 21:29:19.000000 monedadigitalf-1.6.43.post1/forexconnect/SessionStatusListener.py
--rw-rw-rw-   0        0        0     5903 2024-04-09 21:29:21.000000 monedadigitalf-1.6.43.post1/forexconnect/TableListener.py
--rw-rw-rw-   0        0        0     3124 2024-04-09 21:29:23.000000 monedadigitalf-1.6.43.post1/forexconnect/TableManagerListener.py
--rw-rw-rw-   0        0        0      641 2024-04-09 21:19:48.000000 monedadigitalf-1.6.43.post1/forexconnect/__init__.py
--rw-rw-rw-   0        0        0    19131 2024-04-09 21:29:01.000000 monedadigitalf-1.6.43.post1/forexconnect/common.py
--rw-rw-rw-   0        0        0      931 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post1/forexconnect/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:12:11.286465 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/
--rw-rw-rw-   0        0        0     2545 2024-04-10 14:12:11.000000 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2024-04-10 14:12:11.000000 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:12:11.000000 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 14:12:11.000000 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2024-04-10 14:12:11.000000 monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 14:12:11.286465 monedadigitalf-1.6.43.post1/setup.cfg
--rw-rw-rw-   0        0        0      980 2024-04-10 14:12:06.000000 monedadigitalf-1.6.43.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:11:52.787112 monedadigitalf-1.6.43.post2/
+-rw-rw-rw-   0        0        0       36 2024-04-10 17:11:46.000000 monedadigitalf-1.6.43.post2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2545 2024-04-10 17:11:52.769920 monedadigitalf-1.6.43.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     1955 2024-04-10 13:57:11.000000 monedadigitalf-1.6.43.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 17:11:52.699419 monedadigitalf-1.6.43.post2/forexconnect/
+-rw-rw-rw-   0        0        0     1652 2024-04-09 21:29:09.000000 monedadigitalf-1.6.43.post2/forexconnect/EachRowListener.py
+-rw-rw-rw-   0        0        0    24872 2024-04-09 21:31:07.000000 monedadigitalf-1.6.43.post2/forexconnect/ForexConnect.py
+-rw-rw-rw-   0        0        0     9928 2024-04-09 21:31:44.000000 monedadigitalf-1.6.43.post2/forexconnect/LiveHistory.py
+-rw-rw-rw-   0        0        0     8006 2024-04-09 21:29:17.000000 monedadigitalf-1.6.43.post2/forexconnect/ResponseListener.py
+-rw-rw-rw-   0        0        0     4786 2024-04-09 21:29:19.000000 monedadigitalf-1.6.43.post2/forexconnect/SessionStatusListener.py
+-rw-rw-rw-   0        0        0     5903 2024-04-09 21:29:21.000000 monedadigitalf-1.6.43.post2/forexconnect/TableListener.py
+-rw-rw-rw-   0        0        0     3124 2024-04-09 21:29:23.000000 monedadigitalf-1.6.43.post2/forexconnect/TableManagerListener.py
+-rw-rw-rw-   0        0        0      641 2024-04-09 21:19:48.000000 monedadigitalf-1.6.43.post2/forexconnect/__init__.py
+-rw-rw-rw-   0        0        0    19131 2024-04-09 21:29:01.000000 monedadigitalf-1.6.43.post2/forexconnect/common.py
+-rw-rw-rw-   0        0        0      931 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:11:52.764262 monedadigitalf-1.6.43.post2/forexconnect/lib/
+-rw-rw-rw-   0        0        0        0 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:11:52.764262 monedadigitalf-1.6.43.post2/forexconnect/lib/__pycache__/
+-rw-rw-rw-   0        0        0      168 2024-04-09 21:20:49.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0 14199600 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/fxcorepy.so
+-rw-rw-rw-   0        0        0  1987680 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libForexConnect.so
+-rw-rw-rw-   0        0        0   299128 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libboost_python3.so.1.64.0
+-rw-rw-rw-   0        0        0    14640 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libboost_system.so.1.64.0
+-rw-rw-rw-   0        0        0  2741248 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libfxmsg.so
+-rw-rw-rw-   0        0        0   186440 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libfxtp.so
+-rw-rw-rw-   0        0        0  1188656 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libgsexpat.so
+-rw-rw-rw-   0        0        0   148064 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libgstool3.so
+-rw-rw-rw-   0        0        0  3126400 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libhttplib.so
+-rw-rw-rw-   0        0        0   415592 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/liblog4cplus.so
+-rw-rw-rw-   0        0        0    39768 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/liblogger.so
+-rw-rw-rw-   0        0        0   659568 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libpdas.so
+-rw-rw-rw-   0        0        0   303464 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libpricehistorymgr.so.2.8.0
+-rw-rw-rw-   0        0        0  3421160 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libpython3.7m.so
+-rw-rw-rw-   0        0        0  1245248 2021-07-21 13:02:42.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libquotesmgr2.so.2.8
+-rw-rw-rw-   0        0        0   641120 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/libsqlite3.8.so
+-rw-rw-rw-   0        0        0       77 2021-07-21 13:02:40.000000 monedadigitalf-1.6.43.post2/forexconnect/lib/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 17:11:52.769920 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/
+-rw-rw-rw-   0        0        0     2545 2024-04-10 17:11:52.000000 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1177 2024-04-10 17:11:52.000000 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:11:52.000000 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 16:56:03.000000 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:11:52.000000 monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 17:11:52.787112 monedadigitalf-1.6.43.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2024-04-10 17:10:18.000000 monedadigitalf-1.6.43.post2/setup.py
```

### Comparing `monedadigitalf-1.6.43.post1/PKG-INFO` & `monedadigitalf-1.6.43.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monedadigitalf
-Version: 1.6.43.post1
+Version: 1.6.43.post2
 Summary: ForexConnect API is a trading API for the FXCM Group: https://www.fxcm.com/uk/
 Home-page: https://github.com/AmadoRamos/forexconect.git
 Download-URL: https://github.com/AmadoRamos/forexconect/archive/refs/tags/v1.6.43r1.zip
 Author: Gehtsoft USA, LLC
 Author-email: contact@gehtsoftusa.com
 License: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `monedadigitalf-1.6.43.post1/README.md` & `monedadigitalf-1.6.43.post2/README.md`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/EachRowListener.py` & `monedadigitalf-1.6.43.post2/forexconnect/EachRowListener.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/ForexConnect.py` & `monedadigitalf-1.6.43.post2/forexconnect/ForexConnect.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/LiveHistory.py` & `monedadigitalf-1.6.43.post2/forexconnect/LiveHistory.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/ResponseListener.py` & `monedadigitalf-1.6.43.post2/forexconnect/ResponseListener.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/SessionStatusListener.py` & `monedadigitalf-1.6.43.post2/forexconnect/SessionStatusListener.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/TableListener.py` & `monedadigitalf-1.6.43.post2/forexconnect/TableListener.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/TableManagerListener.py` & `monedadigitalf-1.6.43.post2/forexconnect/TableManagerListener.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/__init__.py` & `monedadigitalf-1.6.43.post2/forexconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/common.py` & `monedadigitalf-1.6.43.post2/forexconnect/common.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/forexconnect/errors.py` & `monedadigitalf-1.6.43.post2/forexconnect/errors.py`

 * *Files identical despite different names*

### Comparing `monedadigitalf-1.6.43.post1/monedadigitalf.egg-info/PKG-INFO` & `monedadigitalf-1.6.43.post2/monedadigitalf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monedadigitalf
-Version: 1.6.43.post1
+Version: 1.6.43.post2
 Summary: ForexConnect API is a trading API for the FXCM Group: https://www.fxcm.com/uk/
 Home-page: https://github.com/AmadoRamos/forexconect.git
 Download-URL: https://github.com/AmadoRamos/forexconect/archive/refs/tags/v1.6.43r1.zip
 Author: Gehtsoft USA, LLC
 Author-email: contact@gehtsoftusa.com
 License: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `monedadigitalf-1.6.43.post1/setup.py` & `monedadigitalf-1.6.43.post2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 version = '1.6.43r1'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="monedadigitalf",
-    version=version,
+    version='1.6.43.post2',
 
     author="Gehtsoft USA, LLC",
     author_email="contact@gehtsoftusa.com",
 
     url="https://github.com/AmadoRamos/forexconect.git",
     download_url=f"https://github.com/AmadoRamos/forexconect/archive/refs/tags/v{version}.zip",
 
     description="ForexConnect API is a trading API for the FXCM Group: https://www.fxcm.com/uk/",
 
-    packages=['forexconnect'],
+    packages=find_packages(include=('forexconnect/*',)),
+    package_data={'': ['forexconnect/lib/fxcorepy.so']},
+    #include = ["forexconnect/lib/*", 'lib/*'],
     install_requires=[],
 
     license='Other/Proprietary License',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3.10",
     ],
     include_package_data=True, # for MANIFEST.in
     python_requires='>=3.6.0',
 
-    package_data={package: ["py.typed", "*.pyi", "**/*.pyi"] for package in find_packages()},
+    #package_data={package: ["py.typed", "*.pyi", "**/*.pyi"] for package in find_packages()},
     zip_safe=False,
 )
```

