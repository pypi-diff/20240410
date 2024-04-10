# Comparing `tmp/telepoller-0.0.1.tar.gz` & `tmp/telepoller-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telepoller-0.0.1.tar", last modified: Wed Apr 10 06:05:49 2024, max compression
+gzip compressed data, was "telepoller-0.0.2.tar", last modified: Wed Apr 10 06:09:40 2024, max compression
```

## Comparing `telepoller-0.0.1.tar` & `telepoller-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:05:49.075828 telepoller-0.0.1/
--rw-rw-rw-   0        0        0     2722 2024-04-10 06:05:49.074828 telepoller-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2334 2024-04-10 05:59:34.000000 telepoller-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 06:05:49.076829 telepoller-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-04-10 06:02:55.000000 telepoller-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:05:49.067828 telepoller-0.0.1/telepoller/
--rw-rw-rw-   0        0        0     3362 2024-04-10 05:52:14.000000 telepoller-0.0.1/telepoller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:05:49.074828 telepoller-0.0.1/telepoller.egg-info/
--rw-rw-rw-   0        0        0     2722 2024-04-10 06:05:49.000000 telepoller-0.0.1/telepoller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-10 06:05:49.000000 telepoller-0.0.1/telepoller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:05:49.000000 telepoller-0.0.1/telepoller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 06:05:49.000000 telepoller-0.0.1/telepoller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 06:05:49.000000 telepoller-0.0.1/telepoller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:09:40.094890 telepoller-0.0.2/
+-rw-rw-rw-   0        0        0     2722 2024-04-10 06:09:40.094890 telepoller-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2334 2024-04-10 05:59:34.000000 telepoller-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 06:09:40.095890 telepoller-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-10 06:09:11.000000 telepoller-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:09:40.086890 telepoller-0.0.2/telepoller/
+-rw-rw-rw-   0        0        0     3391 2024-04-10 06:09:11.000000 telepoller-0.0.2/telepoller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:09:40.093890 telepoller-0.0.2/telepoller.egg-info/
+-rw-rw-rw-   0        0        0     2722 2024-04-10 06:09:40.000000 telepoller-0.0.2/telepoller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-10 06:09:40.000000 telepoller-0.0.2/telepoller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:09:40.000000 telepoller-0.0.2/telepoller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 06:09:40.000000 telepoller-0.0.2/telepoller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 06:09:40.000000 telepoller-0.0.2/telepoller.egg-info/top_level.txt
```

### Comparing `telepoller-0.0.1/PKG-INFO` & `telepoller-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepoller
-Version: 0.0.1
+Version: 0.0.2
 Summary: Poller for Telegram Bot on Pytelegrambotapi
 Author: STaper_Admin
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `telepoller-0.0.1/README.md` & `telepoller-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `telepoller-0.0.1/setup.py` & `telepoller-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
 	required = f.read().splitlines()
 
 
 setuptools.setup(
 	name='telepoller',
-	version="0.0.1",
+	version="0.0.2",
 	author="STaper_Admin",
 	description="Poller for Telegram Bot on Pytelegrambotapi",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	install_requires=required,
 	classifiers=[
 		"Programming Language :: Python :: 3.10",
```

### Comparing `telepoller-0.0.1/telepoller/__init__.py` & `telepoller-0.0.2/telepoller/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import types
 from telebot.types import ReplyKeyboardMarkup
 
 class Poller:
-    def __init__(self, questions: dict, filters, buttons, answers, logger=None):
+    def __init__(self, bot, questions: dict, filters, buttons, answers, logger=None):
         """
         Этот класс будет использоваться для определения порядка отправки сообщений. Также будут указываться,
         кнопки для отправки сообщений и фильтры для приёмки сообщений.
         """
         if logger is None:
             import loguru
             self.logger = loguru.logger
         else:
             self.logger = logger
 
+        self.bot = bot
         self.questions = questions
         self.filters = filters
         self.buttons = buttons
         self.bot_answers = answers
         self.user_answers = []
         self.counter = 1
```

### Comparing `telepoller-0.0.1/telepoller.egg-info/PKG-INFO` & `telepoller-0.0.2/telepoller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telepoller
-Version: 0.0.1
+Version: 0.0.2
 Summary: Poller for Telegram Bot on Pytelegrambotapi
 Author: STaper_Admin
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

