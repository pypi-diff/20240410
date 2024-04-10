# Comparing `tmp/airbyte_source_snapchat_marketing-0.5.0.tar.gz` & `tmp/airbyte_source_snapchat_marketing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_snapchat_marketing-0.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_snapchat_marketing-0.6.0.tar", max compression
```

## Comparing `airbyte_source_snapchat_marketing-0.5.0.tar` & `airbyte_source_snapchat_marketing-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4712 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/README.md
--rw-r--r--   0        0        0      811 2024-03-21 01:54:41.240696 airbyte_source_snapchat_marketing-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1156 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/__init__.py
--rw-r--r--   0        0        0      264 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/run.py
--rw-r--r--   0        0        0     1236 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/adaccounts.json
--rw-r--r--   0        0        0      893 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/ads.json
--rw-r--r--   0        0        0     4855 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/adsquads.json
--rw-r--r--   0        0        0     5087 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/basic_stats.json
--rw-r--r--   0        0        0      767 2024-03-21 01:47:20.749995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0     1829 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/creatives.json
--rw-r--r--   0        0        0     1175 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/media.json
--rw-r--r--   0        0        0     1600 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/organizations.json
--rw-r--r--   0        0        0      980 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/segments.json
--rw-r--r--   0        0        0    30712 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/source.py
--rw-r--r--   0        0        0     2666 2024-03-21 01:47:20.753995 airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/spec.json
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4712 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/README.md
+-rw-r--r--   0        0        0      811 2024-04-10 08:57:27.640394 airbyte_source_snapchat_marketing-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1156 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/__init__.py
+-rw-r--r--   0        0        0      264 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/run.py
+-rw-r--r--   0        0        0     1236 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adaccounts.json
+-rw-r--r--   0        0        0      893 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/ads.json
+-rw-r--r--   0        0        0     4855 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adsquads.json
+-rw-r--r--   0        0        0     5087 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/basic_stats.json
+-rw-r--r--   0        0        0      767 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     1829 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/creatives.json
+-rw-r--r--   0        0        0     1175 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/media.json
+-rw-r--r--   0        0        0     1600 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/organizations.json
+-rw-r--r--   0        0        0      980 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/segments.json
+-rw-r--r--   0        0        0    31941 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/source.py
+-rw-r--r--   0        0        0     3503 2024-04-10 08:39:43.000000 airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/spec.json
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_snapchat_marketing-0.6.0/PKG-INFO
```

### Comparing `airbyte_source_snapchat_marketing-0.5.0/README.md` & `airbyte_source_snapchat_marketing-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/pyproject.toml` & `airbyte_source_snapchat_marketing-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.0"
+version = "0.6.0"
 name = "airbyte-source-snapchat-marketing"
 description = "Source implementation for Snapchat Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/__init__.py` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/adaccounts.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adaccounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/ads.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/adsquads.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/adsquads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/basic_stats.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/basic_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/campaigns.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/creatives.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/media.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/media.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/organizations.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/schemas/segments.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/schemas/segments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/source.py` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,18 +161,21 @@
 
 
 class SnapchatMarketingStream(HttpStream, ABC):
     url_base = "https://adsapi.snapchat.com/v1/"
     primary_key = "id"
     raise_on_http_errors = True
 
-    def __init__(self, start_date, end_date, **kwargs):
+    def __init__(self, start_date, end_date, action_report_time, swipe_up_attribution_window, view_attribution_window, **kwargs):
         super().__init__(**kwargs)
         self.start_date = start_date
         self.end_date = end_date
+        self.action_report_time = action_report_time
+        self.swipe_up_attribution_window = swipe_up_attribution_window
+        self.view_attribution_window = view_attribution_window
 
     def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
         next_page_cursor = response.json().get("paging", False)
         if next_page_cursor:
             return {"cursor": dict(parse_qsl(urlparse(next_page_cursor["next_link"]).query))["cursor"]}
 
     def request_params(
@@ -242,15 +245,22 @@
 
     def stream_slices(self, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
 
         stream_state = kwargs.get("stream_state")
         self.initial_state = stream_state.get(self.cursor_field) if stream_state else self.start_date
         self.max_state = self.initial_state
 
-        parent_stream = self.parent(authenticator=self.authenticator, start_date=self.start_date, end_date=self.end_date)
+        parent_stream = self.parent(
+            authenticator=self.authenticator,
+            start_date=self.start_date,
+            end_date=self.end_date,
+            action_report_time=self.action_report_time,
+            swipe_up_attribution_window=self.swipe_up_attribution_window,
+            view_attribution_window=self.view_attribution_window,
+        )
         stream_slices = get_parent_ids(parent_stream)
 
         if stream_slices:
             self.last_slice = stream_slices[-1]
 
         self.logger.info(f"{self.name} stream slices: {stream_slices}")
 
@@ -364,15 +374,22 @@
     @abstractmethod
     def parent(self) -> SnapchatMarketingStream:
         """Stream Class to extract entity ids from"""
 
     def stream_slices(self, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         """Each stream slice represents each entity id from parent stream"""
 
-        parent_stream = self.parent(authenticator=self.authenticator, start_date=self.start_date, end_date=self.end_date)
+        parent_stream = self.parent(
+            authenticator=self.authenticator,
+            start_date=self.start_date,
+            end_date=self.end_date,
+            action_report_time=self.action_report_time,
+            swipe_up_attribution_window=self.swipe_up_attribution_window,
+            view_attribution_window=self.view_attribution_window,
+        )
         self.parent_name = parent_stream.name
         stream_slices = get_parent_ids(parent_stream)
 
         if not stream_slices:
             self.logger.error(f"No {'id'}s found. {self.name} cannot be extracted without {'id'}.")
 
         self.logger.info(f"Stats: stream_slices:{stream_slices}")
@@ -384,14 +401,17 @@
 
     def request_params(
         self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, any] = None, next_page_token: Mapping[str, Any] = None
     ) -> MutableMapping[str, Any]:
 
         params = super().request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
         params["granularity"] = self.granularity.value
+        params["action_report_time"] = self.action_report_time
+        params["swipe_up_attribution_window"] = self.swipe_up_attribution_window
+        params["view_attribution_window"] = self.view_attribution_window
         if self.metrics:
             params["fields"] = ",".join(self.metrics)
 
         return params
 
     def parse_response(
         self,
@@ -804,14 +824,17 @@
                 token_refresh_endpoint="https://accounts.snapchat.com/login/oauth2/access_token",
                 client_id=config["client_id"],
                 client_secret=config["client_secret"],
                 refresh_token=config["refresh_token"],
             ),
             "start_date": config["start_date"],
             "end_date": config.get("end_date", default_end_date),
+            "action_report_time": config.get("action_report_time", "conversion"),
+            "swipe_up_attribution_window": config.get("swipe_up_attribution_window", "28_DAY"),
+            "view_attribution_window": config.get("view_attribution_window", "1_DAY"),
         }
 
         return [
             # Base streams:
             Adaccounts(**kwargs),
             Ads(**kwargs),
             Adsquads(**kwargs),
```

### Comparing `airbyte_source_snapchat_marketing-0.5.0/source_snapchat_marketing/spec.json` & `airbyte_source_snapchat_marketing-0.6.0/source_snapchat_marketing/spec.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'action_report_time': OrderedDict([('type', "*

 * *                              "'string'), ('enum', ['conversion', 'impression']), ('title', "*

 * *                              "'Action Report Time'), ('description', 'Specifies the principle for "*

 * *                              "conversion reporting.'), ('default', 'conversion'), ('order', 5)]), "*

 * *                              "'swipe_up_attribution_window': OrderedDict([('type', 'string'), "*

 * *                           […]*

```diff
@@ -42,14 +42,25 @@
                 "type": "object"
             }
         }
     },
     "connectionSpecification": {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "properties": {
+            "action_report_time": {
+                "default": "conversion",
+                "description": "Specifies the principle for conversion reporting.",
+                "enum": [
+                    "conversion",
+                    "impression"
+                ],
+                "order": 5,
+                "title": "Action Report Time",
+                "type": "string"
+            },
             "client_id": {
                 "airbyte_secret": true,
                 "description": "The Client ID of your Snapchat developer application.",
                 "order": 0,
                 "title": "Client ID",
                 "type": "string"
             },
@@ -85,14 +96,40 @@
                     "2022-01-01"
                 ],
                 "format": "date",
                 "order": 3,
                 "pattern": "^[0-9]{4}-[0-9]{2}-[0-9]{2}$",
                 "title": "Start Date",
                 "type": "string"
+            },
+            "swipe_up_attribution_window": {
+                "default": "28_DAY",
+                "description": "Attribution window for swipe ups.",
+                "enum": [
+                    "1_DAY",
+                    "7_DAY",
+                    "28_DAY"
+                ],
+                "order": 6,
+                "title": "Swipe Up Attribution Window",
+                "type": "string"
+            },
+            "view_attribution_window": {
+                "default": "1_DAY",
+                "description": "Attribution window for views.",
+                "enum": [
+                    "1_HOUR",
+                    "3_HOUR",
+                    "6_HOUR",
+                    "1_DAY",
+                    "7_DAY"
+                ],
+                "order": 7,
+                "title": "View Attribution Window",
+                "type": "string"
             }
         },
         "required": [
             "client_id",
             "client_secret",
             "refresh_token"
         ],
```

### Comparing `airbyte_source_snapchat_marketing-0.5.0/PKG-INFO` & `airbyte_source_snapchat_marketing-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-snapchat-marketing
-Version: 0.5.0
+Version: 0.6.0
 Summary: Source implementation for Snapchat Marketing.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

