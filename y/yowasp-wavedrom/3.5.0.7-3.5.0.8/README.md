# Comparing `tmp/yowasp_wavedrom-3.5.0.7-py3-none-any.whl.zip` & `tmp/yowasp_wavedrom-3.5.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40752 bytes, number of entries: 7
--rw-r--r--  2.0 unx      904 b- defN 24-Apr-07 08:44 yowasp_wavedrom/__init__.py
--rw-r--r--  2.0 unx   392632 b- defN 24-Apr-07 08:45 yowasp_wavedrom/bundle.js
--rw-r--r--  2.0 unx     3362 b- defN 24-Apr-07 08:45 yowasp_wavedrom-3.5.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 08:45 yowasp_wavedrom-3.5.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-07 08:45 yowasp_wavedrom-3.5.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-07 08:45 yowasp_wavedrom-3.5.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      610 b- defN 24-Apr-07 08:45 yowasp_wavedrom-3.5.0.7.dist-info/RECORD
-7 files, 397678 bytes uncompressed, 39658 bytes compressed:  90.0%
+Zip file size: 40764 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      904 b- defN 24-Apr-09 23:45 yowasp_wavedrom/__init__.py
+-rw-r--r--  2.0 unx   392548 b- defN 24-Apr-09 23:45 yowasp_wavedrom/bundle.js
+-rw-r--r--  2.0 unx     3425 b- defN 24-Apr-09 23:46 yowasp_wavedrom-3.5.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 23:46 yowasp_wavedrom-3.5.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-09 23:46 yowasp_wavedrom-3.5.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-09 23:46 yowasp_wavedrom-3.5.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-09 23:46 yowasp_wavedrom-3.5.0.8.dist-info/RECORD
+7 files, 397657 bytes uncompressed, 39670 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yowasp_wavedrom/__init__.py
 Comment: 
 
 Filename: yowasp_wavedrom/bundle.js
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.7.dist-info/METADATA
+Filename: yowasp_wavedrom-3.5.0.8.dist-info/METADATA
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.7.dist-info/WHEEL
+Filename: yowasp_wavedrom-3.5.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.7.dist-info/entry_points.txt
+Filename: yowasp_wavedrom-3.5.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.7.dist-info/top_level.txt
+Filename: yowasp_wavedrom-3.5.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.7.dist-info/RECORD
+Filename: yowasp_wavedrom-3.5.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yowasp_wavedrom/bundle.js

### js-beautify {}

```diff
@@ -26708,28 +26708,27 @@
 var import_narrowerer = __toESM(require_narrowerer(), 1);
 var import_lowkey = __toESM(require_lowkey(), 1);
 var import_dark = __toESM(require_dark(), 1);
 var import_render_signal = __toESM(require_render_signal(), 1);
 var import_render_reg = __toESM(require_render_reg(), 1);
 var import_render_assign = __toESM(require_render_assign(), 1);
 var WaveSkin = {
-    light: import_default.default.default,
+    ...import_default.default,
     ...import_dark.default,
     ...import_narrow.default,
     ...import_narrower.default,
     ...import_narrowerer.default,
     ...import_lowkey.default
 };
-WaveSkin.default = JSON.parse(JSON.stringify(WaveSkin.light));
-WaveSkin.default[2][2] = `@media(prefers-color-scheme:dark){:root{filter:invert(1)}}${WaveSkin.light[2][2]}}`;
 
 function renderSignal(source) {
     const rendered = (0, import_render_signal.default)(0, source, WaveSkin);
     delete rendered[1]["id"];
     rendered[4][2].splice(1, 1);
+    rendered.splice(2, 0, ["style", {}, "@media(prefers-color-scheme:dark){:root{filter:invert(1)}}"]);
     return (0, import_stringify.default)(rendered);
 }
 
 function renderBitField(source) {
     const rendered = (0, import_render_reg.default)(0, source);
     rendered.splice(2, 0, ["style", {}, "@media(prefers-color-scheme:dark){:root{filter:invert(1)}}"]);
     return (0, import_stringify.default)(rendered);
```

## Comparing `yowasp_wavedrom-3.5.0.7.dist-info/METADATA` & `yowasp_wavedrom-3.5.0.8.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yowasp-wavedrom
-Version: 3.5.0.7
+Version: 3.5.0.8
 Summary: WaveDrom generates diagrams for digital waveforms, bit fields, and simple combinational circuits
 Author-email: Catherine <whitequark@whitequark.org>
 License: MIT
 Project-URL: Homepage, https://yowasp.org/
 Project-URL: Source Code, https://github.com/YoWASP/wavedrom
 Project-URL: Bug Tracker, https://github.com/YoWASP/wavedrom/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -60,16 +60,17 @@
 
 Implementation notes
 --------------------
 
 This package embeds the [upstream WaveDrom library][upstream] bundled with the minimal amount of dependencies necessary to produce a serialized SVG, and, for the Python package, with a JavaScript runtime. In addition, the output is post-processed compared to the upstream library as follows:
 
 * The `id` attribute of the root `<svg>` element is removed.
-* The stylesheets are altered to take into account dark color scheme preference via media queries.
-    * By default, the diagrams automatically switch between light and dark color schemes based on the user preference. The light variant is the default upstream WaveDrom color scheme, and the dark variant is the same but with colors inverted. Unfortunately, it is not feasible to use media queries to switch between the default/light skin and the dark skin for waveform diagrams, and an inversion filter is used instead.
+* The stylesheets are altered to take into account dark color scheme preference via media queries. If the user agent reports dark color scheme preference, the colors in the diagram are inverted.
+    * In case of the `dark` waveform diagram skin, this will cause it to use light colors.
+    * When the SVG image is embedded in an HTML document using the `<img>` tag, the color scheme preference can be set per-image using a CSS rule such as `img { color-scheme: light; }`. This can be used to make the images responsive to dynamic theming, or simply to override the default behavior.
 * Several otherwise blocking bugs are worked around.
 
 [upstream]: https://npmjs.org/package/wavedrom
 
 Updates
 -------
```

## Comparing `yowasp_wavedrom-3.5.0.7.dist-info/RECORD` & `yowasp_wavedrom-3.5.0.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 yowasp_wavedrom/__init__.py,sha256=xzEXA9ZmV8f7EBToJ0nghMoyt_PbhjZZe2H4jRvx7Cs,904
-yowasp_wavedrom/bundle.js,sha256=-fK0xEYdAJBkB18NsqGPHLMaGvG8As2ihhJbyqCABD4,392632
-yowasp_wavedrom-3.5.0.7.dist-info/METADATA,sha256=_sXUKSKoMy-a2l9lgYrUPgtbX_OH8oKUkNrZ2E16ysU,3362
-yowasp_wavedrom-3.5.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-yowasp_wavedrom-3.5.0.7.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
-yowasp_wavedrom-3.5.0.7.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
-yowasp_wavedrom-3.5.0.7.dist-info/RECORD,,
+yowasp_wavedrom/bundle.js,sha256=Ln3M1NJppW75D0wDgQY7yZkxCK88_AZd5cLwVuB0-Ig,392548
+yowasp_wavedrom-3.5.0.8.dist-info/METADATA,sha256=AGoQMvJ-ngkT5Q4f09bK6rHRTh-Dtk8QeJQnh6FcrSY,3425
+yowasp_wavedrom-3.5.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+yowasp_wavedrom-3.5.0.8.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
+yowasp_wavedrom-3.5.0.8.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
+yowasp_wavedrom-3.5.0.8.dist-info/RECORD,,
```

