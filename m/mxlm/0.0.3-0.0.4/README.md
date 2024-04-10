# Comparing `tmp/mxlm-0.0.3.tar.gz` & `tmp/mxlm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.3.tar", last modified: Tue Apr  9 09:58:35 2024, max compression
+gzip compressed data, was "mxlm-0.0.4.tar", last modified: Wed Apr 10 03:17:26 2024, max compression
```

## Comparing `mxlm-0.0.3.tar` & `mxlm-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.745833 mxlm-0.0.3/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.3/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-09 09:58:35.741833 mxlm-0.0.3/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.3/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.741833 mxlm-0.0.3/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-09 09:57:04.000000 mxlm-0.0.3/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.3/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     4794 2024-04-09 09:56:46.000000 mxlm-0.0.3/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2023 2024-04-07 12:48:14.000000 mxlm-0.0.3/mxlm/chatmd_utils.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-09 09:58:35.741833 mxlm-0.0.3/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-09 09:58:35.000000 mxlm-0.0.3/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.3/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-09 09:58:35.745833 mxlm-0.0.3/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.3/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 03:17:26.678816 mxlm-0.0.4/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.4/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-10 03:17:26.678816 mxlm-0.0.4/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.4/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 03:17:26.678816 mxlm-0.0.4/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-10 03:14:53.000000 mxlm-0.0.4/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.4/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     4999 2024-04-10 03:15:58.000000 mxlm-0.0.4/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2023 2024-04-07 12:48:14.000000 mxlm-0.0.4/mxlm/chatmd_utils.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 03:17:26.678816 mxlm-0.0.4/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-10 03:17:26.000000 mxlm-0.0.4/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-10 03:17:26.000000 mxlm-0.0.4/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-10 03:17:26.000000 mxlm-0.0.4/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-10 03:17:26.000000 mxlm-0.0.4/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-10 03:17:26.000000 mxlm-0.0.4/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.4/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-10 03:17:26.678816 mxlm-0.0.4/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.4/setup.py
```

### Comparing `mxlm-0.0.3/README.md` & `mxlm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.3/mxlm/__info__.py` & `mxlm-0.0.4/mxlm/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.3/mxlm/chat_api.py` & `mxlm-0.0.4/mxlm/chat_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,69 +53,69 @@
     def convert_to_messages(msgs):
         if msgs is None:
             return None
         if isinstance(msgs, str):
             return [{"role": "user", "content": msgs}]
         if isinstance(msgs, dict):
             messages = []
-            for role in ["system", "context", "user"]:
+            for role in ["system", "context", "user", "assistant"]:
                 if role in msgs:
-                    messages.append(dict(role=role, context=msgs[role]))
+                    messages.append(dict(role=role, content=msgs[role]))
             return messages
         return msgs
 
     def __call__(
         self, messages=None, return_messages=False, return_dict=False, **kwargs_
     ):
         """
-        messages support str, dict for convenient, e.g.:
+        messages support str, dict for convenient single-round dialogue, e.g.:
         >>> client("Tell me a joke.")
         >>> client(
             {
                 "system": "you are a helpful assistant.",
-                "context": "Here are some examples of jokes...",
                 "user": "Tell me a joke."
                 }
             )
         Returns new message.content by default
         """
         messages = messages or self.default_messages
         messages = self.convert_to_messages(messages)
         kwargs = self.default_kwargs.copy()
         kwargs.update(kwargs_)
         if "stream" in kwargs:
             kwargs["stream"] = bool(kwargs["stream"])
         response = self.client.chat.completions.create(messages=messages, **kwargs)
-
         if kwargs.get("stream"):
             content = ""
             chunki = -1
-            for tryi in range(
-                1, 15
-            ):  # TODO: remove this Temporary solution for empty stream
+            for tryi in range(1, 6):
+                # TODO: remove this Temporary solution for empty stream
                 for chunki, chunk in enumerate(response):
                     if not chunki:
                         role = chunk.choices[0].delta.role
                     delta = chunk.choices[0].delta.content
                     if delta:
                         content += delta
                         print(delta, end="")
                 if chunki == -1:
                     # print("retry!"*5)
                     import warnings
 
                     warnings.warn(
-                        f"Empty stream, ChatAPI retry {tryi}st time",
+                        f'Empty stream! ChatAPI(model="{kwargs.get("model")}") retry {tryi}st time',
                         category=UserWarning,
                     )
                     response = self.client.chat.completions.create(
                         messages=messages, **kwargs
                     )
                 else:
                     break
+            assert (
+                response.response.status_code == 200
+            ), f"status_code: {response.response.status_code}"
             chunk.choices[0].message = chunk.choices[0].delta
             del chunk.choices[0].delta
             chunk.choices[0].message.content = content
             chunk.choices[0].message.role = role
             response = chunk
             print(f"<|{response.choices[0].finish_reason}|>")
         # assert response.status_code == 200, response.status_code
@@ -124,14 +124,18 @@
             d["new_messages"] = messages + [d["choices"][0]["message"]]
             if return_dict:
                 return d
             elif return_messages:
                 return d["new_messages"]
         return response.choices[0].message.content
 
+    @property
+    def model(self):
+        return self.default_kwargs.get("model")
+
     def __str__(self):
         import json
 
         kwargs_str = json.dumps(self.default_kwargs, indent=2)
         return f"mxlm.ChatAPI{tuple([self.base_url])}:\n{kwargs_str[2:-2]}"
 
     __repr__ = __str__
```

### Comparing `mxlm-0.0.3/mxlm/chatmd_utils.py` & `mxlm-0.0.4/mxlm/chatmd_utils.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.3/setup.py` & `mxlm-0.0.4/setup.py`

 * *Files identical despite different names*

