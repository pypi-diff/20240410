# Comparing `tmp/mbzero-0.2rc2.tar.gz` & `tmp/mbzero-0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbzero-0.2rc2.tar", last modified: Wed Apr 10 13:25:22 2024, max compression
+gzip compressed data, was "mbzero-0.2rc3.tar", last modified: Wed Apr 10 13:47:16 2024, max compression
```

## Comparing `mbzero-0.2rc2.tar` & `mbzero-0.2rc3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:25:22.348887 mbzero-0.2rc2/
--rw-r--r--   0 louis     (1337) louis     (1337)     1269 2024-04-09 18:56:12.000000 mbzero-0.2rc2/LICENSE
--rw-r--r--   0 louis     (1337) louis     (1337)     2897 2024-04-10 13:25:22.348887 mbzero-0.2rc2/PKG-INFO
--rw-r--r--   0 louis     (1337) louis     (1337)     1976 2024-04-08 21:03:02.000000 mbzero-0.2rc2/README.md
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:25:22.348887 mbzero-0.2rc2/mbzero/
--rw-r--r--   0 louis     (1337) louis     (1337)      309 2024-04-09 21:26:05.000000 mbzero-0.2rc2/mbzero/__init__.py
--rw-r--r--   0 louis     (1337) louis     (1337)     1987 2024-04-10 13:23:13.000000 mbzero-0.2rc2/mbzero/caarequest.py
--rw-r--r--   0 louis     (1337) louis     (1337)     7640 2024-04-10 13:23:54.000000 mbzero-0.2rc2/mbzero/mbzauth.py
--rw-r--r--   0 louis     (1337) louis     (1337)      745 2024-04-09 19:00:53.000000 mbzero-0.2rc2/mbzero/mbzerror.py
--rw-r--r--   0 louis     (1337) louis     (1337)    10024 2024-04-09 19:48:38.000000 mbzero-0.2rc2/mbzero/mbzrequest.py
--rw-r--r--   0 louis     (1337) louis     (1337)     2484 2024-04-09 19:00:38.000000 mbzero-0.2rc2/mbzero/oauth2_session_revoke.py
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:25:22.348887 mbzero-0.2rc2/mbzero.egg-info/
--rw-r--r--   0 louis     (1337) louis     (1337)     2897 2024-04-10 13:25:22.000000 mbzero-0.2rc2/mbzero.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1337) louis     (1337)      424 2024-04-10 13:25:22.000000 mbzero-0.2rc2/mbzero.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1337) louis     (1337)        1 2024-04-10 13:25:22.000000 mbzero-0.2rc2/mbzero.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1337) louis     (1337)      138 2024-04-10 13:25:22.000000 mbzero-0.2rc2/mbzero.egg-info/requires.txt
--rw-r--r--   0 louis     (1337) louis     (1337)        7 2024-04-10 13:25:22.000000 mbzero-0.2rc2/mbzero.egg-info/top_level.txt
--rw-r--r--   0 louis     (1337) louis     (1337)      865 2024-04-10 13:22:52.000000 mbzero-0.2rc2/pyproject.toml
--rw-r--r--   0 louis     (1337) louis     (1337)       38 2024-04-10 13:25:22.348887 mbzero-0.2rc2/setup.cfg
-drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:25:22.348887 mbzero-0.2rc2/tests/
--rw-r--r--   0 louis     (1337) louis     (1337)     6213 2024-04-09 19:01:37.000000 mbzero-0.2rc2/tests/test_auth.py
--rw-r--r--   0 louis     (1337) louis     (1337)     3346 2024-04-10 13:01:10.000000 mbzero-0.2rc2/tests/test_caa.py
--rw-r--r--   0 louis     (1337) louis     (1337)     2873 2024-04-09 19:02:22.000000 mbzero-0.2rc2/tests/test_oauthrequests.py
--rw-r--r--   0 louis     (1337) louis     (1337)    15042 2024-04-09 19:01:56.000000 mbzero-0.2rc2/tests/test_requests.py
--rw-r--r--   0 louis     (1337) louis     (1337)     8400 2024-04-09 19:02:09.000000 mbzero-0.2rc2/tests/test_submission.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:47:16.606916 mbzero-0.2rc3/
+-rw-r--r--   0 louis     (1337) louis     (1337)     1269 2024-04-09 18:56:12.000000 mbzero-0.2rc3/LICENSE
+-rw-r--r--   0 louis     (1337) louis     (1337)     2897 2024-04-10 13:47:16.606916 mbzero-0.2rc3/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)     1976 2024-04-08 21:03:02.000000 mbzero-0.2rc3/README.md
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:47:16.606916 mbzero-0.2rc3/mbzero/
+-rw-r--r--   0 louis     (1337) louis     (1337)      309 2024-04-09 21:26:05.000000 mbzero-0.2rc3/mbzero/__init__.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     1987 2024-04-10 13:23:13.000000 mbzero-0.2rc3/mbzero/caarequest.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     7640 2024-04-10 13:23:54.000000 mbzero-0.2rc3/mbzero/mbzauth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)      745 2024-04-09 19:00:53.000000 mbzero-0.2rc3/mbzero/mbzerror.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    10024 2024-04-09 19:48:38.000000 mbzero-0.2rc3/mbzero/mbzrequest.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     2484 2024-04-09 19:00:38.000000 mbzero-0.2rc3/mbzero/oauth2_session_revoke.py
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:47:16.606916 mbzero-0.2rc3/mbzero.egg-info/
+-rw-r--r--   0 louis     (1337) louis     (1337)     2897 2024-04-10 13:47:16.000000 mbzero-0.2rc3/mbzero.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1337) louis     (1337)      424 2024-04-10 13:47:16.000000 mbzero-0.2rc3/mbzero.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        1 2024-04-10 13:47:16.000000 mbzero-0.2rc3/mbzero.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      138 2024-04-10 13:47:16.000000 mbzero-0.2rc3/mbzero.egg-info/requires.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)        7 2024-04-10 13:47:16.000000 mbzero-0.2rc3/mbzero.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1337) louis     (1337)      865 2024-04-10 13:46:13.000000 mbzero-0.2rc3/pyproject.toml
+-rw-r--r--   0 louis     (1337) louis     (1337)       38 2024-04-10 13:47:16.606916 mbzero-0.2rc3/setup.cfg
+drwxr-xr-x   0 louis     (1337) louis     (1337)        0 2024-04-10 13:47:16.606916 mbzero-0.2rc3/tests/
+-rw-r--r--   0 louis     (1337) louis     (1337)     6213 2024-04-09 19:01:37.000000 mbzero-0.2rc3/tests/test_auth.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     3328 2024-04-10 13:25:44.000000 mbzero-0.2rc3/tests/test_caa.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     2873 2024-04-09 19:02:22.000000 mbzero-0.2rc3/tests/test_oauthrequests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)    15042 2024-04-09 19:01:56.000000 mbzero-0.2rc3/tests/test_requests.py
+-rw-r--r--   0 louis     (1337) louis     (1337)     8364 2024-04-10 13:26:29.000000 mbzero-0.2rc3/tests/test_submission.py
```

### Comparing `mbzero-0.2rc2/LICENSE` & `mbzero-0.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/PKG-INFO` & `mbzero-0.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbzero
-Version: 0.2rc2
+Version: 0.2rc3
 Summary: Python bindings for the MusicBrainz and the Cover Art Archive webservices
 Author-email: Louis Rannou <louson@gresille.org>
 Project-URL: Homepage, https://gitlab.com/Louson-public/personal/python-mbzero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `mbzero-0.2rc2/README.md` & `mbzero-0.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero/caarequest.py` & `mbzero-0.2rc3/mbzero/caarequest.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero/mbzauth.py` & `mbzero-0.2rc3/mbzero/mbzauth.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero/mbzerror.py` & `mbzero-0.2rc3/mbzero/mbzerror.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero/mbzrequest.py` & `mbzero-0.2rc3/mbzero/mbzrequest.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero/oauth2_session_revoke.py` & `mbzero-0.2rc3/mbzero/oauth2_session_revoke.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/mbzero.egg-info/PKG-INFO` & `mbzero-0.2rc3/mbzero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbzero
-Version: 0.2rc2
+Version: 0.2rc3
 Summary: Python bindings for the MusicBrainz and the Cover Art Archive webservices
 Author-email: Louis Rannou <louson@gresille.org>
 Project-URL: Homepage, https://gitlab.com/Louson-public/personal/python-mbzero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `mbzero-0.2rc2/pyproject.toml` & `mbzero-0.2rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires  = [
     "setuptools", "requests", "requests_oauthlib"
 ]
 
 [project]
 name = "mbzero"
-version = "0.2-rc2"
+version = "0.2-rc3"
 description = "Python bindings for the MusicBrainz and the Cover Art Archive webservices"
 readme = "README.md"
 authors = [
     {name = "Louis Rannou", email = "louson@gresille.org"},
 ]
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mbzero-0.2rc2/tests/test_auth.py` & `mbzero-0.2rc3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/tests/test_caa.py` & `mbzero-0.2rc3/tests/test_caa.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,17 @@
         req.send()
         mock_get.assert_called_once_with(
             "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
             self.payload, headers=self.headers)
 
     def testCaaItemRequest(self, mock_get, _):
         caa.CaaRequest(self.user_agent,
-                             "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
-                             "front"
-                             ).send()
+                       "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3",
+                       "front"
+                       ).send()
         mock_get.assert_called_once_with(
             CAA_API + "/artist/0383dadf-2a4e-4d10-a46a-e9e041da8eb3/front",
             self.payload, headers=self.headers)
 
     def testCaaHead(self, _, mock_head):
         caa.CaaRequest(self.user_agent,
                        "artist", "0383dadf-2a4e-4d10-a46a-e9e041da8eb3"
```

### Comparing `mbzero-0.2rc2/tests/test_oauthrequests.py` & `mbzero-0.2rc3/tests/test_oauthrequests.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/tests/test_requests.py` & `mbzero-0.2rc3/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `mbzero-0.2rc2/tests/test_submission.py` & `mbzero-0.2rc3/tests/test_submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             params=expPayload, headers=expHeaders)
 
     def testSendWrongType(self, mock_post):
         try:
             mbr.MbzRequest(self.user_agent, client=self.client
                            ).post("/request", data="data", data_type="WRONG",
                                   credentials=self.cred, headers=self.headers)
-        except Exception as e:
+        except Exception:
             pass
         mock_post.assert_not_called()
 
     def testSendOpts(self, mock_post):
         mbr.MbzRequest(self.user_agent, client=self.client
                        ).post("/request", data="data", data_type="xml",
                               credentials=self.cred,
@@ -160,16 +160,16 @@
         req = mbr.MbzRequest(self.user_agent, client=self.client)
         req.set_url("")
         expPayload = self.payload.copy()
         expPayload["client"] = self.client
         expHeaders = self.headers.copy()
         expHeaders["Content-Type"] = "application/xml; charset=utf-8"
         req.post("/request", data="data", data_type="xml",
-                              credentials=self.cred,
-                              payload=self.payload, headers=self.headers)
+                 credentials=self.cred,
+                 payload=self.payload, headers=self.headers)
         mock_post.assert_called_once_with(
             "/request",
             data=self.data,
             params=expPayload, headers=expHeaders)
 
     def testSubmissionSend(self, mock_post):
         mbr.MbzSubmission(self.user_agent, "request",
@@ -185,10 +185,10 @@
             params=self.payload, headers=self.headers)
 
     def testSubmissionSendWrongType(self, mock_post):
         try:
             mbr.MbzSubmission(self.user_agent, "request",
                               data="data", data_type="WRONG").send(
                                   credentials=self.cred)
-        except Exception as e:
+        except Exception:
             pass
         mock_post.assert_not_called()
```

