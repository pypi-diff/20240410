# Comparing `tmp/ping3-4.0.7.tar.gz` & `tmp/ping3-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping3-4.0.7.tar", last modified: Fri Apr  5 13:01:54 2024, max compression
+gzip compressed data, was "ping3-4.0.8.tar", last modified: Wed Apr 10 16:54:28 2024, max compression
```

## Comparing `ping3-4.0.7.tar` & `ping3-4.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.582811 ping3-4.0.7/
--rw-rw-rw-   0        0        0     1092 2021-02-26 10:16:53.000000 ping3-4.0.7/LICENSE
--rw-rw-rw-   0        0        0    13111 2024-04-05 13:01:54.581804 ping3-4.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10819 2022-12-15 11:51:14.000000 ping3-4.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.528111 ping3-4.0.7/ping3/
--rw-rw-rw-   0        0        0    18068 2024-04-05 12:54:31.000000 ping3-4.0.7/ping3/__init__.py
--rw-rw-rw-   0        0        0       83 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/__main__.py
--rw-rw-rw-   0        0        0     2587 2024-04-05 12:54:52.000000 ping3-4.0.7/ping3/command_line.py
--rw-rw-rw-   0        0        0     1342 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/enums.py
--rw-rw-rw-   0        0        0     1786 2022-05-22 03:29:23.000000 ping3-4.0.7/ping3/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.579741 ping3-4.0.7/ping3.egg-info/
--rw-rw-rw-   0        0        0    13111 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-05 13:01:54.000000 ping3-4.0.7/ping3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1357 2024-04-03 13:46:03.000000 ping3-4.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 13:01:54.582811 ping3-4.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 13:01:54.578740 ping3-4.0.7/tests/
--rw-rw-rw-   0        0        0      721 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_benchmark.py
--rw-rw-rw-   0        0        0     4537 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_command_line.py
--rw-rw-rw-   0        0        0      819 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_multi.py
--rw-rw-rw-   0        0        0     8253 2022-05-22 05:28:04.000000 ping3-4.0.7/tests/test_ping3.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:54:28.392575 ping3-4.0.8/
+-rw-rw-rw-   0        0        0     1092 2021-02-26 10:16:53.000000 ping3-4.0.8/LICENSE
+-rw-rw-rw-   0        0        0    13111 2024-04-10 16:54:28.390578 ping3-4.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10819 2022-12-15 11:51:14.000000 ping3-4.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 16:54:28.364279 ping3-4.0.8/ping3/
+-rw-rw-rw-   0        0        0    18068 2024-04-10 16:48:06.000000 ping3-4.0.8/ping3/__init__.py
+-rw-rw-rw-   0        0        0       83 2022-05-22 03:29:23.000000 ping3-4.0.8/ping3/__main__.py
+-rw-rw-rw-   0        0        0     2590 2024-04-10 16:47:56.000000 ping3-4.0.8/ping3/command_line.py
+-rw-rw-rw-   0        0        0     1342 2022-05-22 03:29:23.000000 ping3-4.0.8/ping3/enums.py
+-rw-rw-rw-   0        0        0     1786 2022-05-22 03:29:23.000000 ping3-4.0.8/ping3/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-10 16:54:28.389578 ping3-4.0.8/ping3.egg-info/
+-rw-rw-rw-   0        0        0    13111 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 16:54:28.000000 ping3-4.0.8/ping3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2024-04-03 13:46:03.000000 ping3-4.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 16:54:28.392575 ping3-4.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 16:54:28.388575 ping3-4.0.8/tests/
+-rw-rw-rw-   0        0        0      721 2022-05-22 05:28:04.000000 ping3-4.0.8/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     4537 2024-04-10 16:51:28.000000 ping3-4.0.8/tests/test_command_line.py
+-rw-rw-rw-   0        0        0      819 2022-05-22 05:28:04.000000 ping3-4.0.8/tests/test_multi.py
+-rw-rw-rw-   0        0        0     8253 2022-05-22 05:28:04.000000 ping3-4.0.8/tests/test_ping3.py
```

### Comparing `ping3-4.0.7/LICENSE` & `ping3-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/PKG-INFO` & `ping3-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ping3
-Version: 4.0.7
+Version: 4.0.8
 Summary: A pure python3 version of ICMP ping implementation using raw socket.
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ping3-4.0.7/README.md` & `ping3-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/ping3/__init__.py` & `ping3-4.0.8/ping3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import functools
 import errno
 
 from . import errors
 from .enums import ICMP_DEFAULT_CODE, IcmpType, IcmpTimeExceededCode, IcmpDestinationUnreachableCode
 
-__version__ = "4.0.7"
+__version__ = "4.0.8"
 DEBUG = False  # DEBUG: Show debug info for developers. (default False)
 EXCEPTIONS = False  # EXCEPTIONS: Raise exception when delay is not available.
 LOGGER = None  # LOGGER: Record logs into console or file. Logger object should have .debug() method.
 
 IP_HEADER_FORMAT = "!BBHHHBBHII"
 ICMP_HEADER_FORMAT = "!BBHHH"  # According to netinet/ip_icmp.h. !=network byte order(big-endian), B=unsigned char, H=unsigned short
 ICMP_TIME_FORMAT = "!d"  # d=double
```

### Comparing `ping3-4.0.7/ping3/command_line.py` & `ping3-4.0.8/ping3/command_line.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 
 import ping3
 
 
-def main(assigned_args: list = []) -> None:
+def main(assigned_args = None) -> None:
     """
     Parse and execute the call from command-line.
 
     Args:
-        assigned_args (list[str]): List of strings to parse. The default is taken from sys.argv.
+        assigned_args (list[str] | None): List of strings to parse. The default is taken from sys.argv.
 
     Returns:
         Formatted ping results printed.
     """
     parser = argparse.ArgumentParser(prog="ping3", description="A pure python3 version of ICMP ping implementation using raw socket.", epilog="!!Note: ICMP messages can only be sent from processes running as root.")
     parser.add_argument("-v", "--version", action="version", version=ping3.__version__)
     parser.add_argument(dest="dest_addr", metavar="DEST_ADDR", nargs="*", default=("example.com", "8.8.8.8"), help="The destination address, can be an IP address or a domain name. Ex. 192.168.1.1/example.com.")
```

### Comparing `ping3-4.0.7/ping3/enums.py` & `ping3-4.0.8/ping3/enums.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/ping3/errors.py` & `ping3-4.0.8/ping3/errors.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/ping3.egg-info/PKG-INFO` & `ping3-4.0.8/ping3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ping3
-Version: 4.0.7
+Version: 4.0.8
 Summary: A pure python3 version of ICMP ping implementation using raw socket.
 Author-email: Kyan <kai@kyan001.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ping3-4.0.7/pyproject.toml` & `ping3-4.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/tests/test_benchmark.py` & `ping3-4.0.8/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/tests/test_command_line.py` & `ping3-4.0.8/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/tests/test_multi.py` & `ping3-4.0.8/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `ping3-4.0.7/tests/test_ping3.py` & `ping3-4.0.8/tests/test_ping3.py`

 * *Files identical despite different names*

