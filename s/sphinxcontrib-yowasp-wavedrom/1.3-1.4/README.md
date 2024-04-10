# Comparing `tmp/sphinxcontrib_yowasp_wavedrom-1.3-py3-none-any.whl.zip` & `tmp/sphinxcontrib_yowasp_wavedrom-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4829 bytes, number of entries: 5
--rw-r--r--  2.0 unx     3687 b- defN 16-Jan-01 00:00 sphinxcontrib/yowasp_wavedrom.py
--rw-r--r--  2.0 unx     2758 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.3.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx     1089 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.3.dist-info/licenses/LICENSE.txt
-?rw-------  2.0 unx      477 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.3.dist-info/RECORD
-5 files, 8116 bytes uncompressed, 3933 bytes compressed:  51.5%
+Zip file size: 5352 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     4007 b- defN 16-Jan-01 00:00 sphinxcontrib/yowasp_wavedrom.py
+-rw-r--r--  2.0 unx     3997 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1089 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.4.dist-info/licenses/LICENSE.txt
+?rw-------  2.0 unx      477 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.4.dist-info/RECORD
+5 files, 9675 bytes uncompressed, 4456 bytes compressed:  53.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: sphinxcontrib/yowasp_wavedrom.py
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.3.dist-info/METADATA
+Filename: sphinxcontrib_yowasp_wavedrom-1.4.dist-info/METADATA
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.3.dist-info/WHEEL
+Filename: sphinxcontrib_yowasp_wavedrom-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.3.dist-info/licenses/LICENSE.txt
+Filename: sphinxcontrib_yowasp_wavedrom-1.4.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.3.dist-info/RECORD
+Filename: sphinxcontrib_yowasp_wavedrom-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphinxcontrib/yowasp_wavedrom.py

```diff
@@ -57,14 +57,22 @@
     except Exception as error:
         sphinx.application.logger.error(
             f'Could not render WaveDrom diagram at {wavedrom_loc}: {error}')
         self.body.append(f'<em style="color:red;font-weight:bold">'
             f'<pre>/!\ Could not render WaveDrom diagram: {self.encode(error)}</pre>'
             f'</em>')
         raise nodes.SkipNode
+
+    # Determine CSS class of the image.
+    if "signal" in wavedrom_src:
+        css_class = "wavedrom wavedrom-signal"
+    if "reg" in wavedrom_src:
+        css_class = "wavedrom wavedrom-reg"
+    if "assign" in wavedrom_src:
+        css_class = "wavedrom wavedrom-assign"
     
     # Write the SVG to output directory. This is necessary because inlining it into the HTML has
     # significantly different behavior: duplicate IDs result in broken rendering, text can be
     # selected, media queries can't be overridden with a `color-scheme` CSS attribute for themes
     # that have a dark/light toggle via JS, etc.
     pathname = Path(self.builder.outdir).joinpath(
         # Note that for documents in subdirectories, the image directory is placed within that
@@ -76,14 +84,15 @@
         f'{basename}.svg'
     )
     pathname.parent.mkdir(parents=True, exist_ok=True)
     pathname.write_text(wavedrom_svg)
 
     # Reference the SVG in the HTML document.
     self.body.append(f'<img src="{self.builder.imagedir}/{basename}.svg" '
+        f'class="{self.encode(css_class)}" '
         f'alt="{self.encode(node["src"])}">')
     raise nodes.SkipNode
 
 
 def setup(app: sphinx.application.Sphinx):
     app.add_config_value("yowasp_wavedrom_skin", "default", "html", str)
     app.add_directive("wavedrom", WaveDromDirective)
```

## Comparing `sphinxcontrib_yowasp_wavedrom-1.3.dist-info/licenses/LICENSE.txt` & `sphinxcontrib_yowasp_wavedrom-1.4.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

