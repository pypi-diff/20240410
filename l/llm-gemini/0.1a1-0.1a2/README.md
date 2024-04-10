# Comparing `tmp/llm-gemini-0.1a1.tar.gz` & `tmp/llm-gemini-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-gemini-0.1a1.tar", last modified: Wed Mar 27 18:41:26 2024, max compression
+gzip compressed data, was "llm-gemini-0.1a2.tar", last modified: Wed Apr 10 03:02:41 2024, max compression
```

## Comparing `llm-gemini-0.1a1.tar` & `llm-gemini-0.1a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:41:26.681644 llm-gemini-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 18:41:15.000000 llm-gemini-0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-27 18:41:26.681644 llm-gemini-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-27 18:41:15.000000 llm-gemini-0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:41:26.681644 llm-gemini-0.1a1/llm_gemini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 18:41:26.000000 llm-gemini-0.1a1/llm_gemini.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-27 18:41:15.000000 llm-gemini-0.1a1/llm_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-27 18:41:15.000000 llm-gemini-0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 18:41:26.681644 llm-gemini-0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:41:26.681644 llm-gemini-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 18:41:15.000000 llm-gemini-0.1a1/tests/test_gemini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:02:41.732829 llm-gemini-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 03:02:31.000000 llm-gemini-0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 03:02:41.732829 llm-gemini-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 03:02:31.000000 llm-gemini-0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:02:41.732829 llm-gemini-0.1a2/llm_gemini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 03:02:41.000000 llm-gemini-0.1a2/llm_gemini.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-10 03:02:31.000000 llm-gemini-0.1a2/llm_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 03:02:31.000000 llm-gemini-0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:02:41.732829 llm-gemini-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:02:41.732829 llm-gemini-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 03:02:31.000000 llm-gemini-0.1a2/tests/test_gemini.py
```

### Comparing `llm-gemini-0.1a1/LICENSE` & `llm-gemini-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-gemini-0.1a1/PKG-INFO` & `llm-gemini-0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gemini
-Version: 0.1a1
+Version: 0.1a2
 Summary: LLM plugin to access Google's Gemini family of models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-gemini
 Project-URL: Changelog, https://github.com/simonw/llm-gemini/releases
 Project-URL: Issues, https://github.com/simonw/llm-gemini/issues
 Project-URL: CI, https://github.com/simonw/llm-gemini/actions
```

### Comparing `llm-gemini-0.1a1/README.md` & `llm-gemini-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `llm-gemini-0.1a1/llm_gemini.egg-info/PKG-INFO` & `llm-gemini-0.1a2/llm_gemini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-gemini
-Version: 0.1a1
+Version: 0.1a2
 Summary: LLM plugin to access Google's Gemini family of models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-gemini
 Project-URL: Changelog, https://github.com/simonw/llm-gemini/releases
 Project-URL: Issues, https://github.com/simonw/llm-gemini/issues
 Project-URL: CI, https://github.com/simonw/llm-gemini/actions
```

### Comparing `llm-gemini-0.1a1/llm_gemini.py` & `llm-gemini-0.1a2/llm_gemini.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,22 +52,25 @@
         key = llm.get_key("", "gemini", "LLM_GEMINI_KEY")
         url = "https://generativelanguage.googleapis.com/v1beta/models/{}:streamGenerateContent?".format(
             self.model_id
         ) + urllib.parse.urlencode(
             {"key": key}
         )
         gathered = []
+        body = {
+            "contents": self.build_messages(prompt, conversation),
+            "safetySettings": SAFETY_SETTINGS,
+        }
+        if prompt.system:
+            body["systemInstruction"] = {"parts": [{"text": prompt.system}]}
         with httpx.stream(
             "POST",
             url,
             timeout=None,
-            json={
-                "contents": self.build_messages(prompt, conversation),
-                "safetySettings": SAFETY_SETTINGS,
-            },
+            json=body,
         ) as http_response:
             events = ijson.sendable_list()
             coro = ijson.items_coro(events, "item")
             for chunk in http_response.iter_bytes():
                 coro.send(chunk)
                 if events:
                     event = events[0]
```

### Comparing `llm-gemini-0.1a1/pyproject.toml` & `llm-gemini-0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-gemini"
-version = "0.1a1"
+version = "0.1a2"
 description = "LLM plugin to access Google's Gemini family of models"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

