# Comparing `tmp/spydir-0.1.0.tar.gz` & `tmp/spydir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spydir-0.1.0.tar", last modified: Mon Apr  8 23:57:29 2024, max compression
+gzip compressed data, was "spydir-0.1.1.tar", last modified: Wed Apr 10 00:46:38 2024, max compression
```

## Comparing `spydir-0.1.0.tar` & `spydir-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-08 23:57:29.625131 spydir-0.1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       46 2024-04-08 23:07:45.000000 spydir-0.1.0/.gitignore
--rw-r--r--   0 sergey    (1000) sergey    (1000)      122 2024-04-08 22:52:28.000000 spydir-0.1.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      806 2024-04-08 23:57:29.625131 spydir-0.1.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      222 2024-04-08 23:14:36.000000 spydir-0.1.0/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2024-04-08 22:56:10.000000 spydir-0.1.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-08 23:57:29.625131 spydir-0.1.0/setup.cfg
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-08 23:57:29.625131 spydir-0.1.0/spydir.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      806 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      235 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        7 2024-04-08 23:57:29.000000 spydir-0.1.0/spydir.egg-info/top_level.txt
--rwxr-xr-x   0 sergey    (1000) sergey    (1000)     8473 2024-04-08 23:15:02.000000 spydir-0.1.0/spydir.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-10 00:46:38.156617 spydir-0.1.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       70 2024-04-10 00:17:14.000000 spydir-0.1.1/.gitignore
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      122 2024-04-08 22:52:28.000000 spydir-0.1.1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      810 2024-04-10 00:46:38.156617 spydir-0.1.1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      226 2024-04-10 00:17:37.000000 spydir-0.1.1/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      663 2024-04-08 22:56:10.000000 spydir-0.1.1/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2024-04-10 00:46:38.156617 spydir-0.1.1/setup.cfg
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-10 00:46:38.156617 spydir-0.1.1/spydir.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      810 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      235 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       45 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       44 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        7 2024-04-10 00:46:38.000000 spydir-0.1.1/spydir.egg-info/top_level.txt
+-rwxr-xr-x   0 sergey    (1000) sergey    (1000)     8967 2024-04-10 00:25:34.000000 spydir-0.1.1/spydir.py
```

### Comparing `spydir-0.1.0/PKG-INFO` & `spydir-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydir
-Version: 0.1.0
+Version: 0.1.1
 Author: Sergey M
 License: FUCK LICENSE
         
         Author attribution is required. Commercial use permitted. If you don't like Russians then go fuck yourself.
         
 Project-URL: Repository, https://github.com/s3rgeym/spydir.git
 Classifier: Topic :: Internet
@@ -22,13 +22,13 @@
 
 Directory listing scanner to search for downloadable archives and other files
 
 ```bash
 # you can use pip instead
 pipx install spydir
 
-# scan list of urls
-spydir -i urls.txt -o found.txt
+# scan list of hosts
+spydir -i hosts.txt -o results.txt
 
 # see help
 spydir -h
 ```
```

### Comparing `spydir-0.1.0/pyproject.toml` & `spydir-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spydir-0.1.0/spydir.egg-info/PKG-INFO` & `spydir-0.1.1/spydir.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spydir
-Version: 0.1.0
+Version: 0.1.1
 Author: Sergey M
 License: FUCK LICENSE
         
         Author attribution is required. Commercial use permitted. If you don't like Russians then go fuck yourself.
         
 Project-URL: Repository, https://github.com/s3rgeym/spydir.git
 Classifier: Topic :: Internet
@@ -22,13 +22,13 @@
 
 Directory listing scanner to search for downloadable archives and other files
 
 ```bash
 # you can use pip instead
 pipx install spydir
 
-# scan list of urls
-spydir -i urls.txt -o found.txt
+# scan list of hosts
+spydir -i hosts.txt -o results.txt
 
 # see help
 spydir -h
 ```
```

### Comparing `spydir-0.1.0/spydir.py` & `spydir-0.1.1/spydir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 # pylint: disable=C,R,W
 """Directery Listing Scanner"""
 from __future__ import annotations
 
 import argparse
+import dataclasses
 import itertools
 import logging
 import multiprocessing as mp
 import re
 import sys
 import threading
 from dataclasses import dataclass
 from typing import Sequence, TextIO, Type
 from urllib.parse import urljoin
 
 import requests
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __author__ = "Sergey M"
 
 logger = mp.get_logger()
 
 requests.packages.urllib3.disable_warnings()
 
@@ -52,17 +53,18 @@
         logging.DEBUG: ANSI.BLUE,
         logging.INFO: ANSI.GREEN,
         logging.WARNING: ANSI.YELLOW,
         logging.ERROR: ANSI.RED,
         logging.CRITICAL: ANSI.BRIGHT_RED,
     }
 
-    _fmt = logging.Formatter(
-        "[%(levelname).1s] %(processName)-16s - %(message)s"
-    )
+    # _fmt = logging.Formatter(
+    #     "[%(levelname).1s] %(processName)-16s - %(message)s"
+    # )
+    _fmt = logging.Formatter("[%(levelname).1s] %(message)s")
 
     def format(self, record: logging.LogRecord) -> str:
         message = self._fmt.format(record)
         return f"{self._log_colors[record.levelno]}{message}{ANSI.RESET}"
 
 
 class Worker(mp.Process):
@@ -239,75 +241,87 @@
     "/logs/",
     "/log/",
 )
 
 
 @dataclass
 class SpyDir:
-    output: TextIO
-    workers_num: int
-    timeout: float
+    output: TextIO = sys.stdout
+    workers_num: int | None = None
+    timeout: float | None = None
+    user_agent: str | None = None
+
+    def __post_init__(self) -> None:
+        self.workers_num = self.workers_num or (mp.cpu_count() * 2 - 1)
 
     class NameSpace(argparse.Namespace):
         input: TextIO
         output: TextIO
         workers_num: int
         debug: bool
         timeout: float
+        user_agent: str | None
 
     @classmethod
     def parse_args(
         cls: Type[SpyDir],
         argv: Sequence[str] | None,
     ) -> tuple[argparse.ArgumentParser, NameSpace]:
         parser = argparse.ArgumentParser(description=__doc__)
         parser.add_argument(
             "-i", "--input", type=argparse.FileType(), default="-"
         )
         parser.add_argument(
             "-o", "--output", type=argparse.FileType("w+"), default="-"
         )
-        parser.add_argument(
-            "-w", "--workers-num", type=int, default=mp.cpu_count() - 1
-        )
+        parser.add_argument("-w", "--workers-num", type=int)
         parser.add_argument("-d", "--debug", action="store_true", default=False)
         parser.add_argument("-t", "--timeout", type=float, default=10.0)
+        parser.add_argument("-ua", "--user-agent")
         return parser, parser.parse_args(args=argv, namespace=cls.NameSpace())
 
     @classmethod
-    def cli(cls: Type[SpyDir], argv: Sequence[str] | None = None) -> None:
+    def cli(cls: Type[SpyDir], argv: Sequence[str] | None = None) -> int | None:
         parser, args = cls.parse_args(argv)
 
         cls.configure_logger(args)
 
         obj = cls(
             output=args.output,
             workers_num=args.workers_num,
             timeout=args.timeout,
+            user_agent=args.user_agent,
         )
 
         sites = map(normalize_url, filter(None, args.input))
 
         try:
             return obj.run(sites)
         except KeyboardInterrupt:
             logger.warning("bye")
+            return 1
 
     def run(self, urls: list[str]) -> None:
         in_q = mp.JoinableQueue()
         out_q = mp.Queue()
         seen = mp.Manager().dict()
 
         for url, path in itertools.product(urls, KNOWN_PATHES):
             in_q.put_nowait(urljoin(url, path))
 
         logger.info("Directory scanning started")
 
         workers = [
-            Worker(in_q=in_q, out_q=out_q, seen=seen, timeout=self.timeout)
+            Worker(
+                in_q=in_q,
+                out_q=out_q,
+                seen=seen,
+                timeout=self.timeout,
+                user_agent=self.user_agent,
+            )
             for _ in range(self.workers_num)
         ]
 
         out_t = OutputThread(queue=out_q, stream=self.output)
         out_t.start()
 
         in_q.join()
```

