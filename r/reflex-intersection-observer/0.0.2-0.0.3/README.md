# Comparing `tmp/reflex-intersection-observer-0.0.2.tar.gz` & `tmp/reflex-intersection-observer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-intersection-observer-0.0.2.tar", last modified: Wed Mar 13 19:42:21 2024, max compression
+gzip compressed data, was "reflex-intersection-observer-0.0.3.tar", last modified: Wed Apr 10 18:25:10 2024, max compression
```

## Comparing `reflex-intersection-observer-0.0.2.tar` & `reflex-intersection-observer-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-03-13 19:42:21.959060 reflex-intersection-observer-0.0.2/
--rw-r--r--   0 masenf     (501) staff       (20)      994 2024-03-13 19:42:21.958871 reflex-intersection-observer-0.0.2/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      450 2024-03-13 18:59:51.000000 reflex-intersection-observer-0.0.2/README.md
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-03-13 19:42:21.957004 reflex-intersection-observer-0.0.2/custom_components/
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-03-13 19:42:21.957668 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer/
--rw-r--r--   0 masenf     (501) staff       (20)       37 2024-03-13 19:13:04.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer/__init__.py
--rw-r--r--   0 masenf     (501) staff       (20)     3530 2024-03-13 19:13:04.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer/intersection_observer.py
-drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-03-13 19:42:21.958563 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/
--rw-r--r--   0 masenf     (501) staff       (20)      994 2024-03-13 19:42:21.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/PKG-INFO
--rw-r--r--   0 masenf     (501) staff       (20)      504 2024-03-13 19:42:21.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/SOURCES.txt
--rw-r--r--   0 masenf     (501) staff       (20)        1 2024-03-13 19:42:21.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/dependency_links.txt
--rw-r--r--   0 masenf     (501) staff       (20)       33 2024-03-13 19:42:21.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/requires.txt
--rw-r--r--   0 masenf     (501) staff       (20)       29 2024-03-13 19:42:21.000000 reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/top_level.txt
--rw-r--r--   0 masenf     (501) staff       (20)      736 2024-03-13 19:16:36.000000 reflex-intersection-observer-0.0.2/pyproject.toml
--rw-r--r--   0 masenf     (501) staff       (20)       38 2024-03-13 19:42:21.959096 reflex-intersection-observer-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:25:10.334011 reflex-intersection-observer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-10 18:25:10.334011 reflex-intersection-observer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-10 18:24:24.000000 reflex-intersection-observer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:25:10.330011 reflex-intersection-observer-0.0.3/custom_components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:25:10.330011 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 18:24:24.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-10 18:24:24.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer/intersection_observer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:25:10.334011 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-10 18:25:10.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 18:25:10.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:25:10.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 18:25:10.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 18:25:10.000000 reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 18:24:24.000000 reflex-intersection-observer-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:25:10.334011 reflex-intersection-observer-0.0.3/setup.cfg
```

### Comparing `reflex-intersection-observer-0.0.2/PKG-INFO` & `reflex-intersection-observer-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: reflex-intersection-observer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reflex custom component intersection-observer
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-intersection-observer
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: reflex>=0.4.6
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # intersection-observer
 
 React to a component coming into view using Reflex event handler.
```

### Comparing `reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer/intersection_observer.py` & `reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer/intersection_observer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 """Reflex custom component IntersectionObserver."""
-from typing import Any
+
+from jinja2 import Environment
 
 import reflex as rx
 
 
+INTERSECTION_OBSERVER_JS = """
+// reflex_intersection_observer.IntersectionObserver
+useEffect(() => {
+    const observer = new IntersectionObserver((entries) => {
+        entries.forEach((entry) => {
+            if ({{ on_intersect }} && entry.isIntersecting) {
+                {{ on_intersect }}(extractEntry(entry))
+            }
+            if ({{ on_non_intersect }} && !entry.isIntersecting) {
+                {{ on_non_intersect }}(extractEntry(entry))
+            }
+        });
+    }, {
+        root: {{ root }},
+        rootMargin: {{ root_margin }},
+        threshold: {{ threshold }},
+    })
+    if ({{ ref }}.current) {
+        observer.observe({{ ref }}.current)
+        return () => observer.disconnect()
+    }
+}, []);
+"""
+
+
 class IntersectionObserver(rx.el.Div):
     root: rx.Var[str]
     root_margin: rx.Var[str]
     threshold: rx.Var[float]
 
+    on_intersect: rx.EventHandler[lambda e0: [e0]]
+    on_non_intersect: rx.EventHandler[lambda e0: [e0]]
+
     @classmethod
     def create(cls, *children, **props):
         if "id" not in props:
             props["id"] = rx.vars.get_unique_variable_name()
         return super().create(*children, **props)
 
-    def get_event_triggers(self) -> dict[str, Any]:
-        return {
-            **super().get_event_triggers(),
-            "on_intersect": lambda e0: [e0],
-            "on_non_intersect": lambda e0: [e0],
-        }
-
     def _exclude_props(self) -> list[str]:
         return ["root", "root_margin", "threshold", "on_intersect", "on_non_intersect"]
 
     def _get_imports(self) -> dict[str, list[rx.utils.imports.ImportVar]]:
         return rx.utils.imports.merge_imports(
             super()._get_imports(),
             {
@@ -56,53 +78,32 @@
                 rx.utils.format.format_prop(on_non_intersect).strip("{}"),
                 "(",
             )
         if on_intersect is None:
             on_intersect = "undefined"
         if on_non_intersect is None:
             on_non_intersect = "undefined"
-        script_props = dict(
-            on_intersect=on_intersect,
-            on_non_intersect=on_non_intersect,
-            root=(
-                f"document.querySelector({rx.utils.format.format_prop(self.root).strip('{}')})"
-                if self.root is not None
-                else "null"
-            ),
-            root_margin=rx.utils.format.format_prop(
-                self.root_margin if self.root_margin is not None else "0px"
-            ).strip("{}"),
-            threshold=(
-                self.threshold._var_name_unwrapped
-                if self.threshold is not None
-                else "1.0"
-            ),
-            ref=self.get_ref(),
-        )
         return (
-            """
-useEffect(() => {
-    const observer = new IntersectionObserver((entries) => {
-        entries.forEach((entry) => {
-            if (%(on_intersect)s && entry.isIntersecting) {
-                %(on_intersect)s(extractEntry(entry))
-            }
-            if (%(on_non_intersect)s && !entry.isIntersecting) {
-                %(on_non_intersect)s(extractEntry(entry))
-            }
-        });
-    }, {
-        root: %(root)s,
-        rootMargin: %(root_margin)s,
-        threshold: %(threshold)s,
-    })
-    if (%(ref)s.current) {
-        observer.observe(%(ref)s.current)
-        return () => observer.disconnect()
-    }
-}, []);
-"""
-            % script_props
+            Environment()
+            .from_string(INTERSECTION_OBSERVER_JS)
+            .render(
+                on_intersect=on_intersect,
+                on_non_intersect=on_non_intersect,
+                root=(
+                    f"document.querySelector({rx.utils.format.format_prop(self.root).strip('{}')})"
+                    if self.root is not None
+                    else "null"
+                ),
+                root_margin=rx.utils.format.format_prop(
+                    self.root_margin if self.root_margin is not None else "0px"
+                ).strip("{}"),
+                threshold=(
+                    self.threshold._var_name_unwrapped
+                    if self.threshold is not None
+                    else "1.0"
+                ),
+                ref=self.get_ref(),
+            )
         )
 
 
 intersection_observer = IntersectionObserver.create
```

### Comparing `reflex-intersection-observer-0.0.2/custom_components/reflex_intersection_observer.egg-info/PKG-INFO` & `reflex-intersection-observer-0.0.3/custom_components/reflex_intersection_observer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: reflex-intersection-observer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reflex custom component intersection-observer
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/masenf/reflex-intersection-observer
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: jinja2>=3.1.2
+Requires-Dist: reflex>=0.4.6
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # intersection-observer
 
 React to a component coming into view using Reflex event handler.
```

### Comparing `reflex-intersection-observer-0.0.2/pyproject.toml` & `reflex-intersection-observer-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-intersection-observer"
-version = "0.0.2"
+version = "0.0.3"
 description = "Reflex custom component intersection-observer"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
 
 dependencies = [
-    "reflex>=0.4.2"
+    "jinja2>=3.1.2",
+    "reflex>=0.4.6",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
 
 [project.urls]
```

