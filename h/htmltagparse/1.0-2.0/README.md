# Comparing `tmp/htmltagparse-1.0.tar.gz` & `tmp/htmltagparse-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmltagparse-1.0.tar", last modified: Wed Apr  3 12:09:20 2024, max compression
+gzip compressed data, was "htmltagparse-2.0.tar", last modified: Wed Apr 10 00:20:04 2024, max compression
```

## Comparing `htmltagparse-1.0.tar` & `htmltagparse-2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-03 12:09:20.138517 htmltagparse-1.0/
--rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-03 11:14:27.000000 htmltagparse-1.0/MANIFEST.in
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2962 2024-04-03 12:09:20.138517 htmltagparse-1.0/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2179 2024-04-03 12:06:43.000000 htmltagparse-1.0/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-03 12:09:20.137517 htmltagparse-1.0/htmltagparse/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      638 2024-04-03 12:00:30.000000 htmltagparse-1.0/htmltagparse/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      743 2024-04-02 14:15:23.000000 htmltagparse-1.0/htmltagparse/build.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      278 2024-04-01 18:51:03.000000 htmltagparse-1.0/htmltagparse/exceptions.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1386 2024-03-30 13:09:45.000000 htmltagparse-1.0/htmltagparse/html_tags.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     4892 2024-04-03 10:11:21.000000 htmltagparse-1.0/htmltagparse/parser.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-03 12:09:20.137517 htmltagparse-1.0/htmltagparse.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2962 2024-04-03 12:09:20.000000 htmltagparse-1.0/htmltagparse.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      349 2024-04-03 12:09:20.000000 htmltagparse-1.0/htmltagparse.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-03 12:09:20.000000 htmltagparse-1.0/htmltagparse.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       65 2024-04-03 12:09:20.000000 htmltagparse-1.0/htmltagparse.egg-info/requires.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-03 12:09:20.000000 htmltagparse-1.0/htmltagparse.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       64 2024-04-03 11:47:50.000000 htmltagparse-1.0/requirements.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-03 12:09:20.138517 htmltagparse-1.0/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1033 2024-04-03 12:02:29.000000 htmltagparse-1.0/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.508975 htmltagparse-2.0/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-03 11:14:27.000000 htmltagparse-2.0/MANIFEST.in
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3374 2024-04-10 00:20:04.508975 htmltagparse-2.0/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2591 2024-04-10 00:16:09.000000 htmltagparse-2.0/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.507975 htmltagparse-2.0/htmltagparse/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      704 2024-04-10 00:18:19.000000 htmltagparse-2.0/htmltagparse/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      747 2024-04-08 02:07:57.000000 htmltagparse-2.0/htmltagparse/build.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      316 2024-04-06 17:27:54.000000 htmltagparse-2.0/htmltagparse/exceptions.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1696 2024-04-06 23:56:18.000000 htmltagparse-2.0/htmltagparse/html_tags.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     8397 2024-04-09 23:46:17.000000 htmltagparse-2.0/htmltagparse/parser.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.508975 htmltagparse-2.0/htmltagparse.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3374 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      349 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       65 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/requires.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       64 2024-04-03 11:47:50.000000 htmltagparse-2.0/requirements.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-10 00:20:04.508975 htmltagparse-2.0/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1011 2024-04-06 15:43:41.000000 htmltagparse-2.0/setup.py
```

### Comparing `htmltagparse-1.0/PKG-INFO` & `htmltagparse-2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmltagparse
-Version: 1.0
+Version: 2.0
 Summary: A tool designed to quickly parse html tags and elements.
 Home-page: https://github.com/xyzpw/htmltagparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -18,21 +18,24 @@
 Description-Content-Type: text/markdown
 Requires-Dist: timeoutcall==1.*
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: requests==2.*
 Requires-Dist: html5lib==1.*
 
 # htmltagparse
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/htmltagparse)
+
 A tool designed to quickly parse html tags and elements.
 
 ## Prerequisites
 - Pip packages:
   - timeoutcall==1.*
   - beautifulsoup4==4.*
   - html5lib==1.*
+  - requests==2.*
 
 ## Usage
 ### Reading Page Titles
 Firstly, if you would like to view a page title alone, you could use the `titleFromUri` function:
 ```python
 from htmltagparse import titleFromUri
 
@@ -49,20 +52,20 @@
 print(brave.tags) #list of tags found on the specified page
 print(brave.searchTag("footer")) #displays a list of innerHtml content to the footer tags
 print(brave.searchTag("footer", htmlFormat=False)[0]) #output: © Brave Software Brave Search API Summarizer Helpful answers Report a security issue
 ```
 
 #### Building Pages via HTML
 ```python
-from htmltagparse import NewPage
+from htmltagparse import HtmlPage
 from requests import get
 
 htmlContent = get("https://duckduckgo.com/").text
-ddg = NewPage(htmlContent)
-print(list(ddg.sources)) #output: script
+ddg = HtmlPage(htmlContent)
+print(list(ddg.sources)) #output: ['script']
 ```
 
 #### Searching A Page
 With this package, you have the ability to search the html page you have created directly through a function:
 ```python
 from htmltagparse import build
 import re
@@ -77,20 +80,35 @@
   videoTags = re.findall(r"(?:\"|\')(?P<tag>.*?)(?:\'|\")(?:\,|\])", videoTags)
 except:
   videoTags = "no tags found"
 
 print(videoTags)
 ```
 
+Another way you could get tags from a Youtube video:
+```python
+import htmltagparse
+
+#youtube video id
+videoId = ""
+video = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
+
+for i in video.metadata:
+  if i.get("name") == "keywords":
+    tags = i.get("content").split(", ")
+    break
+print(i)
+```
+
 ## Developers
-### Building To Wheel File
+### Building to Wheel File
 - cd into root directory of this repository
 - run `python3 -m build`
 
 > [!NOTE]
-> Errors building this package may be due to external package requirements, if this occurs, use `python3 -m build -n` instead.
+> Errors building this package may be due to this packages requirements, if this occurs, use `python3 -m build -n` instead.
 
 ### Contributions
 Must not include:
 - Major changes
 - Breaking code
 - Changes to version number
```

### Comparing `htmltagparse-1.0/htmltagparse/__init__.py` & `htmltagparse-2.0/htmltagparse/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""
-A tool designed to quickly parse html tags and elements.
-"""
+"""A tool designed to quickly parse html tags and elements."""
+
 from . import parser
 import requests
-from .parser import NewPage, html2txt
+from .parser import *
 from . import build
 
-__version__ = "1.0"
+__version__ = "2.0"
 __author__ = "xyzpw"
 __description__ = "A tool designed to quickly parse html tags and elements."
 __license__ = "MIT"
 
 __all__ = [
     "titleFromHtml",
     "titleFromUri",
-    "NewPage",
+    "HtmlPage",
     "build",
+    "getElementAttributeValue",
+    "getElementAttributes",
+    "getTagContents",
 ]
 
 def titleFromHtml(htmlContent: str) -> str:
     htmlTitle = parser.searchForGroup(r"<title>(?P<title>.*?)</title>", htmlContent, "title")
     return html2txt(htmlTitle)
 
 def titleFromUri(url: str) -> str:
```

### Comparing `htmltagparse-1.0/htmltagparse/build.py` & `htmltagparse-2.0/htmltagparse/build.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from .parser import NewPage
+from .parser import HtmlPage
 import requests
 import time
 from .exceptions import *
 
 __all__ = [
     "fromUri",
 ]
 
 def fromUri(uri: str, timeout=5, headers={}) -> object:
+    """Builds an html page from a URI."""
     priorEpoch = time.time()
     try:
         resp = requests.get(uri, timeout=timeout, headers=headers)
-    except (requests.exceptions.ConnectionError, requests.exceptions.ReadTimeout):
-        htmlError = RequestTimeoutException(RequestTimeoutException.__doc__)
-        htmlError.uri = str(uri)
-        htmlError.timeout = float(timeout)
-        return htmlError
+    except (requests.exceptions.ReadTimeout, requests.exceptions.ConnectTimeout):
+        raise HtmlHttpError("did not receive server data within timeout duration")
     tagTimeout = timeout - (time.time() - priorEpoch)
     pageHtml = resp.text
-    page = NewPage(pageHtml, timeout=tagTimeout)
+    page = HtmlPage(pageHtml, timeout=tagTimeout)
     page.uri = resp.url
-    page.status_code = resp.status_code
+    page.response = (resp.status_code, resp.reason)
+    page.elapsed = time.time() - priorEpoch
     return page
```

### Comparing `htmltagparse-1.0/htmltagparse/html_tags.py` & `htmltagparse-2.0/htmltagparse/html_tags.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 __all__ = [
     "tagsWithSrc",
     "all_tags",
     "tagsWithHref",
+    "voidTags",
+    "nonVoidTags",
+]
+
+voidTags = [
+    "area",
+    "base",
+    "br",
+    "col",
+    "embed",
+    "hr",
+    "img",
+    "input",
+    "link",
+    "meta",
+    "param",
+    "source",
+    "track",
+    "wbr",
 ]
 
 tagsWithHref = [
     "a",
     "area",
     "base",
     "link",
@@ -139,7 +158,11 @@
 	"track",
 	"u",
 	"ul",
 	"var",
 	"video",
 	"wbr"
 ]
+nonVoidTags = []
+for t in all_tags:
+    if not t in voidTags:
+        nonVoidTags.append(t)
```

### Comparing `htmltagparse-1.0/htmltagparse.egg-info/PKG-INFO` & `htmltagparse-2.0/htmltagparse.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmltagparse
-Version: 1.0
+Version: 2.0
 Summary: A tool designed to quickly parse html tags and elements.
 Home-page: https://github.com/xyzpw/htmltagparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -18,21 +18,24 @@
 Description-Content-Type: text/markdown
 Requires-Dist: timeoutcall==1.*
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: requests==2.*
 Requires-Dist: html5lib==1.*
 
 # htmltagparse
+![Pepy Total Downlods](https://img.shields.io/pepy/dt/htmltagparse)
+
 A tool designed to quickly parse html tags and elements.
 
 ## Prerequisites
 - Pip packages:
   - timeoutcall==1.*
   - beautifulsoup4==4.*
   - html5lib==1.*
+  - requests==2.*
 
 ## Usage
 ### Reading Page Titles
 Firstly, if you would like to view a page title alone, you could use the `titleFromUri` function:
 ```python
 from htmltagparse import titleFromUri
 
@@ -49,20 +52,20 @@
 print(brave.tags) #list of tags found on the specified page
 print(brave.searchTag("footer")) #displays a list of innerHtml content to the footer tags
 print(brave.searchTag("footer", htmlFormat=False)[0]) #output: © Brave Software Brave Search API Summarizer Helpful answers Report a security issue
 ```
 
 #### Building Pages via HTML
 ```python
-from htmltagparse import NewPage
+from htmltagparse import HtmlPage
 from requests import get
 
 htmlContent = get("https://duckduckgo.com/").text
-ddg = NewPage(htmlContent)
-print(list(ddg.sources)) #output: script
+ddg = HtmlPage(htmlContent)
+print(list(ddg.sources)) #output: ['script']
 ```
 
 #### Searching A Page
 With this package, you have the ability to search the html page you have created directly through a function:
 ```python
 from htmltagparse import build
 import re
@@ -77,20 +80,35 @@
   videoTags = re.findall(r"(?:\"|\')(?P<tag>.*?)(?:\'|\")(?:\,|\])", videoTags)
 except:
   videoTags = "no tags found"
 
 print(videoTags)
 ```
 
+Another way you could get tags from a Youtube video:
+```python
+import htmltagparse
+
+#youtube video id
+videoId = ""
+video = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
+
+for i in video.metadata:
+  if i.get("name") == "keywords":
+    tags = i.get("content").split(", ")
+    break
+print(i)
+```
+
 ## Developers
-### Building To Wheel File
+### Building to Wheel File
 - cd into root directory of this repository
 - run `python3 -m build`
 
 > [!NOTE]
-> Errors building this package may be due to external package requirements, if this occurs, use `python3 -m build -n` instead.
+> Errors building this package may be due to this packages requirements, if this occurs, use `python3 -m build -n` instead.
 
 ### Contributions
 Must not include:
 - Major changes
 - Breaking code
 - Changes to version number
```

### Comparing `htmltagparse-1.0/setup.py` & `htmltagparse-2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import setuptools
 import htmltagparse
 
-def readme():
-    with open("README.md", 'r') as f:
-        return f.read()
+with open("README.md", "r") as f:
+    readme = f.read()
 
 with open("requirements.txt", 'r') as f:
     requirements = f.read().split('\n')
 
 setuptools.setup(
     name="htmltagparse",
     version=htmltagparse.__version__,
     author=htmltagparse.__author__,
     maintainer=htmltagparse.__author__,
     description=htmltagparse.__description__,
     url="https://github.com/xyzpw/htmltagparse/",
-    long_description=readme(),
+    long_description=readme,
     long_description_content_type="text/markdown",
     license=htmltagparse.__license__,
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

