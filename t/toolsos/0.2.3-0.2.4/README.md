# Comparing `tmp/toolsos-0.2.3.tar.gz` & `tmp/toolsos-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolsos-0.2.3.tar", last modified: Tue Apr  2 13:02:06 2024, max compression
+gzip compressed data, was "toolsos-0.2.4.tar", last modified: Wed Apr 10 08:06:58 2024, max compression
```

## Comparing `toolsos-0.2.3.tar` & `toolsos-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.095486 toolsos-0.2.3/
--rw-rw-rw-   0        0        0     2418 2024-04-02 13:02:06.093658 toolsos-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2024-03-28 08:46:48.000000 toolsos-0.2.3/README.md
--rw-rw-rw-   0        0        0     1106 2024-04-02 13:01:51.000000 toolsos-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 13:02:06.095486 toolsos-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.033057 toolsos-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.049548 toolsos-0.2.3/src/toolsos/
--rw-rw-rw-   0        0        0        0 2023-03-09 08:54:45.000000 toolsos-0.2.3/src/toolsos/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-03-03 07:40:20.000000 toolsos-0.2.3/src/toolsos/cbs_tools.py
--rw-rw-rw-   0        0        0      908 2023-10-26 12:51:00.000000 toolsos-0.2.3/src/toolsos/create_tables.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.063713 toolsos-0.2.3/src/toolsos/database/
--rw-rw-rw-   0        0        0     3362 2024-03-17 13:47:51.000000 toolsos-0.2.3/src/toolsos/database/database_connection.py
--rw-rw-rw-   0        0        0     1827 2023-10-26 12:54:46.000000 toolsos-0.2.3/src/toolsos/database/database_transfer.py
--rw-rw-rw-   0        0        0     2652 2023-10-26 12:50:51.000000 toolsos-0.2.3/src/toolsos/download.py
--rw-rw-rw-   0        0        0     2412 2023-10-26 12:54:11.000000 toolsos-0.2.3/src/toolsos/geo.py
--rw-rw-rw-   0        0        0      997 2023-10-26 12:54:09.000000 toolsos-0.2.3/src/toolsos/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.067702 toolsos-0.2.3/src/toolsos/huisstijl/
--rw-rw-rw-   0        0        0        0 2024-03-09 19:45:08.000000 toolsos-0.2.3/src/toolsos/huisstijl/__init__.py
--rw-rw-rw-   0        0        0     1484 2024-03-09 07:47:07.000000 toolsos-0.2.3/src/toolsos/huisstijl/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.080024 toolsos-0.2.3/src/toolsos/huisstijl/graphs/
--rw-rw-rw-   0        0        0        0 2023-10-20 10:05:27.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/__init__.py
--rw-rw-rw-   0        0        0     2582 2023-10-23 07:17:11.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/bargraph.py
--rw-rw-rw-   0        0        0      827 2024-03-16 18:43:22.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/graph_styles.py
--rw-rw-rw-   0        0        0      659 2024-03-28 14:55:10.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/linegraph.py
--rw-rw-rw-   0        0        0      666 2024-03-28 14:54:10.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/piegraph.py
--rw-rw-rw-   0        0        0     6626 2024-03-17 10:18:59.000000 toolsos-0.2.3/src/toolsos/huisstijl/graphs/styler.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.088489 toolsos-0.2.3/src/toolsos/huisstijl/tables/
--rw-rw-rw-   0        0        0        0 2024-03-09 19:50:14.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/__init__.py
--rw-rw-rw-   0        0        0     2037 2024-03-28 10:12:33.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/table_helpers.py
--rw-rw-rw-   0        0        0     1343 2024-03-14 13:23:41.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/table_styles.py
--rw-rw-rw-   0        0        0    23575 2024-04-02 13:01:28.000000 toolsos-0.2.3/src/toolsos/huisstijl/tables/tables.py
--rw-rw-rw-   0        0        0      770 2023-10-26 12:50:56.000000 toolsos-0.2.3/src/toolsos/polars_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:02:06.090487 toolsos-0.2.3/src/toolsos.egg-info/
--rw-rw-rw-   0        0        0     2418 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 13:02:06.000000 toolsos-0.2.3/src/toolsos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.833150 toolsos-0.2.4/
+-rw-rw-rw-   0        0        0     2418 2024-04-10 08:06:58.831152 toolsos-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2024-03-28 08:46:48.000000 toolsos-0.2.4/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-10 08:06:30.000000 toolsos-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 08:06:58.833150 toolsos-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.770338 toolsos-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.787662 toolsos-0.2.4/src/toolsos/
+-rw-rw-rw-   0        0        0        0 2023-03-09 08:54:45.000000 toolsos-0.2.4/src/toolsos/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-03-03 07:40:20.000000 toolsos-0.2.4/src/toolsos/cbs_tools.py
+-rw-rw-rw-   0        0        0      908 2023-10-26 12:51:00.000000 toolsos-0.2.4/src/toolsos/create_tables.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.800454 toolsos-0.2.4/src/toolsos/database/
+-rw-rw-rw-   0        0        0     4920 2024-04-09 14:08:11.000000 toolsos-0.2.4/src/toolsos/database/database_connection.py
+-rw-rw-rw-   0        0        0     1827 2023-10-26 12:54:46.000000 toolsos-0.2.4/src/toolsos/database/database_transfer.py
+-rw-rw-rw-   0        0        0     2652 2023-10-26 12:50:51.000000 toolsos-0.2.4/src/toolsos/download.py
+-rw-rw-rw-   0        0        0     2412 2023-10-26 12:54:11.000000 toolsos-0.2.4/src/toolsos/geo.py
+-rw-rw-rw-   0        0        0      997 2023-10-26 12:54:09.000000 toolsos-0.2.4/src/toolsos/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.803454 toolsos-0.2.4/src/toolsos/huisstijl/
+-rw-rw-rw-   0        0        0        0 2024-03-09 19:45:08.000000 toolsos-0.2.4/src/toolsos/huisstijl/__init__.py
+-rw-rw-rw-   0        0        0     1484 2024-03-09 07:47:07.000000 toolsos-0.2.4/src/toolsos/huisstijl/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.816493 toolsos-0.2.4/src/toolsos/huisstijl/graphs/
+-rw-rw-rw-   0        0        0        0 2023-10-20 10:05:27.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/__init__.py
+-rw-rw-rw-   0        0        0     2815 2024-04-04 09:08:51.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/bargraph.py
+-rw-rw-rw-   0        0        0      975 2024-04-04 09:07:49.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/graph_styles.py
+-rw-rw-rw-   0        0        0      698 2024-04-04 09:13:16.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/linegraph.py
+-rw-rw-rw-   0        0        0      714 2024-04-04 09:13:35.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/piegraph.py
+-rw-rw-rw-   0        0        0     6623 2024-04-04 09:14:54.000000 toolsos-0.2.4/src/toolsos/huisstijl/graphs/styler.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.823595 toolsos-0.2.4/src/toolsos/huisstijl/tables/
+-rw-rw-rw-   0        0        0        0 2024-03-09 19:50:14.000000 toolsos-0.2.4/src/toolsos/huisstijl/tables/__init__.py
+-rw-rw-rw-   0        0        0     2037 2024-03-28 10:12:33.000000 toolsos-0.2.4/src/toolsos/huisstijl/tables/table_helpers.py
+-rw-rw-rw-   0        0        0     1343 2024-03-14 13:23:41.000000 toolsos-0.2.4/src/toolsos/huisstijl/tables/table_styles.py
+-rw-rw-rw-   0        0        0    23967 2024-04-10 08:06:12.000000 toolsos-0.2.4/src/toolsos/huisstijl/tables/tables.py
+-rw-rw-rw-   0        0        0      770 2023-10-26 12:50:56.000000 toolsos-0.2.4/src/toolsos/polars_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-10 08:06:58.826491 toolsos-0.2.4/src/toolsos.egg-info/
+-rw-rw-rw-   0        0        0     2418 2024-04-10 08:06:58.000000 toolsos-0.2.4/src/toolsos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2024-04-10 08:06:58.000000 toolsos-0.2.4/src/toolsos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 08:06:58.000000 toolsos-0.2.4/src/toolsos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-10 08:06:58.000000 toolsos-0.2.4/src/toolsos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 08:06:58.000000 toolsos-0.2.4/src/toolsos.egg-info/top_level.txt
```

### Comparing `toolsos-0.2.3/PKG-INFO` & `toolsos-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolsos
-Version: 0.2.3
+Version: 0.2.4
 Summary: OS tools
 Author-email: OS <d.schmitz@amsterdam.nl>
 Keywords: tools,Onderzoek & Statistiek
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `toolsos-0.2.3/README.md` & `toolsos-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/pyproject.toml` & `toolsos-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toolsos"
-version = "0.2.3"
+version = "0.2.4"
 description = "OS tools"
 readme = "README.md"
 authors = [{ name = "OS", email = "d.schmitz@amsterdam.nl" }]
 
 # license = { file = "LICENSE" }
 
 classifiers = [
```

### Comparing `toolsos-0.2.3/src/toolsos/cbs_tools.py` & `toolsos-0.2.4/src/toolsos/cbs_tools.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/create_tables.py` & `toolsos-0.2.4/src/toolsos/create_tables.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/database/database_connection.py` & `toolsos-0.2.4/src/toolsos/database/database_connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import getpass
 import json
+import os
 import subprocess
 from json import JSONDecodeError
+from pathlib import Path
 from typing import Optional
 
 import keyring
 import yaml
 
 
 def get_db_connection_strings(
@@ -95,14 +97,71 @@
 
     try:
         json.loads(result.stdout)["accessToken"]
     except JSONDecodeError:
         subprocess.run("az login", shell=True)
 
 
+def get_token_from_pgpass() -> None:
+    p = Path(os.getenv("APPDATA")) / "postgresql" / "pgpass.conf"
+    with open(p) as f:
+        token = f.readline().split(":")[4]
+
+    return token
+
+
+def write_pgpass(
+    host: str, port: str, database: str, user: str, path: str | None = None
+) -> None:
+    password = get_azure_access_token()
+    conn_string = f"{host}:{port}:{database}:{user}:{password}"
+
+    if not path:
+        if os.name == "nt":
+            path = Path(os.getenv("APPDATA")) / "postgresql" / "pgpass.conf"
+        else:
+            path = Path("$home/.pgpass")
+
+    if not path.parent.exists():
+        path.parent.mkdir()
+
+    with open(path, "w") as f:
+        f.write(conn_string)
+
+    if os.name != "nt":
+        path.chmod("0600")
+
+
+def write_multiple_pgpass(conn_details, path: str | None = None):
+    password = get_azure_access_token()
+
+    conn_strings = []
+    for c in conn_details:
+        c_string = f'{c["host"]}:{c["port"]}:{c["database"]}:{c["user"]}:{password}'
+        conn_strings.append(c_string)
+
+    if not path:
+        if os.name == "nt":
+            path = Path(os.getenv("APPDATA")) / "postgresql" / "pgpass.conf"
+        else:
+            path = Path("$home/.pgpass")
+
+    if not path.parent.exists():
+        path.parent.mkdir()
+
+    with open(path, "w") as f:
+        f.writelines(line + "\n" for line in conn_strings)
+
+    if os.name != "nt":
+        path.chmod("0600")
+
+
+# Writing connection settings to pgpass.conf
+
+
 if __name__ == "__main__":
     ...
     # Examples
 
     # Get database connection settings from yaml
     engine_strings = get_db_connection_strings(
         "src/toolsos/database/database_config.yml"
```

### Comparing `toolsos-0.2.3/src/toolsos/database/database_transfer.py` & `toolsos-0.2.4/src/toolsos/database/database_transfer.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/download.py` & `toolsos-0.2.4/src/toolsos/download.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/geo.py` & `toolsos-0.2.4/src/toolsos/geo.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/helpers.py` & `toolsos-0.2.4/src/toolsos/helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/colors.py` & `toolsos-0.2.4/src/toolsos/huisstijl/colors.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/graphs/bargraph.py` & `toolsos-0.2.4/src/toolsos/huisstijl/graphs/bargraph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import plotly.express as px
+
 from .styler import BaseStyle
 
 basestyle = BaseStyle()
 
 
 def bar(
     data,
@@ -10,22 +11,23 @@
     y: str,
     color: str = None,
     color_discrete_sequence: list = None,
     orientation: str = None,
     barmode=None,
     width=750,
     height=490,
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = px.bar(
         data_frame=data,
         x=x,
         y=y,
         color=color,
-        template=basestyle.get_base_template("bar", orientation=orientation),
+        template=basestyle.get_base_template("bar", orientation=orientation, font=font),
         width=width,
         color_discrete_sequence=color_discrete_sequence,
         height=height,
         barmode=barmode,
         **kwargs,
     )
 
@@ -39,24 +41,26 @@
 def stacked_single(
     data,
     x: str,
     y: str,
     color: str = None,
     color_discrete_sequence: list = None,
     orientation="v",
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = bar(
         data=data,
         x=x,
         y=y,
         color=color,
         color_discrete_sequence=color_discrete_sequence,
         barmode="relative",
         orientation=orientation,
+        font=font,
         **kwargs,
     )
 
     if orientation == "v":
         fig.update_xaxes(showticklabels=False)
     if orientation == "h":
         fig.update_yaxes(showticklabels=False)
@@ -67,67 +71,73 @@
 def stacked_multiple(
     data,
     x: str,
     y: str,
     color: str = None,
     color_discrete_sequence: list = None,
     orientation="v",
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = bar(
         data=data,
         x=x,
         y=y,
         color=color,
         color_discrete_sequence=color_discrete_sequence,
         barmode="stack",
         orientation=orientation,
+        font=font,
         **kwargs,
     )
 
     return fig
 
 
 def grouped(
     data,
     x: str,
     y: str,
     color: str = None,
     color_discrete_sequence: list = None,
     orientation="v",
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = bar(
         data=data,
         x=x,
         y=y,
         color=color,
         color_discrete_sequence=color_discrete_sequence,
         barmode="group",
         orientation=orientation,
+        font=font,
         **kwargs,
     )
 
     return fig
 
 
 def single(
     data,
     x: str,
     y: str,
     color_discrete_sequence: list = None,
     orientation="v",
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = bar(
         data=data,
         x=x,
         y=y,
         color_discrete_sequence=color_discrete_sequence,
         orientation=orientation,
+        font=font,
         **kwargs,
     )
 
     if orientation == "h":
         fig.update_yaxes(automargin=True)
 
     return fig
```

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/graphs/graph_styles.py` & `toolsos-0.2.4/src/toolsos/huisstijl/graphs/graph_styles.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     "gridcolor": "#E8E8E8",
     "separators": ",",
 }
 
 
 STYLE_NEW = {
     "font_bold": {"family": "Amsterdam Sans ExtraBold, Corbel", "size": 15},
+    "font_bold_corbel": {"family": "Corbel Bold", "size": 15},
     "font": {"family": "Amsterdam Sans, Corbel", "size": 15},
-    "axis_font": {"family": font, "size": 15},
+    "font_corbel": {"family": "Corbel", "size": 15},
+    "axis_font": {"family": "Amsterdam Sans ExtraBold, Corbel", "size": 15},
     "plot_bgcolor": "#FFFFFF",
     "gridline_color": "#dbdbdb",
     "gridline_width": 0.75,
     "showline": True,
     "showgrid": False,
     "zerolinecolor": "#dbdbdb",
     "gridcolor": "#dbdbdb",
```

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/graphs/piegraph.py` & `toolsos-0.2.4/src/toolsos/huisstijl/graphs/piegraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,27 @@
     names,
     values,
     hole: float = 0.4,
     width=750,
     height=490,
     text_format: str = None,
     color_discrete_sequence=None,
+    font="Amsterdam Sans",
     **kwargs,
 ):
     fig = px.pie(
         data_frame=data,
         names=names,
         values=values,
         width=width,
         height=height,
         hole=hole,
         template=BaseStyle().get_base_template(),
         color_discrete_sequence=color_discrete_sequence,
+        font=font,
         **kwargs,
     )
 
     if text_format:
         fig.update_traces(texttemplate=text_format)
 
     return fig
```

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/graphs/styler.py` & `toolsos-0.2.4/src/toolsos/huisstijl/graphs/styler.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,64 +105,71 @@
         if style_path is None:
             self.style = STYLE_NEW
         else:
             with open(style_path) as file:
                 self.style = json.load(file)
 
     def _get_axis_format(self):
-        self.gridline_color = "#dbdbdb"  # Jorren vragen om deze aan te passen
 
         return {
             "zerolinecolor": self.style["gridline_color"],
             "gridcolor": self.style["gridline_color"],
             "gridwidth": self.style["gridline_width"],
             "showline": True,
             "linewidth": self.style["gridline_width"],
             "linecolor": self.style["gridline_color"],
             "showgrid": self.style["showgrid"],
         }
 
-    def _get_base_template_layout(self):
+    def _get_base_template_layout(self, font):
+        if font == "Amsterdam Sans":
+            font_ = self.style["font"]
+            font_bold_ = self.style["font_bold"]
+        elif font == "Corbel":
+            font_ = self.style["font_corbel"]
+            font_bold_ = self.style["font_bold_corbel"]
+        else:
+            raise ValueError("Font should be 'Amsterdam Sans' or 'Corbel'")
+
         return go.layout.Template(
             layout={
-                # "font": self.styles["font_bold"],
                 "xaxis": {
-                    "tickfont": self.style["font_bold"],
+                    "tickfont": font_bold_,
                 },
                 "yaxis": {
-                    "tickfont": {
-                        "family": self.style["axis_font"]["family"],
-                        "size": self.style["axis_font"]["size"],
-                    },
+                    "tickfont": font_bold_,
                 },
-                "legend": {"font": self.style["font"]},
+                "legend": {"font": font_},
                 "plot_bgcolor": self.style["plot_bgcolor"],
-                # "colorway": self.colors["darkblue_lightblue_gradient_5"],
-                "separators": ",",  # Jorren vragen om deze toe te voegen
-                "font": self.style["font_bold"],
+                "separators": ",",
+                "font": font_bold_,
             }
         )
 
     def get_base_template(
-        self, graph_type: str = None, orientation: str = None, colors: str = None
+        self,
+        graph_type: str = None,
+        orientation: str = None,
+        colors: str = None,
+        font: str = "Amsterdam Sans",
     ):
         """[summary]
 
         Args:
             graph_type (str, optional): Pick 'bar', 'line' or 'bar'. Defaults to None.
             orientation (str, optional): [description]. Pick horizontal ('h') or vertical 'v'. Defaults to None.
             colors (str, optional): Set basecolors. Defaults to None.
 
         Raises:
             ValueError: [description]
 
         Returns:
             [type]: [description]
         """
-        base_template = self._get_base_template_layout()
+        base_template = self._get_base_template_layout(font)
         axis_format = self._get_axis_format()
 
         if graph_type == "bar":
             if orientation in ["v", "vertical"]:
                 base_template.layout.xaxis.update(axis_format)
                 base_template.layout.yaxis.update(zeroline=False)
             elif orientation in ["h", "horizontal"]:
```

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/tables/table_helpers.py` & `toolsos-0.2.4/src/toolsos/huisstijl/tables/table_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/tables/table_styles.py` & `toolsos-0.2.4/src/toolsos/huisstijl/tables/table_styles.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos/huisstijl/tables/tables.py` & `toolsos-0.2.4/src/toolsos/huisstijl/tables/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,15 @@
     ws: Any,
     arr: np.ndarray,
     fmt: Fmt,
     title: str | None = None,
     source: str | None = None,
     col_filter: bool | None = None,
     col_widths: list | None = None,
+    min_column_width: int | None = None,
     cells_to_merge: list[list[int]] | None = None,
 ) -> None:
     """Writing data to worksheet. Used for writing values to cells and formatting the cells
     and
 
     Args:
         ws (Any): openpyxl worksheet
@@ -419,26 +420,33 @@
         filters = ws.auto_filter
         filters.ref = f"A1:{excel_style(len(fmt), len(fmt[0]))}"
 
     if source:
         _insert_source(ws, source, arr)
 
     if col_widths:
-        _set_column_widths(ws, col_widths)
+        _set_column_widths(ws, col_widths, min_column_width)
 
     if title:
         _insert_title(ws, title)
 
     if cells_to_merge:
         _merge_cells(ws, cells_to_merge, title)
 
 
-def _set_column_widths(ws: Any, col_widths: list[int]) -> None:
+def _set_column_widths(
+    ws: Any, col_widths: list[int], min_column_width: int | None
+) -> None:
     for idx, col_width in enumerate(col_widths):
         col_letter = get_column_letter(idx + 1)
+
+        if min_column_width:
+            if col_width < min_column_width:
+                col_width = min_column_width
+
         ws.column_dimensions[col_letter].width = col_width
 
 
 def _merge_cells(ws, cells_to_merge, title: str | None = None) -> None:
     add = 0
     if title:
         add = 1
@@ -489,14 +497,15 @@
     perc_ids: list | None = None,
     perc_pattern: str | None = None,
     perc_col_format: str | None = None,
     blue_border: bool | None = True,
     blue_border_row_ids: int | list[int] | None = None,
     number_format: str = "0.0",
     autofit_columns: str | None = "column_names",
+    min_column_width: int | None = None,
     col_filter: bool | None = False,
     style: str = "old",
     combine_multiindex: bool | int = False,
     column_names_to_string: bool = True,
 ):
     wb = Workbook()
     # Empty sheet is created on Workbook creation
@@ -504,17 +513,14 @@
 
     set_global_style(style)
 
     if not isinstance(data, dict):
         data = {"Sheet1": data}
 
     for sheet_name, df in data.items():
-        if column_names_to_string == True:
-            df = cols_to_str(df)
-
         format_worksheet(
             wb=wb,
             df=df,
             sheet_name=sheet_name,
             header_row=header_row,
             title=title,
             source=source,
@@ -530,14 +536,15 @@
             perc_ids=perc_ids,
             perc_pattern=perc_pattern,
             perc_col_format=perc_col_format,
             blue_border=blue_border,
             blue_border_row_ids=blue_border_row_ids,
             number_format=number_format,
             autofit_columns=autofit_columns,
+            min_column_width=min_column_width,
             col_filter=col_filter,
             combine_multiindex=combine_multiindex,
             column_names_to_string=column_names_to_string,
         )
 
     wb.save(file)
 
@@ -578,14 +585,15 @@
     perc_ids: list | None = None,
     perc_pattern: str | None = None,
     perc_col_format: str | None = None,
     blue_border: bool | None = True,
     blue_border_row_ids: int | list[int] | None = None,
     number_format: str = "0.0",
     autofit_columns: str | None = "column_names",
+    min_column_width: int | None = None,
     col_filter: bool | None = False,
     combine_multiindex: bool | int = False,
     column_names_to_string: bool = True,
 ):
     """_summary_
 
     Args:
@@ -603,14 +611,17 @@
         left_align_pattern (str, optional): Pattern of columns to left align. Defaults to None.
         left_align_string (bool, optional): Left align string columns. Defaults to True.
         perc_ids (list, optional): The ids of the columns to format as percentage. Defaults to None.
         perc_pattern (str, optional): The pattern of columns to format as percentage. Defaults to None.
         perc_col_format (str, optional): The formatting string of percentage columns. Defaults to None.
         col_filter (bool, optional): Set filter on columns. Defaults to False.
     """
+    if column_names_to_string == True:
+        df = cols_to_str(df)
+
     arr = df_to_array(df)
 
     blue_rows = []
     light_blue_rows = []
     light_blue_cols = []
     blue_border_ids = []
     r_align_ids = []
@@ -707,8 +718,9 @@
         arr=arr,
         fmt=fmt,
         title=title_tbl,
         source=title_src,
         col_filter=col_filter,
         col_widths=col_widths,
         cells_to_merge=cells_to_merge,
+        min_column_width=min_column_width,
     )
```

### Comparing `toolsos-0.2.3/src/toolsos/polars_helpers.py` & `toolsos-0.2.4/src/toolsos/polars_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsos-0.2.3/src/toolsos.egg-info/PKG-INFO` & `toolsos-0.2.4/src/toolsos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolsos
-Version: 0.2.3
+Version: 0.2.4
 Summary: OS tools
 Author-email: OS <d.schmitz@amsterdam.nl>
 Keywords: tools,Onderzoek & Statistiek
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `toolsos-0.2.3/src/toolsos.egg-info/SOURCES.txt` & `toolsos-0.2.4/src/toolsos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

