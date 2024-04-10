# Comparing `tmp/oceanumlab-4.0.0.tar.gz` & `tmp/oceanumlab-4.0.1.tar.gz`

## Comparing `oceanumlab-4.0.0.tar` & `oceanumlab-4.0.1.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.eslintignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.eslintrc.js
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.prettierrc
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/Makefile
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/RELEASE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/_setup.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/babel.config.js
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/conftest.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/environment.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/jest.config.js
--rw-r--r--   0        0        0   476659 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/package-lock.json
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/setup.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/tsconfig.test.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/webpack.config.js
--rw-r--r--   0        0        0   367662 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/yarn.lock
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/jupyter-config/server-config/oceanumlab.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/_version.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/handlers.py
--rw-r--r--   0        0        0    22225 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/build_log.json
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/package.json
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
--rw-r--r--   0        0        0    68862 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js
--rw-r--r--   0        0        0    64258 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js.map
--rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js
--rw-r--r--   0        0        0    30410 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style.js
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js
--rw-r--r--   0        0        0    15374 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js.map
--rw-r--r--   0        0        0 17743750 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js
--rw-r--r--   0        0        0 10447945 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js.map
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/test_handlers.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/test_settings.ipynb
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/schema/datamesh-connect.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatameshUI.tsx
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatameshWidget.tsx
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatasourceItem.tsx
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/global.d.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/handler.ts
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/svg.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/__tests__/oceanumlab.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/base.css
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/index.js
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/icons/oceanum.png
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/icons/oceanum.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/tests/oceanumlab.spec.ts
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/LICENSE
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/README.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/hatch.toml
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.eslintignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.eslintrc.js
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.prettierrc
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/Makefile
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/RELEASE.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/Untitled.ipynb
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/Untitled1.ipynb
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/_setup.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/babel.config.js
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/conftest.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/environment.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/jest.config.js
+-rw-r--r--   0        0        0   476659 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/package-lock.json
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/setup.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/tsconfig.test.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/webpack.config.js
+-rw-r--r--   0        0        0   367662 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/yarn.lock
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/jupyter-config/server-config/oceanumlab.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/_version.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/handlers.py
+-rw-r--r--   0        0        0    22225 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/build_log.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/install.json
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/package.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
+-rw-r--r--   0        0        0    68862 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js
+-rw-r--r--   0        0        0    64258 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js.map
+-rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js
+-rw-r--r--   0        0        0    30410 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/style.js
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js
+-rw-r--r--   0        0        0    15374 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js.map
+-rw-r--r--   0        0        0 17743750 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js
+-rw-r--r--   0        0        0 10447945 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js.map
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/tests/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/tests/test_handlers.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/oceanumlab/tests/test_settings.ipynb
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/schema/datamesh-connect.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/DatameshUI.tsx
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/DatameshWidget.tsx
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/DatasourceItem.tsx
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/global.d.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/handler.ts
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/svg.d.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/src/__tests__/oceanumlab.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/style/base.css
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/style/index.js
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/style/icons/oceanum.png
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/style/icons/oceanum.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/ui-tests/tests/oceanumlab.spec.ts
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/LICENSE
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/README.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/hatch.toml
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 oceanumlab-4.0.1/PKG-INFO
```

### Comparing `oceanumlab-4.0.0/.eslintrc.js` & `oceanumlab-4.0.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/Makefile` & `oceanumlab-4.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/RELEASE.md` & `oceanumlab-4.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/_setup.py` & `oceanumlab-4.0.1/_setup.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/jest.config.js` & `oceanumlab-4.0.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/package-lock.json` & `oceanumlab-4.0.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/package.json` & `oceanumlab-4.0.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/tsconfig.json` & `oceanumlab-4.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/yarn.lock` & `oceanumlab-4.0.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/__init__.py` & `oceanumlab-4.0.1/oceanumlab/__init__.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/handlers.py` & `oceanumlab-4.0.1/oceanumlab/handlers.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/build_log.json` & `oceanumlab-4.0.1/oceanumlab/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/package.json` & `oceanumlab-4.0.1/oceanumlab/labextension/package.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json` & `oceanumlab-4.0.1/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig` & `oceanumlab-4.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'4.0.1'"}*

```diff
@@ -156,9 +156,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js` & `oceanumlab-4.0.1/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js.map` & `oceanumlab-4.0.1/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js.map`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js` & `oceanumlab-4.0.1/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map` & `oceanumlab-4.0.1/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js` & `oceanumlab-4.0.1/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js.map` & `oceanumlab-4.0.1/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js.map`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js` & `oceanumlab-4.0.1/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js.map` & `oceanumlab-4.0.1/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js.map`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/schema/datamesh-connect.json` & `oceanumlab-4.0.1/schema/datamesh-connect.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'jupyter.lab.setting-icon'": "'oceanum:icon'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "additionalProperties": false,
     "description": "Oceanumlab settings.",
     "icon": "oceanum-io",
-    "jupyter.lab.setting-icon": "oceanum:main",
+    "jupyter.lab.setting-icon": "oceanum:icon",
     "jupyter.lab.setting-icon-label": "Oceanum",
     "jupyter.lab.shortcuts": [],
     "properties": {
         "datameshToken": {
             "default": "",
             "description": "Enter your Datamesh token here. You can obtain this at https://home.oceanum.io/account. You will need to reset your kernel after changing this setting.",
             "title": "Datamesh token",
```

### Comparing `oceanumlab-4.0.0/src/DatameshWidget.tsx` & `oceanumlab-4.0.1/src/DatameshWidget.tsx`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/src/DatasourceItem.tsx` & `oceanumlab-4.0.1/src/DatasourceItem.tsx`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/src/handler.ts` & `oceanumlab-4.0.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/src/index.ts` & `oceanumlab-4.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/style/index.css` & `oceanumlab-4.0.1/style/index.css`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/style/icons/oceanum.png` & `oceanumlab-4.0.1/style/icons/oceanum.png`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/style/icons/oceanum.svg` & `oceanumlab-4.0.1/style/icons/oceanum.svg`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/ui-tests/README.md` & `oceanumlab-4.0.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/ui-tests/tests/oceanumlab.spec.ts` & `oceanumlab-4.0.1/ui-tests/tests/oceanumlab.spec.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/.gitignore` & `oceanumlab-4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/LICENSE` & `oceanumlab-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/README.md` & `oceanumlab-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/pyproject.toml` & `oceanumlab-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oceanumlab-4.0.0/PKG-INFO` & `oceanumlab-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oceanumlab
-Version: 4.0.0
+Version: 4.0.1
 Dynamic: Keywords
 Summary: A Jupyterlab extension to interact with the Oceanum.io platform
 Project-URL: Homepage, https://github.com/oceanum-io/oceanumlab.git
 Project-URL: Bug Tracker, https://github.com/oceanum-io/oceanumlab.git/issues
 Project-URL: Repository, https://github.com/oceanum-io/oceanumlab.git
 Author-email: Oceanum <developers@oceanum.science>
 License: BSD 3-Clause License
```

