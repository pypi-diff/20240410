# Comparing `tmp/velikafkaclient-1.1.8.tar.gz` & `tmp/velikafkaclient-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.1.8.tar", last modified: Mon Oct 30 09:13:01 2023, max compression
+gzip compressed data, was "velikafkaclient-1.1.9.tar", last modified: Mon Oct 30 09:29:21 2023, max compression
```

## Comparing `velikafkaclient-1.1.8.tar` & `velikafkaclient-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:13:01.712510 velikafkaclient-1.1.8/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-10-30 09:13:01.712343 velikafkaclient-1.1.8/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2787 2023-07-17 15:51:48.000000 velikafkaclient-1.1.8/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-10-30 09:13:01.712543 velikafkaclient-1.1.8/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-10-30 09:12:55.000000 velikafkaclient-1.1.8/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:13:01.711007 velikafkaclient-1.1.8/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     6204 2023-10-30 06:51:06.000000 velikafkaclient-1.1.8/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.1.8/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:13:01.711802 velikafkaclient-1.1.8/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.1.8/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.1.8/velikafkaclient/killer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2420 2023-08-09 12:10:38.000000 velikafkaclient-1.1.8/velikafkaclient/producer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1243 2023-07-17 15:51:48.000000 velikafkaclient-1.1.8/velikafkaclient/topicmanager.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:13:01.712157 velikafkaclient-1.1.8/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.1.8/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:13:01.711475 velikafkaclient-1.1.8/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-10-30 09:13:01.000000 velikafkaclient-1.1.8/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-10-30 09:13:01.000000 velikafkaclient-1.1.8/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-10-30 09:13:01.000000 velikafkaclient-1.1.8/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-10-30 09:13:01.000000 velikafkaclient-1.1.8/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:29:21.798446 velikafkaclient-1.1.9/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-10-30 09:29:21.798236 velikafkaclient-1.1.9/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2787 2023-07-17 15:51:48.000000 velikafkaclient-1.1.9/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-10-30 09:29:21.798485 velikafkaclient-1.1.9/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-10-30 09:29:15.000000 velikafkaclient-1.1.9/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:29:21.796461 velikafkaclient-1.1.9/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     6302 2023-10-30 09:28:58.000000 velikafkaclient-1.1.9/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      725 2023-07-12 11:24:44.000000 velikafkaclient-1.1.9/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:29:21.797516 velikafkaclient-1.1.9/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      165 2023-07-12 08:29:23.000000 velikafkaclient-1.1.9/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-12 05:57:42.000000 velikafkaclient-1.1.9/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2420 2023-08-09 12:10:38.000000 velikafkaclient-1.1.9/velikafkaclient/producer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1243 2023-07-17 15:51:48.000000 velikafkaclient-1.1.9/velikafkaclient/topicmanager.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:29:21.797935 velikafkaclient-1.1.9/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.1.9/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-10-30 09:29:21.797059 velikafkaclient-1.1.9/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2973 2023-10-30 09:29:21.000000 velikafkaclient-1.1.9/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      635 2023-10-30 09:29:21.000000 velikafkaclient-1.1.9/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-10-30 09:29:21.000000 velikafkaclient-1.1.9/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-10-30 09:29:21.000000 velikafkaclient-1.1.9/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.1.8/PKG-INFO` & `velikafkaclient-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.1.8/readme.md` & `velikafkaclient-1.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/consumer.py` & `velikafkaclient-1.1.9/velikafkaclient/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         if topic not in self.events:
             self.events[topic] = []
         self.events[topic].append(event)
 
     def reset(self):
         self.events = dict()
 
+    def size(self):
+        res = 0
+        for t in self.events:
+            res += len(self.events[t])
+        return res
+
 
 class EventRate:
     processed_batch_count: int = 0
     batch = Batch()
     session_start_time = time.time()
     batch_session_start_time = time.time()
 
@@ -144,16 +150,15 @@
                     elif event.error():
                         # TODO what to do ?
                         raise KafkaException(event.error())
                 else:
 
                     self.event_rate.batch.add(event)
 
-                    if batch_time_lapse >= self.rate_limit.batch_waiting_time or len(
-                            self.event_rate.batch) >= self.rate_limit.batch_size:
+                    if batch_time_lapse >= self.rate_limit.batch_waiting_time or self.event_rate.batch.size() >= self.rate_limit.batch_size:
                         self.process_events(time_now)
 
                     time_lapse = time_now - self.event_rate.session_start_time
                     if time_lapse >= 60:
                         self.event_rate.processed_batch_count = 0
                         self.event_rate.session_start_time = time_now
                     else:
```

### Comparing `velikafkaclient-1.1.8/velikafkaclient/decorators.py` & `velikafkaclient-1.1.9/velikafkaclient/decorators.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/eventregistration.py` & `velikafkaclient-1.1.9/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.1.9/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/producer.py` & `velikafkaclient-1.1.9/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/topicmanager.py` & `velikafkaclient-1.1.9/velikafkaclient/topicmanager.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.1.9/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.1.8/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.1.9/velikafkaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.1.8/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.1.9/velikafkaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

