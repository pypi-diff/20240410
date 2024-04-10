# Comparing `tmp/confluence.md-0.3.2.tar.gz` & `tmp/confluence.md-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence.md-0.3.2.tar", last modified: Sat Apr  6 19:04:51 2024, max compression
+gzip compressed data, was "confluence.md-0.4.2.tar", last modified: Wed Apr 10 20:02:35 2024, max compression
```

## Comparing `confluence.md-0.3.2.tar` & `confluence.md-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 19:04:51.125210 confluence.md-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-06 19:04:47.000000 confluence.md-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 19:04:47.000000 confluence.md-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-06 19:04:51.125210 confluence.md-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.121210 confluence.md-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/confluence.md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 19:04:51.000000 confluence.md-0.3.2/src/confluence.md.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/md2cf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5608 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:51.125210 confluence.md-0.3.2/src/md2cf/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/confluencemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 19:04:47.000000 confluence.md-0.3.2/src/md2cf/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:35.168466 confluence.md-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-10 20:02:35.168466 confluence.md-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-10 20:02:07.000000 confluence.md-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 20:02:07.000000 confluence.md-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-10 20:02:35.168466 confluence.md-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:35.164466 confluence.md-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:35.168466 confluence.md-0.4.2/src/confluence.md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 20:02:35.000000 confluence.md-0.4.2/src/confluence.md.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:35.168466 confluence.md-0.4.2/src/md2cf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5798 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:35.168466 confluence.md-0.4.2/src/md2cf/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/utils/confluencemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-10 20:02:07.000000 confluence.md-0.4.2/src/md2cf/utils/md2html.py
```

### Comparing `confluence.md-0.3.2/PKG-INFO` & `confluence.md-0.4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,75 @@
-Metadata-Version: 2.1
-Name: confluence.md
-Version: 0.3.2
-Summary: Markdown to Confluence - upload any .md files to your Confluence cloud page
-Home-page: https://github.com/szn/confluence.md
-Download-URL: 
-Author: Szymon Nieradka
-License: MIT
-Project-URL: Bug Tracker, https://github.com/szn/confluence.md/issues
-Keywords: markdown,confluence,md,atlassian
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators
-Classifier: Natural Language :: English
-Classifier: Topic :: Documentation
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: importlib; python_version == "3.7"
-Requires-Dist: atlassian-python-api>=3.41.1
-Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: markdown2>=2.4.10
-Requires-Dist: termcolor>=2.3.0
-
 # confluence.md
 
 Push markdown files straight to a Confluence page.
 
 ## What it does?
 
 `confluence.md` allows you to push any markdown file to Confluence. You can create
 a new page (under given parent) or update an existing one.
 
 ## How to install?
 
 It's as easy as:
 
-```
+```sh
 $ pip install confluence.md
+
+# If the above doesn't work, your `pip` command points to different
+# python than installation than `python` command. If so, run:
+$ python -m pip install confluence.md
 ```
 
-## How to use it?
+## How to use it in command-line?
 
 Markdown to Confluence
 
 Example workflow:
 
-### 1. Create a new page under `--parent_id`:
-```
-$ confluence.md --user user@name.net --token 9a8dsadsh --url https://your-domain.atlassian.net \
-        create --file README.md --parent_id 182371 --title "new title" --add_meta
-```
+#### 1. Create page
 
-### 2. The page is created and the file is decorated with metadata:
+Create a new page under `--parent_id`:
+```sh
+$ confluence.md --user user@name.net \             # Atlassian username
+        --token 9a8dsadsh \                        # API token or --password
+        --url https://your-domain.atlassian.net \  # Confluence instance URL
+        create \                                   # create or update
+        --file README.md \                         # markdown file
+        --parent_id 182371 \                       # parent page
+        --title "new title"                        # title for a new page
+        --add_meta                                 # adds meta to source.md file
 ```
+
+#### 2. Verify markdown
+
+The page is created and the file is decorated with metadata:
+
+```sh
 $ head -n 3 markdown.md
 ---
 confluence-url: https://your-domain.atlassian.net/wiki/spaces/SP/pages/18237182/new+title
 ---
 ```
 
-### 3. Performing an update does not require providing `--page_id` and `--url`:
-```
+#### 3. Update page
+
+Performing an update does not require providing `--page_id` and `--url`:
+
+```sh
 $ confluence.md --user user@name.net --token 9a8dsadsh update --file README.md
 ```
 
 Doing an update with `--page_id` and `--url` is still possible.
 
 Consider adding useful `--add_info` option.
 
 To create Atlassian API Token go to [api-tokens](https://id.atlassian.com/manage-profile/security/api-tokens).
 
+## Command line arguments
+
 **Actions:**
 
 - `update`    		Updates page content based on given `page_id` or metadata in Markdown file
 - `create`    		Creates new page under given `parent_id`
 
 **positional arguments:**
 
@@ -95,25 +78,50 @@
 **optional arguments:**
 
 - `-h`, `--help`            show this help message and exit
 - `--file FILE`             input markdown file to process
 - `--add_meta`              adds metadata to .md file for easy editing
 - `--add_info`              adds info panel **automatic content** do not edit on top of the page
 - `--add_label` `ADD_LABEL` adds label to page
+- `--convert_jira`          convert all Jira links to issue snippets (either short [KEY-ID] format or full URL)
+                            **note**: this options works only in Cloud instances with [Smart Issue for Confluence](https://marketplace.atlassian.com/plugins/smart-issue-view-for-confluence) installed
 - `-v`, `--verbose`         verbose mode
 - `-q`, `--quiet`           quiet mode
 
 **required auth parameters:**
 
 - `-u` `USER`, `--user` `USER`    Atlassian username/email
 - `-t` `TOKEN`, `--token` `TOKEN` Atlassian API token
+- `-p` `PWD`, `--password` `PWD`  Atlassian password (used in on-prem instances)
 - `-l` `URL`, `--url` `URL`       Atlassian instance URL
+- `-n`, `--no_verify_ssl`         don't verify SSL cert (useful in on-prem instances)
 
 **create page parameters:**
 
 - `--parent_id` `PARENT_ID` define parent page id while creating a new page
 - `--title` `TITLE`         define page title while creating a new page
 - `--overwrite`             force overwrite if page with this title already exists
 
 **update page arguments:**
 
--  `--page_id` `PAGE_ID`     define (or override) page id while updating a page
+- `--page_id` `PAGE_ID`     define (or override) page id while updating a page
+
+## How to use it in a Python script?
+
+ConfluenceMD wasn't designed to be used this way, but it's fairly simple to embed
+it in a Python script. See this example:
+
+```python
+from md2cf.utils.confluencemd import ConfluenceMD
+
+conf_md = ConfluenceMD(username=user,
+                       md_file=md_file,
+                       token=token,
+                       url=url,
+                       convert_jira=convert_jira)
+
+# create new page under parent_id
+new_page_id = conf_md.create_new("parent_id", "title")
+
+# update existing page with given page_id
+page_id = conf_md.update_existing("page_id")
+```
```

### Comparing `confluence.md-0.3.2/setup.cfg` & `confluence.md-0.4.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = confluence.md
-version = 0.3.2
+version = 0.4.2
 author = Szymon Nieradka
 description = Markdown to Confluence - upload any .md files to your Confluence cloud page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/szn/confluence.md
 project_urls = 
 	Bug Tracker = https://github.com/szn/confluence.md/issues
@@ -14,15 +14,15 @@
 home_page = https://github.com/szn/confluence.md
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
 	Intended Audience :: System Administrators
 	Natural Language :: English
 	Topic :: Documentation
```

### Comparing `confluence.md-0.3.2/src/confluence.md.egg-info/PKG-INFO` & `confluence.md-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: confluence.md
-Version: 0.3.2
+Version: 0.4.2
 Summary: Markdown to Confluence - upload any .md files to your Confluence cloud page
 Home-page: https://github.com/szn/confluence.md
 Download-URL: 
 Author: Szymon Nieradka
 License: MIT
 Project-URL: Bug Tracker, https://github.com/szn/confluence.md/issues
 Keywords: markdown,confluence,md,atlassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: Topic :: Documentation
@@ -44,49 +44,69 @@
 `confluence.md` allows you to push any markdown file to Confluence. You can create
 a new page (under given parent) or update an existing one.
 
 ## How to install?
 
 It's as easy as:
 
-```
+```sh
 $ pip install confluence.md
+
+# If the above doesn't work, your `pip` command points to different
+# python than installation than `python` command. If so, run:
+$ python -m pip install confluence.md
 ```
 
-## How to use it?
+## How to use it in command-line?
 
 Markdown to Confluence
 
 Example workflow:
 
-### 1. Create a new page under `--parent_id`:
-```
-$ confluence.md --user user@name.net --token 9a8dsadsh --url https://your-domain.atlassian.net \
-        create --file README.md --parent_id 182371 --title "new title" --add_meta
-```
+#### 1. Create page
 
-### 2. The page is created and the file is decorated with metadata:
+Create a new page under `--parent_id`:
+```sh
+$ confluence.md --user user@name.net \             # Atlassian username
+        --token 9a8dsadsh \                        # API token or --password
+        --url https://your-domain.atlassian.net \  # Confluence instance URL
+        create \                                   # create or update
+        --file README.md \                         # markdown file
+        --parent_id 182371 \                       # parent page
+        --title "new title"                        # title for a new page
+        --add_meta                                 # adds meta to source.md file
 ```
+
+#### 2. Verify markdown
+
+The page is created and the file is decorated with metadata:
+
+```sh
 $ head -n 3 markdown.md
 ---
 confluence-url: https://your-domain.atlassian.net/wiki/spaces/SP/pages/18237182/new+title
 ---
 ```
 
-### 3. Performing an update does not require providing `--page_id` and `--url`:
-```
+#### 3. Update page
+
+Performing an update does not require providing `--page_id` and `--url`:
+
+```sh
 $ confluence.md --user user@name.net --token 9a8dsadsh update --file README.md
 ```
 
 Doing an update with `--page_id` and `--url` is still possible.
 
 Consider adding useful `--add_info` option.
 
 To create Atlassian API Token go to [api-tokens](https://id.atlassian.com/manage-profile/security/api-tokens).
 
+## Command line arguments
+
 **Actions:**
 
 - `update`    		Updates page content based on given `page_id` or metadata in Markdown file
 - `create`    		Creates new page under given `parent_id`
 
 **positional arguments:**
 
@@ -95,25 +115,50 @@
 **optional arguments:**
 
 - `-h`, `--help`            show this help message and exit
 - `--file FILE`             input markdown file to process
 - `--add_meta`              adds metadata to .md file for easy editing
 - `--add_info`              adds info panel **automatic content** do not edit on top of the page
 - `--add_label` `ADD_LABEL` adds label to page
+- `--convert_jira`          convert all Jira links to issue snippets (either short [KEY-ID] format or full URL)
+                            **note**: this options works only in Cloud instances with [Smart Issue for Confluence](https://marketplace.atlassian.com/plugins/smart-issue-view-for-confluence) installed
 - `-v`, `--verbose`         verbose mode
 - `-q`, `--quiet`           quiet mode
 
 **required auth parameters:**
 
 - `-u` `USER`, `--user` `USER`    Atlassian username/email
 - `-t` `TOKEN`, `--token` `TOKEN` Atlassian API token
+- `-p` `PWD`, `--password` `PWD`  Atlassian password (used in on-prem instances)
 - `-l` `URL`, `--url` `URL`       Atlassian instance URL
+- `-n`, `--no_verify_ssl`         don't verify SSL cert (useful in on-prem instances)
 
 **create page parameters:**
 
 - `--parent_id` `PARENT_ID` define parent page id while creating a new page
 - `--title` `TITLE`         define page title while creating a new page
 - `--overwrite`             force overwrite if page with this title already exists
 
 **update page arguments:**
 
--  `--page_id` `PAGE_ID`     define (or override) page id while updating a page
+- `--page_id` `PAGE_ID`     define (or override) page id while updating a page
+
+## How to use it in a Python script?
+
+ConfluenceMD wasn't designed to be used this way, but it's fairly simple to embed
+it in a Python script. See this example:
+
+```python
+from md2cf.utils.confluencemd import ConfluenceMD
+
+conf_md = ConfluenceMD(username=user,
+                       md_file=md_file,
+                       token=token,
+                       url=url,
+                       convert_jira=convert_jira)
+
+# create new page under parent_id
+new_page_id = conf_md.create_new("parent_id", "title")
+
+# update existing page with given page_id
+page_id = conf_md.update_existing("page_id")
+```
```

### Comparing `confluence.md-0.3.2/src/md2cf/main.py` & `confluence.md-0.4.2/src/md2cf/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 #!/usr/bin/env python3
+"""
+confluence.md
+Push markdown files straight to a Confluence page.
+"""
+
 import sys
 import argparse
 from argparse import RawTextHelpFormatter
 
 from .utils.log import logger, init_logger, headline
 from .utils.confluencemd import ConfluenceMD
 
 ACTIONS = {}
 
 def register_action(function):
+    """Register command line action function decorator"""
     ACTIONS[function.__name__] = function.__doc__
     def wrapper(args):
         headline(function.__doc__)
         function(args)
-        headline("End " + function.__name__, True)
+        headline("End " + function.__name__)
     return wrapper
 
 def init_confluence(args):
     return ConfluenceMD(username=args.user,
                         token=args.token,
                         password=args.password,
                         md_file=args.file.name,
@@ -36,15 +42,15 @@
 
 @register_action
 def create(args):
     """Creates new page under given parent_id"""
     assert args.url, ("No --url parameter is provided, gave up")
 
     confluence = init_confluence(args)
-    confluence.create_page(args.parent_id, args.title, args.overwrite)
+    confluence.create_new(args.parent_id, args.title, args.overwrite)
 
 def main():
     """Markdown to Confluence
 
 Example workflow:
 
 1/ Create a new page under --parent_id:
@@ -121,15 +127,16 @@
     parser.add_argument("--add_meta", action="store_true",
             help="adds metadata to .md file for easy editing")
     parser.add_argument("--add_info", action="store_true",
             help="adds info panel **automatic content** do not edit on top of the page")
     parser.add_argument("--add_label", action="store",
             help="adds label to page")
     parser.add_argument("--convert_jira", action="store_true",
-            help="convert all Jira links to issue snippets (either short [KEY-ID] format or full URL)")
+            help="convert all Jira links to issue snippets "
+                 "(either short [KEY-ID] format or full URL)")
 
     parser.add_argument("-v", "--verbose", action="store_true",
             help="verbose mode")
     parser.add_argument("-q", "--quiet", action="store_true",
             help="quiet mode")
     parser.add_argument("action", help="Action to run", choices=ACTIONS)
 
@@ -138,14 +145,15 @@
         sys.exit(1)
 
     args = parser.parse_args()
     init_logger(args)
 
     try:
         globals()[args.action](args)
+    # pylint: disable=broad-exception-caught
     except (RuntimeError, AssertionError, Exception) as error:
         logger.error(error)
         if args.verbose:
             raise error
         quit(-1)
```

### Comparing `confluence.md-0.3.2/src/md2cf/utils/confluencemd.py` & `confluence.md-0.4.2/src/md2cf/utils/confluencemd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,135 +1,97 @@
-import re
+"""
+Confluence to Markdown utility
+"""
 import os
-
-from typing import Any, List, Tuple, Optional, Dict
+import re
+from  urllib import parse
+from typing import List, Tuple
+import requests
 
 import atlassian
-import markdown2
 
 from .log import logger
-from pprint import pprint
+from .md2html import md_to_html
 
-CF_URL = re.compile(r"(?P<host>https?://[^/]+)/.*/(?P<page_id>\d+)")
-IMAGE_PATTERN = re.compile(r"\!\[(?P<alt>.*)\]\((?P<path>[^:)]+)\)")
-ISSUE_PATTERN = re.compile(r"\[(?P<key>\w[\w\d]*-\d+)\]")
-ISSUE_PATTERN_URL = re.compile(r"(?P<domain>https:\/\/\w+\.atlassian\.net)\/browse\/(?P<key>\w[\w\d]*-\d+)")
+ISSUE_PATTERN_KEY = re.compile(r"\[(?P<key>\w[\w\d]*-\d+)\]")
+ISSUE_PATTERN_URL = re.compile(r"(?P<domain>https:\/\/\w+\.atlassian\.net)"
+                               r"\/browse\/(?P<key>\w[\w\d]*-\d+)")
 
 class ConfluenceMD(atlassian.Confluence):
+    """Confluence to Markdown utility class"""
+
     def __init__(
         self,
         username: str,
         md_file: str,
         token: str = '',
         password: str = '',
         url: str = None,
         verify_ssl: bool = True,
         add_meta: bool = False,
         add_info_panel: bool = False,
         add_label: str = None,
         convert_jira: bool = False
     ) -> None:
-        
+        jira_url = parse.urljoin(url, '/')
+        conf_url = parse.urljoin(url, '/wiki/')
         super().__init__(
-            url=url,
+            url=conf_url,
             username=username,
             password=(password or token),
             verify_ssl=verify_ssl,
             cloud=bool(token),
             token=token,
         )
-        self.jira = atlassian.Jira(
-            url=url,
-            username=username,
-            password=(password or token),
-            verify_ssl=verify_ssl,
-            cloud=bool(token),
-            token=token
-        )
+
+        self.license = self.__init_jira(
+                url=jira_url,
+                username=username,
+                password=(password or token),
+                verify_ssl=verify_ssl,
+                token=token
+            )
         self.md_file = md_file
         self.add_meta = add_meta
         self.add_info_panel = add_info_panel
         self.add_label = add_label
         self.md_file_dir = os.path.dirname(md_file)
         self.convert_jira = convert_jira
 
-    def rewrite_issues(self, html: str) -> str:
-        if not self.convert_jira:
-            return html
-        logger.debug("Replacing [ISSUE-KEY] with html links")
-        issues = []
-        for issue in ISSUE_PATTERN.finditer(html):
-            issues.append((issue.group(), issue.group("key")))
-        for issue in ISSUE_PATTERN_URL.finditer(html):
-            if self.url.startswith(issue.group("domain")):
-                issues.append((issue.group(), issue.group("key")))
-            else:
-                logger.info("Ignoring %s - domain mismatch (%s != %s)", issue.group(), issue.group("domain"), self.url)
-
-        for (replace, key) in issues:
-            logger.debug(f"  - [{key}] with html link")
-            (summary, status, issuetypeurl) = self.get_jira_issue(key)
-            if summary:
-                html = html.replace(replace,
-                    f"<a href=\"{self.url}/browse/{key}\"><ac:image><ri:url ri:value=\"{issuetypeurl}\" /></ac:image> {key}: {summary} [{status}]</a>")
-        return html
-
-    def get_jira_issue(self, key: str) -> tuple:
+    def __init_jira(self,
+                    url: str,
+                    username: str,
+                    password: str,
+                    verify_ssl: bool,
+                    token: str) -> bool:
+        self.jira = atlassian.Jira(
+                url=url,
+                username=username,
+                password=(password or token),
+                verify_ssl=verify_ssl,
+                cloud=bool(token),
+                token=token
+            )
         try:
-            issue = self.jira.issue(key)
-            summary = issue['fields']['summary']
-            status = issue['fields']['status']['name']
-            issuetypeurl = issue['fields']['issuetype']['iconUrl']
-            return (summary, status, issuetypeurl)
-        except (RuntimeError, AssertionError, Exception) as error:
-            logger.info("Unable to convert %s to Jira link: %s", key, error)
-            return (None, None, None)
+            uri = parse.urljoin(url, 'wiki/rest/atlassian-connect/1/addons/smart-issue-view-for-confluence')
+            res = requests.get(uri, auth=(username, password or token), timeout=30)
+            license_obj = res.json()
+            if res.status_code != 200:
+                return
+            return bool (license_obj["license"]["active"])
+        # pylint: disable=broad-exception-caught
+        except (RuntimeError, AssertionError, Exception):
+            return False
 
-    def rewrite_images(
-        self, html: str, images: List[Tuple[str, str]]
-    ) -> str:
-        """Replaces <img> html tags with Confluence specific <ac:image> and uploads
-           images as attachements"""
-        for (alt, path) in images:
-            rel_path = os.path.join(self.md_file_dir, path)
-            if not os.path.isfile(rel_path):
-                assert os.path.isfile(path), f"File `{path}` does not exist"
-                logger.warning("file `%s` does not exist, using file relative to current dir `%s`", rel_path, path)
-                rel_path = path
-
-            old = f'<img src="{path}" alt="{alt}" />'
-            new = f'<ac:image> <ri:attachment ri:filename="{os.path.basename(rel_path)}" /> </ac:image>'
-            if html.find(old) != -1:
-                logger.debug("replace image tag `%s` with `%s`", old, new)
-                html = html.replace(old, new)
-            else:
-                logger.warning("image tag `%s` not found in html", old)
-        return html
-
-    def attach_images(
-            self, page_id: str, images: List[Tuple[str, str]]
-    ) -> None:
-        """Replaces <img> html tags with Confluence specific <ac:image> and uploads
-           images as attachements"""
-        for (alt, path) in images:
-            rel_path = os.path.join(self.md_file_dir, path)
-            if not os.path.isfile(rel_path):
-                assert os.path.isfile(path), f"File `{path}` does not exist"
-                logger.warning("file `%s` does not exist, using file relative to current dir `%s`", rel_path, path)
-                rel_path = path
-
-            logger.debug("register image file `%s`", rel_path)
-            self.attach_file(filename=rel_path, page_id=page_id)
-
-    def update_existing(self, page_id: str = None) -> None:
+    def update_existing(self, page_id: str = None) -> int:
         """Updates an existing page by given page_id"""
         logger.debug("Updating page `%s` based on `md_file` file", page_id)
-        html, page_id_from_meta, url, _has_images = self.md_file_to_html(page_id)
-        images = self.get_images_from_file()
-        self.attach_images(page_id, images)
+        html, page_id_from_meta, url, images = md_to_html(self.md_file, self.add_info_panel)
+        html = self.__rewrite_issues(html)
+        self.__attach_images(page_id, images)
 
         if page_id is None:
             logger.debug("Using `page_id` from `%s` file", self.md_file)
             page_id = page_id_from_meta
 
         assert page_id, (
             f"Can't update page without page_id given either by "
@@ -139,55 +101,57 @@
         if self.url is None:
             logger.debug("Using URL (%s) from `%s` file", url, self.md_file)
             self.url = url
             assert self.url, (
                 f"Can't update page without url given either by "
                 f"`--url` parameter or via `confluence-url` tag in `{self.md_file}` file`"
             )
-            self.init()
 
-        title = self.get_page_title_by_id(page_id)
+        title = self.__get_page_title_by_id(page_id)
 
         logger.debug("Updating page_id `%s` titled `%s`", page_id, title)
         response = self.update_page(
             page_id,
             title,
             html,
             parent_id=None,
             type="page",
             representation="storage",
             minor_edit=True,
         )
 
         if self.add_meta:
-            confluence_url = ConfluenceMD.get_link_from_response(response)
-            self.add_meta_to_file(confluence_url)
+            confluence_url = ConfluenceMD.__get_link_from_response(response)
+            self.__add_meta_to_file(confluence_url)
 
         if self.add_label:
-            self.add_label_to_page(page_id)
+            self.__add_label_to_page(page_id)
+
+        return page_id
 
-    def create_page(self, parent_id: str, title: str, overwrite: bool) -> None:
+    def create_new(self, parent_id: str, title: str, overwrite: bool) -> int:
         """Creates a new page under give parent_id"""
         assert title, "Provide a title for a newly created page"
         assert parent_id, "Provide parent_id for a newly created page"
         space = self.get_page_space(parent_id)
 
         page_id = None
         if self.page_exists(space, title):
             page_id = self.get_page_id(space, title)
             assert overwrite, (
                 f"Page titled `{title}` already exists in "
-                f"the `{space}` space. Use --overwrite to force it."
+                f"the `{space}` space. Use `--overwrite` to force it."
             )
 
-        html, page_id_from_meta, _url, has_images = self.md_file_to_html(page_id)
+        html, page_id_from_meta, _url, images = md_to_html(self.md_file, self.add_info_panel)
+        html = self.__rewrite_issues(html)
         assert not page_id_from_meta or overwrite, (
             f"Metadata pointing to an existing page "
             f"id `{page_id_from_meta}` present in the given markdown file. "
-            f"Use --overwrite to force it."
+            f"Use `--overwrite` to force it."
         )
 
         overwrite_id = page_id if page_id else page_id_from_meta
 
         if overwrite_id:
             logger.debug(
                 "Overwriting existing page `%s` based on `%s` file", title, self.md_file
@@ -209,120 +173,130 @@
                 title,
                 body=html,
                 parent_id=parent_id,
                 type="page",
                 representation="storage",
                 editor="v2",
             )
-            if has_images:
+            if images:
                 logger.debug("Uploading images to newly created page")
-                page_id = ConfluenceMD.get_page_id_from_response(response)
-                images = self.get_images_from_file()
-                self.attach_images(page_id, images)
+                page_id = ConfluenceMD.__get_page_id_from_response(response)
+                self.__attach_images(page_id, images)
 
-        confluence_url = ConfluenceMD.get_link_from_response(response)
+        confluence_url = ConfluenceMD.__get_link_from_response(response)
         logger.debug(
             "%s %s", 'Page overwritten' if overwrite_id else 'New page created', confluence_url
         )
 
-        self.add_meta_to_file(confluence_url)
+        self.__add_meta_to_file(confluence_url)
+
+        page_id = ConfluenceMD.__get_page_id_from_response(response)
+        self.__add_label_to_page(page_id)
+        return page_id
+
+    def __rewrite_issues(self, html):
+        if self.convert_jira:
+            logger.debug("Replacing [ISSUE-KEY] with html links")
+
+        issues = []
+        for issue in ISSUE_PATTERN_KEY.finditer(html):
+            issues.append((issue.group(), issue.group("key")))
+        for issue in ISSUE_PATTERN_URL.finditer(html):
+            if self.url.startswith(issue.group("domain")):
+                issues.append((issue.group(), issue.group("key")))
+            else:
+                if self.convert_jira:
+                    logger.info("Ignoring %s - domain mismatch (%s != %s)",
+                                issue.group(),
+                                issue.group("domain"),
+                                self.url)
+
+        if issues and not self.convert_jira:
+            (replace, key) = issues[0]
+            logger.info("Use `--convert_jira` to replace %i Jira link(s) (such as %s) "
+                        "with issue snippets - KEY: summary [status]",
+                        len(issues), key)
+            return html
+
+        if not self.license and self.convert_jira:
+            logger.warning("To use `--convert_jira` you must have „Smart Issue for Confluence” installed (free for small business)")
+            logger.warning("See: https://marketplace.atlassian.com/plugins/smart-issue-view-for-confluence")
+            return html
+
+        for (replace, key) in issues:
+            logger.debug("  - [%s] with html link", key)
+            (summary, status, issuetypeurl) = self.__get_jira_issue(key)
+            if summary:
+                html = html.replace(replace,
+                    f"<a href=\"{self.url}/browse/{key}\"><ac:image>"
+                    f"<ri:url ri:value=\"{issuetypeurl}\" />"
+                    f"</ac:image> {key}: {summary} [{status}]</a>")
+        return html
+
+    def __get_jira_issue(self, key: str) -> tuple:
+        try:
+            issue = self.jira.issue(key)
+            summary = issue['fields']['summary']
+            status = issue['fields']['status']['name']
+            issuetypeurl = issue['fields']['issuetype']['iconUrl']
+            return (summary, status, issuetypeurl)
+        # pylint: disable=broad-exception-caught
+        except (RuntimeError, AssertionError, Exception) as error:
+            logger.info("Unable to convert %s to Jira link: %s", key, error)
+            return (None, None, None)
+
+    def __attach_images(
+            self, page_id: str, images: List[Tuple[str, str]]
+    ) -> None:
+        """Replaces <img> html tags with Confluence specific <ac:image> and uploads
+           images as attachements"""
+        for (_alt, path) in images:
+            rel_path = os.path.join(self.md_file_dir, path)
+            if not os.path.isfile(rel_path):
+                assert os.path.isfile(path), f"File `{path}` does not exist"
+                logger.warning("File `%s` does not exist, using file relative "
+                               "to current dir `%s`", rel_path, path)
+                rel_path = path
 
-        page_id = ConfluenceMD.get_page_id_from_response(response)
-        self.add_label_to_page(page_id)
+            logger.debug("register image file `%s`", rel_path)
+            self.attach_file(filename=rel_path, page_id=page_id)
 
     @staticmethod
-    def get_link_from_response(response) -> str:
+    def __get_link_from_response(response) -> str:
         """Returns URL to page from Confluence API response"""
         return response["_links"]["base"] + response["_links"]["webui"]
 
     @staticmethod
-    def get_page_id_from_response(response) -> str:
+    def __get_page_id_from_response(response) -> str:
         """Returns page_id from Confluence API response"""
         return response["id"]
 
-    def add_meta_to_file(self, confluence_url: str) -> None:
+    def __add_meta_to_file(self, confluence_url: str) -> None:
         """Decorates markdown file with metadata in comments"""
         if not self.add_meta:
             return
 
-        markdown = ConfluenceMD.get_file_contents(self.md_file)
+        markdown = ConfluenceMD.__get_file_contents(self.md_file)
         markdown = ("---\n" f"confluence-url: {confluence_url}\n" "---\n") + markdown
 
         with open(self.md_file, "w", encoding="utf-8") as stream:
             stream.write(markdown)
 
-    def get_page_title_by_id(self, page_id: str) -> str:
+    def __get_page_title_by_id(self, page_id: str) -> str:
         """Returns page title by given page_id"""
         logger.debug("Getting page title from page id `%s`", page_id)
         page = self.get_page_by_id(page_id)
         assert "title" in page, f"Expected page-object while getting page by id, got {page}"
         return page["title"]
 
     @staticmethod
-    def get_file_contents(file: str) -> str:
+    def __get_file_contents(file: str) -> str:
         """Return file contents"""
         with open(file, "r", encoding="utf-8") as stream:
             return stream.read()
 
-    def md_file_to_html(self, page_id: Optional[str]) -> Tuple[Any, Optional[str], Optional[str], bool]:
-        """Converts given md_file to html"""
 
-        logger.debug("Converting MD to HTML")
-        images = self.get_images_from_file()
-
-        html = markdown2.markdown_path(
-            path=self.md_file,
-            extras=[
-                "metadata",
-                "strike",
-                "tables",
-                "wiki-tables",
-                "code-friendly",
-                "fenced-code-blocks",
-                "footnotes",
-            ],
-        )
-        page_id_from_meta, url = ConfluenceMD.parse_confluence_url(html.metadata)
-        if self.add_info_panel:
-            html = self.get_info_panel() + html
-
-        html = self.rewrite_issues(html)
-        html = self.rewrite_images(html, images)
-        return html, page_id_from_meta, url, len(images) > 0
-
-    @staticmethod
-    def parse_confluence_url(meta: Dict[str, str]) -> Tuple[Optional[str], Optional[str]]:
-        """Parses Confluence page URL and returns page_id and host"""
-        if "confluence-url" not in meta:
-            return (None, None)
-
-        url = meta["confluence-url"]
-
-        logger.debug("Looking for host and page_id in %s url", url)
-        cf_url = CF_URL.search(url)
-        if cf_url:
-            page_id = cf_url.group("page_id")
-            host = cf_url.group("host")
-            logger.debug("  found page_id `%s` and host `%s`", page_id, host)
-            return (page_id, host)
-        logger.debug("  no valid Confluence url found")
-        return (None, None)
-
-    def get_images_from_file(self) -> List:
-        logger.debug("Getting list of images from MD file")
-        content = self.get_file_contents(self.md_file)
-        images = []
-        for image in IMAGE_PATTERN.finditer(content):
-            images.append((image.group("alt"), image.group("path")))
-        return images
-
-    def add_label_to_page(self, page_id: str) -> None:
+    def __add_label_to_page(self, page_id: str) -> None:
         """Selfdescriptive"""
         if not self.add_label:
             return
         self.set_page_label(page_id, self.add_label)
-
-    def get_info_panel(self) -> str:
-        """Returns str with html info page to be placed on a Confluence page if --add_info is added"""
-        return f"""<p><strong>Automatic content</strong> This page was generated automatically from <code>{self.md_file}</code> file.
-        Do not edit it on Confluence.</p><hr />
-        """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `confluence.md-0.3.2/src/md2cf/utils/log.py` & `confluence.md-0.4.2/src/md2cf/utils/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+"""
+confluence.md logging utility
+"""
 import logging
 
 import coloredlogs
 from termcolor import colored
 
 logger = logging.getLogger("net.dirtyagile.confluence.md")
 
 
 def init_logger(args):
+    """Inits logger based on commandline args"""
     coloredlogs.install(
             level='WARN' if args.quiet else ('DEBUG' if args.verbose else 'INFO'),
             logger=logger,
             fmt='%(asctime)s %(programname)s %(message)s',
             programname='>',
             datefmt='%H:%m:%S',
             field_styles= {
@@ -24,14 +28,15 @@
                     'critical': {'bold': True, 'color': 'red'},
                     'debug': {'color': 'white', 'faint': True},
                     'error': {'color': 'red'},
                     'info': {'color': 'white', 'faint': False},
                     'notice': {'color': 'magenta'},
                     'warning': {'color': 'yellow'}})
 
-    logging.getLogger("net.dirtyagile.confluence.md").level = logging.WARN if args.quiet else (logging.DEBUG if args.verbose else logging.INFO)
+    logging.getLogger("net.dirtyagile.confluence.md").level = \
+        logging.WARN if args.quiet else (logging.DEBUG if args.verbose else logging.INFO)
 
 
-def headline(msg, end=False):
+def headline(msg):
+    """Bold headline"""
     logger.info(colored(" {:80}".format(msg), 'blue',
             attrs=['reverse']))
-
```

