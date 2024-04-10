# Comparing `tmp/rose_pine_jupyterlab-0.1.4.tar.gz` & `tmp/rose_pine_jupyterlab-0.1.5.tar.gz`

## Comparing `rose_pine_jupyterlab-0.1.4.tar` & `rose_pine_jupyterlab-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/.copier-answers.yml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/.yarnrc.yml
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/contributing.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/install.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/license
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/package.json
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/release.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/tsconfig.json
--rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/yarn.lock
--rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/assets/rose-pine-dawn.png
--rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/assets/rose-pine-moon.png
--rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/assets/rose-pine.png
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/examples/example_notebook.ipynb
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/_version.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/517.aa7ed00aa2e020ed780c.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/remoteEntry.87a2355737f64f41319d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/index.ts
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/pallettes.d.ts
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/pallettes.ts
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/rose-pine-dawn.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/rose-pine-moon.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/rose-pine.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/src/templates.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/style/index.css
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/.gitignore
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/readme.md
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.copier-answers.yml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.yarnrc.yml
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/contributing.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/install.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/license
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/package.json
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/release.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/tsconfig.json
+-rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/yarn.lock
+-rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine-dawn.png
+-rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine-moon.png
+-rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/assets/rose-pine.png
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/examples/example_notebook.ipynb
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/_version.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/517.56cb28c4b8230b0f86c3.js
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/remoteEntry.ad3e3d6d7fd32586ac09.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/index.ts
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/pallettes.d.ts
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/pallettes.ts
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine-dawn.json
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine-moon.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/rose-pine.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/src/templates.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/style/index.css
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/readme.md
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.5/PKG-INFO
```

### Comparing `rose_pine_jupyterlab-0.1.4/.pre-commit-config.yaml` & `rose_pine_jupyterlab-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/CHANGELOG.md` & `rose_pine_jupyterlab-0.1.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.5
+
+([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.4...b770b8a44a7348efb306861e7d449108bd7095ea))
+
+### Maintenance and upkeep improvements
+
+- update template to v4.2.6 [#6](https://github.com/aaravind100/jupyterlab/pull/6) ([@aaravind100](https://github.com/aaravind100))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-01-28&to=2024-04-10&type=c))
+
+[@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-01-28..2024-04-10&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.4
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.3...bb0738f57092f86a380e1e56aced95d4c3c22321))
 
 ### Enhancements made
 
 - refactor: :recycle: Pallette implementation out of loop [#5](https://github.com/aaravind100/jupyterlab/pull/5) ([@aaravind100](https://github.com/aaravind100))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-01-28&to=2024-01-28&type=c))
 
 [@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-01-28..2024-01-28&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.3
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.2...4525937871d260d2994d93633b7f0f4a69d68c20))
 
 ### Enhancements made
 
 - refactor: :recycle: move pallette to a json file [#4](https://github.com/aaravind100/jupyterlab/pull/4) ([@aaravind100](https://github.com/aaravind100))
```

### Comparing `rose_pine_jupyterlab-0.1.4/contributing.md` & `rose_pine_jupyterlab-0.1.5/contributing.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/license` & `rose_pine_jupyterlab-0.1.5/license`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/package.json` & `rose_pine_jupyterlab-0.1.5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -180,9 +180,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.4/release.md` & `rose_pine_jupyterlab-0.1.5/release.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/tsconfig.json` & `rose_pine_jupyterlab-0.1.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/yarn.lock` & `rose_pine_jupyterlab-0.1.5/yarn.lock`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/assets/rose-pine-dawn.png` & `rose_pine_jupyterlab-0.1.5/assets/rose-pine-dawn.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/assets/rose-pine-moon.png` & `rose_pine_jupyterlab-0.1.5/assets/rose-pine-moon.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/assets/rose-pine.png` & `rose_pine_jupyterlab-0.1.5/assets/rose-pine.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/examples/example_notebook.ipynb` & `rose_pine_jupyterlab-0.1.5/examples/example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/__init__.py` & `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/package.json` & `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ad3e3d6d7fd32586ac09.js'}}",*

 * * "'version'": "'0.1.5'"}*

```diff
@@ -100,15 +100,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aaravind100/jupyterlab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.87a2355737f64f41319d.js"
+            "load": "static/remoteEntry.ad3e3d6d7fd32586ac09.js"
         },
         "extension": true,
         "outputDir": "rose_pine_jupyterlab/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/517.aa7ed00aa2e020ed780c.js` & `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/517.56cb28c4b8230b0f86c3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 "use strict";
 (self.webpackChunkrose_pine_jupyterlab = self.webpackChunkrose_pine_jupyterlab || []).push([
     [517], {
         517: (e, p, t) => {
             t.r(p), t.d(p, {
                 default: () => d
             });
-            var l = t(123);
+            var l = t(464);
             const r = JSON.parse('{"name":"Rosé Pine","type":"dark","pallette":{"--rp-plt-base":"#191724","--rp-plt-surface":"#1f1d2e","--rp-plt-overlay":"#26233a","--rp-plt-muted":"#6e6a86","--rp-plt-subtle":"#908caa","--rp-plt-text":"#e0def4","--rp-plt-love":"#eb6f92","--rp-plt-gold":"#f6c177","--rp-plt-rose":"#ebbcba","--rp-plt-pine":"#31748f","--rp-plt-foam":"#9ccfd8","--rp-plt-iris":"#c4a7e7","--rp-plt-highlight-low":"#21202e","--rp-plt-highlight-med":"#403d52","--rp-plt-highlight-high":"#524f67"}}'),
                 a = JSON.parse('{"name":"Rosé Pine Moon","type":"dark","pallette":{"--rp-plt-base":"#232136","--rp-plt-surface":"#2a273f","--rp-plt-overlay":"#393552","--rp-plt-muted":"#6e6a86","--rp-plt-subtle":"#908caa","--rp-plt-text":"#e0def4","--rp-plt-love":"#eb6f92","--rp-plt-gold":"#f6c177","--rp-plt-rose":"#ea9a97","--rp-plt-pine":"#3e8fb0","--rp-plt-foam":"#9ccfd8","--rp-plt-iris":"#c4a7e7","--rp-plt-highlight-low":"#2a283e","--rp-plt-highlight-med":"#44415a","--rp-plt-highlight-high":"#56526e"}}'),
                 i = JSON.parse('{"name":"Rosé Pine Dawn","type":"light","pallette":{"--rp-plt-base":"#faf4ed","--rp-plt-surface":"#fffaf3","--rp-plt-overlay":"#f2e9e1","--rp-plt-muted":"#9893a5","--rp-plt-subtle":"#797593","--rp-plt-text":"#575279","--rp-plt-love":"#b4637a","--rp-plt-gold":"#ea9d34","--rp-plt-rose":"#d7827e","--rp-plt-pine":"#286983","--rp-plt-foam":"#56949f","--rp-plt-iris":"#907aa9","--rp-plt-highlight-low":"#f4ede8","--rp-plt-highlight-med":"#dfdad9","--rp-plt-highlight-high":"#cecacd"}}');
             class s {
                 constructor(e, p, t) {
                     this.name = e, this.type = p, this.pallette = t
                 }
```

### Comparing `rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/static/remoteEntry.87a2355737f64f41319d.js` & `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/static/remoteEntry.ad3e3d6d7fd32586ac09.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, l, s, f, p, c, d, h, v, g = {
+    var e, r, t, n, o, i, a, u, l, s, f, p, d, c, h, v, g = {
             368: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(517).then((() => () => t(517))),
                         "./extension": () => t.e(517).then((() => () => t(517)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -35,15 +35,15 @@
         return g[e](t, t.exports, m), t.exports
     }
     m.m = g, m.c = b, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".aa7ed00aa2e020ed780c.js?v=aa7ed00aa2e020ed780c", m.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".56cb28c4b8230b0f86c3.js?v=56cb28c4b8230b0f86c3", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "rose_pine_jupyterlab:", m.l = (t, n, o, i) => {
@@ -56,19 +56,19 @@
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         a = f;
                         break
                     }
                 }
             a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var p = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
+                    a.onerror = a.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(p.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -93,15 +93,15 @@
                     var o = i[e] = i[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
                         get: () => m.e(517).then((() => () => m(517))),
                         from: a,
                         eager: !1
                     })
-                })("rose_pine_jupyterlab", "0.1.4"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("rose_pine_jupyterlab", "0.1.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -172,56 +172,56 @@
                     l = !1, u--
                 } else {
                     if (u <= n || f < p != o) return !1;
                     l = !1
                 } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var c = [],
-            d = c.pop.bind(c);
+        var d = [],
+            c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? i(h, r) : !d())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
-        return !!d()
+        return !!c()
     }, a = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
         return i(n, o) || f(l(e, t, o, n)), p(e[t][o])
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), c = (e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var i = m.I(r);
         return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), d = {}, h = {
-        123: () => c("default", "@jupyterlab/apputils", [1, 4, 1, 11])
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), c = {}, h = {
+        464: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 6])
     }, v = {
-        517: [123]
+        517: [464]
     }, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
-            if (m.o(d, e)) return r.push(d[e]);
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    d[e] = 0, m.m[e] = t => {
+                    c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete d[e], m.m[e] = t => {
+                    delete c[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
                 var o = h[e]();
-                o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             488: 0
```

### Comparing `rose_pine_jupyterlab-0.1.4/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css` & `rose_pine_jupyterlab-0.1.5/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/index.ts` & `rose_pine_jupyterlab-0.1.5/src/index.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/pallettes.ts` & `rose_pine_jupyterlab-0.1.5/src/pallettes.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/rose-pine-dawn.json` & `rose_pine_jupyterlab-0.1.5/src/rose-pine-dawn.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/rose-pine-moon.json` & `rose_pine_jupyterlab-0.1.5/src/rose-pine-moon.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/rose-pine.json` & `rose_pine_jupyterlab-0.1.5/src/rose-pine.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/src/templates.json` & `rose_pine_jupyterlab-0.1.5/src/templates.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/style/variables.css` & `rose_pine_jupyterlab-0.1.5/style/variables.css`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/.gitignore` & `rose_pine_jupyterlab-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/pyproject.toml` & `rose_pine_jupyterlab-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/readme.md` & `rose_pine_jupyterlab-0.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.4/PKG-INFO` & `rose_pine_jupyterlab-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rose_pine_jupyterlab
-Version: 0.1.4
+Version: 0.1.5
+Dynamic: Keywords
 Summary: Soho Vibes for JupyterLab
 Project-URL: Homepage, https://github.com/aaravind100/jupyterlab
 Project-URL: Bug Tracker, https://github.com/aaravind100/jupyterlab/issues
 Project-URL: Repository, https://github.com/aaravind100/jupyterlab.git
 Author-email: Ajith Aravind <ajith.aravind100@gmail.com>
 License: BSD 3-Clause License
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: rose_pine_jupyterlab Version: 0.1.4 Summary: Soho
-Vibes for JupyterLab Project-URL: Homepage, https://github.com/aaravind100/
-jupyterlab Project-URL: Bug Tracker, https://github.com/aaravind100/jupyterlab/
-issues Project-URL: Repository, https://github.com/aaravind100/jupyterlab.git
-Author-email: Ajith Aravind
+Metadata-Version: 2.3 Name: rose_pine_jupyterlab Version: 0.1.5 Dynamic:
+Keywords Summary: Soho Vibes for JupyterLab Project-URL: Homepage, https://
+github.com/aaravind100/jupyterlab Project-URL: Bug Tracker, https://github.com/
+aaravind100/jupyterlab/issues Project-URL: Repository, https://github.com/
+aaravind100/jupyterlab.git Author-email: Ajith Aravind
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ajith Aravind All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
 and the following disclaimer in the documentation and/or other materials
```

