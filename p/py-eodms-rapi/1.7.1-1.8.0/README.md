# Comparing `tmp/py-eodms-rapi-1.7.1.tar.gz` & `tmp/py-eodms-rapi-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-eodms-rapi-1.7.1.tar", last modified: Wed Feb 28 20:11:56 2024, max compression
+gzip compressed data, was "py-eodms-rapi-1.8.0.tar", last modified: Wed Apr 10 15:45:17 2024, max compression
```

## Comparing `py-eodms-rapi-1.7.1.tar` & `py-eodms-rapi-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 20:11:56.555923 py-eodms-rapi-1.7.1/
--rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.7.1/LICENSE
--rw-rw-rw-   0        0        0     2841 2024-02-28 20:11:56.555923 py-eodms-rapi-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 20:11:56.471657 py-eodms-rapi-1.7.1/eodms_rapi/
--rw-rw-rw-   0        0        0      550 2024-02-27 21:15:05.000000 py-eodms-rapi-1.7.1/eodms_rapi/__init__.py
--rw-rw-rw-   0        0        0       21 2024-02-28 15:41:19.000000 py-eodms-rapi-1.7.1/eodms_rapi/__version__.py
--rw-rw-rw-   0        0        0   114829 2024-02-28 19:39:07.000000 py-eodms-rapi-1.7.1/eodms_rapi/eodms.py
--rw-rw-rw-   0        0        0    23889 2024-02-15 18:38:42.000000 py-eodms-rapi-1.7.1/eodms_rapi/geo.py
--rw-rw-rw-   0        0        0     1126 2023-09-18 18:59:45.000000 py-eodms-rapi-1.7.1/eodms_rapi/query_error.py
--rw-rw-rw-   0        0        0    15844 2024-02-28 19:39:10.000000 py-eodms-rapi-1.7.1/eodms_rapi/rapi_requests.py
-drwxrwxrwx   0        0        0        0 2024-02-28 20:11:56.527615 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/
--rw-rw-rw-   0        0        0     2841 2024-02-28 20:11:56.000000 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-02-28 20:11:56.000000 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 20:11:56.000000 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-02-28 20:11:56.000000 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-28 20:11:56.000000 py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      827 2024-02-28 20:11:56.555923 py-eodms-rapi-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1195 2024-02-28 15:41:18.000000 py-eodms-rapi-1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 20:11:56.539277 py-eodms-rapi-1.7.1/test/
--rw-rw-rw-   0        0        0     7134 2023-09-28 19:04:53.000000 py-eodms-rapi-1.7.1/test/test_pyeodmsrapi.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:45:17.047066 py-eodms-rapi-1.8.0/
+-rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2841 2024-04-10 15:45:17.047066 py-eodms-rapi-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 15:45:16.945072 py-eodms-rapi-1.8.0/eodms_rapi/
+-rw-rw-rw-   0        0        0      550 2024-02-27 21:15:05.000000 py-eodms-rapi-1.8.0/eodms_rapi/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-09 21:05:05.000000 py-eodms-rapi-1.8.0/eodms_rapi/__version__.py
+-rw-rw-rw-   0        0        0   118233 2024-04-09 21:05:15.000000 py-eodms-rapi-1.8.0/eodms_rapi/eodms.py
+-rw-rw-rw-   0        0        0    23889 2024-02-15 18:38:42.000000 py-eodms-rapi-1.8.0/eodms_rapi/geo.py
+-rw-rw-rw-   0        0        0     1126 2023-09-18 18:59:45.000000 py-eodms-rapi-1.8.0/eodms_rapi/query_error.py
+-rw-rw-rw-   0        0        0    16089 2024-04-09 21:05:17.000000 py-eodms-rapi-1.8.0/eodms_rapi/rapi_requests.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:45:17.007594 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/
+-rw-rw-rw-   0        0        0     2841 2024-04-10 15:45:16.000000 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-04-10 15:45:16.000000 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 15:45:16.000000 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-10 15:45:16.000000 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 15:45:16.000000 py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      827 2024-04-10 15:45:17.051452 py-eodms-rapi-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1212 2024-04-09 21:05:03.000000 py-eodms-rapi-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:45:17.043067 py-eodms-rapi-1.8.0/test/
+-rw-rw-rw-   0        0        0     7134 2023-09-28 19:04:53.000000 py-eodms-rapi-1.8.0/test/test_pyeodmsrapi.py
```

### Comparing `py-eodms-rapi-1.7.1/LICENSE` & `py-eodms-rapi-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.7.1/PKG-INFO` & `py-eodms-rapi-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.7.1
+Version: 1.8.0
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.7.1/README.md` & `py-eodms-rapi-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.7.1/eodms_rapi/__init__.py` & `py-eodms-rapi-1.8.0/eodms_rapi/__init__.py`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.7.1/eodms_rapi/eodms.py` & `py-eodms-rapi-1.8.0/eodms_rapi/eodms.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import urllib
 import json
 import datetime
 import pytz
 import time
 import dateparser
 import re
+from lxml import html, etree
 import dateutil.parser
 from dateutil.tz import tzlocal
-from urllib.parse import urlencode
+from urllib.parse import urlencode, urlparse
 # from urllib.parse import urlparse
 from concurrent.futures import ThreadPoolExecutor
 from xml.etree import ElementTree
 from warnings import warn
 
 from tqdm.auto import tqdm
 
@@ -1351,14 +1352,114 @@
 
         :param url: The new URL.
         :type  url: str
         """
 
         self.rapi_root = url
 
+    def _check_exists(self, dest_fn, fsize):
+        """
+        Compares the fsize variable to the size of a file.
+        """
+
+        # print(f"dest_fn: {dest_fn}")
+        # print(os.path.exists(dest_fn))
+        if os.path.exists(dest_fn):
+            # if all-good, continue to next file
+            print(f"os.stat: {os.stat(dest_fn).st_size}")
+            if os.stat(dest_fn).st_size == fsize:
+                self.msg = f"No download necessary. Local file already " \
+                    f"exists: {dest_fn}"
+                self.log_msg(self.msg)
+                return True
+            # Otherwise, delete the incomplete/malformed local file and
+            #   redownload
+            else:
+                self.msg = f'Filesize mismatch with ' \
+                    f'{os.path.basename(dest_fn)}. Re-downloading...'
+                self.log_msg(self.msg, 'warning')
+                os.remove(dest_fn)
+
+        return False
+
+    def download_folder(self, url, dest_folder, fsize=None, show_progress=True):
+        """
+        Downloads the contents of an online folder to the dest_folder.
+
+        :param url: The download URL of the image.
+        :type  url: str
+        :param dest_folder: The local destination folder for the download.
+        :type  dest_folder: str
+        :param fsize: The total filesize of the image.
+        :type  fsize: int
+        :param show_progress: Determines whether to show progress while
+        downloading an image
+        :type  show_progress: bool
+        """
+
+        print(f"Downloading folder...")
+
+        # print(f"dest_folder: {dest_folder}")
+
+         # If we have an existing local file, check the filesize against the
+        #   manifest
+        # if self._check_exists(dest_folder, fsize):
+        #     return None
+
+        if self._check_auth():
+            return None
+
+        if not os.path.exists(dest_folder):
+            os.makedirs(dest_folder)
+        
+        # print(f"url: {url}")
+
+        domain = urlparse(url).netloc
+
+        html_str = self.rapi_session.download(url, fsize, show_progress=False)
+
+        # print(f"html_str: {html_str}")
+
+        # Parse the HTML text of the destination string
+        html = etree.HTML(html_str.decode('utf-8'))
+        # result = etree.tostring(html, pretty_print=True, method="html")
+
+        # print(f"html: {dir(html)}")
+
+        links = [a for a in html.iterfind(".//a")]
+
+        # print(f"links: {links}")
+
+        for l in links[1:]:
+            href = f"https://{domain}{l.get('href')}"
+            href = href.rstrip('/')
+            
+            # print(f"href: {href}")
+
+            path = urlparse(href).path
+            ext = os.path.splitext(path)[1]
+            # print(ext)
+
+            if ext == '':
+                new_dest = os.path.join(dest_folder, os.path.basename(href))
+                # print(f"new_dest: {new_dest}")
+                self.download_folder(href, new_dest,
+                                     show_progress=show_progress)
+                continue
+
+            dest_fn = os.path.join(dest_folder, os.path.basename(href))
+
+            # print(f"dest_fn: {dest_fn}")
+
+            self.rapi_session.download(href, dest_fn=dest_fn,
+                                       show_progress=show_progress)
+
+            self.msg = f'{dest_fn} has been downloaded.'
+            self.log_msg(self.msg)
+
     def download_image(self, url, dest_fn, fsize, show_progress=True):
         """
         Given a list of remote and local items, download the remote data if
         it is not already found locally.
 
         (Adapted from the eodms-api-client (
         https://pypi.org/project/eodms-api-client/) developed by Mike Brady)
@@ -1372,33 +1473,24 @@
         :param show_progress: Determines whether to show progress while
         downloading an image
         :type  show_progress: bool
         """
 
         # If we have an existing local file, check the filesize against the
         #   manifest
-        if os.path.exists(dest_fn):
-            # if all-good, continue to next file
-            if os.stat(dest_fn).st_size == fsize:
-                self.msg = f"No download necessary. Local file already " \
-                    f"exists: {dest_fn}"
-                self.log_msg(self.msg)
-                return None
-            # Otherwise, delete the incomplete/malformed local file and
-            #   redownload
-            else:
-                self.msg = f'Filesize mismatch with ' \
-                    f'{os.path.basename(dest_fn)}. Re-downloading...'
-                self.log_msg(self.msg, 'warning')
-                os.remove(dest_fn)
+        if self._check_exists(dest_fn, fsize):
+            return None
 
         if self._check_auth():
             return None
+        
+        # print(f"url: {url}")
+        # answer = input("Press enter...")
 
-        self.rapi_session.download(url, dest_fn, fsize, show_progress)
+        self.rapi_session.download(url, fsize, dest_fn, show_progress)
 
         self.msg = f'{dest_fn} has been downloaded.'
         self.log_msg(self.msg)
 
     def download(self, items, dest, wait=10.0, max_attempts=None,
                  show_progress=True):
         """
@@ -1547,16 +1639,17 @@
                         # Get the string value of the destination
                         str_val = d['stringValue']
                         str_val = str_val.replace('</br>', '')
 
                         str_val = str_val.replace('&', '?')
 
                         # Parse the HTML text of the destination string
-                        root = ElementTree.fromstring(str_val)
+                        root = etree.fromstring(str_val)
                         url = root.text
+                        # url = root.tostring(root)
                         url = url.split("?")[0]
 
                         fn = os.path.basename(url)
 
                         # Download the image
                         msg = f"Downloading image from Collection " \
                                 f"{coll_id} with Record Id {record_id} ({fn})."
@@ -1566,24 +1659,30 @@
                         out_fn = os.path.join(dest, fn)
                         full_path = os.path.realpath(out_fn)
 
                         if not os.path.exists(dest):
                             os.makedirs(dest, exist_ok=True)
 
                         try:
-                            self.download_image(url, out_fn, fsize,
-                                                show_progress=show_progress)
+                            if url.endswith('.zip'):
+                                self.download_image(url, out_fn, fsize,
+                                                    show_progress=show_progress)
+                            else:
+                                self.download_folder(url, out_fn, fsize,
+                                                    show_progress=show_progress)
                         except Exception as e:
                             self.log_msg(e, 'warning')
                             continue
 
                         print('')
 
                         # Record the URL and downloaded file to a dictionary
                         dest_info = {'url': url, 'local_destination': full_path}
+                        # print(f"dest_info: {dest_info}")
+                        # answer = input("Press enter...")
                         download_paths.append(dest_info)
 
                     cur_item['downloadPaths'] = download_paths
 
                     complete_items.append(cur_item)
 
             if new_count == 0 and len(complete_items) == 0:
```

### Comparing `py-eodms-rapi-1.7.1/eodms_rapi/geo.py` & `py-eodms-rapi-1.8.0/eodms_rapi/geo.py`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.7.1/eodms_rapi/query_error.py` & `py-eodms-rapi-1.8.0/eodms_rapi/query_error.py`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.7.1/eodms_rapi/rapi_requests.py` & `py-eodms-rapi-1.8.0/eodms_rapi/rapi_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
         if res.text == '':
             return res
 
         if res.text.find('BRB!') > -1:
             self.err_msg = f"There was a problem while attempting to access the " \
                       f"EODMS RAPI server. If the problem persists, please " \
-                      f"contact the EODMS Support Team at {self._email}."
+                      f"contact the EODMS Support Team at {self.eodms._email}."
             self.eodms.log_msg(self.err_msg, 'error')
             self.err_occurred = True
             query_err = QueryError(self.err_msg)
             return query_err
 
         return res.json() if as_json else res
 
@@ -362,15 +362,15 @@
 
         :param number: The value for the number of attempts.
         :type  number: int
 
         """
         self.attempts = int(number)
 
-    def download(self, url, dest_fn, fsize, show_progress=True):
+    def download(self, url, fsize=None, dest_fn=None, show_progress=True):
         """
         Given a list of remote and local items, download the remote data if
         it is not already found locally.
 
         (Adapted from the eodms-api-client (
         https://pypi.org/project/eodms-api-client/) developed by Mike Brady)
 
@@ -379,27 +379,33 @@
         :param dest_fn: The local destination filename for the download.
         :type  dest_fn: str
         :param fsize: The total filesize of the image.
         :type  fsize: int
         :param show_progress: Determines whether to show progress while
         downloading an image
         :type  show_progress: bool
+        :param no_file: Determines whether to download as a file.
+        :type  no_file: bool
         """
 
         # Use streamed download so we can wrap nicely with tqdm
         if show_progress:
-            with self._session.get(url, stream=True, verify=self.verify) as stream:
+            with self._session.get(url, stream=True, verify=self.verify) \
+                    as stream:
                 with open(dest_fn, 'wb') as pipe:
                     with tqdm.wrapattr(
                             pipe,
                             method='write',
                             miniters=1,
                             total=fsize,
-                            desc=f"{self.eodms.header}{os.path.basename(dest_fn)}"
+                            desc=f"{self.eodms.header}\
+                                {os.path.basename(dest_fn)}"
                     ) as file_out:
                         for chunk in stream.iter_content(chunk_size=1024):
                             file_out.write(chunk)
         else:
             response = self._session.get(url, stream=True, verify=self.verify)
+            if dest_fn is None:
+                return response.content
             open(dest_fn, "wb").write(response.content)
 
         return dest_fn
```

### Comparing `py-eodms-rapi-1.7.1/py_eodms_rapi.egg-info/PKG-INFO` & `py-eodms-rapi-1.8.0/py_eodms_rapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.7.1
+Version: 1.8.0
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.7.1/setup.cfg` & `py-eodms-rapi-1.8.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 656f 646d 732d 7261 7069   = py-eodms-rapi
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 372e  ..version = 1.7.
-00000030: 310d 0a61 7574 686f 7220 3d20 4b65 7669  1..author = Kevi
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 382e  ..version = 1.8.
+00000030: 300d 0a61 7574 686f 7220 3d20 4b65 7669  0..author = Kevi
 00000040: 6e20 4261 6c6c 616e 7479 6e65 2028 4e61  n Ballantyne (Na
 00000050: 7475 7261 6c20 5265 736f 7572 6365 7320  tural Resources 
 00000060: 4361 6e61 6461 290d 0a61 7574 686f 725f  Canada)..author_
 00000070: 656d 6169 6c20 3d20 6b65 7669 6e2e 6261  email = kevin.ba
 00000080: 6c6c 616e 7479 6e65 406e 7263 616e 2d72  llantyne@nrcan-r
 00000090: 6e63 616e 2e67 632e 6361 0d0a 6465 7363  ncan.gc.ca..desc
 000000a0: 7269 7074 696f 6e20 3d20 454f 444d 5320  ription = EODMS
```

### Comparing `py-eodms-rapi-1.7.1/setup.py` & `py-eodms-rapi-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='py-eodms-rapi',
-    version='1.7.1', 
+    version='1.8.0', 
     author='Kevin Ballantyne (Natural Resources Canada)',
     author_email='kevin.ballantyne@nrcan-rncan.gc.ca',
     packages=find_packages(),
     include_package_data=True, 
     url='https://py-eodms-rapi.readthedocs.io/en/latest/',
     license='LICENSE',
     description='EODMS RAPI Client is a Python3 package used to access the ' \
@@ -15,14 +15,15 @@
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     install_requires=[
         "dateparser", 
         "requests",
         "tqdm",
         "geomet",
+        "lxml",
     ],
     project_urls={
         "Source": "https://github.com/eodms-sgdot/py-eodms-rapi", 
         "Bug Tracker": "https://github.com/eodms-sgdot/py-eodms-rapi/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `py-eodms-rapi-1.7.1/test/test_pyeodmsrapi.py` & `py-eodms-rapi-1.8.0/test/test_pyeodmsrapi.py`

 * *Files identical despite different names*

