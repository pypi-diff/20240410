# Comparing `tmp/alibabacloud_tingwu20230930_py2-2.0.6.tar.gz` & `tmp/alibabacloud_tingwu20230930_py2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tingwu20230930_py2-2.0.6.tar", last modified: Mon Mar 18 09:04:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_tingwu20230930_py2-2.0.7.tar", last modified: Wed Apr 10 17:10:54 2024, max compression
```

## Comparing `alibabacloud_tingwu20230930_py2-2.0.6.tar` & `alibabacloud_tingwu20230930_py2-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/
--rw-r--r--   0 root         (0) root         (0)      834 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9485 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/client.py
--rw-r--r--   0 root         (0) root         (0)    52824 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-18 09:04:03.000000 alibabacloud_tingwu20230930_py2-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      954 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9485 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)    53082 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/setup.py
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/ChangeLog.md` & `alibabacloud_tingwu20230930_py2-2.0.7/ChangeLog.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-03-18 Version: 2.0.6
+- Update API CreateTask: update param body.
+- Update API CreateTask: update response param.
+
+
 2024-03-15 Version: 2.0.5
 - Update API CreateTask: update param body.
 
 
 2024-03-12 Version: 2.0.4
 - Update API CreateTask: update response param.
 - Update API GetTaskInfo: update response param.
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/LICENSE` & `alibabacloud_tingwu20230930_py2-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/PKG-INFO` & `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_tingwu20230930_py2
-Version: 2.0.6
+Name: alibabacloud-tingwu20230930-py2
+Version: 2.0.7
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/README-CN.md` & `alibabacloud_tingwu20230930_py2-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/README.md` & `alibabacloud_tingwu20230930_py2-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/client.py` & `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930/models.py` & `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,19 +767,20 @@
             temp_model = DeleteTranscriptionPhrasesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetTaskInfoResponseBodyDataResult(TeaModel):
     def __init__(self, auto_chapters=None, meeting_assistance=None, ppt_extraction=None, summarization=None,
-                 transcription=None, translation=None):
+                 text_polish=None, transcription=None, translation=None):
         self.auto_chapters = auto_chapters  # type: str
         self.meeting_assistance = meeting_assistance  # type: str
         self.ppt_extraction = ppt_extraction  # type: str
         self.summarization = summarization  # type: str
+        self.text_polish = text_polish  # type: str
         self.transcription = transcription  # type: str
         self.translation = translation  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -792,14 +793,16 @@
             result['AutoChapters'] = self.auto_chapters
         if self.meeting_assistance is not None:
             result['MeetingAssistance'] = self.meeting_assistance
         if self.ppt_extraction is not None:
             result['PptExtraction'] = self.ppt_extraction
         if self.summarization is not None:
             result['Summarization'] = self.summarization
+        if self.text_polish is not None:
+            result['TextPolish'] = self.text_polish
         if self.transcription is not None:
             result['Transcription'] = self.transcription
         if self.translation is not None:
             result['Translation'] = self.translation
         return result
 
     def from_map(self, m=None):
@@ -808,14 +811,16 @@
             self.auto_chapters = m.get('AutoChapters')
         if m.get('MeetingAssistance') is not None:
             self.meeting_assistance = m.get('MeetingAssistance')
         if m.get('PptExtraction') is not None:
             self.ppt_extraction = m.get('PptExtraction')
         if m.get('Summarization') is not None:
             self.summarization = m.get('Summarization')
+        if m.get('TextPolish') is not None:
+            self.text_polish = m.get('TextPolish')
         if m.get('Transcription') is not None:
             self.transcription = m.get('Transcription')
         if m.get('Translation') is not None:
             self.translation = m.get('Translation')
         return self
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO` & `alibabacloud_tingwu20230930_py2-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-tingwu20230930-py2
-Version: 2.0.6
+Name: alibabacloud_tingwu20230930_py2
+Version: 2.0.7
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.6/setup.py` & `alibabacloud_tingwu20230930_py2-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tingwu20230930_py2.
 
-Created on 18/03/2024
+Created on 10/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tingwu20230930"
 NAME = "alibabacloud_tingwu20230930_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud tingwu (20230930) SDK Library for Python2"
```

