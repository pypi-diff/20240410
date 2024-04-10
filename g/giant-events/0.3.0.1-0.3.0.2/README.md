# Comparing `tmp/giant_events-0.3.0.1.tar.gz` & `tmp/giant_events-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant_events-0.3.0.1.tar", max compression
+gzip compressed data, was "giant_events-0.3.0.2.tar", max compression
```

## Comparing `giant_events-0.3.0.1.tar` & `giant_events-0.3.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/LICENSE
--rw-r--r--   0        0        0     3023 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/README.md
--rw-r--r--   0        0        0       22 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/__init__.py
--rw-r--r--   0        0        0     2774 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/admin.py
--rw-r--r--   0        0        0       87 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/apps.py
--rw-r--r--   0        0        0      378 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/cms_apps.py
--rw-r--r--   0        0        0     5508 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0001_initial.py
--rw-r--r--   0        0        0     1065 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0002_add_climatecare_fields.py
--rw-r--r--   0        0        0      704 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/0003_make_fields_optional.py
--rw-r--r--   0        0        0     1034 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/migrations/0004_auto_20220509_0816.py
--rw-r--r--   0        0        0      861 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/migrations/0005_event_hero_image.py
--rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/migrations/__init__.py
--rw-r--r--   0        0        0     3871 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/models.py
--rw-r--r--   0        0        0      324 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/sitemaps.py
--rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/templates/base.html
--rw-r--r--   0        0        0      285 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/templates/events/detail.html
--rw-r--r--   0        0        0     1183 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/templates/events/index.html
--rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.1/events/tests/__init__.py
--rw-r--r--   0        0        0      699 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/conftest.py
--rw-r--r--   0        0        0      279 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/test_cms_apps.py
--rw-r--r--   0        0        0     2601 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/test_models.py
--rw-r--r--   0        0        0     3222 2024-04-09 08:53:51.251891 giant_events-0.3.0.1/events/tests/test_views.py
--rw-r--r--   0        0        0      150 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/tests/urls.py
--rw-r--r--   0        0        0      227 2023-03-22 13:44:55.503946 giant_events-0.3.0.1/events/urls.py
--rw-r--r--   0        0        0     2038 2024-04-09 08:53:51.255891 giant_events-0.3.0.1/events/views.py
--rw-r--r--   0        0        0     1069 2024-04-09 12:53:13.974602 giant_events-0.3.0.1/pyproject.toml
--rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 giant_events-0.3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/LICENSE
+-rw-r--r--   0        0        0     3023 2024-04-09 08:53:51.251891 giant_events-0.3.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/__init__.py
+-rw-r--r--   0        0        0     2774 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/admin.py
+-rw-r--r--   0        0        0       87 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/apps.py
+-rw-r--r--   0        0        0      378 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/cms_apps.py
+-rw-r--r--   0        0        0     5508 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1065 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/migrations/0002_add_climatecare_fields.py
+-rw-r--r--   0        0        0      704 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/migrations/0003_make_fields_optional.py
+-rw-r--r--   0        0        0     1034 2024-04-09 08:53:51.251891 giant_events-0.3.0.2/events/migrations/0004_auto_20220509_0816.py
+-rw-r--r--   0        0        0      861 2024-04-09 08:53:51.251891 giant_events-0.3.0.2/events/migrations/0005_event_hero_image.py
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/migrations/__init__.py
+-rw-r--r--   0        0        0     3871 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/models.py
+-rw-r--r--   0        0        0      324 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/sitemaps.py
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/templates/base.html
+-rw-r--r--   0        0        0      285 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/templates/events/detail.html
+-rw-r--r--   0        0        0     1183 2024-04-09 08:53:51.251891 giant_events-0.3.0.2/events/templates/events/index.html
+-rw-r--r--   0        0        0        0 2023-03-22 13:44:55.499945 giant_events-0.3.0.2/events/tests/__init__.py
+-rw-r--r--   0        0        0      699 2023-03-22 13:44:55.503946 giant_events-0.3.0.2/events/tests/conftest.py
+-rw-r--r--   0        0        0      279 2023-03-22 13:44:55.503946 giant_events-0.3.0.2/events/tests/test_cms_apps.py
+-rw-r--r--   0        0        0     2601 2023-03-22 13:44:55.503946 giant_events-0.3.0.2/events/tests/test_models.py
+-rw-r--r--   0        0        0     3222 2024-04-09 08:53:51.251891 giant_events-0.3.0.2/events/tests/test_views.py
+-rw-r--r--   0        0        0      150 2023-03-22 13:44:55.503946 giant_events-0.3.0.2/events/tests/urls.py
+-rw-r--r--   0        0        0      227 2023-03-22 13:44:55.503946 giant_events-0.3.0.2/events/urls.py
+-rw-r--r--   0        0        0     1961 2024-04-10 13:29:59.796167 giant_events-0.3.0.2/events/views.py
+-rw-r--r--   0        0        0     1069 2024-04-10 13:41:35.758468 giant_events-0.3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4057 1970-01-01 00:00:00.000000 giant_events-0.3.0.2/PKG-INFO
```

### Comparing `giant_events-0.3.0.1/LICENSE` & `giant_events-0.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/README.md` & `giant_events-0.3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/admin.py` & `giant_events-0.3.0.2/events/admin.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/migrations/0001_initial.py` & `giant_events-0.3.0.2/events/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/migrations/0002_add_climatecare_fields.py` & `giant_events-0.3.0.2/events/migrations/0002_add_climatecare_fields.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/migrations/0003_make_fields_optional.py` & `giant_events-0.3.0.2/events/migrations/0003_make_fields_optional.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/migrations/0004_auto_20220509_0816.py` & `giant_events-0.3.0.2/events/migrations/0004_auto_20220509_0816.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/migrations/0005_event_hero_image.py` & `giant_events-0.3.0.2/events/migrations/0005_event_hero_image.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/models.py` & `giant_events-0.3.0.2/events/models.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/templates/events/index.html` & `giant_events-0.3.0.2/events/templates/events/index.html`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/tests/conftest.py` & `giant_events-0.3.0.2/events/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/tests/test_models.py` & `giant_events-0.3.0.2/events/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/tests/test_views.py` & `giant_events-0.3.0.2/events/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `giant_events-0.3.0.1/events/views.py` & `giant_events-0.3.0.2/events/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         if self.TimeDirection.PAST in self.request.GET:
             return self.TimeDirection.PAST
         elif self.TimeDirection.FUTURE in self.request.GET:
             return self.TimeDirection.FUTURE
         else:
             return settings.DEFAULT_TIME_DIRECTION
 
+    @property
+    def extra_context(self):
+        return {"time_direction": self.time_direction}
+
     def get_queryset(self):
         """
         Override get method here to allow us to filter using tags
         """
         time_direction_queryset_mapping = {
             self.TimeDirection.PAST: Event.objects.past(user=self.request.user).order_by(
                 "-start_at", "-publish_at",
@@ -40,20 +44,14 @@
                 "start_at", "-publish_at",
             ),
             "default": Event.objects.published(user=self.request.user).order_by("-publish_at"),
         }
         default = time_direction_queryset_mapping.get("default")
         return time_direction_queryset_mapping.get(self.time_direction, default)
 
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        context["time_direction"] = self.time_direction
-
-        return context
-
 
 class EventDetail(DetailView):
     """
     Detail view for an events object
     """
 
     template_name = "events/detail.html"
```

### Comparing `giant_events-0.3.0.1/pyproject.toml` & `giant_events-0.3.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-events"
-version = "0.3.0.1"
+version = "0.3.0.2"
 description = "A small reusable package that adds an Events app to a project"
 authors = ["Will-Hoey <will.hoey@giantmade.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-events"
 repository = "https://github.com/giantmade/giant-events"
 keywords = ["events", "app"]
```

### Comparing `giant_events-0.3.0.1/PKG-INFO` & `giant_events-0.3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giant-events
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: A small reusable package that adds an Events app to a project
 Home-page: https://github.com/giantmade/giant-events
 License: MIT
 Keywords: events,app
 Author: Will-Hoey
 Author-email: will.hoey@giantmade.com
 Requires-Python: >=3.6.2,<4.0.0
```

