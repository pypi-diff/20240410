# Comparing `tmp/istari-0.1.0.tar.gz` & `tmp/istari-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.1.0.tar", last modified: Mon Apr  8 18:38:02 2024, max compression
+gzip compressed data, was "istari-0.1.2.tar", last modified: Tue Apr  9 21:36:27 2024, max compression
```

## Comparing `istari-0.1.0.tar` & `istari-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.391557 istari-0.1.0/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-08 18:38:02.391327 istari-0.1.0/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.0/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388004 istari-0.1.0/istari/
--rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-08 18:37:31.000000 istari-0.1.0/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388888 istari-0.1.0/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.0/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.0/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.389316 istari-0.1.0/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.0/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.0/istari/cli/base.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.389813 istari-0.1.0/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.0/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     2267 2024-04-08 18:18:38.000000 istari-0.1.0/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.0/istari/commands/startproject.py
--rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.0/istari/constants.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390159 istari-0.1.0/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.0/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.0/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-06 00:40:42.000000 istari-0.1.0/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390345 istari-0.1.0/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.0/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.0/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.390843 istari-0.1.0/istari/templates/plugins/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.0/istari/templates/plugins/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      578 2024-04-08 17:57:08.000000 istari-0.1.0/istari/templates/plugins/base.py
--rw-r--r--   0 jay        (501) staff       (20)     1541 2024-04-08 18:33:07.000000 istari-0.1.0/istari/templates/plugins/defaultuser.py
--rw-r--r--   0 jay        (501) staff       (20)     1715 2024-04-08 17:57:39.000000 istari-0.1.0/istari/templates/plugins/editable.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.391042 istari-0.1.0/istari/utils/
--rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.0/istari/utils/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-08 18:38:02.388698 istari-0.1.0/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      678 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-08 18:38:02.000000 istari-0.1.0/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-08 18:38:02.391591 istari-0.1.0/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.0/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729934 istari-0.1.2/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-09 21:36:27.729693 istari-0.1.2/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.2/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.726924 istari-0.1.2/istari/
+-rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-09 21:35:38.000000 istari-0.1.2/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727518 istari-0.1.2/istari/admin/
+-rw-r--r--   0 jay        (501) staff       (20)     1661 2024-04-09 21:28:02.000000 istari-0.1.2/istari/admin/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727718 istari-0.1.2/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.2/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.2/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727913 istari-0.1.2/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.2/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.2/istari/cli/base.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728174 istari-0.1.2/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.2/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     2339 2024-04-09 21:32:52.000000 istari-0.1.2/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.2/istari/commands/startproject.py
+-rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.2/istari/constants.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728426 istari-0.1.2/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.2/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.2/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-09 21:23:29.000000 istari-0.1.2/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728629 istari-0.1.2/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.2/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.2/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729253 istari-0.1.2/istari/templates/plugins/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.2/istari/templates/plugins/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1045 2024-04-09 02:44:58.000000 istari-0.1.2/istari/templates/plugins/base.py
+-rw-r--r--   0 jay        (501) staff       (20)     1344 2024-04-09 02:35:05.000000 istari-0.1.2/istari/templates/plugins/defaultuser.py
+-rw-r--r--   0 jay        (501) staff       (20)     1100 2024-04-09 03:00:11.000000 istari-0.1.2/istari/templates/plugins/drf.py
+-rw-r--r--   0 jay        (501) staff       (20)     1194 2024-04-09 03:01:28.000000 istari-0.1.2/istari/templates/plugins/editable.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729373 istari-0.1.2/istari/utils/
+-rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.2/istari/utils/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729496 istari-0.1.2/istari/utils/io/
+-rw-r--r--   0 jay        (501) staff       (20)     1438 2024-04-09 03:00:36.000000 istari-0.1.2/istari/utils/io/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727406 istari-0.1.2/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      763 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-09 21:36:27.729967 istari-0.1.2/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.2/setup.py
```

### Comparing `istari-0.1.0/istari/auth/models.py` & `istari-0.1.2/istari/auth/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/cli/__init__.py` & `istari-0.1.2/istari/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/commands/startapp.py` & `istari-0.1.2/istari/commands/startapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         with open(settings, 'w') as f:
             f.writelines(contents)
 
     def handle(self, **options):
         options['target_dir'] = options.get('target_dir', Path.cwd())
         options['variables'] = {
             'app_name': options['app_name'],
+            'config_name': f"{options['app_name'].capitalize()}Config",
         }
 
         if not (options['target_dir'] / 'manage.py').is_file():
             raise Exception('File manage.py not found. Please run in root directory of Django project.')
         
         settings = None
         for path in options['target_dir'].rglob('*'):
```

### Comparing `istari-0.1.0/istari/commands/startproject.py` & `istari-0.1.2/istari/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/db/fields.py` & `istari-0.1.2/istari/db/fields.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/db/models.py` & `istari-0.1.2/istari/db/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/templates/commands.py` & `istari-0.1.2/istari/templates/commands.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.0/istari/templates/plugins/defaultuser.py` & `istari-0.1.2/istari/templates/plugins/defaultuser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 from istari.commands.startapp import Command as StartAppCommand
 from istari.templates.plugins.base import BasePlugin
+from istari.utils.io import File
 
 
 class Plugin(BasePlugin):
     help = 'Define custom AUTH_USER_MODEL'
 
     template = 'project'
 
@@ -23,25 +24,21 @@
             'class User(EmailUser):\n',
             '    pass\n',
         ]
         with open(path, 'w') as f:
             f.writelines(contents)
 
     def define_auth_user_model(self):
-        path = self.target_dir / self.project_name / 'settings.py'
-        with open(path, 'r') as f:
-            contents = f.readlines()
-        fp = 0
-        for i, line in enumerate(contents):
-            if line.lstrip().startswith('ALLOWED_HOSTS'):
-                fp = i + 1
-                break
-        contents.insert(fp, "\nAUTH_USER_MODEL = 'users.User'\n")
-        with open(path, 'w') as f:
-            f.writelines(contents)
+        f = File(self.target_dir / self.project_name / 'settings.py')
+        f.seek('ALLOWED_HOSTS')
+        f.insert([
+            '',
+            "AUTH_USER_MODEL = 'users.User'",
+        ])
+        f.save()
 
     def process(self, **options):
         self.project_name: str = options['project_name']
         self.target_dir: Path = options['target_dir']
         self.create_users_app()
         self.add_users_model()
         self.define_auth_user_model()
```

### Comparing `istari-0.1.0/istari.egg-info/SOURCES.txt` & `istari-0.1.2/istari.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 istari/__init__.py
 istari/constants.py
 istari.egg-info/PKG-INFO
 istari.egg-info/SOURCES.txt
 istari.egg-info/dependency_links.txt
 istari.egg-info/entry_points.txt
 istari.egg-info/top_level.txt
+istari/admin/__init__.py
 istari/auth/__init__.py
 istari/auth/models.py
 istari/cli/__init__.py
 istari/cli/base.py
 istari/commands/__init__.py
 istari/commands/startapp.py
 istari/commands/startproject.py
@@ -18,9 +19,11 @@
 istari/db/fields.py
 istari/db/models.py
 istari/templates/__init__.py
 istari/templates/commands.py
 istari/templates/plugins/__init__.py
 istari/templates/plugins/base.py
 istari/templates/plugins/defaultuser.py
+istari/templates/plugins/drf.py
 istari/templates/plugins/editable.py
-istari/utils/__init__.py
+istari/utils/__init__.py
+istari/utils/io/__init__.py
```

