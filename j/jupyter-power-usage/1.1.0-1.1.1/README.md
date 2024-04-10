# Comparing `tmp/jupyter_power_usage-1.1.0.tar.gz` & `tmp/jupyter_power_usage-1.1.1.tar.gz`

## Comparing `jupyter_power_usage-1.1.0.tar` & `jupyter_power_usage-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.flake8
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.prettierignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.yarnrc.yml
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/RELEASE.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/install.json
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/setup.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/tsconfig.json
--rw-r--r--   0        0        0   183801 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/yarn.lock
--rw-r--r--   0        0        0    69248 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/doc/frontend-settings.png
--rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/doc/power-usage.gif
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/_version.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/api.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/config.py
--rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/metrics.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/utils.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/etc/jupyter_server_config.d/jupyter-power-usage.json
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/package.json
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/32.d626a962b7bd9192a1da.js
--rw-r--r--   0        0        0    28319 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/remoteEntry.20fe913e7d7c5e7492d8.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/style.js
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/tests/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/tests/test_basic.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/schema/plugin.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/cpuPowerView.tsx
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/emissionsHandler.ts
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/emissionsView.tsx
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/format.ts
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/gpuPowerView.tsx
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/index.ts
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/indicator.tsx
--rw-r--r--   0        0        0    15438 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/model.ts
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/index.js
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/LICENSE
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/README.md
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    21077 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/.flake8
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/RELEASE.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/install.json
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/setup.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/tsconfig.json
+-rw-r--r--   0        0        0   183801 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/yarn.lock
+-rw-r--r--   0        0        0    69248 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/doc/frontend-settings.png
+-rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/doc/power-usage.gif
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/_version.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/api.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/config.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/metrics.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/utils.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/etc/jupyter_server_config.d/jupyter-power-usage.json
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/package.json
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json
+-rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/32.ae09c753b840c00bc1d6.js
+-rw-r--r--   0        0        0    28319 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js
+-rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/remoteEntry.96f3977247742fc77a67.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/style.js
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/tests/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/jupyter_power_usage/tests/test_basic.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/schema/plugin.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/cpuPowerView.tsx
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/emissionsHandler.ts
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/emissionsView.tsx
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/format.ts
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/gpuPowerView.tsx
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/index.ts
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/indicator.tsx
+-rw-r--r--   0        0        0    15438 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/src/model.ts
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/style/index.js
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/README.md
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    21077 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.1/PKG-INFO
```

### Comparing `jupyter_power_usage-1.1.0/.pre-commit-config.yaml` & `jupyter_power_usage-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/CHANGELOG.md` & `jupyter_power_usage-1.1.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.1.1
+
+([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/v1.1.0...e4bed2566bee4ad972523c2fa1dced4121dbca9e))
+
+### Bugs fixed
+
+- Force new instance of  `ASyncHTTPclient` [#10](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/10) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mahendrapaipuri/jupyter-power-usage/graphs/contributors?from=2024-04-03&to=2024-04-10&type=c))
+
+[@mahendrapaipuri](https://github.com/search?q=repo%3Amahendrapaipuri%2Fjupyter-power-usage+involves%3Amahendrapaipuri+updated%3A2024-04-03..2024-04-10&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.1.0
 
 ([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/v1.0.0...43f5a12b352e65bd810d75bb06608e605836ca4c))
 
 ### Enhancements made
 
 - Electricity Maps Support [#9](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/9) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
@@ -20,16 +36,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mahendrapaipuri/jupyter-power-usage/graphs/contributors?from=2023-10-12&to=2024-04-03&type=c))
 
 [@mahendrapaipuri](https://github.com/search?q=repo%3Amahendrapaipuri%2Fjupyter-power-usage+involves%3Amahendrapaipuri+updated%3A2023-10-12..2024-04-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.0.0
 
 ([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/v0.1.1...62b1ee6d0ed0a662330c0156807b07e493eeb85a))
 
 ### Enhancements made
 
 - Upgrade to JupyterLab 4 [#4](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/4) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
```

### Comparing `jupyter_power_usage-1.1.0/CONTRIBUTING.md` & `jupyter_power_usage-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/package.json` & `jupyter_power_usage-1.1.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -170,9 +170,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `jupyter_power_usage-1.1.0/tsconfig.json` & `jupyter_power_usage-1.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/yarn.lock` & `jupyter_power_usage-1.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/doc/frontend-settings.png` & `jupyter_power_usage-1.1.1/doc/frontend-settings.png`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/doc/power-usage.gif` & `jupyter_power_usage-1.1.1/doc/power-usage.gif`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/__init__.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from jupyter_server.utils import url_path_join as ujoin
 
-from ._version import __version__
+from ._version import __version__  # noqa
 from .api import ElectrictyMapsHandler
 from .api import PowerMetricHandler
 from .config import PowerUsageDisplay
 from .metrics import CpuPowerUsage
 from .metrics import GpuPowerUsage
 
 
+def _jupyter_server_extension_points():
+    return [{"module": "jupyter_power_usage"}]
+
+
 def _jupyter_labextension_paths():
     return [{"src": "labextension", "dest": "@mahendrapaipuri/jupyter-power-usage"}]
 
 
 def load_jupyter_server_extension(server_app):
     """
     Called when the extension is loaded.
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/api.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,26 +104,33 @@
 class ElectrictyMapsHandler(JupyterHandler):
     """
     A proxy for the Electricity Maps API v3.
 
     The purpose of this proxy is to provide authentication to the API requests.
     """
 
-    client = AsyncHTTPClient()
+    # Force a new instance to not to mess up with other instances that might exist in
+    # JupyterHub or other Jupyter related stacks
+    #
+    # Without this we noticed that JupyterHub will fail to spawn instances when internal
+    # TLS is on. The reason is that this new instantiation will override the already
+    # existing instance in single user extension that has SSL context configured. So
+    # we lose SSL context and hence cert verification will fail eventually failing spawn.
+    client = AsyncHTTPClient(force_instance=True)
 
     def initialize(self):
         # Get access token(s) from config
         self.access_tokens = {}
         self.access_tokens['emaps'] = self.settings[
             'jupyter_power_usage_config'
         ].emaps_access_token
 
     @web.authenticated
     async def get(self, path):
-        """Return emission factor data from electticity maps"""
+        """Return emission factor data from electricity maps"""
         try:
             query = self.request.query_arguments
             params = {key: query[key][0].decode() for key in query}
             api_path = url_path_join('https://api.electricitymap.org', url_escape(path))
 
             access_token = params.pop('access_token', None)
             if self.access_tokens['emaps']:
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/config.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/config.py`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/metrics.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/metrics.py`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/utils.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/package.json` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.96f3977247742fc77a67.js'}}",*

 * * "'version'": "'1.1.1'"}*

```diff
@@ -110,15 +110,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/mahendrapaipuri/jupyter-power-usage",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.20fe913e7d7c5e7492d8.js",
+            "load": "static/remoteEntry.96f3977247742fc77a67.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_power_usage/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -175,9 +175,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.1.1'"}*

```diff
@@ -170,9 +170,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.1.1"
 }
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/32.d626a962b7bd9192a1da.js` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/32.ae09c753b840c00bc1d6.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunk_mahendrapaipuri_jupyter_power_usage = self.webpackChunk_mahendrapaipuri_jupyter_power_usage || []).push([
     [32], {
         32: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => z
             });
-            var s = n(510),
-                r = n(8),
+            var s = n(464),
+                r = n(99),
                 i = n(29),
                 a = n.n(i),
                 o = n(496);
             const c = ({
                     percentage: e,
                     color: t
                 }) => a().createElement("div", {
@@ -156,16 +156,16 @@
                 };
             var v;
             ! function(e) {
                 e.createEmissionsView = e => s.ReactWidget.create(a().createElement(f, {
                     model: e
                 }))
             }(v || (v = {}));
-            var w = n(311),
-                _ = n(217),
+            var w = n(671),
+                _ = n(818),
                 b = n(797),
                 y = n(901);
             const P = 1e3,
                 E = 1e6;
             var x, A;
             ! function(e) {
                 e.getOpenDataSoftEmissionFactor = async () => {
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/remoteEntry.20fe913e7d7c5e7492d8.js` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/remoteEntry.96f3977247742fc77a67.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, u, l, s, p, f, d, c, h, v, g, m, b, y = {
+    var e, r, t, a, n, o, i, u, l, s, p, d, f, c, h, v, g, m, b, y = {
             624: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(29), t.e(32)]).then((() => () => t(32))),
                         "./extension": () => Promise.all([t.e(29), t.e(32)]).then((() => () => t(32))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -44,20 +44,20 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         29: "264e3efb1b2477b15441",
-        32: "d626a962b7bd9192a1da",
+        32: "ae09c753b840c00bc1d6",
         646: "92e3ed3d9aea0d36c6a9",
         747: "19551df7a36576f1c11f"
     } [e] + ".js?v=" + {
         29: "264e3efb1b2477b15441",
-        32: "d626a962b7bd9192a1da",
+        32: "ae09c753b840c00bc1d6",
         646: "92e3ed3d9aea0d36c6a9",
         747: "19551df7a36576f1c11f"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -72,24 +72,24 @@
                     var p = l[s];
                     if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + n) {
                         i = p;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var f = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(d);
+            var d = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(f);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                d = setTimeout(f.bind(null, void 0, {
+                f = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -111,15 +111,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@mahendrapaipuri/jupyter-power-usage", "1.1.0", (() => Promise.all([j.e(29), j.e(32)]).then((() => () => j(32))))), u("react-sparklines", "1.7.0", (() => Promise.all([j.e(646), j.e(29)]).then((() => () => j(646)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@mahendrapaipuri/jupyter-power-usage", "1.1.1", (() => Promise.all([j.e(29), j.e(32)]).then((() => () => j(32))))), u("react-sparklines", "1.7.0", (() => Promise.all([j.e(646), j.e(29)]).then((() => () => j(646)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -169,75 +169,75 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, p, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (p = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > a && !n : "" == f != n);
+                var s, p, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (p = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > a && !n : "" == d != n);
                 if ("u" == p) {
-                    if (!l || "u" != f) return !1
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == p)
+                    if (d == p)
                         if (u <= a) {
                             if (s != e[u]) return !1
                         } else {
                             if (n ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= a || p < f != n) return !1;
+                    if (u <= a || p < d != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
+        var f = [],
+            c = f.pop.bind(f);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            f.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
         var n = u(e, t);
-        return o(a, n) || f(l(e, t, n, a)), d(e[t][n])
+        return o(a, n) || d(l(e, t, n, a)), f(e[t][n])
     }, p = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, f = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, a, n) {
+    }, f = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, a, n) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), v = c(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && p(r, t, a);
-        return o ? d(o) : n()
+        return o ? f(o) : n()
     })), g = {}, m = {
         29: () => h("default", "react", [1, 18, 2, 0]),
-        8: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
-        217: () => h("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        311: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
+        99: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
+        464: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
         496: () => v("default", "react-sparklines", [1, 1, 7, 0], (() => j.e(646).then((() => () => j(646))))),
-        510: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        671: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
         797: () => h("default", "@lumino/polling", [1, 2, 0, 0]),
+        818: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
         901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, b = {
         29: [29],
-        32: [8, 217, 311, 496, 510, 797, 901]
+        32: [99, 464, 496, 671, 797, 818, 901]
     }, j.f.consumes = (e, r) => {
         j.o(b, e) && b[e].forEach((e => {
             if (j.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/third-party-licenses.json` & `jupyter_power_usage-1.1.1/jupyter_power_usage/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/jupyter_power_usage/tests/test_basic.py` & `jupyter_power_usage-1.1.1/jupyter_power_usage/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/schema/plugin.json` & `jupyter_power_usage-1.1.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/cpuPowerView.tsx` & `jupyter_power_usage-1.1.1/src/cpuPowerView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/emissionsHandler.ts` & `jupyter_power_usage-1.1.1/src/emissionsHandler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/emissionsView.tsx` & `jupyter_power_usage-1.1.1/src/emissionsView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/format.ts` & `jupyter_power_usage-1.1.1/src/format.ts`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/gpuPowerView.tsx` & `jupyter_power_usage-1.1.1/src/gpuPowerView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/index.ts` & `jupyter_power_usage-1.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/indicator.tsx` & `jupyter_power_usage-1.1.1/src/indicator.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/src/model.ts` & `jupyter_power_usage-1.1.1/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/style/base.css` & `jupyter_power_usage-1.1.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/.gitignore` & `jupyter_power_usage-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/LICENSE` & `jupyter_power_usage-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/README.md` & `jupyter_power_usage-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/pyproject.toml` & `jupyter_power_usage-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.1.0/PKG-INFO` & `jupyter_power_usage-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter_power_usage
-Version: 1.1.0
+Version: 1.1.1
 Dynamic: Keywords
 Summary: Extension that shows system power usage
 Project-URL: Homepage, https://github.com/mahendrapaipuri/jupyter-power-usage
 Project-URL: Bug Tracker, https://github.com/mahendrapaipuri/jupyter-power-usage/issues
 Project-URL: Repository, https://github.com/mahendrapaipuri/jupyter-power-usage.git
 Author-email: Mahendra Paipuri <mahendra.paipuri@cnrs.fr>
 License:                                  Apache License
```

