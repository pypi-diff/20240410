# Comparing `tmp/pih-web-0.1.tar.gz` & `tmp/pih-web-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-web-0.1.tar", last modified: Mon Feb 26 06:03:02 2024, max compression
+gzip compressed data, was "pih-web-0.11.tar", last modified: Wed Apr 10 02:31:54 2024, max compression
```

## Comparing `pih-web-0.1.tar` & `pih-web-0.11.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:02.077496 pih-web-0.1/
--rw-rw-rw-   0        0        0      248 2024-02-26 06:03:02.796223 pih-web-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:02.108745 pih-web-0.1/WebServerService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.1/WebServerService/__init__.py
--rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.1/WebServerService/__main__.py
--rw-rw-rw-   0        0        0    76961 2024-02-26 06:02:42.000000 pih-web-0.1/WebServerService/const.py
--rw-rw-rw-   0        0        0    36834 2024-02-19 05:55:34.000000 pih-web-0.1/WebServerService/service copy.py
--rw-rw-rw-   0        0        0    39360 2024-02-20 07:05:29.000000 pih-web-0.1/WebServerService/service.py
-drwxrwxrwx   0        0        0        0 2024-02-26 06:03:02.577867 pih-web-0.1/pih_web.egg-info/
--rw-rw-rw-   0        0        0      248 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-02-26 06:03:01.000000 pih-web-0.1/pih_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 06:03:02.796223 pih-web-0.1/setup.cfg
--rw-rw-rw-   0        0        0       96 2024-02-14 00:36:56.000000 pih-web-0.1/web_build.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.388451 pih-web-0.11/
+-rw-rw-rw-   0        0        0      377 2024-04-10 02:31:54.357202 pih-web-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.013465 pih-web-0.11/WebServerService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-web-0.11/WebServerService/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-02-14 00:18:05.000000 pih-web-0.11/WebServerService/__main__.py
+-rw-rw-rw-   0        0        0    76962 2024-04-09 05:06:36.000000 pih-web-0.11/WebServerService/const.py
+-rw-rw-rw-   0        0        0     4960 2024-04-09 05:06:40.000000 pih-web-0.11/WebServerService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:31:54.325954 pih-web-0.11/pih_web.egg-info/
+-rw-rw-rw-   0        0        0      377 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 02:31:53.000000 pih-web-0.11/pih_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:31:54.388451 pih-web-0.11/setup.cfg
```

### Comparing `pih-web-0.1/WebServerService/const.py` & `pih-web-0.11/WebServerService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME: str = "WebServer"
 
 HOST = Hosts.WS255
 
 PACKAGES: tuple[str, ...] = ("fastapi", "uvicorn", "python-multipart", "dicttoxml")
 
-VERSION: str = "0.1"
+VERSION: str = "0.11"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Web Server service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="web",
```

