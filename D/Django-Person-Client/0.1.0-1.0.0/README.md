# Comparing `tmp/Django-Person-Client-0.1.0.tar.gz` & `tmp/Django-Person-Client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Django-Person-Client-0.1.0.tar", last modified: Fri Apr  5 00:14:53 2024, max compression
+gzip compressed data, was "Django-Person-Client-1.0.0.tar", last modified: Wed Apr 10 18:02:18 2024, max compression
```

## Comparing `Django-Person-Client-0.1.0.tar` & `Django-Person-Client-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.231269 Django-Person-Client-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.227269 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 00:14:53.000000 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-05 00:14:53.000000 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:14:53.000000 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 00:14:53.000000 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 00:14:53.000000 Django-Person-Client-0.1.0/Django_Person_Client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-05 00:14:53.231269 Django-Person-Client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:14:53.231269 Django-Person-Client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.227269 Django-Person-Client-0.1.0/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 00:14:51.000000 Django-Person-Client-0.1.0/uw_person_client/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.227269 Django-Person-Client-0.1.0/uw_person_client/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/adviser.json
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/degree.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/employee.json
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/hold.json
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/major.json
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/person.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/sport.json
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/student.json
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/term.json
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/transcript.json
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/fixtures/transfer.json
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.231269 Django-Person-Client-0.1.0/uw_person_client/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/test_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/test_migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:14:53.231269 Django-Person-Client-0.1.0/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/tests/test_adviser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/tests/test_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 00:14:42.000000 Django-Person-Client-0.1.0/uw_person_client/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.934142 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.934142 Django-Person-Client-1.0.0/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/uw_person_client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/adviser.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/degree.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/employee.json
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/hold.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/major.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/person.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/sport.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/student.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/term.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/transcript.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/transfer.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31339 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/test_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/test_migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/test_adviser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/urls.py
```

### Comparing `Django-Person-Client-0.1.0/Django_Person_Client.egg-info/PKG-INFO` & `Django-Person-Client-1.0.0/Django_Person_Client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 0.1.0
+Version: 1.0.0
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-0.1.0/Django_Person_Client.egg-info/SOURCES.txt` & `Django-Person-Client-1.0.0/Django_Person_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/LICENSE` & `Django-Person-Client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/PKG-INFO` & `Django-Person-Client-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 0.1.0
+Version: 1.0.0
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-0.1.0/setup.py` & `Django-Person-Client-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/adviser.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/adviser.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/degree.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/degree.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/employee.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/employee.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/hold.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/hold.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/major.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/major.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/person.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/person.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/sport.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/sport.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/student.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/student.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/transcript.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/transcript.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/fixtures/transfer.json` & `Django-Person-Client-1.0.0/uw_person_client/fixtures/transfer.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/models.py` & `Django-Person-Client-1.0.0/uw_person_client/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,14 +675,15 @@
     enroll_status_request_code = models.TextField(blank=True, null=True)
     enroll_status_desc = models.TextField(blank=True, null=True)
     special_program_desc = models.TextField(blank=True, null=True)
 
     class Meta:
         db_table = 'transcript'
         managed = False
+        ordering = ['-tran_term__year', '-tran_term__quarter']
 
     def to_dict(self):
         data = model_to_dict(self)
         if self.tran_term is not None:
             data['tran_term'] = self.tran_term.to_dict()
         if self.leave_ends_term is not None:
             data['leave_ends_term'] = self.leave_ends_term.to_dict()
```

### Comparing `Django-Person-Client-0.1.0/uw_person_client/test_migrations/0001_initial.py` & `Django-Person-Client-1.0.0/uw_person_client/test_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/tests/test_adviser.py` & `Django-Person-Client-1.0.0/uw_person_client/tests/test_adviser.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-0.1.0/uw_person_client/tests/test_person.py` & `Django-Person-Client-1.0.0/uw_person_client/tests/test_person.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,20 @@
 
     def test_get_student_includes_by_uwnetid(self):
         p = Person.objects.get_person_by_uwnetid(
             'javerage', include_student=True, include_student_transcripts=True)
         self.assertEqual(p.uwnetid, 'javerage')
         self.assertEqual(len(p.student.transcripts.all()), 2)
 
+        # default transcript sorting
+        t1 = p.student.transcripts.all()[0]
+        t2 = p.student.transcripts.all()[1]
+        self.assertLess(int(f'{t2.tran_term.year}{t2.tran_term.quarter}'),
+                        int(f'{t1.tran_term.year}{t1.tran_term.quarter}'))
+
         p = Person.objects.get_person_by_uwnetid(
             'javerage', include_student=True, include_student_transfers=True)
         self.assertEqual(p.uwnetid, 'javerage')
         self.assertEqual(len(p.student.transfers.all()), 1)
 
         p = Person.objects.get_person_by_uwnetid(
             'javerage', include_student=True, include_student_holds=True)
```

