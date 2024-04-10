# Comparing `tmp/grote-0.1.5.tar.gz` & `tmp/grote-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grote-0.1.5.tar", max compression
+gzip compressed data, was "grote-0.1.6.tar", max compression
```

## Comparing `grote-0.1.5.tar` & `grote-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.5/LICENSE
--rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.5/README.md
--rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.5/grote/__init__.py
--rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.5/grote/app.py
--rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.5/grote/collections/__init__.py
--rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.5/grote/collections/base.py
--rw-r--r--   0        0        0     1338 2024-04-09 15:45:56.211676 grote-0.1.5/grote/collections/config.yaml
--rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.5/grote/collections/load.py
--rw-r--r--   0        0        0     8448 2024-04-09 15:48:52.382493 grote-0.1.5/grote/collections/translate.py
--rw-r--r--   0        0        0     1855 2024-02-13 15:36:18.636884 grote-0.1.5/grote/config.py
--rw-r--r--   0        0        0      231 2024-02-14 16:45:55.348690 grote-0.1.5/grote/config.yaml
--rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.5/grote/event_logging.py
--rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.5/grote/functions/__init__.py
--rw-r--r--   0        0        0     5543 2024-04-09 15:48:39.327509 grote-0.1.5/grote/functions/load.py
--rw-r--r--   0        0        0     3420 2024-04-09 16:19:21.659348 grote-0.1.5/grote/functions/translate.py
--rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.5/grote/style.py
--rw-r--r--   0        0        0     3659 2024-04-09 16:26:11.762663 grote-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.6/README.md
+-rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.6/grote/__init__.py
+-rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.6/grote/app.py
+-rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.6/grote/collections/__init__.py
+-rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.6/grote/collections/base.py
+-rw-r--r--   0        0        0     1218 2024-04-10 21:30:35.209116 grote-0.1.6/grote/collections/config.yaml
+-rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.6/grote/collections/load.py
+-rw-r--r--   0        0        0     8298 2024-04-10 21:30:05.986989 grote-0.1.6/grote/collections/translate.py
+-rw-r--r--   0        0        0     2451 2024-04-10 21:36:18.537577 grote-0.1.6/grote/config.py
+-rw-r--r--   0        0        0      299 2024-04-10 21:31:45.750995 grote-0.1.6/grote/config.yaml
+-rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.6/grote/event_logging.py
+-rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.6/grote/functions/__init__.py
+-rw-r--r--   0        0        0     5543 2024-04-10 21:18:52.959276 grote-0.1.6/grote/functions/load.py
+-rw-r--r--   0        0        0     3529 2024-04-10 21:35:57.692323 grote-0.1.6/grote/functions/translate.py
+-rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.6/grote/style.py
+-rw-r--r--   0        0        0     3659 2024-04-10 21:37:15.973066 grote-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.6/PKG-INFO
```

### Comparing `grote-0.1.5/LICENSE` & `grote-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/README.md` & `grote-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/app.py` & `grote-0.1.6/grote/app.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/collections/base.py` & `grote-0.1.6/grote/collections/base.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/collections/config.yaml` & `grote-0.1.6/grote/collections/config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -13,13 +13,7 @@
     target_side_label: "<h3>Translations with&nbsp;<span style='background-color: #fee2e2; color: black;'>potential issues</span></h3><p>Use the green checkmark to remove remaining highlights after editing.</p>"
     reload_button_label: "⬅️ Back to data loading"
     done_button_label: "✅ Done"
     download_button_label: "📥 Download translations"
     source_textbox_label: "Source text"
     target_textbox_label: "Translation"
     legend_label: "Potential issue severity"
-    highlight_labels:
-        - "Minor"
-        - "Major"
-    highlight_colors:
-        - "#ffedd5"
-        - "#fcd29a"
```

### Comparing `grote-0.1.5/grote/collections/load.py` & `grote-0.1.6/grote/collections/load.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/collections/translate.py` & `grote-0.1.6/grote/collections/translate.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     def get_target_side_label_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
         if not value:
             value = TRANS_CFG["target_side_label"]
         return gr.Markdown(value, visible=visible, elem_id="target_side_label_cap")
 
     @classmethod
     def get_target_side_legend_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
-        if not value and TRANS_CFG["highlight_labels"] and TRANS_CFG["highlight_colors"]:
+        if not value and cfg.tag_labels and cfg.tag_colors:
             value = f"<b>{TRANS_CFG['legend_label']}:</b>" + "".join(
                 f'<span style="background-color:{color}; margin-left: 0.5em; color: black; padding: 0px 5px;">{label}</span>'
-                for label, color in zip(TRANS_CFG["highlight_labels"], TRANS_CFG["highlight_colors"])
+                for label, color in zip(cfg.tag_labels, cfg.tag_colors)
             )
         return gr.Markdown(value, visible=visible, elem_id="target_side_legend_cap")
 
     @classmethod
     def get_reload_btn(cls, visible: bool = False) -> gr.Button:
         return gr.Button(TRANS_CFG["reload_button_label"], variant="secondary", elem_id="reload_btn", visible=visible)
 
@@ -105,23 +105,23 @@
                 visible=visible,
                 elem_classes=["source-textbox"],
                 show_label=False,
             )
         elif type == "target":
             tuples = HighlightedTextbox.tagged_text_to_tuples(
                 value,
-                tag_ids=TRANS_CFG["highlight_labels"],
+                tag_ids=cfg.tag_labels,
                 tags_open=[f"<{tag}>" for tag in cfg.allowed_tags],
                 tags_close=[f"</{tag}>" for tag in cfg.allowed_tags],
             )
             color_map = None
-            if TRANS_CFG["highlight_colors"]:
-                if len(TRANS_CFG["highlight_colors"]) != len(TRANS_CFG["highlight_labels"]):
+            if cfg.tag_colors:
+                if len(cfg.tag_colors) != len(cfg.tag_labels):
                     raise ValueError("highlight_colors and highlight_labels must have the same length")
-                color_map = dict(zip(TRANS_CFG["highlight_labels"], TRANS_CFG["highlight_colors"]))
+                color_map = dict(zip(cfg.tag_labels, cfg.tag_colors))
             return HighlightedTextbox(
                 value=tuples,
                 label=TRANS_CFG["target_textbox_label"],
                 elem_id=f"{type}_{id}_txt",
                 interactive=True,
                 show_label=False,
                 show_legend=False,
```

### Comparing `grote-0.1.5/grote/config.py` & `grote-0.1.6/grote/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,19 +30,34 @@
         The Hugging Face token to use to create (and write the logged sample to) the Hugging Face dataset
         (defaults to the registered one).
     allowed_tags: list[str]
         The list of allowed tags to be used in the translation tab.
     """
 
     max_num_sentences: int = 100
-    login_codes: list[str] = field(default_factory=["admin"])
+    login_codes: str | list[str] = "admin"
     event_logs_save_frequency: int = 50
     event_logs_hf_dataset_id: str = "grote-logs"
     event_logs_local_dir: str = "logs"
     hf_token: str | None = None
-    allowed_tags: list[str] = field(default_factory=["minor", "major", "critical"])
+    allowed_tags: str | list[str] = field(default_factory=["minor", "major"])
+    tag_labels: str | list[str] = field(default_factory=["Minor", "Major"])
+    tag_colors: str | list[str] = field(default_factory=["#ffedd5", "#fcd29a"])
 
+    @staticmethod
+    def init_list(val: str | list) -> list:
+        if isinstance(val, str):
+            return val.split(",")
+        return val
 
+    def __post_init__(self):
+        self.login_codes = self.init_list(self.login_codes)
+        self.allowed_tags = self.init_list(self.allowed_tags)
+        self.tag_labels = self.init_list(self.tag_labels)
+        self.tag_colors = self.init_list(self.tag_colors)
+
+
+# Priority: environment variables > config.yaml
 CONFIG = GroteConfig(
     **yaml.safe_load(open(Path(__file__).parent / "config.yaml", encoding="utf8")),
     **{k.lower(): v for k, v in os.environ.items() if k.lower() in [f.name.lower() for f in fields(GroteConfig)]},
 )
```

### Comparing `grote-0.1.5/grote/event_logging.py` & `grote-0.1.6/grote/event_logging.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/functions/__init__.py` & `grote-0.1.6/grote/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/functions/load.py` & `grote-0.1.6/grote/functions/load.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/grote/functions/translate.py` & `grote-0.1.6/grote/functions/translate.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     }
     state["events"].append(out)
     return state
 
 
 def record_textbox_input_fn(state: dict[str, Any], textbox_content: dict, lc_state: dict[str, Any]) -> dict[str, Any]:
     current_text = "".join(
-        f"<{tag_id.lower()}>{text}</{tag_id.lower()}>" if tag_id is not None else text for text, tag_id in textbox_content["data"]
+        f"<{tag_id.lower()}>{text}</{tag_id.lower()}>" if tag_id is not None else text
+        for text, tag_id in textbox_content["data"]
     )
     if textbox_content["id"] not in state or current_text != state[textbox_content["id"]]:
         out = {
             "time": get_current_time(),
             "login_code": lc_state["login_code_txt"],
             "text_id": textbox_content["id"],
             "event_type": "change",
@@ -61,43 +62,44 @@
     return state
 
 
 def record_textbox_remove_highlights_fn(
     state: dict[str, Any], textbox_content: dict, lc_state: dict[str, Any]
 ) -> dict[str, Any]:
     current_text = "".join(
-        f"<{tag_id.lower()}>{text}</{tag_id.lower()}>" if tag_id is not None else text for text, tag_id in textbox_content["data"]
+        f"<{tag_id.lower()}>{text}</{tag_id.lower()}>" if tag_id is not None else text
+        for text, tag_id in textbox_content["data"]
     )
     out = {
         "time": get_current_time(),
         "login_code": lc_state["login_code_txt"],
         "text_id": textbox_content["id"],
         "event_type": "remove_highlights",
         "text": current_text,
     }
     state[textbox_content["id"]] = current_text
     state["events"].append(out)
     return state
 
 
 def record_trial_end_fn(state: dict[str, Any], lc_state: dict[str, Any]) -> dict[str, Any]:
-    gr.Info("Saving trial information. Please wait...")
+    gr.Info("Saving trial information. Don't close the tab until the download button is available!")
     out = {
         "time": get_current_time(),
         "login_code": lc_state["login_code_txt"],
         "event_type": "end",
     }
     state["events"].append(out)
     return state
 
 
 def save_outputs_to_file(lc_state, *txts) -> None:
     fname = f"{lc_state['login_code_txt']}_{lc_state['_filename']}_output.txt"
     with open(fname, "w") as f:
         f.write("\n".join("".join(x[0] for x in txt["data"]) for txt in txts if txt["data"]))
-    gr.Info("Saving complete! Download the output file below")
+    gr.Info("Saving complete! Download the output file by clicking the 'Download translations' button below.")
     return gr.DownloadButton(
         label=TRANS_CFG["download_button_label"],
         value=fname,
         visible=True,
         interactive=True,
     ), gr.Button(interactive=False)
```

### Comparing `grote-0.1.5/grote/style.py` & `grote-0.1.6/grote/style.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.5/pyproject.toml` & `grote-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "grote"
-version = "0.1.5"
+version = "0.1.6"
 description = "Groningen Translation Environment"
 readme = "README.md"
 authors = ["Gabriele Sarti"]
 maintainers = ["Gabriele Sarti <gabriele.sarti996@gmail.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/gsarti/grote"
 homepage = "https://github.com/gsarti/grote"
```

### Comparing `grote-0.1.5/PKG-INFO` & `grote-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grote
-Version: 0.1.5
+Version: 0.1.6
 Summary: Groningen Translation Environment
 Home-page: https://github.com/gsarti/grote
 License: Apache Software License 2.0
 Keywords: translation environment,gradio
 Author: Gabriele Sarti
 Maintainer: Gabriele Sarti
 Maintainer-email: gabriele.sarti996@gmail.com
```

