# Comparing `tmp/neon-messagebus-mq-connector-0.4.1a1.tar.gz` & `tmp/neon-messagebus-mq-connector-0.4.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-messagebus-mq-connector-0.4.1a1.tar", last modified: Sat Jan 20 01:16:05 2024, max compression
+gzip compressed data, was "neon-messagebus-mq-connector-0.4.1a2.tar", last modified: Wed Apr 10 00:21:29 2024, max compression
```

## Comparing `neon-messagebus-mq-connector-0.4.1a1.tar` & `neon-messagebus-mq-connector-0.4.1a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 01:16:05.818692 neon-messagebus-mq-connector-0.4.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-20 01:16:05.818692 neon-messagebus-mq-connector-0.4.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 01:16:05.814692 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 01:16:05.818692 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-20 01:16:05.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-20 01:16:05.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 01:16:05.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-20 01:16:05.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-20 01:16:05.000000 neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 01:16:05.818692 neon-messagebus-mq-connector-0.4.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-20 01:16:02.000000 neon-messagebus-mq-connector-0.4.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:21:29.925107 neon-messagebus-mq-connector-0.4.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 00:21:29.925107 neon-messagebus-mq-connector-0.4.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:21:29.925107 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20636 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:21:29.925107 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 00:21:29.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 00:21:29.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:21:29.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 00:21:29.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 00:21:29.000000 neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:21:29.925107 neon-messagebus-mq-connector-0.4.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-10 00:21:26.000000 neon-messagebus-mq-connector-0.4.1a2/setup.py
```

### Comparing `neon-messagebus-mq-connector-0.4.1a1/LICENSE.md` & `neon-messagebus-mq-connector-0.4.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/PKG-INFO` & `neon-messagebus-mq-connector-0.4.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.4.1a1
+Version: 0.4.1a2
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/__init__.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/__main__.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/config.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/controller.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         self._bus.on('neon.audio_input.response', self.handle_neon_message)
         self._bus.on('neon.get_tts.response', self.handle_neon_message)
         self._bus.on('neon.get_stt.response', self.handle_neon_message)
         self._bus.on('ovos.languages.stt.response', self.handle_neon_message)
         self._bus.on('ovos.languages.tts.response', self.handle_neon_message)
         self._bus.on('neon.languages.skills.response', self.handle_neon_message)
         self._bus.on('neon.languages.get.response', self.handle_neon_message)
+        self._bus.on('neon.alert_expired', self.handle_neon_message)
 
     def connect_bus(self, refresh: bool = False):
         """
         Convenience method for establishing connection to message bus
         :param refresh: To refresh existing connection
         """
         if not self._bus or refresh:
@@ -249,15 +250,17 @@
                 matching_template_model = templates.get(requested_template)
                 if not matching_template_model:
                     LOG.warning(f'Template under keyword '
                                 f'"{requested_template}" does not exist')
                 else:
                     message_templates.append(matching_template_model)
         else:
-            raise ValueError(f"Unable to validate input message: {msg_data}")
+            LOG.warning(f"Handling arbitrary message: {msg_type}")
+            message_templates = [templates.get('message')]
+            # raise ValueError(f"Unable to validate input message: {msg_data}")
         detected_error, msg_data = cls.__validate_message_templates(
             msg_data=msg_data, message_templates=message_templates)
         return detected_error, msg_data
 
     @staticmethod
     def validate_message_context(message: Message) -> bool:
         """
```

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/enums.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/enums.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector/messages.py` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
         extra = "allow"
 
 
+class MessageModel(BaseModel):
+    msg_type: str
+    data: dict
+    context: dict
+
+
 class RecognizerMessage(BaseModel):
     msg_type: str = "recognizer_loop:utterance"
     data: create_model("Data",
                        utterances=(list, ...),
                        lang=(str, ...),
                        __base__=BaseModel,
                        )
@@ -47,15 +53,15 @@
                           client_name=(str, "pyklatchat"),
                           client=(str, "browser"),
                           source=(str, "mq_api"),
                           destination=(list, ["skills"]),
                           timing=(dict, {}),
                           neon_should_respond=(bool, True),
                           username=(str, "guest"),
-                          klat_data=(dict, {'key': 'val'}),
+                          klat_data=(dict, {}),
                           mq=(dict, None),
                           user_profiles=(list, []),
                           request_skills=(List[str], None),
                           __base__=BaseModel,
                           )
 
 
@@ -104,8 +110,9 @@
 
 
 templates = {
     "stt": STTMessage,
     "tts": TTSMessage,
     "audio_input": AudioInput,
     "recognizer": RecognizerMessage,
+    "message": MessageModel
 }
```

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/PKG-INFO` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.4.1a1
+Version: 0.4.1a2
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.4.1a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt` & `neon-messagebus-mq-connector-0.4.1a2/neon_messagebus_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.4.1a1/setup.py` & `neon-messagebus-mq-connector-0.4.1a2/setup.py`

 * *Files identical despite different names*

