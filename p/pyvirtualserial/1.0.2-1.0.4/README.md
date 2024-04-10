# Comparing `tmp/pyvirtualserial-1.0.2.tar.gz` & `tmp/pyvirtualserial-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvirtualserial-1.0.2.tar", last modified: Sun Mar 10 03:11:34 2024, max compression
+gzip compressed data, was "pyvirtualserial-1.0.4.tar", last modified: Wed Apr 10 18:07:12 2024, max compression
```

## Comparing `pyvirtualserial-1.0.2.tar` & `pyvirtualserial-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.504169 pyvirtualserial-1.0.2/
--rw-rw-rw-   0        0        0      626 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/.coveragerc
--rw-rw-rw-   0        0        0      620 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/.gitignore
--rw-rw-rw-   0        0        0      557 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/.readthedocs.yml
--rw-rw-rw-   0        0        0       85 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0       82 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14271 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1102 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3182 2024-03-10 03:11:34.504169 pyvirtualserial-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.480114 pyvirtualserial-1.0.2/docs/
--rw-rw-rw-   0        0        0     1183 2024-03-10 01:05:44.000000 pyvirtualserial-1.0.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.481114 pyvirtualserial-1.0.2/docs/_static/
--rw-rw-rw-   0        0        0       19 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/changelog.rst
--rw-rw-rw-   0        0        0    10136 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/contributing.rst
--rw-rw-rw-   0        0        0     1473 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/docs/index.rst
--rw-rw-rw-   0        0        0       74 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/license.rst
--rw-rw-rw-   0        0        0       41 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/docs/readme.rst
--rw-rw-rw-   0        0        0      509 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/docs/requirements.txt
--rw-rw-rw-   0        0        0      355 2024-03-10 02:33:30.000000 pyvirtualserial-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       57 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/requirements.in
--rw-rw-rw-   0        0        0      411 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0     1381 2024-03-10 03:11:34.509173 pyvirtualserial-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-03-10 02:33:35.000000 pyvirtualserial-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.457423 pyvirtualserial-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.482113 pyvirtualserial-1.0.2/src/pyvirtualserial/
--rw-rw-rw-   0        0        0     2487 2024-03-10 02:40:54.000000 pyvirtualserial-1.0.2/src/pyvirtualserial/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.500661 pyvirtualserial-1.0.2/src/pyvirtualserial/bases/
--rw-rw-rw-   0        0        0     1730 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/src/pyvirtualserial/bases/linux_virtual_serial.py
--rw-rw-rw-   0        0        0     2403 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/src/pyvirtualserial/bases/window_virtual_serial.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.501661 pyvirtualserial-1.0.2/src/pyvirtualserial/utils/
--rw-rw-rw-   0        0        0      480 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/src/pyvirtualserial/utils/context_managers.py
--rw-rw-rw-   0        0        0     2558 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/src/pyvirtualserial/virtual_serial.py
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.502662 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/
--rw-rw-rw-   0        0        0     3182 2024-03-10 03:11:34.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2024-03-10 03:11:34.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 03:11:34.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-10 02:36:48.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      102 2024-03-10 03:11:34.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-10 03:11:34.000000 pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-10 03:11:34.502662 pyvirtualserial-1.0.2/tests/
--rw-rw-rw-   0        0        0       86 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.2/tests/conftest.py
--rw-rw-rw-   0        0        0     2944 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.2/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.817884 pyvirtualserial-1.0.4/
+-rw-rw-rw-   0        0        0      626 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.coveragerc
+-rw-rw-rw-   0        0        0      620 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0      557 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/.readthedocs.yml
+-rw-rw-rw-   0        0        0       85 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0       82 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14271 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1102 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3182 2024-04-10 18:07:12.817884 pyvirtualserial-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.804741 pyvirtualserial-1.0.4/docs/
+-rw-rw-rw-   0        0        0     1183 2024-03-10 01:05:44.000000 pyvirtualserial-1.0.4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.804741 pyvirtualserial-1.0.4/docs/_static/
+-rw-rw-rw-   0        0        0       19 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0       43 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10136 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1473 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/license.rst
+-rw-rw-rw-   0        0        0       41 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/docs/readme.rst
+-rw-rw-rw-   0        0        0      509 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/docs/requirements.txt
+-rw-rw-rw-   0        0        0      355 2024-03-10 02:33:30.000000 pyvirtualserial-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       57 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/requirements.in
+-rw-rw-rw-   0        0        0      411 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0     1381 2024-04-10 18:07:12.818884 pyvirtualserial-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-03-10 02:33:35.000000 pyvirtualserial-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.781946 pyvirtualserial-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.805742 pyvirtualserial-1.0.4/src/pyvirtualserial/
+-rw-rw-rw-   0        0        0      851 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.814829 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/
+-rw-rw-rw-   0        0        0     3137 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/linux_virtual_serial.py
+-rw-rw-rw-   0        0        0     4096 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/bases/window_virtual_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.815828 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/
+-rw-rw-rw-   0        0        0     1489 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/com0com.py
+-rw-rw-rw-   0        0        0      480 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/utils/context_managers.py
+-rw-rw-rw-   0        0        0     1759 2024-04-10 18:03:25.000000 pyvirtualserial-1.0.4/src/pyvirtualserial/virtual_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.816885 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/
+-rw-rw-rw-   0        0        0     3182 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-10 18:07:12.000000 pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 18:07:12.815828 pyvirtualserial-1.0.4/tests/
+-rw-rw-rw-   0        0        0       86 2024-03-10 02:25:56.000000 pyvirtualserial-1.0.4/tests/conftest.py
+-rw-rw-rw-   0        0        0     2944 2024-02-29 19:28:26.000000 pyvirtualserial-1.0.4/tox.ini
```

### Comparing `pyvirtualserial-1.0.2/.coveragerc` & `pyvirtualserial-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/.gitignore` & `pyvirtualserial-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/.readthedocs.yml` & `pyvirtualserial-1.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/CONTRIBUTING.rst` & `pyvirtualserial-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/LICENSE.txt` & `pyvirtualserial-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/PKG-INFO` & `pyvirtualserial-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvirtualserial
-Version: 1.0.2
+Version: 1.0.4
 Summary: Library to create virtual serial ports on Windows and Linux.
 Home-page: https://github.com/byrondelgithub/PyVirtualSerial
 Author: byrondelgithub
 Author-email: rhurtado5c@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/byrondelgithub/PyVirtualSerial
```

### Comparing `pyvirtualserial-1.0.2/README.rst` & `pyvirtualserial-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/docs/Makefile` & `pyvirtualserial-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/docs/conf.py` & `pyvirtualserial-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/docs/index.rst` & `pyvirtualserial-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/setup.cfg` & `pyvirtualserial-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/setup.py` & `pyvirtualserial-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyvirtualserial-1.0.2/src/pyvirtualserial/virtual_serial.py` & `pyvirtualserial-1.0.4/src/pyvirtualserial/virtual_serial.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from loguru import logger
-from pyvirtualserial import OS_NAME
+import os
 
 __author__ = "byrondelgithub"
 __copyright__ = "byrondelgithub"
 __license__ = "MIT"
 
-if OS_NAME == "nt":
+if os.name == "nt":
     from pyvirtualserial.bases.window_virtual_serial import (
         WindowsBaseVirtualSerial as BaseVirtualSerial,
     )
 else:
     from pyvirtualserial.bases.linux_virtual_serial import (
         LinuxBaseVirtualSerial as BaseVirtualSerial,
     )
@@ -25,52 +25,25 @@
     You can communicate with the slave serial using ``write``, ``read``, ``readline``, ``readline_CR`` and ``readlines``.
 
     Please check ``WindowsBaseVirtualSerial`` and ``LinuxBaseVirtualSerial`` for more information
     on how It works.
     """
 
     def __init__(
-        self, port: int = 10000, baudrate: int = 9600, timeout: int = 5
+        self, port: int = 4000, baudrate: int = 9600, timeout: int = 5
     ) -> None:
         """
         At the moment you initialize this class the pair of serial ports will be created.
 
         Args:
             port (int, optional): Number of the serial port COM{port} (Only for windows). Defaults to 10000.
             baudrate (int, optional): Baudrate of the communication (Only for windows). Defaults to 9600.
             timeout (int, optional): Time before the Serial sends a ``TimeoutException`` when reading (Only for windows). Defaults to 5.
         """
-        super().__init__(port, baudrate, timeout)
+        super().__init__(port, baudrate)
+        self._timeout = timeout
 
     def write(self, bytes: bytes):
         logger.debug(f"Writing {bytes}")
         self._writer.write(bytes)
         self._writer.flush()
 
-    def read(self, bytes: int = 1) -> bytes:
-        b = self._reader.read(bytes)
-        logger.debug(f"Reading {b}")
-        return b
-
-    def readline(self) -> bytes:
-        line = self._reader.readline()
-        logger.debug(f"Reading line {line}")
-        return line
-
-    def readline_CR(self) -> list[bytes]:
-        eol = b"\r"
-        leneol = len(eol)
-        line = b""
-        while True:
-            c = self._reader.read(1)
-            if c:
-                line += c
-                if line[-leneol:] == eol:
-                    break
-            else:
-                break
-        return bytes(line)
-
-    def readlines(self) -> list[bytes]:
-        lines = self._reader.readlines()
-        logger.debug(f"Reading lines {lines}")
-        return lines
```

### Comparing `pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/PKG-INFO` & `pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvirtualserial
-Version: 1.0.2
+Version: 1.0.4
 Summary: Library to create virtual serial ports on Windows and Linux.
 Home-page: https://github.com/byrondelgithub/PyVirtualSerial
 Author: byrondelgithub
 Author-email: rhurtado5c@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/byrondelgithub/PyVirtualSerial
```

### Comparing `pyvirtualserial-1.0.2/src/pyvirtualserial.egg-info/SOURCES.txt` & `pyvirtualserial-1.0.4/src/pyvirtualserial.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 src/pyvirtualserial.egg-info/SOURCES.txt
 src/pyvirtualserial.egg-info/dependency_links.txt
 src/pyvirtualserial.egg-info/not-zip-safe
 src/pyvirtualserial.egg-info/requires.txt
 src/pyvirtualserial.egg-info/top_level.txt
 src/pyvirtualserial/bases/linux_virtual_serial.py
 src/pyvirtualserial/bases/window_virtual_serial.py
+src/pyvirtualserial/utils/com0com.py
 src/pyvirtualserial/utils/context_managers.py
 tests/conftest.py
```

### Comparing `pyvirtualserial-1.0.2/tox.ini` & `pyvirtualserial-1.0.4/tox.ini`

 * *Files identical despite different names*

