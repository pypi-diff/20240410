# Comparing `tmp/orji-4.0.0.tar.gz` & `tmp/orji-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orji-4.0.0.tar", last modified: Sun Dec 24 09:11:53 2023, max compression
+gzip compressed data, was "orji-4.2.0.tar", last modified: Tue Apr  9 23:50:49 2024, max compression
```

## Comparing `orji-4.0.0.tar` & `orji-4.2.0.tar`

### file list

```diff
@@ -1,51 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 09:11:53.591856 orji-4.0.0/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-12-24 09:11:15.000000 orji-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      120 2023-12-24 09:11:15.000000 orji-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3252 2023-12-24 09:11:53.591856 orji-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2368 2023-12-24 09:11:15.000000 orji-4.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 09:11:15.000000 orji-4.0.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 09:11:53.583855 orji-4.0.0/hitch/
--rw-r--r--   0 root         (0) root         (0)      523 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/Dockerfile-hitch
--rw-r--r--   0 root         (0) root         (0)       84 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/debugrequirements.txt
--rw-r--r--   0 root         (0) root         (0)     3394 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/docgen.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/docstory.yml
--rw-r--r--   0 root         (0) root         (0)     3921 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/engine.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/hitchreqs.in
--rw-r--r--   0 root         (0) root         (0)     4293 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/hitchreqs.txt
--rw-r--r--   0 root         (0) root         (0)     3914 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 09:11:53.587855 orji-4.0.0/hitch/story/
--rw-r--r--   0 root         (0) root         (0)     2971 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/all-template-features.story
--rw-r--r--   0 root         (0) root         (0)     1474 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/errors.story
--rw-r--r--   0 root         (0) root         (0)      701 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/fail.story
--rw-r--r--   0 root         (0) root         (0)      749 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/in.story
--rw-r--r--   0 root         (0) root         (0)    18631 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/latex-cv.story
--rw-r--r--   0 root         (0) root         (0)     8511 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/latex-letter.story
--rw-r--r--   0 root         (0) root         (0)      512 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/lookup.story
--rw-r--r--   0 root         (0) root         (0)      602 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/markdown.story
--rw-r--r--   0 root         (0) root         (0)      624 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/module.story
--rw-r--r--   0 root         (0) root         (0)      745 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/quickstart.story
--rw-r--r--   0 root         (0) root         (0)     1041 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/script-multiple-matching.story
--rw-r--r--   0 root         (0) root         (0)     1471 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/script.story
--rw-r--r--   0 root         (0) root         (0)       36 2023-12-24 09:11:15.000000 orji-4.0.0/hitch/story/todo.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 09:11:53.587855 orji-4.0.0/orji/
--rw-r--r--   0 root         (0) root         (0)       58 2023-12-24 09:11:15.000000 orji-4.0.0/orji/__init__.py
--rw-r--r--   0 root         (0) root         (0)      219 2023-12-24 09:11:15.000000 orji-4.0.0/orji/app.py
--rw-r--r--   0 root         (0) root         (0)       74 2023-12-24 09:11:15.000000 orji-4.0.0/orji/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-12-24 09:11:15.000000 orji-4.0.0/orji/insert.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-12-24 09:11:15.000000 orji-4.0.0/orji/lookup.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-12-24 09:11:15.000000 orji-4.0.0/orji/note.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-12-24 09:11:15.000000 orji-4.0.0/orji/output.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-12-24 09:11:15.000000 orji-4.0.0/orji/run.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-12-24 09:11:15.000000 orji-4.0.0/orji/tempdir.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-12-24 09:11:15.000000 orji-4.0.0/orji/template.py
--rw-r--r--   0 root         (0) root         (0)      277 2023-12-24 09:11:15.000000 orji-4.0.0/orji/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 09:11:53.591856 orji-4.0.0/orji.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3252 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      912 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-12-24 09:11:53.000000 orji-4.0.0/orji.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1125 2023-12-24 09:11:15.000000 orji-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-24 09:11:53.591856 orji-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-24 09:11:15.000000 orji-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.914145 orji-4.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-09 23:50:21.000000 orji-4.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      120 2024-04-09 23:50:21.000000 orji-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-09 23:50:49.914145 orji-4.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-04-09 23:50:21.000000 orji-4.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-09 23:50:21.000000 orji-4.2.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.902145 orji-4.2.0/hitch/
+-rw-r--r--   0 root         (0) root         (0)      523 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/Dockerfile-hitch
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/debugrequirements.txt
+-rw-r--r--   0 root         (0) root         (0)     3394 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/docgen.py
+-rw-r--r--   0 root         (0) root         (0)      692 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/docstory.yml
+-rw-r--r--   0 root         (0) root         (0)     3971 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/engine.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/hitchreqs.in
+-rw-r--r--   0 root         (0) root         (0)     4293 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/hitchreqs.txt
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.906145 orji-4.2.0/hitch/story/
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/all-template-features.story
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/errors.story
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/fail.story
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/in.story
+-rw-r--r--   0 root         (0) root         (0)     1407 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/insert-ical.story
+-rw-r--r--   0 root         (0) root         (0)    18631 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/latex-cv.story
+-rw-r--r--   0 root         (0) root         (0)     8511 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/latex-letter.story
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/links.story
+-rw-r--r--   0 root         (0) root         (0)     1415 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/lookup-cli.story
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/lookup-in-file.story
+-rw-r--r--   0 root         (0) root         (0)      602 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/markdown.story
+-rw-r--r--   0 root         (0) root         (0)      624 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/module.story
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/multiple-files.story
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/quickstart.story
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/rm.story
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/script-multiple-matching.story
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/script.story
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/todo.txt
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-09 23:50:21.000000 orji-4.2.0/hitch/story/walk.story
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.910145 orji-4.2.0/orji/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-09 23:50:21.000000 orji-4.2.0/orji/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      281 2024-04-09 23:50:21.000000 orji-4.2.0/orji/app.py
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-09 23:50:21.000000 orji-4.2.0/orji/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-09 23:50:21.000000 orji-4.2.0/orji/ical.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2024-04-09 23:50:21.000000 orji-4.2.0/orji/insert.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-09 23:50:21.000000 orji-4.2.0/orji/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-04-09 23:50:21.000000 orji-4.2.0/orji/lookup.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2024-04-09 23:50:21.000000 orji-4.2.0/orji/note.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-04-09 23:50:21.000000 orji-4.2.0/orji/output.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-09 23:50:21.000000 orji-4.2.0/orji/remove.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2024-04-09 23:50:21.000000 orji-4.2.0/orji/run.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-09 23:50:21.000000 orji-4.2.0/orji/tempdir.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2024-04-09 23:50:21.000000 orji-4.2.0/orji/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:50:49.910145 orji-4.2.0/orji.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-09 23:50:49.000000 orji-4.2.0/orji.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-09 23:50:21.000000 orji-4.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 23:50:49.914145 orji-4.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 23:50:21.000000 orji-4.2.0/setup.py
```

### Comparing `orji-4.0.0/LICENSE` & `orji-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/PKG-INFO` & `orji-4.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orji
-Version: 4.0.0
+Version: 4.2.0
 Summary: Org mode to jinja2 templating.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/orji
 Project-URL: documentation, https://hitchdev.com/orji/using
 Project-URL: repository, https://github.com/crdoconnor/orji
 Project-URL: changelog, https://hitchdev.com/orji/changelog
@@ -17,14 +17,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: orgmunge>=0.2.0
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: click>=8.1.3
 Requires-Dist: python-slugify>=7.0.0
+Requires-Dist: icalendar>=5.0.11
 
 # OrJi
 
 [![Main branch status](https://github.com/crdoconnor/orji/actions/workflows/regression.yml/badge.svg)](https://github.com/crdoconnor/orji/actions/workflows/regression.yml)
 
 OrJi is a command line tool to generate text files using [jinja2](https://en.wikipedia.org/wiki/Jinja_(template_engine))
 and [orgmode](https://en.wikipedia.org/wiki/Org-mode) files. It can be used to generate LaTeX, Markdown or HTML or any other kind of text from an orgmode file.
@@ -38,15 +39,15 @@
 Simple org mode file used with simple template.
 
 
 
 
 
 simple.org
-```org
+```
 * A normal note
 
 Just a note
 
 * TODO Wash car :morning:
 
 Car wash.
@@ -57,15 +58,15 @@
 
 * DONE Watch TV
 
 ```
 
 
 simple.jinja2
-```jinja2
+```
 {% for note in root %}
 {%- if note.state == "TODO" -%}
 # {{ note.name }} ({% for tag in note.tags %}{{ tag }}{% endfor %})
 
 {{ note.body }}
 {% endif %}
 {% endfor %}
@@ -73,15 +74,15 @@
 ```
 
 
 
 
 Running:
 ```bash
-orji cat simple.org simple.jinja2
+orji out simple.org simple.jinja2
 ```
 
 Will output:
 ```
 
 # Wash car (morning)
 
@@ -108,22 +109,25 @@
 OrJi can be installed with pip:
 
 ```bash
 pip install orji
 ```
 
 As a command line app, it is typically best installed via
-[pipx](https://pypa.github.io/pipx/).
+[pipx](https://pipx.pypa.io/stable/).
 
 ```bash
 pipx install orji
 ```
 
 ### Using OrJi
 
 - [Demonstration of all template features](https://hitchdev.com/orji/using/all-template-features)
 - [Deliberately trigger a template failure](https://hitchdev.com/orji/using/deliberate-failure)
+- [Insert file](https://hitchdev.com/orji/using/insert)
 - [Example of Generated LaTeX A4 CV](https://hitchdev.com/orji/using/latex-cv)
 - [Example of Generated LaTeX A4 Letter](https://hitchdev.com/orji/using/latex-letter)
 - [Convert chunks of orgmode text into markdown](https://hitchdev.com/orji/using/markdown)
 - [Use a python module with template variables and methods](https://hitchdev.com/orji/using/module)
+- [Templated with more than one note](https://hitchdev.com/orji/using/orji-run-multiple)
+- [Run](https://hitchdev.com/orji/using/orji-run)
```

### Comparing `orji-4.0.0/README.md` & `orji-4.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Simple org mode file used with simple template.
 
 
 
 
 
 simple.org
-```org
+```
 * A normal note
 
 Just a note
 
 * TODO Wash car :morning:
 
 Car wash.
@@ -33,15 +33,15 @@
 
 * DONE Watch TV
 
 ```
 
 
 simple.jinja2
-```jinja2
+```
 {% for note in root %}
 {%- if note.state == "TODO" -%}
 # {{ note.name }} ({% for tag in note.tags %}{{ tag }}{% endfor %})
 
 {{ note.body }}
 {% endif %}
 {% endfor %}
@@ -49,15 +49,15 @@
 ```
 
 
 
 
 Running:
 ```bash
-orji cat simple.org simple.jinja2
+orji out simple.org simple.jinja2
 ```
 
 Will output:
 ```
 
 # Wash car (morning)
 
@@ -84,22 +84,25 @@
 OrJi can be installed with pip:
 
 ```bash
 pip install orji
 ```
 
 As a command line app, it is typically best installed via
-[pipx](https://pypa.github.io/pipx/).
+[pipx](https://pipx.pypa.io/stable/).
 
 ```bash
 pipx install orji
 ```
 
 ### Using OrJi
 
 - [Demonstration of all template features](https://hitchdev.com/orji/using/all-template-features)
 - [Deliberately trigger a template failure](https://hitchdev.com/orji/using/deliberate-failure)
+- [Insert file](https://hitchdev.com/orji/using/insert)
 - [Example of Generated LaTeX A4 CV](https://hitchdev.com/orji/using/latex-cv)
 - [Example of Generated LaTeX A4 Letter](https://hitchdev.com/orji/using/latex-letter)
 - [Convert chunks of orgmode text into markdown](https://hitchdev.com/orji/using/markdown)
 - [Use a python module with template variables and methods](https://hitchdev.com/orji/using/module)
+- [Templated with more than one note](https://hitchdev.com/orji/using/orji-run-multiple)
+- [Run](https://hitchdev.com/orji/using/orji-run)
```

### Comparing `orji-4.0.0/hitch/Dockerfile-hitch` & `orji-4.2.0/hitch/Dockerfile-hitch`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/docgen.py` & `orji-4.2.0/hitch/docgen.py`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/docstory.yml` & `orji-4.2.0/hitch/docstory.yml`

 * *Files 23% similar despite different names*

```diff
@@ -14,18 +14,18 @@
   
   {% for step in steps %}
   {{ step.documentation() }}
   {% endfor %}
 
 given:
   files: |
-    {% for filename, contents in files.items() %}
+    {% for filename, contents in files.items() %}{% set ext = filename.split(".")[-1] %}
 
     {{ filename }}
-    ```{{ filename.split(".")[1] }}
+    ```{% if ext == "py" %}python{% elif ext == "sh" %}bash{% endif %}
     {{ contents }}
     ```
     {% endfor %}
 steps:
   orji: |
     Running:
     ```bash
```

### Comparing `orji-4.0.0/hitch/engine.py` & `orji-4.2.0/hitch/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         """Set up your applications and the test environment."""
         self.path.profile = self.path.gen.joinpath("profile")
         self.path.working = self.path.gen.joinpath("working")
 
         if self.path.working.exists():
             self.path.working.rmtree()
         self.path.working.mkdir()
+        self.path.working.joinpath("tmp").mkdir()
 
         for filename, contents in self.given["files"].items():
             filepath = self.path.working.joinpath(filename)
             if not filepath.dirname().exists():
                 filepath.dirname().mkdir()
             self.path.working.joinpath(filename).write_text(contents)
```

### Comparing `orji-4.0.0/hitch/hitchreqs.txt` & `orji-4.2.0/hitch/hitchreqs.txt`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/key.py` & `orji-4.2.0/hitch/key.py`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/all-template-features.story` & `orji-4.2.0/hitch/story/all-template-features.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/errors.story` & `orji-4.2.0/hitch/story/errors.story`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
       example.jinja2: |
         {{ root.at("nonexistent") }}
   steps:
   - orji:
       cmd: out example.org example.jinja2
       error: yes
       output: |
-        Failure on line 1 of example.jinja2: No notes found in ROOT with name nonexistent
+        Failure on line 1 of example.jinja2: No notes matching 'nonexistent' found.
 
 Template syntax error:
   given:
     files:
       example.org: |
         * existent
       example.jinja2: |
```

### Comparing `orji-4.0.0/hitch/story/fail.story` & `orji-4.2.0/hitch/story/fail.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/latex-cv.story` & `orji-4.2.0/hitch/story/latex-cv.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/latex-letter.story` & `orji-4.2.0/hitch/story/latex-letter.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/markdown.story` & `orji-4.2.0/hitch/story/markdown.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/module.story` & `orji-4.2.0/hitch/story/module.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/hitch/story/quickstart.story` & `orji-4.2.0/hitch/story/quickstart.story`

 * *Files identical despite different names*

### Comparing `orji-4.0.0/orji/output.py` & `orji-4.2.0/orji/output.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .note import Note
 from pathlib import Path
 import click
 from .template import Template
-import orgmunge
 from .tempdir import TempDir
 from .lookup import Lookup
+from .loader import Loader
+from .note import Note
 
 
 @click.command()
 @click.argument("orglookup")
 @click.argument("jinjafile")
 @click.option(
     "--latexmode",
@@ -20,29 +20,24 @@
 @click.option(
     "--module",
     "pymodule",
     help="Specify python module to use in template.",
 )
 def output(orglookup, jinjafile, latexmode, pymodule):
     lookup = Lookup(orglookup)
-    orgfile = lookup.filepath
-    indexlookup = lookup.ref
     temp_dir = TempDir()
     temp_dir.create()
-    org_text = Path(orgfile).read_text()
+    loader = Loader(temp_dir, multiple_files_ok=True)
     template_text = Path(jinjafile).read_text()
-    munge_parsed = orgmunge.Org(
-        org_text,
-        from_file=False,
-        todos={"todo_states": {"todo": "TODO"}, "done_states": {"done": "DONE"}},
-    )
-    notes = Note(munge_parsed.root, temp_dir=temp_dir)
-
-    if indexlookup is not None:
-        notes = notes.from_indexlookup(indexlookup)
+    notes = lookup.load(loader)
 
-    output_text = Template(
-        template_text, jinjafile, latexmode=latexmode, pymodule_filename=pymodule
-    ).render(notes=notes, root=notes)
+    if isinstance(notes, Note):
+        output_text = Template(
+            template_text, jinjafile, latexmode=latexmode, pymodule_filename=pymodule
+        ).render(note=notes, notes=notes, root=notes, at=notes.at, has=notes.has)
+    else:
+        output_text = Template(
+            template_text, jinjafile, latexmode=latexmode, pymodule_filename=pymodule
+        ).render(orgfiles=notes)
 
     click.echo(output_text)
     temp_dir.destroy()
```

### Comparing `orji-4.0.0/orji/run.py` & `orji-4.2.0/orji/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from click import echo
 from sys import exit
 import stat
 import subprocess
 from .template import Template
 import orgmunge
 from .tempdir import TempDir
+from .loader import Loader
 
 
 @click.command()
 @click.argument("orgdir")
 @click.argument("rundir")
 @click.option(
     "--out",
@@ -21,14 +22,15 @@
     "--multiple/--single",
     help="Output folder. Defaults to current.",
     default=False,
 )
 def run(orgdir, rundir, out, multiple):
     temp_dir = TempDir()
     temp_dir.create()
+    loader = Loader(temp_dir)
     orgdir = Path(orgdir).absolute()
     rundir = Path(rundir).absolute()
 
     assert orgdir.is_dir()
     assert rundir.is_dir()
     assert len(list(orgdir.glob("*.org"))), "orgdir must contain org files"
     assert len(list(rundir.glob("*.sh"))), "rundir must contain sh files"
@@ -45,15 +47,15 @@
     for orgfile in orgdir.glob("*.org"):
         parsed_munge = orgmunge.Org(
             Path(orgfile).read_text(),
             from_file=False,
             todos={"todo_states": {"todo": "TODO"}, "done_states": {"done": "DONE"}},
         )
 
-        for note in Note(parsed_munge.root, temp_dir=temp_dir):
+        for note in Note(parsed_munge.root, loader=loader, org=parsed_munge):
             if note.state == "TODO":
                 for tag in note.tags:
                     if tag in scripts.keys():
                         matching_notes.append((orgfile, tag, note))
 
     if len(matching_notes) == 0 and not multiple:
         temp_dir.destroy()
```

### Comparing `orji-4.0.0/orji/template.py` & `orji-4.2.0/orji/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,12 +96,12 @@
         except Failure as error:
             lineno = traceback.extract_tb(error.__traceback__)[-2].lineno
             click.echo(
                 f"Failure on line {lineno} of {self._jinjafile}: {error}", err=True
             )
             exit(1)
         except OrjiError as error:
-            lineno = traceback.extract_tb(error.__traceback__)[-2].lineno
+            lineno = traceback.extract_tb(error.__traceback__)[-3].lineno
             click.echo(
                 f"Failure on line {lineno} of {self._jinjafile}: {error}", err=True
             )
             exit(1)
```

### Comparing `orji-4.0.0/orji.egg-info/PKG-INFO` & `orji-4.2.0/orji.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orji
-Version: 4.0.0
+Version: 4.2.0
 Summary: Org mode to jinja2 templating.
 Author-email: Colm O'Connor <colm.oconnor.github@gmail.com>
 License: MIT
 Project-URL: homepage, https://hitchdev.com/orji
 Project-URL: documentation, https://hitchdev.com/orji/using
 Project-URL: repository, https://github.com/crdoconnor/orji
 Project-URL: changelog, https://hitchdev.com/orji/changelog
@@ -17,14 +17,15 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: orgmunge>=0.2.0
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: click>=8.1.3
 Requires-Dist: python-slugify>=7.0.0
+Requires-Dist: icalendar>=5.0.11
 
 # OrJi
 
 [![Main branch status](https://github.com/crdoconnor/orji/actions/workflows/regression.yml/badge.svg)](https://github.com/crdoconnor/orji/actions/workflows/regression.yml)
 
 OrJi is a command line tool to generate text files using [jinja2](https://en.wikipedia.org/wiki/Jinja_(template_engine))
 and [orgmode](https://en.wikipedia.org/wiki/Org-mode) files. It can be used to generate LaTeX, Markdown or HTML or any other kind of text from an orgmode file.
@@ -38,15 +39,15 @@
 Simple org mode file used with simple template.
 
 
 
 
 
 simple.org
-```org
+```
 * A normal note
 
 Just a note
 
 * TODO Wash car :morning:
 
 Car wash.
@@ -57,15 +58,15 @@
 
 * DONE Watch TV
 
 ```
 
 
 simple.jinja2
-```jinja2
+```
 {% for note in root %}
 {%- if note.state == "TODO" -%}
 # {{ note.name }} ({% for tag in note.tags %}{{ tag }}{% endfor %})
 
 {{ note.body }}
 {% endif %}
 {% endfor %}
@@ -73,15 +74,15 @@
 ```
 
 
 
 
 Running:
 ```bash
-orji cat simple.org simple.jinja2
+orji out simple.org simple.jinja2
 ```
 
 Will output:
 ```
 
 # Wash car (morning)
 
@@ -108,22 +109,25 @@
 OrJi can be installed with pip:
 
 ```bash
 pip install orji
 ```
 
 As a command line app, it is typically best installed via
-[pipx](https://pypa.github.io/pipx/).
+[pipx](https://pipx.pypa.io/stable/).
 
 ```bash
 pipx install orji
 ```
 
 ### Using OrJi
 
 - [Demonstration of all template features](https://hitchdev.com/orji/using/all-template-features)
 - [Deliberately trigger a template failure](https://hitchdev.com/orji/using/deliberate-failure)
+- [Insert file](https://hitchdev.com/orji/using/insert)
 - [Example of Generated LaTeX A4 CV](https://hitchdev.com/orji/using/latex-cv)
 - [Example of Generated LaTeX A4 Letter](https://hitchdev.com/orji/using/latex-letter)
 - [Convert chunks of orgmode text into markdown](https://hitchdev.com/orji/using/markdown)
 - [Use a python module with template variables and methods](https://hitchdev.com/orji/using/module)
+- [Templated with more than one note](https://hitchdev.com/orji/using/orji-run-multiple)
+- [Run](https://hitchdev.com/orji/using/orji-run)
```

### Comparing `orji-4.0.0/orji.egg-info/SOURCES.txt` & `orji-4.2.0/orji.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,33 +12,41 @@
 hitch/hitchreqs.in
 hitch/hitchreqs.txt
 hitch/key.py
 hitch/story/all-template-features.story
 hitch/story/errors.story
 hitch/story/fail.story
 hitch/story/in.story
+hitch/story/insert-ical.story
 hitch/story/latex-cv.story
 hitch/story/latex-letter.story
-hitch/story/lookup.story
+hitch/story/links.story
+hitch/story/lookup-cli.story
+hitch/story/lookup-in-file.story
 hitch/story/markdown.story
 hitch/story/module.story
+hitch/story/multiple-files.story
 hitch/story/quickstart.story
+hitch/story/rm.story
 hitch/story/script-multiple-matching.story
 hitch/story/script.story
 hitch/story/todo.txt
+hitch/story/walk.story
 orji/__init__.py
 orji/app.py
 orji/exceptions.py
+orji/ical.py
 orji/insert.py
+orji/loader.py
 orji/lookup.py
 orji/note.py
 orji/output.py
+orji/remove.py
 orji/run.py
 orji/tempdir.py
 orji/template.py
-orji/utils.py
 orji.egg-info/PKG-INFO
 orji.egg-info/SOURCES.txt
 orji.egg-info/dependency_links.txt
 orji.egg-info/entry_points.txt
 orji.egg-info/requires.txt
 orji.egg-info/top_level.txt
```

### Comparing `orji-4.0.0/pyproject.toml` & `orji-4.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Natural Language :: English",
 ]
 dependencies = [
     "orgmunge>=0.2.0",
     "jinja2>=3.1.2",
     "click>=8.1.3",
     "python-slugify>=7.0.0",
+    "icalendar>=5.0.11"
 ]
 dynamic = ["version", "readme"]
 
 [project.scripts]
 orji = "orji:cli"
 
 [project.urls]
```

