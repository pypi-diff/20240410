# Comparing `tmp/pih-msg_q-0.1.tar.gz` & `tmp/pih-msg_q-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-msg_q-0.1.tar", last modified: Mon Feb 26 09:02:54 2024, max compression
+gzip compressed data, was "pih-msg_q-0.11.tar", last modified: Wed Apr 10 01:50:57 2024, max compression
```

## Comparing `pih-msg_q-0.1.tar` & `pih-msg_q-0.11.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 09:02:53.932912 pih-msg_q-0.1/
-drwxrwxrwx   0        0        0        0 2024-02-26 09:02:53.964152 pih-msg_q-0.1/MessageQueueService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.1/MessageQueueService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.1/MessageQueueService/__main__.py
--rw-rw-rw-   0        0        0      440 2024-02-26 08:55:15.000000 pih-msg_q-0.1/MessageQueueService/const.py
--rw-rw-rw-   0        0        0     3197 2024-02-15 01:56:53.000000 pih-msg_q-0.1/MessageQueueService/service.py
--rw-rw-rw-   0        0        0      253 2024-02-26 09:02:54.307892 pih-msg_q-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-15 00:50:20.000000 pih-msg_q-0.1/msg_q_build.py
-drwxrwxrwx   0        0        0        0 2024-02-26 09:02:54.073630 pih-msg_q-0.1/pih_msg_q.egg-info/
--rw-rw-rw-   0        0        0      253 2024-02-26 09:02:52.000000 pih-msg_q-0.1/pih_msg_q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-02-26 09:02:53.000000 pih-msg_q-0.1/pih_msg_q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 09:02:52.000000 pih-msg_q-0.1/pih_msg_q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-02-26 09:02:52.000000 pih-msg_q-0.1/pih_msg_q.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-02-26 09:02:52.000000 pih-msg_q-0.1/pih_msg_q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-26 09:02:53.000000 pih-msg_q-0.1/pih_msg_q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 09:02:54.323514 pih-msg_q-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.889932 pih-msg_q-0.11/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.529487 pih-msg_q-0.11/MessageQueueService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.11/MessageQueueService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.11/MessageQueueService/__main__.py
+-rw-rw-rw-   0        0        0      441 2024-04-10 00:33:19.000000 pih-msg_q-0.11/MessageQueueService/const.py
+-rw-rw-rw-   0        0        0     3184 2024-04-10 00:34:39.000000 pih-msg_q-0.11/MessageQueueService/service.py
+-rw-rw-rw-   0        0        0      275 2024-04-10 01:50:57.858682 pih-msg_q-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.826376 pih-msg_q-0.11/pih_msg_q.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:50:57.905562 pih-msg_q-0.11/setup.cfg
```

### Comparing `pih-msg_q-0.1/MessageQueueService/service.py` & `pih-msg_q-0.11/MessageQueueService/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ipih
 
 from pih import A, PIHThread
 from pih.collections import Message
 from MessageQueueService.const import SD
 from pih.tools import ParameterList, while_not_do, ne, j, js
 
-# version 1.0
+
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 from collections import defaultdict
 from time import sleep
 import random
```

