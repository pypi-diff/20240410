# Comparing `tmp/streamlit-cookies-controller-0.0.3.tar.gz` & `tmp/streamlit-cookies-controller-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-cookies-controller-0.0.3.tar", last modified: Sat Mar  9 05:50:18 2024, max compression
+gzip compressed data, was "streamlit-cookies-controller-0.0.4.tar", last modified: Wed Apr 10 03:49:35 2024, max compression
```

## Comparing `streamlit-cookies-controller-0.0.3.tar` & `streamlit-cookies-controller-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.573221 streamlit-cookies-controller-0.0.3/
--rw-rw-rw-   0        0        0     1089 2024-03-09 02:00:01.000000 streamlit-cookies-controller-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       63 2024-03-09 02:00:01.000000 streamlit-cookies-controller-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3409 2024-03-09 05:50:18.571221 streamlit-cookies-controller-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2542 2024-03-09 05:50:09.000000 streamlit-cookies-controller-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-09 05:50:18.573221 streamlit-cookies-controller-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1366 2024-03-09 05:45:33.000000 streamlit-cookies-controller-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.548220 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/
--rw-rw-rw-   0        0        0      153 2024-03-09 02:00:01.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/__init__.py
--rw-rw-rw-   0        0        0     5963 2024-03-09 05:42:11.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/cookie_controller.py
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.534225 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.562220 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-03-09 05:42:12.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   225947 2024-03-09 02:00:01.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-03-09 05:42:12.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.536223 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.567220 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/
--rw-rw-rw-   0        0        0   340775 2024-03-09 05:42:12.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js
--rw-rw-rw-   0        0        0     1638 2024-03-09 05:42:12.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1320364 2024-03-09 05:42:12.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.map
--rw-rw-rw-   0        0        0      321 2024-03-09 02:00:01.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-09 05:50:18.557218 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/
--rw-rw-rw-   0        0        0     3409 2024-03-09 05:50:18.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2024-03-09 05:50:18.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 05:50:18.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-03-09 05:50:18.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-03-09 05:50:18.000000 streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.876495 streamlit-cookies-controller-0.0.4/
+-rw-rw-rw-   0        0        0     1089 2024-03-08 06:41:00.000000 streamlit-cookies-controller-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       63 2024-03-08 16:33:18.000000 streamlit-cookies-controller-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3410 2024-04-10 03:49:35.876495 streamlit-cookies-controller-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2545 2024-03-11 00:10:15.000000 streamlit-cookies-controller-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:49:35.882696 streamlit-cookies-controller-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2024-04-10 03:47:56.000000 streamlit-cookies-controller-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.822807 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/
+-rw-rw-rw-   0        0        0      153 2024-03-08 15:41:16.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/__init__.py
+-rw-rw-rw-   0        0        0     5963 2024-03-11 00:09:54.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/cookie_controller.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.795738 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.848450 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-10 03:46:11.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0      452 2024-04-10 03:46:11.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.797735 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.863437 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   340775 2024-04-10 03:46:11.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js
+-rw-rw-rw-   0        0        0     1638 2024-04-10 03:46:11.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1320364 2024-04-10 03:46:11.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.map
+-rw-rw-rw-   0        0        0      321 2024-03-08 16:23:22.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:49:35.842549 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/
+-rw-rw-rw-   0        0        0     3410 2024-04-10 03:49:35.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2024-04-10 03:49:35.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:49:35.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-10 03:49:35.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-10 03:49:35.000000 streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/top_level.txt
```

### Comparing `streamlit-cookies-controller-0.0.3/LICENSE` & `streamlit-cookies-controller-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-cookies-controller-0.0.3/PKG-INFO` & `streamlit-cookies-controller-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cookies-controller
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamlit cookies controller
 Home-page: https://github.com/NathanChen198/streamlit-cookies-controller
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Control client browser cookie for the site.
 
 ## What is Streamlit Cookie Controller?
-`streamlit-cookie-controller` let you
+`streamlit-cookies-controller` let you
 
 - get cookie(s)
 - set cookie
 - remove cookie
 
 from/to the client browser.
 It use [universal-cookie](https://www.npmjs.com/package/universal-cookie) package to access the cookies.
```

### Comparing `streamlit-cookies-controller-0.0.3/README.md` & `streamlit-cookies-controller-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Control client browser cookie for the site.
 
 ## What is Streamlit Cookie Controller?
-`streamlit-cookie-controller` let you
+`streamlit-cookies-controller` let you
 
 - get cookie(s)
 - set cookie
 - remove cookie
 
 from/to the client browser.
 It use [universal-cookie](https://www.npmjs.com/package/universal-cookie) package to access the cookies.
@@ -74,8 +74,8 @@
 [github_badge]: https://badgen.net/badge/icon/GitHub?icon=github&color=black&label
 [github_link]: https://github.com/NathanChen198/streamlit-cookies-controller
 [license_badge]: https://img.shields.io/badge/Licence-MIT-gr.svg
 [license_link]: https://github.com/NathanChen198/streamlit-cookies-controller/blob/main/LICENSE
 [issue_badge]: https://img.shields.io/github/issues/NathanChen198/streamlit-cookies-controller
 [issue_link]: https://github.com/NathanChen198/streamlit-cookies-controller/issues
 [pull_badge]: https://img.shields.io/github/issues-pr/NathanChen198/streamlit-cookies-controller
-[pull_link]: https://github.com/NathanChen198/streamlit-cookies-controller/pulls
+[pull_link]: https://github.com/NathanChen198/streamlit-cookies-controller/pulls
```

### Comparing `streamlit-cookies-controller-0.0.3/setup.py` & `streamlit-cookies-controller-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Author   : Nathan Chen
-# Date     : 08-Mar-2024
+# Date     : 10-Apr-2024
 
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='UTF-8')
 
 setup(
     name='streamlit-cookies-controller',
-    version='0.0.3',
+    version='0.0.4',
     author='Nathan Chen',
     author_email='nathan.chen.198@gmail.com',
     description='Streamlit cookies controller',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NathanChen198/streamlit-cookies-controller',
     packages=find_packages(),
```

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/cookie_controller.py` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/cookie_controller.py`

 * *Files identical despite different names*

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js`

 * *Files identical despite different names*

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.LICENSE.txt` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.map` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/PKG-INFO` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cookies-controller
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamlit cookies controller
 Home-page: https://github.com/NathanChen198/streamlit-cookies-controller
 Author: Nathan Chen
 Author-email: nathan.chen.198@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 [![GitHub license][license_badge]][license_link]
 [![GitHub issues][issue_badge]][issue_link]
 [![GitHub pull requests][pull_badge]][pull_link]
 
 Control client browser cookie for the site.
 
 ## What is Streamlit Cookie Controller?
-`streamlit-cookie-controller` let you
+`streamlit-cookies-controller` let you
 
 - get cookie(s)
 - set cookie
 - remove cookie
 
 from/to the client browser.
 It use [universal-cookie](https://www.npmjs.com/package/universal-cookie) package to access the cookies.
```

### Comparing `streamlit-cookies-controller-0.0.3/streamlit_cookies_controller.egg-info/SOURCES.txt` & `streamlit-cookies-controller-0.0.4/streamlit_cookies_controller.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,12 +7,11 @@
 streamlit_cookies_controller/utils.py
 streamlit_cookies_controller.egg-info/PKG-INFO
 streamlit_cookies_controller.egg-info/SOURCES.txt
 streamlit_cookies_controller.egg-info/dependency_links.txt
 streamlit_cookies_controller.egg-info/requires.txt
 streamlit_cookies_controller.egg-info/top_level.txt
 streamlit_cookies_controller/frontend/build/asset-manifest.json
-streamlit_cookies_controller/frontend/build/bootstrap.min.css
 streamlit_cookies_controller/frontend/build/index.html
 streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js
 streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.LICENSE.txt
 streamlit_cookies_controller/frontend/build/static/js/main.ab7915bb.js.map
```

