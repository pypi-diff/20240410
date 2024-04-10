# Comparing `tmp/pytiqs-1.0.1.tar.gz` & `tmp/pytiqs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.1.tar", last modified: Tue Apr  9 04:39:21 2024, max compression
+gzip compressed data, was "pytiqs-1.0.2.tar", last modified: Wed Apr 10 04:14:57 2024, max compression
```

## Comparing `pytiqs-1.0.1.tar` & `pytiqs-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488705 pytiqs-1.0.1/
--rw-r--r--   0 nitin      (501) staff       (20)      369 2024-04-09 04:39:21.488641 pytiqs-1.0.1/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)       19 2024-04-08 12:31:10.000000 pytiqs-1.0.1/README.md
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488394 pytiqs-1.0.1/pytiqs.egg-info/
--rw-r--r--   0 nitin      (501) staff       (20)      369 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)      267 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/SOURCES.txt
--rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/dependency_links.txt
--rw-r--r--   0 nitin      (501) staff       (20)       52 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/requires.txt
--rw-r--r--   0 nitin      (501) staff       (20)        5 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/top_level.txt
--rw-r--r--   0 nitin      (501) staff       (20)      575 2024-04-09 04:39:21.489078 pytiqs-1.0.1/setup.cfg
--rw-r--r--   0 nitin      (501) staff       (20)     1051 2024-04-09 04:38:33.000000 pytiqs-1.0.1/setup.py
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488021 pytiqs-1.0.1/tiqs/
--rw-r--r--   0 nitin      (501) staff       (20)      104 2024-04-02 04:30:57.000000 pytiqs-1.0.1/tiqs/__init__.py
--rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-09 04:39:11.000000 pytiqs-1.0.1/tiqs/__version__.py
--rw-r--r--   0 nitin      (501) staff       (20)    17659 2024-04-08 11:39:51.000000 pytiqs-1.0.1/tiqs/connect.py
--rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-02 20:18:14.000000 pytiqs-1.0.1/tiqs/constants.py
--rw-r--r--   0 nitin      (501) staff       (20)      555 2024-03-21 12:32:16.000000 pytiqs-1.0.1/tiqs/exceptions.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-10 04:14:57.591711 pytiqs-1.0.2/
+-rw-r--r--   0 nitin      (501) staff       (20)      522 2024-04-10 04:14:57.591614 pytiqs-1.0.2/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)       19 2024-04-09 08:29:46.000000 pytiqs-1.0.2/README.md
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-10 04:14:57.590169 pytiqs-1.0.2/pytiqs/
+-rw-r--r--   0 nitin      (501) staff       (20)      172 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/__init__.py
+-rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/__version__.py
+-rw-r--r--   0 nitin      (501) staff       (20)    17733 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/connect.py
+-rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/constants.py
+-rw-r--r--   0 nitin      (501) staff       (20)      555 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/exceptions.py
+-rw-r--r--   0 nitin      (501) staff       (20)    19225 2024-04-10 04:14:30.000000 pytiqs-1.0.2/pytiqs/sockets.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-10 04:14:57.591284 pytiqs-1.0.2/pytiqs.egg-info/
+-rw-r--r--   0 nitin      (501) staff       (20)      522 2024-04-10 04:14:57.000000 pytiqs-1.0.2/pytiqs.egg-info/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)      295 2024-04-10 04:14:57.000000 pytiqs-1.0.2/pytiqs.egg-info/SOURCES.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-10 04:14:57.000000 pytiqs-1.0.2/pytiqs.egg-info/dependency_links.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      145 2024-04-10 04:14:57.000000 pytiqs-1.0.2/pytiqs.egg-info/requires.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        7 2024-04-10 04:14:57.000000 pytiqs-1.0.2/pytiqs.egg-info/top_level.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      290 2024-04-10 04:14:57.592073 pytiqs-1.0.2/setup.cfg
+-rw-r--r--   0 nitin      (501) staff       (20)     1192 2024-04-10 04:14:30.000000 pytiqs-1.0.2/setup.py
```

### Comparing `pytiqs-1.0.1/setup.py` & `pytiqs-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict
 
 from setuptools import setup, find_packages
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 about = {}  # type: Dict[str, str]
 
-with open(os.path.join(current_dir, "tiqs", "__version__.py"), "r", encoding="utf-8") as f:
+with open(os.path.join(current_dir, "pytiqs", "__version__.py"), "r", encoding="utf-8") as f:
     exec(f.read(), about)
 
 with io.open('README.md', 'rt', encoding='utf8') as f:
     readme = f.read()
 
 
 setup(
@@ -23,17 +23,21 @@
     long_description=readme,
     long_description_content_type='text/markdown',
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     download_url=about["__download_url__"],
     license=about["__license__"],
-    packages=["tiqs"],
+    packages=["pytiqs"],
     install_requires=[
+        "service_identity>=18.1.0",
         "requests>=2.18.4",
         "python-dateutil>=2.6.1",
-        "six>=1.11.0"
+        "six>=1.11.0",
+        "pyOpenSSL>=17.5.0",
+        "python-dateutil>=2.6.1",
+        "autobahn[twisted]==19.11.2"
     ],
     tests_require=["pytest", "responses", "pytest-cov", "mock", "flake8"],
     test_suite="tests",
     setup_requires=["pytest-runner"]
 )
```

### Comparing `pytiqs-1.0.1/tiqs/connect.py` & `pytiqs-1.0.2/pytiqs/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import logging
 import traceback
 
 import dateutil.parser
 import requests
 import urllib3
 import hashlib
-import tiqs.exceptions as ex
+import pytiqs.exceptions as ex
 
-import tiqs.constants as constants
-from tiqs.constants import Variety, Exchange, ProductType, TransactionType, OrderType, Retention
+import pytiqs.constants as constants
+from pytiqs.constants import Variety, Exchange, ProductType, TransactionType, OrderType, Retention
 
 from typing import Dict, Any, Optional, List, Union
 from six import StringIO, PY2
-from tiqs.__version__ import __version__, __title__
+from pytiqs.__version__ import __version__, __title__
 
 log = logging.getLogger(__name__)
 
 
 class Tiqs(object):
     _default_timeout = 5  # type: int
     _token = None
@@ -65,14 +65,17 @@
             if self.debug:
                 log.debug("token received from generate_session: " + resp["token"])
             self.set_token(resp["token"])
 
     def set_token(self, value: str) -> None:
         self._token = value
 
+    def get_token(self) -> str:
+        return self._token or ""
+
     def invalidate_session(self) -> None:
         self._token = None
 
     def get_instruments(self) -> Any:
         return self._parse_instrument(self._get(self._routes.ALL_INSTRUMENTS))
 
     def user_details(self) -> Dict[str, Any]:
```

### Comparing `pytiqs-1.0.1/tiqs/constants.py` & `pytiqs-1.0.2/pytiqs/constants.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.1/tiqs/exceptions.py` & `pytiqs-1.0.2/pytiqs/exceptions.py`

 * *Files identical despite different names*

