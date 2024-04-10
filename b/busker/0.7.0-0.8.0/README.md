# Comparing `tmp/busker-0.7.0.tar.gz` & `tmp/busker-0.8.0.tar.gz`

## Comparing `busker-0.7.0.tar` & `busker-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 busker-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.7.0/busker/__init__.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 busker-0.7.0/busker/executive.py
--rw-r--r--   0        0        0    20767 2020-02-02 00:00:00.000000 busker-0.7.0/busker/gui.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.7.0/busker/history.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 busker-0.7.0/busker/main.py
--rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 busker-0.7.0/busker/runner.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 busker-0.7.0/busker/scraper.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 busker-0.7.0/busker/tagger.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 busker-0.7.0/busker/types.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 busker-0.7.0/busker/visitor.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 busker-0.7.0/busker/zone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_executive.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_history.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_runner.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_scraper.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_tagger.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_zone.py
--rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.7.0/LICENSE
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 busker-0.7.0/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 busker-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    42031 2020-02-02 00:00:00.000000 busker-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 busker-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.8.0/busker/__init__.py
+-rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 busker-0.8.0/busker/actions.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 busker-0.8.0/busker/executive.py
+-rw-r--r--   0        0        0    20767 2020-02-02 00:00:00.000000 busker-0.8.0/busker/gui.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.8.0/busker/history.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 busker-0.8.0/busker/main.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 busker-0.8.0/busker/runner.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 busker-0.8.0/busker/scraper.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 busker-0.8.0/busker/tagger.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 busker-0.8.0/busker/types.py
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 busker-0.8.0/busker/visitor.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 busker-0.8.0/busker/zone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/__init__.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_executive.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_history.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_runner.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_scraper.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_tagger.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.8.0/busker/test/test_zone.py
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 busker-0.8.0/README.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 busker-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    42031 2020-02-02 00:00:00.000000 busker-0.8.0/PKG-INFO
```

### Comparing `busker-0.7.0/CHANGELOG.md` & `busker-0.8.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+0.8.0
+-----
+
+* Refactored several classes and modules.
+* Better counting by Witness.
+
 0.7.0
 -----
 
 * Interactive tab fully working.
 * Hosting workflow robust.
 * Tested on Windows (Python 3.12).
```

### Comparing `busker-0.7.0/busker/executive.py` & `busker-0.8.0/busker/executive.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/gui.py` & `busker-0.8.0/busker/gui.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/history.py` & `busker-0.8.0/busker/history.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/main.py` & `busker-0.8.0/busker/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,33 +40,36 @@
 
 
 def main(args):
     history = SharedHistory(log_name="busker")
     history.log(f"Busker {busker.__version__}")
 
     if args.with_automation:
-        witness = Counter()
+        counter = Counter()
 
         n = 0
         while n < args.number:
             n += 1
             history.log(f"Run: {n:03d}")
             visitor = Visitor(args.url)
-            while visitor.tactics:
-                tactic = visitor.tactics.popleft()
-                node = visitor(tactic)
+            while visitor.actions:
+                action = visitor.actions.popleft()
+                node = visitor(action, timeout=10)
                 if node:
                     history.log(f"Page: {node.title}")
 
-            witness[visitor.turns] += 1
+            counter[visitor.turns] += 1
 
         history.log(f"{visitor.turns} done.")
 
-        print(*visitor.toml_lines(visitor.history), sep="\n")
-        print({k: witness[k] for k in sorted(witness.keys())})
+        # print(*visitor.toml_lines(visitor.history), sep="\n")
+        print(visitor.witness.words)
+        print(f"{visitor.witness.duration=}")
+        print({k: counter[k] for k in sorted(counter.keys())})
+        visitor.witness.reset()
         return 0
 
     try:
         text = args.config.read_text()
         config = tomllib.loads(text)
     except FileNotFoundError:
         config = {}
```

### Comparing `busker-0.7.0/busker/runner.py` & `busker-0.8.0/busker/runner.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/scraper.py` & `busker-0.8.0/busker/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
 from busker.history import SharedHistory
 
 
 Node = namedtuple(
     "Node", [
         "ts", "hash",
-        "tactic", "params",
+        "action", "params",
         "url",
         "title", "links", "blocks", "media",
-        "options", "actions",
+        "options", "forms",
         "text"
     ],
     defaults=[
         None, None,
         None,
         None, None, None, None,
         None, None,
@@ -124,29 +124,29 @@
                 inputs=inputs,
                 button=getattr(form_node.find(".//button[@type='submit']"), "text", None),
             ))
 
     def get(self, url=None, **kwargs) -> Node:
         self.log(f"GET {url=}")
         client = LocalClient()
-        with client.open(url) as response:
+        with client.open(url, **kwargs) as response:
             reply = response.read()
 
         return Node(
             ts=datetime.datetime.now(datetime.timezone.utc),
             hash=hashlib.blake2b(reply).hexdigest(),
             url=response.url,
             text = reply.decode("utf8"),
         )
 
     def post(self, url, data=None, **kwargs) -> Node:
         params = urllib.parse.urlencode(data).encode("utf8")
         self.log(f"POST {url=} {params=}")
         client = LocalClient()
-        with client.open(url, params) as response:
+        with client.open(url, data=params, **kwargs) as response:
             reply = response.read()
 
         return Node(
             ts=datetime.datetime.now(datetime.timezone.utc),
             hash=hashlib.blake2b(reply).hexdigest(),
             url=response.url,
             text = reply.decode("utf8"),
```

### Comparing `busker-0.7.0/busker/tagger.py` & `busker-0.8.0/busker/tagger.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/types.py` & `busker-0.8.0/busker/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 import enum
 import multiprocessing
 import multiprocessing.managers
 import multiprocessing.pool
 import pathlib
 
 
+Choice = namedtuple("Choice", ["form", "input", "value"], defaults=[None, None])
+
 Completion = namedtuple("Completion", ["runner", "exenv", "data"], defaults=[None])
 
 
 class Host(enum.Enum):
 
     IPV4_LOOPBACK = "127.0.0.1"
     IPV4_NET_HOST = "0.0.0.0"
```

### Comparing `busker-0.7.0/busker/zone.py` & `busker-0.8.0/busker/zone.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_executive.py` & `busker-0.8.0/busker/test/test_executive.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_history.py` & `busker-0.8.0/busker/test/test_history.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_runner.py` & `busker-0.8.0/busker/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_scraper.py` & `busker-0.8.0/busker/test/test_scraper.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_tagger.py` & `busker-0.8.0/busker/test/test_tagger.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/busker/test/test_zone.py` & `busker-0.8.0/busker/test/test_zone.py`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/LICENSE` & `busker-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/README.md` & `busker-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `busker-0.7.0/pyproject.toml` & `busker-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # For possible options see https://peps.python.org/pep-0621/
  
 [project]
 name = "busker"
-version = "0.7.0"
+version = "0.8.0"
 description = "A utility for testing Balladeer projects."
 readme = "README.md"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 keywords = ["interactive fiction", "balladeer"]
 authors = [
     {name = "D E Haynes", email = "tundish@gigeconomy.org.uk"}
```

### Comparing `busker-0.7.0/PKG-INFO` & `busker-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: busker
-Version: 0.7.0
+Version: 0.8.0
 Summary: A utility for testing Balladeer projects.
 Author-email: D E Haynes <tundish@gigeconomy.org.uk>
 Maintainer-email: Tundish <tundish@gigeconomy.org.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

