# Comparing `tmp/plotlyshare-1.0.7.tar.gz` & `tmp/plotlyshare-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\dead\plotlyshare\plotlyshare\dist\1.0.7\.tmp-29liswij\plotlyshare-1.0.7.tar", last modified: Thu Jan 25 18:32:54 2024, max compression
+gzip compressed data, was "plotlyshare-1.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `plotlyshare-1.0.7.tar` & `plotlyshare-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 18:32:54.723227 plotlyshare-1.0.7/
--rw-rw-rw-   0        0        0     1840 2024-01-25 18:32:54.723227 plotlyshare-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2024-01-25 18:31:35.000000 plotlyshare-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 18:32:54.695228 plotlyshare-1.0.7/plotlyshare/
--rw-rw-rw-   0        0        0      716 2024-01-25 14:05:33.000000 plotlyshare-1.0.7/plotlyshare/__init__.py
--rw-rw-rw-   0        0        0     2520 2024-01-25 14:03:25.000000 plotlyshare-1.0.7/plotlyshare/__main__.py
--rw-rw-rw-   0        0        0     4132 2024-01-25 12:55:51.000000 plotlyshare-1.0.7/plotlyshare/custom_plotly_renderer.py
-drwxrwxrwx   0        0        0        0 2024-01-25 18:32:54.723227 plotlyshare-1.0.7/plotlyshare.egg-info/
--rw-rw-rw-   0        0        0     1840 2024-01-25 18:32:54.000000 plotlyshare-1.0.7/plotlyshare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-01-25 18:32:54.000000 plotlyshare-1.0.7/plotlyshare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 18:32:54.000000 plotlyshare-1.0.7/plotlyshare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-01-25 18:32:54.000000 plotlyshare-1.0.7/plotlyshare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-25 18:32:54.000000 plotlyshare-1.0.7/plotlyshare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      753 2024-01-25 18:32:37.000000 plotlyshare-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-25 18:32:54.723227 plotlyshare-1.0.7/setup.cfg
+-rw-r--r--   0        0        0     1262 2024-04-07 06:24:50.555594 plotlyshare-1.0.8/README.md
+-rw-r--r--   0        0        0      716 2024-01-25 14:05:33.949412 plotlyshare-1.0.8/plotlyshare/__init__.py
+-rw-r--r--   0        0        0     2952 2024-04-10 07:32:05.473490 plotlyshare-1.0.8/plotlyshare/__main__.py
+-rw-r--r--   0        0        0      206 2024-04-10 07:36:38.133527 plotlyshare-1.0.8/plotlyshare/config.json
+-rw-r--r--   0        0        0     4132 2024-01-25 12:55:51.235790 plotlyshare-1.0.8/plotlyshare/custom_plotly_renderer.py
+-rw-r--r--   0        0        0      754 2024-04-10 07:35:56.969936 plotlyshare-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 plotlyshare-1.0.8/PKG-INFO
```

### Comparing `plotlyshare-1.0.7/README.md` & `plotlyshare-1.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # `plotlyshare`
+[![Downloads](https://static.pepy.tech/badge/plotlyshare)](https://pepy.tech/project/plotlyshare)
 
 The purpose of this package is to provide a seamless way to share interactive `plotly` plots, providing a similar experience to google docs/etc. 
 
 This requires a free account on deta space: https://deta.space, which is essentially a *personal* cloud computer *at no cost*.
 
 The idea is to preserve the interactivity and responsiveness of `plotly` plots with the ease of **link-based sharing** and without all the hassle of sending an html file, or worse, a static image/document.
```

### Comparing `plotlyshare-1.0.7/plotlyshare/__init__.py` & `plotlyshare-1.0.8/plotlyshare/__init__.py`

 * *Files identical despite different names*

### Comparing `plotlyshare-1.0.7/plotlyshare/__main__.py` & `plotlyshare-1.0.8/plotlyshare/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os, sys, json
 import time
 from rich import console, pretty
 from plotlyshare.custom_plotly_renderer import test_connection
 
-allowed_commands = ['setup']
+allowed_commands = ['setup', 'test']
 assert len(sys.argv) == 2, f'Please give only one argument out of {allowed_commands}'
 command = sys.argv[1]
 assert command in allowed_commands, f'Given command not in {allowed_commands}'
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 config_file_path = f'{dir_path}/config.json'
 
@@ -62,7 +62,18 @@
 
 			with open(config_file_path, 'w') as f:
 				json.dump(config, f, indent=4)
 
 			c.print('[bold green]Setup completed!🚀[/bold green]')
 		else:
 			c.print('[bold red]Setup failed:[/bold red]\n'+display)
+elif command == 'test':
+	if old_config['setup_done']:
+		c = console.Console()
+		with c.status('Testing credentials...', spinner='shark'):
+			passed, display = test_connection(old_config['DETA_APP_URL'], old_config['DETA_PROJECT_KEY'])
+
+			if passed:
+				old_config['setup_done'] = True
+				c.print('[bold green]It works!🚀[/bold green]')
+			else:
+				c.print('[bold red]There was an error:[/bold red]\n'+display)
```

### Comparing `plotlyshare-1.0.7/plotlyshare/custom_plotly_renderer.py` & `plotlyshare-1.0.8/plotlyshare/custom_plotly_renderer.py`

 * *Files identical despite different names*

### Comparing `plotlyshare-1.0.7/pyproject.toml` & `plotlyshare-1.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61"]
-build-backend = "setuptools.build_meta"
+build-backend = "flit_core.buildapi"
+requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "plotlyshare"
-version = "1.0.7"
+version = "1.0.8"
 authors = [{name="plutonium239", email="plutonium.239.811@gmail.com"}]
 description = "Link-based sharing of `plotly` plots with a private web app"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

