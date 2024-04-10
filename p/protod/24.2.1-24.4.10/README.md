# Comparing `tmp/protod-24.2.1.tar.gz` & `tmp/protod-24.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protod-24.2.1.tar", last modified: Thu Feb  1 14:00:04 2024, max compression
+gzip compressed data, was "protod-24.4.10.tar", last modified: Wed Apr 10 11:11:24 2024, max compression
```

## Comparing `protod-24.2.1.tar` & `protod-24.4.10.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:04.355461 protod-24.2.1/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-11-08 06:18:17.000000 protod-24.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      226 2024-02-01 14:00:04.355461 protod-24.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2024-02-01 13:54:33.000000 protod-24.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:04.355461 protod-24.2.1/protod/
--rw-r--r--   0 root         (0) root         (0)       94 2024-02-01 13:36:15.000000 protod-24.2.1/protod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4216 2024-02-01 12:00:36.000000 protod-24.2.1/protod/decode.py
--rw-r--r--   0 root         (0) root         (0)      424 2024-01-29 17:52:18.000000 protod-24.2.1/protod/definition.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-02-01 11:55:10.000000 protod-24.2.1/protod/field.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-11-13 15:47:29.000000 protod-24.2.1/protod/main.py
--rw-r--r--   0 root         (0) root         (0)     4596 2024-02-01 12:57:22.000000 protod-24.2.1/protod/renderer.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-02-01 11:57:23.000000 protod-24.2.1/protod/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:00:04.355461 protod-24.2.1/protod.egg-info/
--rw-r--r--   0 root         (0) root         (0)      226 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-01 14:00:04.000000 protod-24.2.1/protod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 14:00:04.355461 protod-24.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-01 13:59:06.000000 protod-24.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:11:24.109353 protod-24.4.10/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-11-08 06:18:17.000000 protod-24.4.10/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-10 11:11:24.109353 protod-24.4.10/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-04-10 11:05:09.000000 protod-24.4.10/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:11:24.108353 protod-24.4.10/protod/
+-rw-r--r--   0 root         (0) root         (0)       94 2024-02-01 13:36:15.000000 protod-24.4.10/protod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2024-04-10 11:03:56.000000 protod-24.4.10/protod/decode.py
+-rw-r--r--   0 root         (0) root         (0)      424 2024-01-29 17:52:18.000000 protod-24.4.10/protod/definition.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-02-01 11:55:10.000000 protod-24.4.10/protod/field.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-11-13 15:47:29.000000 protod-24.4.10/protod/main.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2024-02-01 12:57:22.000000 protod-24.4.10/protod/renderer.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-02-01 11:57:23.000000 protod-24.4.10/protod/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:11:24.108353 protod-24.4.10/protod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-10 11:11:24.000000 protod-24.4.10/protod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 11:11:24.109353 protod-24.4.10/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-10 11:10:42.000000 protod-24.4.10/setup.py
```

### Comparing `protod-24.2.1/LICENSE` & `protod-24.4.10/LICENSE`

 * *Files identical despite different names*

### Comparing `protod-24.2.1/README.md` & `protod-24.4.10/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 - `protod --file ~/pb.bin`
 - `protod` for help
   
 ## library protod
 It uses different `Renderer` to generate different output:
 - For console:
 ```python
-print(protod.dump(proto)) # ConsoleRenderer is used by default
+print(protod.dump(proto_bytes)) # ConsoleRenderer is used by default
 ```
-- For html:
-```python
-html_tag = protod.dump(proto, protod.HtmlRenderer())
-# send the html_tag to client browser
- $('#div').text(html_tag)
-```
-- For other format:   
-This [example](https://github.com/aj3423/protod/blob/master/example/mitmproxy_proto_view.py) demonstrates how to implemente custom `Renderer`, it's an addon for [mitmproxy](https://github.com/mitmproxy/mitmproxy/)
 
-   ![image](https://github.com/aj3423/protod/assets/4710875/aca8a5b1-4c05-4cc4-8346-f3b91a6ca8d7)
+There are [examples](https://github.com/aj3423/protod/blob/master/example) demonstrate how to write custom `Renderer`s:
+- json
+
+ ![image](https://github.com/aj3423/protod/assets/4710875/2c3bddb2-06e7-44b4-844f-eaaff6a26d6f)
+
+- html
+
+ ![image](https://github.com/aj3423/protod/assets/4710875/39583ae3-1d77-4c22-b4a0-ed9d12bd8305)
+
+- Mitmproxy addon:
+ 
+ ![image](https://github.com/aj3423/protod/assets/4710875/aca8a5b1-4c05-4cc4-8346-f3b91a6ca8d7)
```

### Comparing `protod-24.2.1/protod/decode.py` & `protod-24.4.10/protod/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,20 @@
             ret.append(repeated)
 
     return ret
 
 
 def dump(
     data: bytes,
-    renderer=ConsoleRenderer(),
+    renderer=None,
     str_decoder=detect_multi_charset,
 ):
+    if renderer == None:
+        renderer = ConsoleRenderer()
+
     view = memoryview(data)
 
     fields = decode_all_fields(str_decoder=str_decoder, parent=None, view=view)
 
     for ch in fields:
         ch.render(renderer)
```

### Comparing `protod-24.2.1/protod/field.py` & `protod-24.4.10/protod/field.py`

 * *Files identical despite different names*

### Comparing `protod-24.2.1/protod/main.py` & `protod-24.4.10/protod/main.py`

 * *Files identical despite different names*

### Comparing `protod-24.2.1/protod/renderer.py` & `protod-24.4.10/protod/renderer.py`

 * *Files identical despite different names*

### Comparing `protod-24.2.1/protod/util.py` & `protod-24.4.10/protod/util.py`

 * *Files identical despite different names*

