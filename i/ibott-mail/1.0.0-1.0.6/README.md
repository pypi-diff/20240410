# Comparing `tmp/ibott-mail-1.0.0.tar.gz` & `tmp/ibott-mail-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibott-mail-1.0.0.tar", last modified: Sun Oct 29 18:43:31 2023, max compression
+gzip compressed data, was "ibott-mail-1.0.6.tar", last modified: Wed Apr 10 09:37:42 2024, max compression
```

## Comparing `ibott-mail-1.0.0.tar` & `ibott-mail-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2023-10-29 18:43:31.896066 ibott-mail-1.0.0/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-mail-1.0.0/LICENSE
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15984 2023-10-29 18:43:31.895640 ibott-mail-1.0.0/PKG-INFO
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2023-10-29 18:43:31.893264 ibott-mail-1.0.0/email_activities/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2022-05-16 11:27:00.000000 ibott-mail-1.0.0/email_activities/__init__.py
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     4935 2023-10-29 17:55:02.000000 ibott-mail-1.0.0/email_activities/mails.py
-drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2023-10-29 18:43:31.895072 ibott-mail-1.0.0/ibott_mail.egg-info/
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15984 2023-10-29 18:43:31.000000 ibott-mail-1.0.0/ibott_mail.egg-info/PKG-INFO
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      255 2023-10-29 18:43:31.000000 ibott-mail-1.0.0/ibott_mail.egg-info/SOURCES.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2023-10-29 18:43:31.000000 ibott-mail-1.0.0/ibott_mail.egg-info/dependency_links.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       29 2023-10-29 18:43:31.000000 ibott-mail-1.0.0/ibott_mail.egg-info/requires.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       17 2023-10-29 18:43:31.000000 ibott-mail-1.0.0/ibott_mail.egg-info/top_level.txt
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2023-10-29 18:38:07.000000 ibott-mail-1.0.0/pyproject.toml
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2023-10-29 18:43:31.896170 ibott-mail-1.0.0/setup.cfg
--rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      700 2023-10-29 18:38:48.000000 ibott-mail-1.0.0/setup.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.678427 ibott-mail-1.0.6/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    11355 2023-10-14 17:23:38.000000 ibott-mail-1.0.6/LICENSE
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-04-10 09:37:42.678142 ibott-mail-1.0.6/PKG-INFO
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.676325 ibott-mail-1.0.6/email_activities/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        0 2022-05-16 11:27:00.000000 ibott-mail-1.0.6/email_activities/__init__.py
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)     5139 2024-04-10 07:25:15.000000 ibott-mail-1.0.6/email_activities/mails.py
+drwxr-xr-x   0 enriquecrespodebenito   (501) staff       (20)        0 2024-04-10 09:37:42.677711 ibott-mail-1.0.6/ibott_mail.egg-info/
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)    15986 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/PKG-INFO
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      255 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)        1 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       29 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/requires.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       17 2024-04-10 09:37:42.000000 ibott-mail-1.0.6/ibott_mail.egg-info/top_level.txt
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      710 2024-04-10 09:37:34.000000 ibott-mail-1.0.6/pyproject.toml
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)       38 2024-04-10 09:37:42.678500 ibott-mail-1.0.6/setup.cfg
+-rw-r--r--   0 enriquecrespodebenito   (501) staff       (20)      700 2024-04-10 09:37:34.000000 ibott-mail-1.0.6/setup.py
```

### Comparing `ibott-mail-1.0.0/LICENSE` & `ibott-mail-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibott-mail-1.0.0/PKG-INFO` & `ibott-mail-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-mail
-Version: 1.0.0
+Version: 1.0.6
 Summary: This packages crates a simple way to work with, emails, send, read and download attachments
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -212,15 +212,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Mail Activities
+## Mail Activitiesal
 This Python package contains Mail class to work with emails,
 for more information about how to develop your RPA projects with python check https://automatehub.es/
 
 # Mail class
 
 The `Mail` class represents a mail account and provides methods for sending and fetching emails.
```

### Comparing `ibott-mail-1.0.0/email_activities/mails.py` & `ibott-mail-1.0.6/email_activities/mails.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,16 +75,24 @@
                 ext = f.split('.')[-1:]
                 attached = MIMEApplication(fil.read(), _subtype=ext)
                 attached.add_header(
                     'content-disposition', 'attachment', filename=basename(f))
             msg.attach(attached)
 
         context = ssl.create_default_context()
-        smtp = smtplib.SMTP_SSL(self.smtp_server, self.smtp_port, context=context)
-        smtp.login(self.username, self.password)
+
+        try:
+            smtp = smtplib.SMTP_SSL(self.smtp_server, self.smtp_port, context=context)
+        except:
+            smtp = smtplib.SMTP(self.smtp_server, self.smtp_port)
+        try:
+            smtp.login(self.username, self.password)
+        except:
+            print("El servidor de correo no requiere autenticación")
+
         smtp.sendmail(self.username, send_to, msg.as_string())
         smtp.close()
 
     def fetch(self, folder=None, Query=None):
         """
         Get list of emails from Mailbox server
         Arguments:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibott-mail-1.0.0/ibott_mail.egg-info/PKG-INFO` & `ibott-mail-1.0.6/ibott_mail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott-mail
-Version: 1.0.0
+Version: 1.0.6
 Summary: This packages crates a simple way to work with, emails, send, read and download attachments
 Home-page: https://github.com/ecrespo66/files_and_folders
 Author: OnameDohe
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -212,15 +212,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Mail Activities
+## Mail Activitiesal
 This Python package contains Mail class to work with emails,
 for more information about how to develop your RPA projects with python check https://automatehub.es/
 
 # Mail class
 
 The `Mail` class represents a mail account and provides methods for sending and fetching emails.
```

### Comparing `ibott-mail-1.0.0/pyproject.toml` & `ibott-mail-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "imap-tools==0.16.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ibott-mail"
-version = "1.0.0"
+version = "1.0.6"
 authors = [
     { name="OnameDohe", email="enrique.crespo.debenito@gmail.com" },
 ]
 description = "This packages crates a simple way to work with, emails, send, read and download attachments"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `ibott-mail-1.0.0/setup.py` & `ibott-mail-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ibott-files",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     install_requires=["hatchling", "imap-tools==0.16.1"],
     author="OnameDohe",
     author_email="enrique.crespo.debenito@gmail.com",
     description="This packages crates a simple way to work with, emails, send, read and download attachments",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

