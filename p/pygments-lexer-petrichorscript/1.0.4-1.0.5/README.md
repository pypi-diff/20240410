# Comparing `tmp/pygments-lexer-petrichorscript-1.0.4.tar.gz` & `tmp/pygments-lexer-petrichorscript-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments-lexer-petrichorscript-1.0.4.tar", last modified: Sat Apr  6 08:37:14 2024, max compression
+gzip compressed data, was "pygments-lexer-petrichorscript-1.0.5.tar", last modified: Wed Apr 10 09:13:36 2024, max compression
```

## Comparing `pygments-lexer-petrichorscript-1.0.4.tar` & `pygments-lexer-petrichorscript-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 08:37:14.965320 pygments-lexer-petrichorscript-1.0.4/
--rw-rw-rw-   0        0        0     5152 2024-04-06 04:43:16.000000 pygments-lexer-petrichorscript-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1464 2024-04-06 08:37:14.963321 pygments-lexer-petrichorscript-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      866 2024-04-06 07:20:56.000000 pygments-lexer-petrichorscript-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 08:37:14.941321 pygments-lexer-petrichorscript-1.0.4/lexer/
--rw-rw-rw-   0        0        0        0 2024-04-06 04:43:16.000000 pygments-lexer-petrichorscript-1.0.4/lexer/__init__.py
--rw-rw-rw-   0        0        0      951 2024-04-06 08:27:49.000000 pygments-lexer-petrichorscript-1.0.4/lexer/lexer.py
-drwxrwxrwx   0        0        0        0 2024-04-06 08:37:14.962125 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/
--rw-rw-rw-   0        0        0     1464 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 08:37:14.000000 pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-04-06 08:14:00.000000 pygments-lexer-petrichorscript-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 08:37:14.965320 pygments-lexer-petrichorscript-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 09:13:36.127421 pygments-lexer-petrichorscript-1.0.5/
+-rw-rw-rw-   0        0        0     5152 2024-04-06 04:43:16.000000 pygments-lexer-petrichorscript-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1464 2024-04-10 09:13:36.124421 pygments-lexer-petrichorscript-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2024-04-06 07:20:56.000000 pygments-lexer-petrichorscript-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 09:13:36.082422 pygments-lexer-petrichorscript-1.0.5/lexer/
+-rw-rw-rw-   0        0        0        0 2024-04-06 04:43:16.000000 pygments-lexer-petrichorscript-1.0.5/lexer/__init__.py
+-rw-rw-rw-   0        0        0     1158 2024-04-10 09:11:04.000000 pygments-lexer-petrichorscript-1.0.5/lexer/lexer.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:13:36.122420 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/
+-rw-rw-rw-   0        0        0     1464 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 09:13:36.000000 pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-04-10 08:35:05.000000 pygments-lexer-petrichorscript-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 09:13:36.128421 pygments-lexer-petrichorscript-1.0.5/setup.cfg
```

### Comparing `pygments-lexer-petrichorscript-1.0.4/LICENSE` & `pygments-lexer-petrichorscript-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments-lexer-petrichorscript-1.0.4/PKG-INFO` & `pygments-lexer-petrichorscript-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-lexer-petrichorscript
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pygments lexer for Petrichor Script.
 Author-email: SparkliTwizzl <github@sparklitwizzl.com>
 License: Anti-Exploitation License Noncommercial Attribution 1.1
 Project-URL: Homepage, https://github.com/sparklitwizzl/pygments-lexer-petrichorscript
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: OS Independent
```

### Comparing `pygments-lexer-petrichorscript-1.0.4/README.md` & `pygments-lexer-petrichorscript-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pygments-lexer-petrichorscript-1.0.4/lexer/lexer.py` & `pygments-lexer-petrichorscript-1.0.5/lexer/lexer.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     aliases = ['petrichor','ptcr']
     filenames = ['*.petrichor','*.ptcr']
 
     tokens = {
         'root': [
             (r'\s+', Text), # whitespace
             (r'\\.', String.Escape), # escaped character
-            (r'//.*\n', Comment.Single),
-            (r',', Punctuation),
-            (r'[\{\}]', Operator),
-            (r'>>', Operator),
-            (r'([a-z][a-z0-9\-]*)(\s*)(:)', bygroups(Keyword.Reserved, Text, Operator)),
-            (r'\[[a-z\-]+\]', Name.Variable),
-            (r'"', String, 'string'),
-            (r'[0-9]+', Number),
+            (r'//.*\n', Comment.Single), # line comment
+            (r',', Punctuation), # comma
+            (r'[\{\}]', Operator), # token body boundaries
+            (r'(?<!>)>>(?!>)', Operator), # text shortcut template divider operator
+            (r'(^\s*[a-z]+(?:-[a-z0-9]+)*(?:-[a-z]+)?)(\s*)(:)', bygroups(Keyword.Reserved, Text, Operator)), # token name, whitespacae, token divider
+            (r'\[[a-z\-]+\]', Name.Variable), # field
+            (r'"', String, 'string'), # string start
+            (r'\b(-)?[0-9.]+\b', Number),
             (r'.', Text),
         ],
         'string': [
             (r'\\.', String.Escape),
-            (r'"', String, '#pop'),
+            (r'"', String, '#pop'), # string end
             (r'[^\\"]+', String),
         ]
     }
```

### Comparing `pygments-lexer-petrichorscript-1.0.4/pygments_lexer_petrichorscript.egg-info/PKG-INFO` & `pygments-lexer-petrichorscript-1.0.5/pygments_lexer_petrichorscript.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-lexer-petrichorscript
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pygments lexer for Petrichor Script.
 Author-email: SparkliTwizzl <github@sparklitwizzl.com>
 License: Anti-Exploitation License Noncommercial Attribution 1.1
 Project-URL: Homepage, https://github.com/sparklitwizzl/pygments-lexer-petrichorscript
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: OS Independent
```

### Comparing `pygments-lexer-petrichorscript-1.0.4/pyproject.toml` & `pygments-lexer-petrichorscript-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pygments-lexer-petrichorscript"
-version = "1.0.4"
+version = "1.0.5"
 description = "Pygments lexer for Petrichor Script."
 license = { text = "Anti-Exploitation License Noncommercial Attribution 1.1" }
 authors = [
     { name = "SparkliTwizzl", email = "github@sparklitwizzl.com" }
 ]
 readme = "README.md"
 urls = { Homepage = "https://github.com/sparklitwizzl/pygments-lexer-petrichorscript" }
```

