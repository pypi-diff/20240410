# Comparing `tmp/msrestazure-0.6.4.tar.gz` & `tmp/msrestazure-0.6.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/msrestazure-0.6.4.tar", last modified: Mon Jun 29 20:04:02 2020, max compression
+gzip compressed data, was "msrestazure-0.6.4.post1.tar", last modified: Tue Feb 27 01:37:43 2024, max compression
```

## Comparing `msrestazure-0.6.4.tar` & `msrestazure-0.6.4.post1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-06-29 20:03:12.000000 msrestazure-0.6.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    19917 2020-06-29 20:04:02.000000 msrestazure-0.6.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-06-29 20:04:02.000000 msrestazure-0.6.4/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11480 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19239 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/azure_operation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3875 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/azure_configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10427 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/azure_exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure/polling/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17467 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/polling/arm_polling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5152 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/polling/async_arm_polling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/polling/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29612 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/azure_active_directory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1470 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11837 2020-06-29 20:03:12.000000 msrestazure-0.6.4/msrestazure/azure_cloud.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14513 2020-06-29 20:03:12.000000 msrestazure-0.6.4/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19917 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      795 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       44 2020-06-29 20:04:02.000000 msrestazure-0.6.4/msrestazure.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2434 2020-06-29 20:03:12.000000 msrestazure-0.6.4/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    22592 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-29 20:04:02.000000 msrestazure-0.6.4/tests/asynctests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15272 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/asynctests/test_async_arm_polling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19331 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_arm_polling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15726 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_operation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14691 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27741 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_auth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3896 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/test_cloud.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2404 2020-06-29 20:03:12.000000 msrestazure-0.6.4/tests/conftest.py
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1072 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/LICENSE.md
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)       43 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/MANIFEST.in
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    15769 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/PKG-INFO
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    14901 2024-02-27 00:58:26.000000 msrestazure-0.6.4.post1/README.rst
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/msrestazure/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1470 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/__init__.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    29613 2024-02-27 00:58:26.000000 msrestazure-0.6.4.post1/msrestazure/azure_active_directory.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    11837 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/azure_cloud.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     3875 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/azure_configuration.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    10427 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/azure_exceptions.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    19239 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/azure_operation.py
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/msrestazure/polling/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1303 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/polling/__init__.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    17467 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/polling/arm_polling.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     5152 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/polling/async_arm_polling.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    11480 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/msrestazure/tools.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1407 2024-02-27 00:58:26.000000 msrestazure-0.6.4.post1/msrestazure/version.py
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/msrestazure.egg-info/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    15769 2024-02-27 01:37:43.000000 msrestazure-0.6.4.post1/msrestazure.egg-info/PKG-INFO
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)      806 2024-02-27 01:37:43.000000 msrestazure-0.6.4.post1/msrestazure.egg-info/SOURCES.txt
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)        1 2024-02-27 01:37:43.000000 msrestazure-0.6.4.post1/msrestazure.egg-info/dependency_links.txt
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)       44 2024-02-27 01:37:43.000000 msrestazure-0.6.4.post1/msrestazure.egg-info/requires.txt
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)       12 2024-02-27 01:37:43.000000 msrestazure-0.6.4.post1/msrestazure.egg-info/top_level.txt
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)       67 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/setup.cfg
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     2444 2024-02-27 00:58:26.000000 msrestazure-0.6.4.post1/setup.py
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/tests/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1599 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/__init__.py
+drwxr-xr-x   0 lmazuel   (1000) lmazuel   (1000)        0 2024-02-27 01:37:43.780400 msrestazure-0.6.4.post1/tests/asynctests/
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    15272 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/asynctests/test_async_arm_polling.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     2404 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/conftest.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    19331 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_arm_polling.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    27741 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_auth.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     3896 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_cloud.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)     1658 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_configuration.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    14691 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_exceptions.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    15726 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_operation.py
+-rw-r--r--   0 lmazuel   (1000) lmazuel   (1000)    22592 2024-02-27 00:31:16.000000 msrestazure-0.6.4.post1/tests/test_tools.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `msrestazure-0.6.4/msrestazure/tools.py` & `msrestazure-0.6.4.post1/msrestazure/tools.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/azure_operation.py` & `msrestazure-0.6.4.post1/msrestazure/azure_operation.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/azure_configuration.py` & `msrestazure-0.6.4.post1/msrestazure/azure_configuration.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/azure_exceptions.py` & `msrestazure-0.6.4.post1/msrestazure/azure_exceptions.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/polling/arm_polling.py` & `msrestazure-0.6.4.post1/msrestazure/polling/arm_polling.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/polling/async_arm_polling.py` & `msrestazure-0.6.4.post1/msrestazure/polling/async_arm_polling.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/polling/__init__.py` & `msrestazure-0.6.4.post1/msrestazure/polling/__init__.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/version.py` & `msrestazure-0.6.4.post1/msrestazure/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 #: version of the package. Use msrestazure.__version__ instead.
-msrestazure_version = "0.6.4"
+msrestazure_version = "0.6.4.post1"
```

### Comparing `msrestazure-0.6.4/msrestazure/azure_active_directory.py` & `msrestazure-0.6.4.post1/msrestazure/azure_active_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         # let us hit the cache first
         token_entry = self.cache.get(resource, None)
         if token_entry:
             expires_on = int(token_entry['expires_on'])
             expires_on_datetime = datetime.datetime.fromtimestamp(expires_on)
             expiration_margin = 5  # in minutes
             if datetime.datetime.now() + datetime.timedelta(minutes=expiration_margin) <= expires_on_datetime:
-                _LOGGER.info("MSI: token is found in cache.")
+                _LOGGER.debug("MSI: token is found in cache.")
                 return token_entry
             _LOGGER.info("MSI: cache is found but expired within %s minutes, so getting a new one.", expiration_margin)
             self.cache.pop(resource)
 
         token_entry = self._retrieve_token_from_imds_with_retry(resource)
         self.cache[resource] = token_entry
         return token_entry
```

### Comparing `msrestazure-0.6.4/msrestazure/__init__.py` & `msrestazure-0.6.4.post1/msrestazure/__init__.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/msrestazure/azure_cloud.py` & `msrestazure-0.6.4.post1/msrestazure/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/README.rst` & `msrestazure-0.6.4.post1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
 .. image:: https://travis-ci.org/Azure/msrestazure-for-python.svg?branch=master
  :target: https://travis-ci.org/Azure/msrestazure-for-python
 
 .. image:: https://codecov.io/gh/azure/msrestazure-for-python/branch/master/graph/badge.svg
  :target: https://codecov.io/gh/azure/msrestazure-for-python
 
+Disclaimer
+----------
+
+*This package is deprecated and no longer receives updates*
+
+- The authentication part of this package has been moved to `azure-identity <https://pypi.org/project/azure-identity/>`_
+- The other parts of this library are covered by `azure-mgmt-core <https://pypi.org/project/azure-mgmt-core/>`_
+
+As such, we will no longer accept PR and fix issues on this project.
+
 Installation
 ------------
 
 To install:
 
 .. code-block:: bash
```

### Comparing `msrestazure-0.6.4/msrestazure.egg-info/SOURCES.txt` & `msrestazure-0.6.4.post1/msrestazure.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 msrestazure/__init__.py
 msrestazure/azure_active_directory.py
 msrestazure/azure_cloud.py
```

### Comparing `msrestazure-0.6.4/setup.py` & `msrestazure-0.6.4.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 #
 # --------------------------------------------------------------------------
 
 from setuptools import setup, find_packages
 
 setup(
     name='msrestazure',
-    version='0.6.4',
+    version='0.6.4.post1',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     packages=find_packages(exclude=["tests", "tests.*"]),
     url='https://github.com/Azure/msrestazure-for-python',
     license='MIT License',
     description=('AutoRest swagger generator Python client runtime. '
                  'Azure-specific module.'),
     long_description=open('README.rst').read(),
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 7 - Inactive',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `msrestazure-0.6.4/tests/test_tools.py` & `msrestazure-0.6.4.post1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/asynctests/test_async_arm_polling.py` & `msrestazure-0.6.4.post1/tests/asynctests/test_async_arm_polling.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_arm_polling.py` & `msrestazure-0.6.4.post1/tests/test_arm_polling.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_operation.py` & `msrestazure-0.6.4.post1/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_exceptions.py` & `msrestazure-0.6.4.post1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_configuration.py` & `msrestazure-0.6.4.post1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_auth.py` & `msrestazure-0.6.4.post1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/test_cloud.py` & `msrestazure-0.6.4.post1/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/__init__.py` & `msrestazure-0.6.4.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `msrestazure-0.6.4/tests/conftest.py` & `msrestazure-0.6.4.post1/tests/conftest.py`

 * *Files identical despite different names*

