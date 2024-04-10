# Comparing `tmp/oceanumlab-0.4.3.tar.gz` & `tmp/oceanumlab-4.0.0.tar.gz`

## Comparing `oceanumlab-0.4.3.tar` & `oceanumlab-4.0.0.tar`

### file list

```diff
@@ -1,108 +1,69 @@
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.copier-answers.yml
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.eslintrc.js
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.prettierrc
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/Makefile
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/babel.config.js
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/jest.config.js
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/package.json
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/tsconfig.test.json
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/webpack.config.js
--rw-r--r--   0        0        0   384785 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/yarn.lock
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.vscode/launch.json
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/.copier-answers.yml
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/.gitignore
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/CHANGELOG.md
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/LICENSE
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/README.md
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/babel.config.js
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/jest.config.js
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/pyproject.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/tsconfig.test.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/jupyter-config/nb-config/oceanumlab.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/jupyter-config/server-config/oceanumlab.json
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/oceanumlab/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/oceanumlab/handlers.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/oceanumlab/tests/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/oceanumlab/tests/test_handlers.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/schema/plugin.json
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/src/handler.ts
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/src/index.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/src/__tests__/oceanumlab.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/yarn.lock
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/_temp_extension/ui-tests/tests/oceanumlab.spec.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/jupyter-config/nb-config/oceanumlab.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/jupyter-config/server-config/oceanumlab.json
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/_version.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/handlers.py
--rw-r--r--   0        0        0    21384 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/build_log.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/install.json
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/package.json
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json
--rw-r--r--   0        0        0    49514 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/lib_index_js.05207cdbfaf8569aa6ae.js
--rw-r--r--   0        0        0    42504 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/lib_index_js.05207cdbfaf8569aa6ae.js.map
--rw-r--r--   0        0        0    49512 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/lib_index_js.fe271c5a1524b3150109.js
--rw-r--r--   0        0        0    42504 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/lib_index_js.fe271c5a1524b3150109.js.map
--rw-r--r--   0        0        0    32179 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.adac79c2b11ab53ec7cf.js
--rw-r--r--   0        0        0    31008 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.adac79c2b11ab53ec7cf.js.map
--rw-r--r--   0        0        0    32179 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.d6c53f9a8466e60ef1b1.js
--rw-r--r--   0        0        0    31008 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.d6c53f9a8466e60ef1b1.js.map
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/style.js
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/style_index_css.35da1c86a5689163d63d.js
--rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/style_index_css.35da1c86a5689163d63d.js.map
--rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.cdb07a33d62465011526.js
--rw-r--r--   0        0        0    13805 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.cdb07a33d62465011526.js.map
--rw-r--r--   0        0        0  8818198 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/vendors-node_modules_phosphor-react_dist_index_esm_js.a2d73cddf27390da0fec.js
--rw-r--r--   0        0        0 10430236 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/labextension/static/vendors-node_modules_phosphor-react_dist_index_esm_js.a2d73cddf27390da0fec.js.map
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/tests/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/oceanumlab/tests/test_handlers.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/schema/plugin.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/DatameshUI.tsx
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/DatameshWidget.tsx
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/DatasourceItem.tsx
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/handler.ts
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/svg.d.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/src/__tests__/oceanumlab.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/style/base.css
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/style/index.js
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/style/icons/oceanum.png
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/style/icons/oceanum.svg
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/ui-tests/tests/oceanumlab.spec.ts
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/LICENSE
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/README.md
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 oceanumlab-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.eslintignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.prettierrc
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/Makefile
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/RELEASE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/_setup.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/babel.config.js
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/conftest.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/environment.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/jest.config.js
+-rw-r--r--   0        0        0   476659 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/package-lock.json
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/setup.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/tsconfig.test.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/webpack.config.js
+-rw-r--r--   0        0        0   367662 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/yarn.lock
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/jupyter-config/server-config/oceanumlab.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/_version.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/handlers.py
+-rw-r--r--   0        0        0    22225 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/build_log.json
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/package.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/package.json.orig
+-rw-r--r--   0        0        0    68862 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js
+-rw-r--r--   0        0        0    64258 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js.map
+-rw-r--r--   0        0        0    31593 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js
+-rw-r--r--   0        0        0    30410 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style.js
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js
+-rw-r--r--   0        0        0    15374 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/style_index_js.089f3d25ce6bfdcec72d.js.map
+-rw-r--r--   0        0        0 17743750 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js
+-rw-r--r--   0        0        0 10447945 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/labextension/static/vendors-node_modules_phosphor-icons_react_dist_index_mjs.d28fe157162aff53d727.js.map
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/test_handlers.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/oceanumlab/tests/test_settings.ipynb
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/schema/datamesh-connect.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatameshUI.tsx
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatameshWidget.tsx
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/DatasourceItem.tsx
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/global.d.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/handler.ts
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/svg.d.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/src/__tests__/oceanumlab.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/base.css
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/index.js
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/icons/oceanum.png
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/style/icons/oceanum.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/ui-tests/tests/oceanumlab.spec.ts
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/README.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/hatch.toml
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 oceanumlab-4.0.0/PKG-INFO
```

### Comparing `oceanumlab-0.4.3/.eslintrc.js` & `oceanumlab-4.0.0/.eslintrc.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -24,14 +24,15 @@
         ],
         '@typescript-eslint/no-unused-vars': ['warn', {
             args: 'none'
         }],
         '@typescript-eslint/no-explicit-any': 'off',
         '@typescript-eslint/no-namespace': 'off',
         '@typescript-eslint/no-use-before-define': 'off',
+        '@typescript-eslint/no-non-null-assertion': 'off',
         '@typescript-eslint/quotes': [
             'error',
             'single', {
                 avoidEscape: true,
                 allowTemplateLiterals: false
             }
         ],
```

### Comparing `oceanumlab-0.4.3/Makefile` & `oceanumlab-4.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/RELEASE.md` & `oceanumlab-4.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/jest.config.js` & `oceanumlab-4.0.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/setup.py` & `oceanumlab-4.0.0/_setup.py`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/tsconfig.json` & `oceanumlab-4.0.0/tsconfig.json`

 * *Files 4% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 00000190: 6972 223a 2022 6c69 6222 2c0a 2020 2020  ir": "lib",.    
 000001a0: 2272 6f6f 7444 6972 223a 2022 7372 6322  "rootDir": "src"
 000001b0: 2c0a 2020 2020 2273 7472 6963 7422 3a20  ,.    "strict": 
 000001c0: 7472 7565 2c0a 2020 2020 2273 7472 6963  true,.    "stric
 000001d0: 744e 756c 6c43 6865 636b 7322 3a20 6661  tNullChecks": fa
 000001e0: 6c73 652c 0a20 2020 2022 7461 7267 6574  lse,.    "target
 000001f0: 223a 2022 4553 3230 3138 222c 0a20 2020  ": "ES2018",.   
-00000200: 2022 7479 7065 7322 3a20 5b22 6a65 7374   "types": ["jest
-00000210: 225d 2c0a 2020 2020 2262 6173 6555 726c  "],.    "baseUrl
-00000220: 223a 2022 2e22 0a20 207d 2c0a 2020 2269  ": ".".  },.  "i
-00000230: 6e63 6c75 6465 223a 205b 2273 7263 2f2a  nclude": ["src/*
-00000240: 225d 0a7d 0a                             "].}.
+00000200: 2022 7374 7269 6374 5072 6f70 6572 7479   "strictProperty
+00000210: 496e 6974 6961 6c69 7a61 7469 6f6e 223a  Initialization":
+00000220: 2066 616c 7365 2c0a 2020 7d2c 0a20 2022   false,.  },.  "
+00000230: 696e 636c 7564 6522 3a20 5b22 7372 632f  include": ["src/
+00000240: 2a22 5d0a 7d0a                           *"].}.
```

### Comparing `oceanumlab-0.4.3/_temp_extension/.gitignore` & `oceanumlab-4.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -119,7 +119,12 @@
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
 
 # Yarn cache
 .yarn/
+
+.vscode
+
+_temp_extension
+.pypirc
```

### Comparing `oceanumlab-0.4.3/_temp_extension/LICENSE` & `oceanumlab-4.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Oceanum
+Copyright (c) 2022, Oceanum
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `oceanumlab-0.4.3/_temp_extension/README.md` & `oceanumlab-4.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # oceanumlab
 
-[![Github Actions Status](https://github.com/oceanum-io/oceanumlab.git/workflows/Build/badge.svg)](https://github.com/oceanum-io/oceanumlab.git/actions/workflows/build.yml)
+<<<<<<< before updating
+[![Github Actions Status](https://github.com/oceanum-io/oceanumlab/workflows/Build/badge.svg)](https://github.com/oceanum-io/oceanumlab/actions/workflows/build.yml)
 A Jupyterlab extension to interact with the Oceanum.io platform
 
 This extension is composed of a Python package named `oceanumlab`
-for the server extension and a NPM package named `@oceanum/oceanumlab`
+for the server extension and a NPM package named `oceanumlab`
 for the frontend extension.
+=======
+[![Github Actions Status](https://github.com/oceanum-io/oceanumlab.git/workflows/Build/badge.svg)](https://github.com/oceanum-io/oceanumlab.git/actions/workflows/build.yml)
+
+A Jupyterlab extension to interact with the Oceanum.io platform
+>>>>>>> after updating
 
 ## Requirements
 
-- JupyterLab >= 4.0.0
+- JupyterLab >= 3.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install oceanumlab
@@ -23,49 +29,31 @@
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall oceanumlab
 ```
 
-## Troubleshoot
-
-If you are seeing the frontend extension, but it is not working, check
-that the server extension is enabled:
-
-```bash
-jupyter server extension list
-```
-
-If the server extension is installed and enabled, but you are not seeing
-the frontend extension, check the frontend extension is installed:
-
-```bash
-jupyter labextension list
-```
-
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the oceanumlab directory
 # Install package in development mode
-pip install -e ".[test]"
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Server extension must be manually installed in develop mode
-jupyter server extension enable oceanumlab
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -82,35 +70,31 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-# Server extension must be manually disabled in develop mode
-jupyter server extension disable oceanumlab
 pip uninstall oceanumlab
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `@oceanum/oceanumlab` within that folder.
+folder is located. Then you can remove the symlink named `oceanumlab` within that folder.
 
 ### Testing the extension
 
 #### Server tests
 
 This extension is using [Pytest](https://docs.pytest.org/) for Python code testing.
 
 Install test dependencies (needed only once):
 
 ```sh
 pip install -e ".[test]"
-# Each time you install the Python package, you need to restore the front-end extension link
-jupyter labextension develop . --overwrite
 ```
 
 To execute them, run:
 
 ```sh
 pytest -vv -r ap --cov oceanumlab
 ```
@@ -124,15 +108,15 @@
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `oceanumlab-0.4.3/_temp_extension/package.json` & `oceanumlab-4.0.0/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8802222222222222%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.1.6', '@jupyterlab/settingregistry': '^4.1.6', "*

 * *                   "'@phosphor-icons/react': '^2.1.4', delete: ['@jupyterlab/coreutils', "*

 * *                   "'@jupyterlab/services']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.1.6', '@jupyterlab/testutils': '^4.1.6', "*

 * *                      "'@types/jest': '^29.5.12', '@types/json-schema': '^7.0.15', '@types/react': "*

 * *                      "'^18.2.75', '@typescript-eslint/eslint-plugin': '^7.6.0 […]*

```diff
@@ -3,130 +3,86 @@
         "email": "developers@oceanum.science",
         "name": "Oceanum"
     },
     "bugs": {
         "url": "https://github.com/oceanum-io/oceanumlab.git/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0",
-        "@jupyterlab/coreutils": "^6.0.0",
-        "@jupyterlab/services": "^7.0.0",
-        "@jupyterlab/settingregistry": "^4.0.0"
+        "@jupyterlab/application": "^4.1.6",
+        "@jupyterlab/settingregistry": "^4.1.6",
+        "@phosphor-icons/react": "^2.1.4"
     },
     "description": "A Jupyterlab extension to interact with the Oceanum.io platform",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0",
-        "@jupyterlab/testutils": "^4.0.0",
-        "@types/jest": "^29.2.0",
-        "@types/json-schema": "^7.0.11",
-        "@types/react": "^18.0.26",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
-        "css-loader": "^6.7.1",
-        "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
-        "eslint-plugin-prettier": "^4.2.1",
-        "jest": "^29.2.0",
-        "mkdirp": "^1.0.3",
+        "@jupyterlab/builder": "^4.1.6",
+        "@jupyterlab/testutils": "^4.1.6",
+        "@types/jest": "^29.5.12",
+        "@types/json-schema": "^7.0.15",
+        "@types/react": "^18.2.75",
+        "@types/react-addons-linked-state-mixin": "^0.14.27",
+        "@typescript-eslint/eslint-plugin": "^7.6.0",
+        "@typescript-eslint/parser": "^7.6.0",
+        "css-loader": "^7.1.0",
+        "eslint": "^9.0.0",
+        "eslint-config-prettier": "^9.1.0",
+        "eslint-plugin-prettier": "^5.1.3",
+        "jest": "^29.7.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.7",
-        "rimraf": "^4.4.1",
-        "source-map-loader": "^1.0.2",
-        "style-loader": "^3.3.1",
-        "stylelint": "^14.9.1",
-        "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^8.0.0",
-        "stylelint-config-standard": "^26.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~5.0.2",
-        "yjs": "^13.5.0"
+        "prettier": "^3.2.5",
+        "rimraf": "^5.0.5",
+        "source-map-loader": "^5.0.0",
+        "style-loader": "^4.0.0",
+        "stylelint": "^16.3.1",
+        "stylelint-config-recommended": "^14.0.0",
+        "stylelint-config-standard": "^36.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^5.0.0",
+        "typescript": "~5.4.4",
+        "yjs": "^13.6.14"
     },
     "eslintConfig": {
+        "base": {
+            "name": "oceanumlab"
+        },
         "extends": [
             "eslint:recommended",
             "plugin:@typescript-eslint/eslint-recommended",
             "plugin:@typescript-eslint/recommended",
             "plugin:prettier/recommended"
         ],
         "parser": "@typescript-eslint/parser",
         "parserOptions": {
             "project": "tsconfig.json",
             "sourceType": "module"
         },
         "plugins": [
             "@typescript-eslint"
-        ],
-        "rules": {
-            "@typescript-eslint/naming-convention": [
-                "error",
-                {
-                    "custom": {
-                        "match": true,
-                        "regex": "^I[A-Z]"
-                    },
-                    "format": [
-                        "PascalCase"
-                    ],
-                    "selector": "interface"
-                }
-            ],
-            "@typescript-eslint/no-explicit-any": "off",
-            "@typescript-eslint/no-namespace": "off",
-            "@typescript-eslint/no-unused-vars": [
-                "warn",
-                {
-                    "args": "none"
-                }
-            ],
-            "@typescript-eslint/no-use-before-define": "off",
-            "@typescript-eslint/quotes": [
-                "error",
-                "single",
-                {
-                    "allowTemplateLiterals": false,
-                    "avoidEscape": true
-                }
-            ],
-            "curly": [
-                "error",
-                "all"
-            ],
-            "eqeqeq": "error",
-            "prefer-arrow-callback": "error"
-        }
+        ]
     },
     "eslintIgnore": [
         "node_modules",
         "dist",
         "coverage",
         "**/*.d.ts",
         "tests",
         "**/__tests__",
         "ui-tests"
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/oceanum-io/oceanumlab.git",
     "jupyterlab": {
-        "discovery": {
-            "server": {
-                "base": {
-                    "name": "oceanumlab"
-                },
-                "managers": [
-                    "pip"
-                ]
-            }
-        },
         "extension": true,
         "outputDir": "oceanumlab/labextension",
-        "schemaDir": "schema"
+        "schemaDir": "schema",
+        "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -147,15 +103,15 @@
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/oceanum-io/oceanumlab.git.git"
+        "url": "https://github.com/oceanum-io/oceanumlab.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
@@ -188,19 +144,21 @@
     "styleModule": "style/index.js",
     "stylelint": {
         "extends": [
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
         "rules": {
+            "csstree/validator": true,
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0",
-    "workspaces": [
-        "ui-tests"
-    ]
+    "version": "4.0.0"
 }
```

### Comparing `oceanumlab-0.4.3/_temp_extension/pyproject.toml` & `oceanumlab-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
-requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "oceanumlab"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "jupyter_server>=2.0.1,<3"
 ]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
@@ -34,26 +33,29 @@
     "pytest-cov",
     "pytest-jupyter[server]>=0.6.0"
 ]
 
 [tool.hatch.version]
 source = "nodejs"
 
+[tool.hatch.envs.oceanumlab]
+description = "OceanumLab JupyterLab extension"
+type="conda"
+
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
 artifacts = ["oceanumlab/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "oceanumlab/labextension" = "share/jupyter/labextensions/@oceanum/oceanumlab"
 "install.json" = "share/jupyter/labextensions/@oceanum/oceanumlab/install.json"
 "jupyter-config/server-config" = "etc/jupyter/jupyter_server_config.d"
-"jupyter-config/nb-config" = "etc/jupyter/jupyter_notebook_config.d"
 
 [tool.hatch.build.hooks.version]
 path = "oceanumlab/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
```

### Comparing `oceanumlab-0.4.3/_temp_extension/oceanumlab/__init__.py` & `oceanumlab-4.0.0/oceanumlab/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+import os
+import json
+from pathlib import Path
+
+from .handlers import setup_handlers
+
+
+HERE = Path(__file__).parent.resolve()
+
 try:
     from ._version import __version__
 except ImportError:
     # Fallback when using the package in dev mode without installing
     # in editable mode with pip. It is highly recommended to install
     # the package from a stable release or in editable mode: https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs
     import warnings
-    warnings.warn("Importing 'oceanumlab' outside a proper installation.")
+
+    warnings.warn(
+        "Importing 'jupyterlab_examples_hello_world' outside a proper installation."
+    )
     __version__ = "dev"
-from .handlers import setup_handlers
 
 
 def _jupyter_labextension_paths():
-    return [{
-        "src": "labextension",
-        "dest": "@oceanum/oceanumlab"
-    }]
+    return [{"src": "labextension", "dest": "@oceanum/oceanumlab"}]
 
 
 def _jupyter_server_extension_points():
-    return [{
-        "module": "oceanumlab"
-    }]
+    return [{"module": "oceanumlab"}]
 
 
 def _load_jupyter_server_extension(server_app):
     """Registers the API handler to receive HTTP requests from the frontend extension.
-
     Parameters
     ----------
     server_app: jupyterlab.labapp.LabApp
         JupyterLab application instance
     """
-    setup_handlers(server_app.web_app)
-    name = "oceanumlab"
-    server_app.log.info(f"Registered {name} server extension")
+    url_path = "oceanum"
+    setup_handlers(server_app.web_app, url_path)
+    server_app.log.info(f"Registered oceanumlab extension at URL path /{url_path}")
 
 
-# For backward compatibility with notebook server - useful for Binder/JupyterHub
+# For backward compatibility with the classical notebook
 load_jupyter_server_extension = _load_jupyter_server_extension
```

### Comparing `oceanumlab-0.4.3/_temp_extension/src/handler.ts` & `oceanumlab-4.0.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/_temp_extension/ui-tests/README.md` & `oceanumlab-4.0.0/ui-tests/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Integration Testing
 
 This folder contains the integration tests of the extension.
 
 They are defined using [Playwright](https://playwright.dev/docs/intro) test runner
-and [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) helper.
+and [Galata](https://github.com/jupyterlab/jupyterlab/tree/main/galata) helper.
 
 The Playwright configuration is defined in [playwright.config.js](./playwright.config.js).
 
 The JupyterLab server configuration to use for the integration test is defined
 in [jupyter_server_test_config.py](./jupyter_server_test_config.py).
 
 The default configuration will produce video for failing tests and an HTML report.
```

### Comparing `oceanumlab-0.4.3/_temp_extension/ui-tests/tests/oceanumlab.spec.ts` & `oceanumlab-4.0.0/ui-tests/tests/oceanumlab.spec.ts`

 * *Files 26% similar despite different names*

```diff
@@ -12,10 +12,10 @@
   page.on('console', message => {
     logs.push(message.text());
   });
 
   await page.goto();
 
   expect(
-    logs.filter(s => s === 'JupyterLab extension @oceanum/oceanumlab is activated!')
+    logs.filter(s => s === 'Oceanum datamesh connect extension is loaded')
   ).toHaveLength(1);
 });
```

### Comparing `oceanumlab-0.4.3/oceanumlab/handlers.py` & `oceanumlab-4.0.0/oceanumlab/handlers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 def setup_handlers(web_app, url_path):
     host_pattern = ".*$"
     base_url = web_app.settings["base_url"]
 
     # Prepend the base_url so that it works in a JupyterHub setting
     env_pattern = url_path_join(base_url, url_path, "env/(.*)")
     handlers = [(env_pattern, EnvarsHandler)]
-    web_app.add_handlers(host_pattern, handlers)
+    web_app.add_handlers(host_pattern, handlers)
```

### Comparing `oceanumlab-0.4.3/oceanumlab/labextension/package.json` & `oceanumlab-4.0.0/oceanumlab/labextension/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.657088888888889%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/oceanum-io/oceanumlab.git/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.1.6', '@jupyterlab/settingregistry': '^4.1.6', "*

 * *                   "'@phosphor-icons/react': '^2.1.4', delete: ['@jupyterlab/apputils', "*

 * *                   "'@jupyterlab/coreutils', '@jupyterlab/services', "*

 * *                   "'@jupyterlab/rendermime-interfaces', 'phosphor-react']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.1.6', '@jupyterlab/testutils': '^4.1.6', "*

 * *  […]*

```diff
@@ -1,128 +1,169 @@
 {
     "author": {
         "email": "developers@oceanum.science",
         "name": "Oceanum"
     },
     "bugs": {
-        "url": "https://github.com/oceanum-io/oceanumlab/issues"
+        "url": "https://github.com/oceanum-io/oceanumlab.git/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.1",
-        "@jupyterlab/apputils": "3.6.1",
-        "@jupyterlab/coreutils": "^5.6.1",
-        "@jupyterlab/rendermime-interfaces": "3.6.1",
-        "@jupyterlab/services": "^6.6.1",
-        "@jupyterlab/settingregistry": "^3.6.1",
-        "phosphor-react": "^1.4.1"
+        "@jupyterlab/application": "^4.1.6",
+        "@jupyterlab/settingregistry": "^4.1.6",
+        "@phosphor-icons/react": "^2.1.4"
     },
     "description": "A Jupyterlab extension to interact with the Oceanum.io platform",
     "devDependencies": {
-        "@babel/core": "^7.21.0",
-        "@babel/preset-env": "^7.20.2",
-        "@jupyterlab/builder": "^3.6.1",
-        "@jupyterlab/testutils": "^3.6.1",
-        "@types/jest": "~26.0.0",
-        "@typescript-eslint/eslint-plugin": "^5.54.0",
-        "@typescript-eslint/parser": "^5.54.0",
-        "eslint": "^8.35.0",
-        "eslint-config-prettier": "^8.6.0",
-        "eslint-plugin-prettier": "^4.2.1",
-        "jest": "~26.0.0",
-        "mkdirp": "^2.1.3",
+        "@jupyterlab/builder": "^4.1.6",
+        "@jupyterlab/testutils": "^4.1.6",
+        "@types/jest": "^29.5.12",
+        "@types/json-schema": "^7.0.15",
+        "@types/react": "^18.2.75",
+        "@types/react-addons-linked-state-mixin": "^0.14.27",
+        "@typescript-eslint/eslint-plugin": "^7.6.0",
+        "@typescript-eslint/parser": "^7.6.0",
+        "css-loader": "^7.1.0",
+        "eslint": "^9.0.0",
+        "eslint-config-prettier": "^9.1.0",
+        "eslint-plugin-prettier": "^5.1.3",
+        "jest": "^29.7.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.4",
-        "rimraf": "^4.1.2",
-        "stylelint": "^15.2.0",
-        "stylelint-config-prettier": "^9.0.5",
-        "stylelint-config-recommended": "^10.0.1",
-        "stylelint-config-standard": "~30.0.1",
-        "stylelint-prettier": "^3.0.0",
-        "ts-jest": "^29.0.5",
-        "typescript": "4.1.6"
-    },
+        "prettier": "^3.2.5",
+        "rimraf": "^5.0.5",
+        "source-map-loader": "^5.0.0",
+        "style-loader": "^4.0.0",
+        "stylelint": "^16.3.1",
+        "stylelint-config-recommended": "^14.0.0",
+        "stylelint-config-standard": "^36.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^5.0.0",
+        "typescript": "~5.4.4",
+        "yjs": "^13.6.14"
+    },
+    "eslintConfig": {
+        "base": {
+            "name": "oceanumlab"
+        },
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ]
+    },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
-    "homepage": "https://github.com/oceanum-io/oceanumlab",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
-        }
-    },
+    "homepage": "https://github.com/oceanum-io/oceanumlab.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d6c53f9a8466e60ef1b1.js",
+            "load": "static/remoteEntry.1c4cc02ec4ec7f0e8dba.js",
             "style": "./style"
         },
-        "discovery": {
-            "server": {
-                "base": {
-                    "name": "oceanumlab"
-                },
-                "managers": [
-                    "pip"
-                ]
-            }
-        },
         "extension": true,
         "outputDir": "oceanumlab/labextension",
         "schemaDir": "schema",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@oceanum/oceanumlab",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/oceanum-io/oceanumlab.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "npx tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf oceanumlab/labextension",
+        "clean:labextension": "rimraf oceanumlab/labextension oceanumlab/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest --coverage --passWithNoTests",
+        "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "npx tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
-        "style/*.css"
+        "style/*.css",
+        "style/index.js"
     ],
     "style": "style/index.css",
+    "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
+        "rules": {
+            "csstree/validator": true,
+            "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.4.2"
+    "version": "4.0.0"
 }
```

### Comparing `oceanumlab-0.4.3/oceanumlab/labextension/schemas/@oceanum/oceanumlab/plugin.json` & `oceanumlab-4.0.0/oceanumlab/labextension/schemas/@oceanum/oceanumlab/datamesh-connect.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'description'": "'Oceanumlab settings.'", "'icon'": "'oceanum-io'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "additionalProperties": false,
-    "description": "oceanumlab settings.",
-    "icon": "oceanum",
+    "description": "Oceanumlab settings.",
+    "icon": "oceanum-io",
     "jupyter.lab.setting-icon": "oceanum:main",
     "jupyter.lab.setting-icon-label": "Oceanum",
     "jupyter.lab.shortcuts": [],
     "properties": {
         "datameshToken": {
             "default": "",
             "description": "Enter your Datamesh token here. You can obtain this at https://home.oceanum.io/account. You will need to reset your kernel after changing this setting.",
```

### Comparing `oceanumlab-0.4.3/oceanumlab/labextension/static/lib_index_js.05207cdbfaf8569aa6ae.js` & `oceanumlab-4.0.0/oceanumlab/labextension/static/lib_index_js.4c53e7d97d745fd9dd50.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,40 +1,182 @@
 "use strict";
 (self["webpackChunk_oceanum_oceanumlab"] = self["webpackChunk_oceanum_oceanumlab"] || []).push([
     ["lib_index_js"], {
 
         /***/
-        "./node_modules/css-loader/dist/cjs.js!./style/index.css":
-            /*!***************************************************************!*\
-              !*** ./node_modules/css-loader/dist/cjs.js!./style/index.css ***!
-              \***************************************************************/
+        "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/cjs.js!./style/index.css":
+            /*!************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/cjs.js!./style/index.css ***!
+              \************************************************************************************************/
             /***/
             ((module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
                 /* harmony import */
-                var _node_modules_css_loader_dist_runtime_cssWithMappingToString_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ../node_modules/css-loader/dist/runtime/cssWithMappingToString.js */ "./node_modules/css-loader/dist/runtime/cssWithMappingToString.js");
+                var _node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_sourceMaps_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! ../node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/sourceMaps.js */ "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/sourceMaps.js");
                 /* harmony import */
-                var _node_modules_css_loader_dist_runtime_cssWithMappingToString_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_css_loader_dist_runtime_cssWithMappingToString_js__WEBPACK_IMPORTED_MODULE_0__);
+                var _node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_sourceMaps_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_sourceMaps_js__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
-                var _node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ../node_modules/css-loader/dist/runtime/api.js */ "./node_modules/css-loader/dist/runtime/api.js");
+                var _node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ../node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/api.js */ "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/api.js");
                 /* harmony import */
-                var _node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1__);
+                var _node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1__);
                 // Imports
 
 
-                var ___CSS_LOADER_EXPORT___ = _node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default()((_node_modules_css_loader_dist_runtime_cssWithMappingToString_js__WEBPACK_IMPORTED_MODULE_0___default()));
+                var ___CSS_LOADER_EXPORT___ = _node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_api_js__WEBPACK_IMPORTED_MODULE_1___default()((_node_modules_jupyterlab_builder_node_modules_css_loader_dist_runtime_sourceMaps_js__WEBPACK_IMPORTED_MODULE_0___default()));
                 // Module
-                ___CSS_LOADER_EXPORT___.push([module.id, ".datasource-drag-image {\n  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);\n  width: var(--jp-private-notebook-dragImage-width);\n  height: var(--jp-private-notebook-dragImage-height);\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n}\n\n.datamesh-iframe {\n  width: 98%;\n  height: 98%;\n  padding: 5px;\n}\n\n.datamesh-connect {\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n  height: 100%;\n}\n\n.datamesh-connect a {\n  color: var(--jp-content-link-color);\n}\n\n.datamesh-connect-header {\n  font-weight: bold;\n  padding: 8px 10px;\n  display: flex;\n  justify-content: space-between;\n}\n\n.datamesh-connect-header p {\n  font-weight: bold;\n}\n\n.add-connection {\n  border-radius: 4px;\n}\n\n.add-connection :hover {\n  background-color: #ddd;\n}\n\n.datasource-list-item {\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  display: flex;\n  flex-direction: column;\n  margin: 0;\n  padding: 0;\n}\n\n.open-datamesh-ui {\n  cursor: pointer;\n}\n\n.datamesh-workspace-name {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  padding: 8px 8px 8px 12px;\n  margin: 0;\n  margin-left: 0;\n  margin-bottom: 10px;\n  font-size: var(--jp-ui-font-size1);\n}\n\n.datasource-item-expand,\n.datasource-item-action,\n.datasource-item-expand.jp-mod-styled {\n  background-color: transparent;\n  vertical-align: middle;\n  padding: 0;\n  width: 20px;\n  border: none;\n}\n\n.datasource-item-expand:hover {\n  cursor: pointer;\n}\n\n.datasource-item-details {\n  overflow-x: auto;\n  overflow-y: auto;\n  display: block;\n  padding: 5px;\n  margin: 5px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color1);\n  background-color: var(--jp-layout-color1);\n}\n\n.datasource-item-details textarea {\n  color: var(--jp-ui-font-color1);\n}\n\n.datasource-item-action {\n  display: inline-flex;\n  align-self: flex-end;\n  align-items: center;\n  height: 100%;\n  border: none;\n}\n\n.datasource-item-name {\n  flex-grow: 1;\n  font-size: var(--jp-ui-font-size1);\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  padding: 4px 0 4px 2px;\n  line-height: 28px;\n}\n\n.datasource-item-action:hover,\n.datasource-item-name:hover {\n  cursor: pointer;\n}\n\n.datasource-item-title {\n  align-items: center;\n  display: flex;\n  flex-direction: row;\n  padding: 0 4px;\n  height: 36px;\n}\n\n.datasource-item-title:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.datasource-query-field span {\n  margin-left: 5px;\n  white-space: nowrap;\n  font-size: var(--jp-ui-font-size0);\n}\n\n.expanded {\n  background-color: var(--jp-layout-color2);\n  padding: 2px;\n}\n", "", {
+                ___CSS_LOADER_EXPORT___.push([module.id, `.datasource-drag-image {
+  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
+  width: var(--jp-private-notebook-dragImage-width);
+  height: var(--jp-private-notebook-dragImage-height);
+  color: var(--jp-ui-font-color1);
+  background: var(--jp-layout-color1);
+}
+
+.datamesh-iframe {
+  width: 98%;
+  height: 98%;
+  padding: 5px;
+}
+
+.datamesh-connect {
+  color: var(--jp-ui-font-color1);
+  background: var(--jp-layout-color1);
+  height: 100%;
+}
+
+.datamesh-connect a {
+  color: var(--jp-content-link-color);
+}
+
+.datamesh-connect-header {
+  font-weight: bold;
+  padding: 8px 10px;
+  display: flex;
+  justify-content: space-between;
+}
+
+.datamesh-connect-header p {
+  font-weight: bold;
+}
+
+.add-connection {
+  border-radius: 4px;
+}
+
+.add-connection :hover {
+  background-color: #ddd;
+}
+
+.datasource-list-item {
+  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
+  display: flex;
+  flex-direction: column;
+  margin: 0;
+  padding: 0;
+}
+
+.open-datamesh-ui {
+  cursor: pointer;
+}
+
+.datamesh-workspace-name {
+  flex: 0 0 auto;
+  font-weight: 600;
+  text-transform: uppercase;
+  letter-spacing: 1px;
+  padding: 8px 8px 8px 12px;
+  margin: 0;
+  margin-left: 0;
+  margin-bottom: 10px;
+  font-size: var(--jp-ui-font-size1);
+}
+
+.datasource-item-expand,
+.datasource-item-action,
+.datasource-item-expand.jp-mod-styled {
+  background-color: transparent;
+  vertical-align: middle;
+  padding: 0;
+  width: 20px;
+  border: none;
+}
+
+.datasource-item-expand:hover {
+  cursor: pointer;
+}
+
+.datasource-item-details {
+  overflow-x: auto;
+  overflow-y: auto;
+  display: block;
+  padding: 5px;
+  margin: 5px;
+  border: 1px solid var(--jp-border-color2);
+  border-radius: 2px;
+  color: var(--jp-ui-font-color1);
+  background-color: var(--jp-layout-color1);
+}
+
+.datasource-item-details textarea {
+  color: var(--jp-ui-font-color1);
+}
+
+.datasource-item-action {
+  display: inline-flex;
+  align-self: flex-end;
+  align-items: center;
+  height: 100%;
+  border: none;
+}
+
+.datasource-item-name {
+  flex-grow: 1;
+  font-size: var(--jp-ui-font-size1);
+  white-space: nowrap;
+  overflow: hidden;
+  text-overflow: ellipsis;
+  padding: 4px 0 4px 2px;
+  line-height: 28px;
+}
+
+.datasource-item-action:hover,
+.datasource-item-name:hover {
+  cursor: pointer;
+}
+
+.datasource-item-title {
+  align-items: center;
+  display: flex;
+  flex-direction: row;
+  padding: 0 4px;
+  height: 36px;
+}
+
+.datasource-item-title:hover {
+  background-color: var(--jp-layout-color2);
+}
+
+.datasource-query-field span {
+  margin-left: 5px;
+  white-space: nowrap;
+  font-size: var(--jp-ui-font-size0);
+}
+
+.expanded {
+  background-color: var(--jp-layout-color2);
+  padding: 2px;
+}
+`, "", {
                     "version": 3,
                     "sources": ["webpack://./style/index.css"],
                     "names": [],
                     "mappings": "AAAA;EACE,uEAAuE;EACvE,iDAAiD;EACjD,mDAAmD;EACnD,+BAA+B;EAC/B,mCAAmC;AACrC;;AAEA;EACE,UAAU;EACV,WAAW;EACX,YAAY;AACd;;AAEA;EACE,+BAA+B;EAC/B,mCAAmC;EACnC,YAAY;AACd;;AAEA;EACE,mCAAmC;AACrC;;AAEA;EACE,iBAAiB;EACjB,iBAAiB;EACjB,aAAa;EACb,8BAA8B;AAChC;;AAEA;EACE,iBAAiB;AACnB;;AAEA;EACE,kBAAkB;AACpB;;AAEA;EACE,sBAAsB;AACxB;;AAEA;EACE,mEAAmE;EACnE,aAAa;EACb,sBAAsB;EACtB,SAAS;EACT,UAAU;AACZ;;AAEA;EACE,eAAe;AACjB;;AAEA;EACE,cAAc;EACd,gBAAgB;EAChB,yBAAyB;EACzB,mBAAmB;EACnB,yBAAyB;EACzB,SAAS;EACT,cAAc;EACd,mBAAmB;EACnB,kCAAkC;AACpC;;AAEA;;;EAGE,6BAA6B;EAC7B,sBAAsB;EACtB,UAAU;EACV,WAAW;EACX,YAAY;AACd;;AAEA;EACE,eAAe;AACjB;;AAEA;EACE,gBAAgB;EAChB,gBAAgB;EAChB,cAAc;EACd,YAAY;EACZ,WAAW;EACX,yCAAyC;EACzC,kBAAkB;EAClB,+BAA+B;EAC/B,yCAAyC;AAC3C;;AAEA;EACE,+BAA+B;AACjC;;AAEA;EACE,oBAAoB;EACpB,oBAAoB;EACpB,mBAAmB;EACnB,YAAY;EACZ,YAAY;AACd;;AAEA;EACE,YAAY;EACZ,kCAAkC;EAClC,mBAAmB;EACnB,gBAAgB;EAChB,uBAAuB;EACvB,sBAAsB;EACtB,iBAAiB;AACnB;;AAEA;;EAEE,eAAe;AACjB;;AAEA;EACE,mBAAmB;EACnB,aAAa;EACb,mBAAmB;EACnB,cAAc;EACd,YAAY;AACd;;AAEA;EACE,yCAAyC;AAC3C;;AAEA;EACE,gBAAgB;EAChB,mBAAmB;EACnB,kCAAkC;AACpC;;AAEA;EACE,yCAAyC;EACzC,YAAY;AACd",
                     "sourcesContent": [".datasource-drag-image {\n  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);\n  width: var(--jp-private-notebook-dragImage-width);\n  height: var(--jp-private-notebook-dragImage-height);\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n}\n\n.datamesh-iframe {\n  width: 98%;\n  height: 98%;\n  padding: 5px;\n}\n\n.datamesh-connect {\n  color: var(--jp-ui-font-color1);\n  background: var(--jp-layout-color1);\n  height: 100%;\n}\n\n.datamesh-connect a {\n  color: var(--jp-content-link-color);\n}\n\n.datamesh-connect-header {\n  font-weight: bold;\n  padding: 8px 10px;\n  display: flex;\n  justify-content: space-between;\n}\n\n.datamesh-connect-header p {\n  font-weight: bold;\n}\n\n.add-connection {\n  border-radius: 4px;\n}\n\n.add-connection :hover {\n  background-color: #ddd;\n}\n\n.datasource-list-item {\n  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);\n  display: flex;\n  flex-direction: column;\n  margin: 0;\n  padding: 0;\n}\n\n.open-datamesh-ui {\n  cursor: pointer;\n}\n\n.datamesh-workspace-name {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  padding: 8px 8px 8px 12px;\n  margin: 0;\n  margin-left: 0;\n  margin-bottom: 10px;\n  font-size: var(--jp-ui-font-size1);\n}\n\n.datasource-item-expand,\n.datasource-item-action,\n.datasource-item-expand.jp-mod-styled {\n  background-color: transparent;\n  vertical-align: middle;\n  padding: 0;\n  width: 20px;\n  border: none;\n}\n\n.datasource-item-expand:hover {\n  cursor: pointer;\n}\n\n.datasource-item-details {\n  overflow-x: auto;\n  overflow-y: auto;\n  display: block;\n  padding: 5px;\n  margin: 5px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color1);\n  background-color: var(--jp-layout-color1);\n}\n\n.datasource-item-details textarea {\n  color: var(--jp-ui-font-color1);\n}\n\n.datasource-item-action {\n  display: inline-flex;\n  align-self: flex-end;\n  align-items: center;\n  height: 100%;\n  border: none;\n}\n\n.datasource-item-name {\n  flex-grow: 1;\n  font-size: var(--jp-ui-font-size1);\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  padding: 4px 0 4px 2px;\n  line-height: 28px;\n}\n\n.datasource-item-action:hover,\n.datasource-item-name:hover {\n  cursor: pointer;\n}\n\n.datasource-item-title {\n  align-items: center;\n  display: flex;\n  flex-direction: row;\n  padding: 0 4px;\n  height: 36px;\n}\n\n.datasource-item-title:hover {\n  background-color: var(--jp-layout-color2);\n}\n\n.datasource-query-field span {\n  margin-left: 5px;\n  white-space: nowrap;\n  font-size: var(--jp-ui-font-size0);\n}\n\n.expanded {\n  background-color: var(--jp-layout-color2);\n  padding: 2px;\n}\n"],
                     "sourceRoot": ""
                 }]);
@@ -43,35 +185,14 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (___CSS_LOADER_EXPORT___);
 
 
                 /***/
             }),
 
         /***/
-        "./style/icons/oceanum.svg":
-            /*!*********************************!*\
-              !*** ./style/icons/oceanum.svg ***!
-              \*********************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony export */
-                __webpack_require__.d(__webpack_exports__, {
-                    /* harmony export */
-                    "default": () => (__WEBPACK_DEFAULT_EXPORT__)
-                    /* harmony export */
-                });
-                /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = ("<svg xmlns=\"http://www.w3.org/2000/svg\" width=\"44\" height=\"44\" viewBox=\"0 0 44.079582 44.079582\" version=\"1.1\" id=\"svg5870\">\n  <g\n     id=\"layer1\"\n     transform=\"translate(-82.281595,-124.52568)\">\n    <g\n       style=\"stroke:#3b547c;stroke-opacity:1\"\n       transform=\"matrix(0.26458333,0,0,0.26458333,69.475762,109.81485)\"\n       id=\"g2915\"\n       >\n      <g\n         style=\"stroke:#3b547c;stroke-opacity:1\"\n         id=\"g2903\">\n        <path\n           id=\"path2897\"\n           d=\"m 212.3,149.9 c -35.8,19.1 -58.2,-11 -80.6,-11 -22.4,0 -44.7,30.1 -80.6,11 1.2,8.7 3.8,17.2 7.7,25.1 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4 3.9,-7.9 6.5,-16.3 7.7,-25.1 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n        <path\n           id=\"path2899\"\n           d=\"m 204.6,175 c -38.7,13.5 -55.8,-8.4 -72.9,-8.4 -17.1,0 -34.1,22 -72.9,8.4 4.4,8.9 10.4,16.9 17.7,23.6 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 7.3,-6.7 13.3,-14.7 17.7,-23.6 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n        <path\n           id=\"path2901\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 -15,13.9 -34.7,21.6 -55.2,21.6 -20.4,-0.1 -40.2,-7.8 -55.2,-21.6 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n      </g>\n      <g\n         style=\"stroke:#3b547c;stroke-opacity:1\"\n         id=\"g2913\">\n        <path\n           id=\"path2905\"\n           d=\"m 58.8,175 c 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2907\"\n           d=\"m 51.1,149.9 c 35.8,19.1 58.2,-11 80.6,-11 22.4,0 44.7,30.1 80.6,11\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2909\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2911\"\n           d=\"m 131.7,220.2 c 10.3,0 20.4,-1.9 29.9,-5.7 10.3,-4.1 19.7,-10.2 27.6,-18.1 7.9,-7.9 14,-17.2 18.1,-27.6 3.8,-9.5 5.7,-19.7 5.7,-29.9 0,-10.3 -1.9,-20.4 -5.7,-29.9 -4.1,-10.3 -10.2,-19.7 -18.1,-27.6 -7.9,-7.9 -17.2,-14 -27.6,-18.1 -9.5,-3.8 -19.7,-5.7 -29.9,-5.7 -10.3,0 -20.4,1.9 -29.9,5.7 -10.3,4.1 -19.7,10.2 -27.6,18.1 -7.9,7.9 -14,17.2 -18.1,27.6 -3.8,9.5 -5.7,19.7 -5.7,29.9 0,10.3 1.9,20.4 5.7,29.9 4.1,10.3 10.2,19.7 18.1,27.6 7.9,7.9 17.2,14 27.6,18.1 9.5,3.8 19.6,5.7 29.9,5.7 z\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n      </g>\n    </g>\n    <g\n       id=\"g3308\"\n       transform=\"matrix(0.26458333,0,0,0.26458333,69.475762,109.81485)\"\n       style=\"stroke:#3b547c;stroke-opacity:1\">\n      <g\n         id=\"g3296\"\n         style=\"stroke:#3b547c;stroke-opacity:1\">\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 212.3,149.9 c -35.8,19.1 -58.2,-11 -80.6,-11 -22.4,0 -44.7,30.1 -80.6,11 1.2,8.7 3.8,17.2 7.7,25.1 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4 3.9,-7.9 6.5,-16.3 7.7,-25.1 z\"\n           id=\"path3290\" />\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 204.6,175 c -38.7,13.5 -55.8,-8.4 -72.9,-8.4 -17.1,0 -34.1,22 -72.9,8.4 4.4,8.9 10.4,16.9 17.7,23.6 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 7.3,-6.7 13.3,-14.7 17.7,-23.6 z\"\n           id=\"path3292\" />\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 -15,13.9 -34.7,21.6 -55.2,21.6 -20.4,-0.1 -40.2,-7.8 -55.2,-21.6 z\"\n           id=\"path3294\" />\n      </g>\n      <g\n         id=\"g3306\"\n         style=\"stroke:#3b547c;stroke-opacity:1\">\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 58.8,175 c 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4\"\n           id=\"path3298\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 51.1,149.9 c 35.8,19.1 58.2,-11 80.6,-11 22.4,0 44.7,30.1 80.6,11\"\n           id=\"path3300\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5\"\n           id=\"path3302\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 131.7,220.2 c 10.3,0 20.4,-1.9 29.9,-5.7 10.3,-4.1 19.7,-10.2 27.6,-18.1 7.9,-7.9 14,-17.2 18.1,-27.6 3.8,-9.5 5.7,-19.7 5.7,-29.9 0,-10.3 -1.9,-20.4 -5.7,-29.9 -4.1,-10.3 -10.2,-19.7 -18.1,-27.6 -7.9,-7.9 -17.2,-14 -27.6,-18.1 -9.5,-3.8 -19.7,-5.7 -29.9,-5.7 -10.3,0 -20.4,1.9 -29.9,5.7 -10.3,4.1 -19.7,10.2 -27.6,18.1 -7.9,7.9 -14,17.2 -18.1,27.6 -3.8,9.5 -5.7,19.7 -5.7,29.9 0,10.3 1.9,20.4 5.7,29.9 4.1,10.3 10.2,19.7 18.1,27.6 7.9,7.9 17.2,14 27.6,18.1 9.5,3.8 19.6,5.7 29.9,5.7 z\"\n           id=\"path3304\" />\n      </g>\n    </g>\n  </g>\n</svg>\n");
-
-                /***/
-            }),
-
-        /***/
         "./lib/DatameshUI.js":
             /*!***************************!*\
               !*** ./lib/DatameshUI.js ***!
               \***************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -91,15 +212,15 @@
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__);
 
 
                 class DatameshUI extends _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget {
                     render() {
                         return (react__WEBPACK_IMPORTED_MODULE_0___default().createElement("iframe", {
-                            src: `${"https://ui.datamesh.oceanum.tech"}`,
+                            src: `${"https://ui.datamesh.oceanum.io"}`,
                             className: "datamesh-iframe"
                         }));
                     }
                 }
 
 
                 /***/
@@ -159,15 +280,18 @@
 
 
 
 
 
 
 
+
                 const JUPYTER_CELL_MIME = 'application/vnd.jupyter.cells';
+                const DRAG_IMAGE = new Image();
+                DRAG_IMAGE.src = 'data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMiIgaGVpZ2h0PSIzMiIgZmlsbD0iIzAwMDAwMCIgdmlld0JveD0iMCAwIDI1NiAyNTYiPjxwYXRoIGQ9Ik02OS4xMiw5NC4xNSwyOC41LDEyOGw0MC42MiwzMy44NWE4LDgsMCwxLDEtMTAuMjQsMTIuMjlsLTQ4LTQwYTgsOCwwLDAsMSwwLTEyLjI5bDQ4LTQwYTgsOCwwLDAsMSwxMC4yNCwxMi4zWm0xNzYsMjcuNy00OC00MGE4LDgsMCwxLDAtMTAuMjQsMTIuM0wyMjcuNSwxMjhsLTQwLjYyLDMzLjg1YTgsOCwwLDEsMCwxMC4yNCwxMi4yOWw0OC00MGE4LDgsMCwwLDAsMC0xMi4yOVpNMTYyLjczLDMyLjQ4YTgsOCwwLDAsMC0xMC4yNSw0Ljc5bC02NCwxNzZhOCw4LDAsMCwwLDQuNzksMTAuMjZBOC4xNCw4LjE0LDAsMCwwLDk2LDIyNGE4LDgsMCwwLDAsNy41Mi01LjI3bDY0LTE3NkE4LDgsMCwwLDAsMTYyLjczLDMyLjQ4WiI+PC9wYXRoPjwvc3ZnPg==';
                 const datameshToken = (notebook) => {
                     const datameshTokenInjected = notebook &&
                         notebook.widgets.find(cell => {
                             if (cell.editor) {
                                 const line = cell.editor.getLine(0);
                                 if (line && line.indexOf('DATAMESH_TOKEN=') >= 0) {
                                     return true;
@@ -218,62 +342,70 @@
                     }
                     return datasourceStr;
                 };
                 class DatameshWorkspaceDisplay extends(react__WEBPACK_IMPORTED_MODULE_7___default().Component) {
                     constructor(props) {
                         super(props);
                         this.injectToken = (notebookWidget) => {
+                            var _a;
                             const notebookContent = notebookWidget.content;
                             const datameshTokenInject = datameshToken(notebookContent);
+                            //const codeCell=new CodeCellModel({});
                             if (datameshTokenInject) {
-                                const tokenCell = notebookContent.model.contentFactory.createCodeCell({
-                                    cell: {
-                                        cell_type: 'code',
-                                        source: datameshTokenInject,
-                                        metadata: {
-                                            tags: ['hide_input']
-                                        }
-                                    }
+                                // const tokenCell = notebookContent.contentFactory.createCodeCell({
+                                //   model: codeCell,
+                                //   rendermime: notebookContent.rendermime,
+                                //   contentFactory: notebookContent.contentFactory,
+                                // })
+                                // tokenCell.model.sharedModel.setSource(datameshTokenInject);
+                                (_a = notebookContent.model) === null || _a === void 0 ? void 0 : _a.sharedModel.insertCell(0, {
+                                    cell_type: 'code',
+                                    source: datameshTokenInject,
+                                    metadata: {},
                                 });
-                                notebookContent.model.cells.insert(0, tokenCell);
-                                _jupyterlab_cells__WEBPACK_IMPORTED_MODULE_1__.CodeCell.execute(notebookContent.widgets[0], notebookWidget.sessionContext);
+                                // CodeCell.execute(
+                                //   notebookContent.widgets[0] as CodeCell,
+                                //   notebookWidget.sessionContext
+                                // );
                             }
                         };
                         // Handle code datasource insert into an editor
                         this.insertDatameshConnect = async (datasource) => {
                             const widget = this.props.getCurrentWidget();
                             if (widget instanceof _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_2__.NotebookPanel) {
                                 const notebookWidget = widget;
                                 const notebookContent = notebookWidget.content;
                                 const notebookCell = notebookContent.activeCell;
                                 const notebookCellIndex = notebookContent.activeCellIndex;
                                 const notebookCellEditor = notebookCell.editor;
                                 const datasourceStr = datasourceCode(datasource, notebookContent, notebookCellIndex);
-                                if (notebookCell instanceof _jupyterlab_cells__WEBPACK_IMPORTED_MODULE_1__.CodeCell) {
-                                    this.verifyLanguageAndInsert(datasourceStr, 'python', notebookCellEditor);
+                                if (notebookCellEditor) {
+                                    if (notebookCell instanceof _jupyterlab_cells__WEBPACK_IMPORTED_MODULE_1__.CodeCell) {
+                                        this.verifyLanguageAndInsert(datasourceStr, 'python', notebookCellEditor);
+                                    } else {
+                                        notebookCellEditor.replaceSelection(datasourceStr);
+                                    }
+                                    if (window.injectToken) {
+                                        this.injectToken(notebookWidget);
+                                    }
                                 } else {
-                                    notebookCellEditor.replaceSelection(datasourceStr);
+                                    this.showErrDialog('Datamesh datasource insert failed: Please select code cell');
                                 }
-                                if (window.injectToken) {
-                                    this.injectToken(notebookWidget);
-                                }
-                            } else {
-                                this.showErrDialog('Datamesh datasource insert failed: Please select code cell');
                             }
                         };
                         // Handle language compatibility between code datasource and editor
                         this.verifyLanguageAndInsert = async (datasourceStr, editorLanguage, editor) => {
-                            if (editorLanguage && 'python' !== editorLanguage.toLowerCase()) {
+                            if (editor && editorLanguage && 'python' !== editorLanguage.toLowerCase()) {
                                 const result = await this.showWarnDialog(editorLanguage);
                                 if (result.button.accept) {
                                     editor.replaceSelection(datasourceStr);
                                 }
                             } else {
                                 // Language match or editorLanguage is unavailable
-                                editor.replaceSelection(datasourceStr);
+                                editor === null || editor === void 0 ? void 0 : editor.replaceSelection(datasourceStr);
                             }
                         };
                         // Display warning dialog when inserting a code datasource incompatible with editor's language
                         this.showWarnDialog = async (editorLanguage) => {
                             return (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showDialog)({
                                 title: 'Warning',
                                 body: `Datamesh connector is incompatible with ${editorLanguage}. Continue?`,
@@ -324,15 +456,15 @@
                         // do nothing if left mouse button is clicked
                         if (button !== 0) {
                             return;
                         }
                         this._dragData = {
                             pressX: event.clientX,
                             pressY: event.clientY,
-                            dragImage: null
+                            dragImage: DRAG_IMAGE
                         };
                         const mouseUpListener = (event) => {
                             this._evtMouseUp(event, datasource, mouseMoveListener);
                         };
                         const mouseMoveListener = (event) => {
                             this.handleDragMove(event, datasource, mouseMoveListener, mouseUpListener);
                         };
@@ -380,30 +512,36 @@
                      */
                     shouldStartDrag(prevX, prevY, nextX, nextY) {
                         const dx = Math.abs(nextX - prevX);
                         const dy = Math.abs(nextY - prevY);
                         return dx >= 0 || dy >= 5;
                     }
                     async startDrag(dragImage, datasource, clientX, clientY) {
-                        const contentFactory = new _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_2__.NotebookModel.ContentFactory({});
-                        const model = contentFactory.createCodeCell({});
-                        let content = datasourceCode(datasource, null, 0);
+                        const notebookPanel = this.props.getCurrentWidget();
+                        const notebookContent = notebookPanel.content;
+                        const codeCell = new _jupyterlab_cells__WEBPACK_IMPORTED_MODULE_1__.CodeCellModel({});
+                        const cell = notebookContent.contentFactory.createCodeCell({
+                            model: codeCell,
+                            rendermime: notebookContent.rendermime,
+                            contentFactory: notebookContent.contentFactory
+                        });
+                        let content = datasourceCode(datasource, notebookContent, 0);
                         if (window.injectToken) {
                             const notebookPanel = this.props.getCurrentWidget();
                             content = datameshToken(notebookPanel.content) + '\n' + content;
                         }
-                        model.value.text = content;
+                        cell.model.sharedModel.setSource(content);
                         this._drag = new _lumino_dragdrop__WEBPACK_IMPORTED_MODULE_5__.Drag({
                             mimeData: new _lumino_coreutils__WEBPACK_IMPORTED_MODULE_4__.MimeData(),
                             dragImage: dragImage,
                             supportedActions: 'copy-move',
                             proposedAction: 'copy',
                             source: this
                         });
-                        const selected = [model.toJSON()];
+                        const selected = [cell.model.toJSON()];
                         this._drag.mimeData.setData(JUPYTER_CELL_MIME, selected);
                         this._drag.mimeData.setData('text/plain', datasource.description);
                         return this._drag.start(clientX, clientY).then(() => {
                             this._drag = null;
                             this._dragData = null;
                         });
                     }
@@ -498,17 +636,17 @@
                 /* harmony import */
                 var react__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
-                var phosphor_react__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! phosphor-react */ "webpack/sharing/consume/default/phosphor-react/phosphor-react");
+                var _phosphor_icons_react__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! @phosphor-icons/react */ "webpack/sharing/consume/default/@phosphor-icons/react/@phosphor-icons/react");
                 /* harmony import */
-                var phosphor_react__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(phosphor_react__WEBPACK_IMPORTED_MODULE_2__);
+                var _phosphor_icons_react__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_phosphor_icons_react__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
                 var _style_index_css__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! ../style/index.css */ "./style/index.css");
 
 
 
 
                 /**
@@ -516,19 +654,24 @@
                  */
                 const DatasourceItem = ({
                     datasource,
                     insertDatasource,
                     onMouseDown
                 }) => {
                     const [expanded, setExpandedValue] = (0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(false);
+                    const [isDragging, setIsDragging] = (0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(false);
                     const handleToggleExpand = () => {
                         setExpandedValue(!expanded);
                     };
+                    const startDrag = (e) => {
+                        setIsDragging(true);
+                        onMouseDown(e, datasource);
+                    };
                     return (react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
-                            className: expanded && 'expanded'
+                            className: expanded ? 'expanded' : ''
                         },
                         react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
                                 key: datasource.id,
                                 className: "datasource-item-title"
                             },
                             react__WEBPACK_IMPORTED_MODULE_0___default().createElement("button", {
                                 title: expanded ? 'Hide Details' : 'Show Details',
@@ -541,26 +684,27 @@
                             })) : (react__WEBPACK_IMPORTED_MODULE_0___default().createElement(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_1__.caretRightIcon.react, {
                                 tag: "span",
                                 elementPosition: "center",
                                 width: "20px"
                             }))),
                             react__WEBPACK_IMPORTED_MODULE_0___default().createElement("span", {
                                 title: datasource.description,
-                                className: onMouseDown ?
+                                className: isDragging ?
                                     'datasource-item-name' :
                                     'datasource-item-name draggable',
                                 onClick: handleToggleExpand,
-                                onMouseDown: e => onMouseDown(e, datasource)
+                                onMouseDown: startDrag,
+                                onMouseUp: () => setIsDragging(false)
                             }, datasource.description),
                             react__WEBPACK_IMPORTED_MODULE_0___default().createElement("button", {
                                     title: "Insert code to load datasource",
                                     onClick: handleToggleExpand,
                                     className: "datasource-item-action"
                                 },
-                                react__WEBPACK_IMPORTED_MODULE_0___default().createElement(phosphor_react__WEBPACK_IMPORTED_MODULE_2__.ArrowBendDownRight, {
+                                react__WEBPACK_IMPORTED_MODULE_0___default().createElement(_phosphor_icons_react__WEBPACK_IMPORTED_MODULE_2__.ArrowBendDownRight, {
                                     size: 18,
                                     onClick: e => insertDatasource(datasource)
                                 }))),
                         expanded && (react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
                                 className: 'datasource-item-details'
                             },
                             react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
@@ -667,22 +811,23 @@
 
 
 
 
 
 
                 const oceanumIcon = new _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_3__.LabIcon({
-                    name: 'oceanum:main',
-                    svgstr: _style_icons_oceanum_svg__WEBPACK_IMPORTED_MODULE_9__["default"]
+                    name: 'oceanum:icon',
+                    svgstr: _style_icons_oceanum_svg__WEBPACK_IMPORTED_MODULE_9__
                 });
+                const PLUGIN_ID = '@oceanum/oceanumlab:datamesh-connect';
                 /**
                  * Initialization data for the extension.
                  */
                 const datamesh_connect_extension = {
-                    id: 'datamesh-connect',
+                    id: PLUGIN_ID,
                     autoStart: true,
                     requires: [
                         _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ICommandPalette,
                         _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILayoutRestorer,
                         _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabStatus,
                         _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_6__.ISettingRegistry,
                         _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_7__.IStateDB
@@ -706,18 +851,24 @@
                                         DATAMESH_TOKEN: token.user
                                     })
                                 }).then(res => console.log(res));
                             }
                             window.injectToken = set.get('injectToken').user;
                         };
                         //Try to get the datamesh token from the envars
-                        settingRegistry.load('@oceanum/oceanumlab:plugin').then(set => {
-                            set.changed.connect(updateSettings, undefined);
-                            updateSettings(set);
-                        });
+                        Promise.all([app.restored, settingRegistry.load(PLUGIN_ID)])
+                            .then(([, setting]) => {
+                                // Read the settings
+                                updateSettings(setting);
+                                // Listen for your plugin setting changes using Signal
+                                setting.changed.connect(updateSettings);
+                            })
+                            .catch(reason => {
+                                console.error(`Something went wrong when reading the Oceanumlab settings.\n${reason}`);
+                            });
                         const getCurrentWidget = () => {
                             return app.shell.currentWidget;
                         };
                         const openDatameshUI = (event) => {
                             const widgetId = 'datamesh-ui';
                             const openWidget = (0, _lumino_algorithm__WEBPACK_IMPORTED_MODULE_4__.find)(app.shell.widgets('main'), (widget, index) => {
                                 return widget.id === widgetId;
@@ -761,14 +912,430 @@
                 const __WEBPACK_DEFAULT_EXPORT__ = (datamesh_connect_extension);
 
 
                 /***/
             }),
 
         /***/
+        "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/api.js":
+            /*!**************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/api.js ***!
+              \**************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                /*
+                  MIT License http://www.opensource.org/licenses/mit-license.php
+                  Author Tobias Koppers @sokra
+                */
+                module.exports = function(cssWithMappingToString) {
+                    var list = [];
+
+                    // return the list of modules as css string
+                    list.toString = function toString() {
+                        return this.map(function(item) {
+                            var content = "";
+                            var needLayer = typeof item[5] !== "undefined";
+                            if (item[4]) {
+                                content += "@supports (".concat(item[4], ") {");
+                            }
+                            if (item[2]) {
+                                content += "@media ".concat(item[2], " {");
+                            }
+                            if (needLayer) {
+                                content += "@layer".concat(item[5].length > 0 ? " ".concat(item[5]) : "", " {");
+                            }
+                            content += cssWithMappingToString(item);
+                            if (needLayer) {
+                                content += "}";
+                            }
+                            if (item[2]) {
+                                content += "}";
+                            }
+                            if (item[4]) {
+                                content += "}";
+                            }
+                            return content;
+                        }).join("");
+                    };
+
+                    // import a list of modules into the list
+                    list.i = function i(modules, media, dedupe, supports, layer) {
+                        if (typeof modules === "string") {
+                            modules = [
+                                [null, modules, undefined]
+                            ];
+                        }
+                        var alreadyImportedModules = {};
+                        if (dedupe) {
+                            for (var k = 0; k < this.length; k++) {
+                                var id = this[k][0];
+                                if (id != null) {
+                                    alreadyImportedModules[id] = true;
+                                }
+                            }
+                        }
+                        for (var _k = 0; _k < modules.length; _k++) {
+                            var item = [].concat(modules[_k]);
+                            if (dedupe && alreadyImportedModules[item[0]]) {
+                                continue;
+                            }
+                            if (typeof layer !== "undefined") {
+                                if (typeof item[5] === "undefined") {
+                                    item[5] = layer;
+                                } else {
+                                    item[1] = "@layer".concat(item[5].length > 0 ? " ".concat(item[5]) : "", " {").concat(item[1], "}");
+                                    item[5] = layer;
+                                }
+                            }
+                            if (media) {
+                                if (!item[2]) {
+                                    item[2] = media;
+                                } else {
+                                    item[1] = "@media ".concat(item[2], " {").concat(item[1], "}");
+                                    item[2] = media;
+                                }
+                            }
+                            if (supports) {
+                                if (!item[4]) {
+                                    item[4] = "".concat(supports);
+                                } else {
+                                    item[1] = "@supports (".concat(item[4], ") {").concat(item[1], "}");
+                                    item[4] = supports;
+                                }
+                            }
+                            list.push(item);
+                        }
+                    };
+                    return list;
+                };
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/sourceMaps.js":
+            /*!*********************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/runtime/sourceMaps.js ***!
+              \*********************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                module.exports = function(item) {
+                    var content = item[1];
+                    var cssMapping = item[3];
+                    if (!cssMapping) {
+                        return content;
+                    }
+                    if (typeof btoa === "function") {
+                        var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(cssMapping))));
+                        var data = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(base64);
+                        var sourceMapping = "/*# ".concat(data, " */");
+                        return [content].concat([sourceMapping]).join("\n");
+                    }
+                    return [content].join("\n");
+                };
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js":
+            /*!*************************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js ***!
+              \*************************************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                var stylesInDOM = [];
+
+                function getIndexByIdentifier(identifier) {
+                    var result = -1;
+                    for (var i = 0; i < stylesInDOM.length; i++) {
+                        if (stylesInDOM[i].identifier === identifier) {
+                            result = i;
+                            break;
+                        }
+                    }
+                    return result;
+                }
+
+                function modulesToDom(list, options) {
+                    var idCountMap = {};
+                    var identifiers = [];
+                    for (var i = 0; i < list.length; i++) {
+                        var item = list[i];
+                        var id = options.base ? item[0] + options.base : item[0];
+                        var count = idCountMap[id] || 0;
+                        var identifier = "".concat(id, " ").concat(count);
+                        idCountMap[id] = count + 1;
+                        var indexByIdentifier = getIndexByIdentifier(identifier);
+                        var obj = {
+                            css: item[1],
+                            media: item[2],
+                            sourceMap: item[3],
+                            supports: item[4],
+                            layer: item[5]
+                        };
+                        if (indexByIdentifier !== -1) {
+                            stylesInDOM[indexByIdentifier].references++;
+                            stylesInDOM[indexByIdentifier].updater(obj);
+                        } else {
+                            var updater = addElementStyle(obj, options);
+                            options.byIndex = i;
+                            stylesInDOM.splice(i, 0, {
+                                identifier: identifier,
+                                updater: updater,
+                                references: 1
+                            });
+                        }
+                        identifiers.push(identifier);
+                    }
+                    return identifiers;
+                }
+
+                function addElementStyle(obj, options) {
+                    var api = options.domAPI(options);
+                    api.update(obj);
+                    var updater = function updater(newObj) {
+                        if (newObj) {
+                            if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap && newObj.supports === obj.supports && newObj.layer === obj.layer) {
+                                return;
+                            }
+                            api.update(obj = newObj);
+                        } else {
+                            api.remove();
+                        }
+                    };
+                    return updater;
+                }
+                module.exports = function(list, options) {
+                    options = options || {};
+                    list = list || [];
+                    var lastIdentifiers = modulesToDom(list, options);
+                    return function update(newList) {
+                        newList = newList || [];
+                        for (var i = 0; i < lastIdentifiers.length; i++) {
+                            var identifier = lastIdentifiers[i];
+                            var index = getIndexByIdentifier(identifier);
+                            stylesInDOM[index].references--;
+                        }
+                        var newLastIdentifiers = modulesToDom(newList, options);
+                        for (var _i = 0; _i < lastIdentifiers.length; _i++) {
+                            var _identifier = lastIdentifiers[_i];
+                            var _index = getIndexByIdentifier(_identifier);
+                            if (stylesInDOM[_index].references === 0) {
+                                stylesInDOM[_index].updater();
+                                stylesInDOM.splice(_index, 1);
+                            }
+                        }
+                        lastIdentifiers = newLastIdentifiers;
+                    };
+                };
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertBySelector.js":
+            /*!*****************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertBySelector.js ***!
+              \*****************************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                var memo = {};
+
+                /* istanbul ignore next  */
+                function getTarget(target) {
+                    if (typeof memo[target] === "undefined") {
+                        var styleTarget = document.querySelector(target);
+
+                        // Special case to return head of iframe instead of iframe itself
+                        if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {
+                            try {
+                                // This will throw an exception if access to iframe is blocked
+                                // due to cross-origin restrictions
+                                styleTarget = styleTarget.contentDocument.head;
+                            } catch (e) {
+                                // istanbul ignore next
+                                styleTarget = null;
+                            }
+                        }
+                        memo[target] = styleTarget;
+                    }
+                    return memo[target];
+                }
+
+                /* istanbul ignore next  */
+                function insertBySelector(insert, style) {
+                    var target = getTarget(insert);
+                    if (!target) {
+                        throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    }
+                    target.appendChild(style);
+                }
+                module.exports = insertBySelector;
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertStyleElement.js":
+            /*!*******************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertStyleElement.js ***!
+              \*******************************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                /* istanbul ignore next  */
+                function insertStyleElement(options) {
+                    var element = document.createElement("style");
+                    options.setAttributes(element, options.attributes);
+                    options.insert(element, options.options);
+                    return element;
+                }
+                module.exports = insertStyleElement;
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js":
+            /*!*******************************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js ***!
+              \*******************************************************************************************************************/
+            /***/
+            ((module, __unused_webpack_exports, __webpack_require__) => {
+
+
+
+                /* istanbul ignore next  */
+                function setAttributesWithoutAttributes(styleElement) {
+                    var nonce = true ? __webpack_require__.nc : 0;
+                    if (nonce) {
+                        styleElement.setAttribute("nonce", nonce);
+                    }
+                }
+                module.exports = setAttributesWithoutAttributes;
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleDomAPI.js":
+            /*!************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleDomAPI.js ***!
+              \************************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                /* istanbul ignore next  */
+                function apply(styleElement, options, obj) {
+                    var css = "";
+                    if (obj.supports) {
+                        css += "@supports (".concat(obj.supports, ") {");
+                    }
+                    if (obj.media) {
+                        css += "@media ".concat(obj.media, " {");
+                    }
+                    var needLayer = typeof obj.layer !== "undefined";
+                    if (needLayer) {
+                        css += "@layer".concat(obj.layer.length > 0 ? " ".concat(obj.layer) : "", " {");
+                    }
+                    css += obj.css;
+                    if (needLayer) {
+                        css += "}";
+                    }
+                    if (obj.media) {
+                        css += "}";
+                    }
+                    if (obj.supports) {
+                        css += "}";
+                    }
+                    var sourceMap = obj.sourceMap;
+                    if (sourceMap && typeof btoa !== "undefined") {
+                        css += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), " */");
+                    }
+
+                    // For old IE
+                    /* istanbul ignore if  */
+                    options.styleTagTransform(css, styleElement, options.options);
+                }
+
+                function removeStyleElement(styleElement) {
+                    // istanbul ignore if
+                    if (styleElement.parentNode === null) {
+                        return false;
+                    }
+                    styleElement.parentNode.removeChild(styleElement);
+                }
+
+                /* istanbul ignore next  */
+                function domAPI(options) {
+                    if (typeof document === "undefined") {
+                        return {
+                            update: function update() {},
+                            remove: function remove() {}
+                        };
+                    }
+                    var styleElement = options.insertStyleElement(options);
+                    return {
+                        update: function update(obj) {
+                            apply(styleElement, options, obj);
+                        },
+                        remove: function remove() {
+                            removeStyleElement(styleElement);
+                        }
+                    };
+                }
+                module.exports = domAPI;
+
+                /***/
+            }),
+
+        /***/
+        "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleTagTransform.js":
+            /*!******************************************************************************************************!*\
+              !*** ./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleTagTransform.js ***!
+              \******************************************************************************************************/
+            /***/
+            ((module) => {
+
+
+
+                /* istanbul ignore next  */
+                function styleTagTransform(css, styleElement) {
+                    if (styleElement.styleSheet) {
+                        styleElement.styleSheet.cssText = css;
+                    } else {
+                        while (styleElement.firstChild) {
+                            styleElement.removeChild(styleElement.firstChild);
+                        }
+                        styleElement.appendChild(document.createTextNode(css));
+                    }
+                }
+                module.exports = styleTagTransform;
+
+                /***/
+            }),
+
+        /***/
         "./style/index.css":
             /*!*************************!*\
               !*** ./style/index.css ***!
               \*************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
@@ -776,33 +1343,81 @@
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
                 /* harmony import */
-                var _node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! !../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js */ "./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js");
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js");
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0__);
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleDomAPI_js__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleDomAPI.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleDomAPI.js");
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleDomAPI_js__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleDomAPI_js__WEBPACK_IMPORTED_MODULE_1__);
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertBySelector_js__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertBySelector.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertBySelector.js");
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertBySelector_js__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertBySelector_js__WEBPACK_IMPORTED_MODULE_2__);
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_setAttributesWithoutAttributes_js__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/setAttributesWithoutAttributes.js");
                 /* harmony import */
-                var _node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0__);
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_setAttributesWithoutAttributes_js__WEBPACK_IMPORTED_MODULE_3___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_setAttributesWithoutAttributes_js__WEBPACK_IMPORTED_MODULE_3__);
                 /* harmony import */
-                var _node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! !!../node_modules/css-loader/dist/cjs.js!./index.css */ "./node_modules/css-loader/dist/cjs.js!./style/index.css");
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertStyleElement_js__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertStyleElement.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/insertStyleElement.js");
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertStyleElement_js__WEBPACK_IMPORTED_MODULE_4___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertStyleElement_js__WEBPACK_IMPORTED_MODULE_4__);
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleTagTransform_js__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! !../node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleTagTransform.js */ "./node_modules/@jupyterlab/builder/node_modules/style-loader/dist/runtime/styleTagTransform.js");
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleTagTransform_js__WEBPACK_IMPORTED_MODULE_5___default = /*#__PURE__*/ __webpack_require__.n(_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleTagTransform_js__WEBPACK_IMPORTED_MODULE_5__);
+                /* harmony import */
+                var _node_modules_jupyterlab_builder_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! !!../node_modules/@jupyterlab/builder/node_modules/css-loader/dist/cjs.js!./index.css */ "./node_modules/@jupyterlab/builder/node_modules/css-loader/dist/cjs.js!./style/index.css");
+
+
+
+
+
+
+
+
 
 
 
                 var options = {};
 
-                options.insert = "head";
-                options.singleton = false;
+                options.styleTagTransform = (_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleTagTransform_js__WEBPACK_IMPORTED_MODULE_5___default());
+                options.setAttributes = (_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_setAttributesWithoutAttributes_js__WEBPACK_IMPORTED_MODULE_3___default());
+
+                options.insert = _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertBySelector_js__WEBPACK_IMPORTED_MODULE_2___default().bind(null, "head");
+
+                options.domAPI = (_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_styleDomAPI_js__WEBPACK_IMPORTED_MODULE_1___default());
+                options.insertStyleElement = (_node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_insertStyleElement_js__WEBPACK_IMPORTED_MODULE_4___default());
+
+                var update = _node_modules_jupyterlab_builder_node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0___default()(_node_modules_jupyterlab_builder_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_6__["default"], options);
 
-                var update = _node_modules_style_loader_dist_runtime_injectStylesIntoStyleTag_js__WEBPACK_IMPORTED_MODULE_0___default()(_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_1__["default"], options);
 
 
 
                 /* harmony default export */
-                const __WEBPACK_DEFAULT_EXPORT__ = (_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_1__["default"].locals || {});
+                const __WEBPACK_DEFAULT_EXPORT__ = (_node_modules_jupyterlab_builder_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_6__["default"] && _node_modules_jupyterlab_builder_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_6__["default"].locals ? _node_modules_jupyterlab_builder_node_modules_css_loader_dist_cjs_js_index_css__WEBPACK_IMPORTED_MODULE_6__["default"].locals : undefined);
+
+
+                /***/
+            }),
+
+        /***/
+        "./style/icons/oceanum.svg":
+            /*!*********************************!*\
+              !*** ./style/icons/oceanum.svg ***!
+              \*********************************/
+            /***/
+            ((module) => {
+
+                module.exports = "<svg xmlns=\"http://www.w3.org/2000/svg\" width=\"44\" height=\"44\" viewBox=\"0 0 44.079582 44.079582\" version=\"1.1\" id=\"svg5870\">\n  <g\n     id=\"layer1\"\n     transform=\"translate(-82.281595,-124.52568)\">\n    <g\n       style=\"stroke:#3b547c;stroke-opacity:1\"\n       transform=\"matrix(0.26458333,0,0,0.26458333,69.475762,109.81485)\"\n       id=\"g2915\"\n       >\n      <g\n         style=\"stroke:#3b547c;stroke-opacity:1\"\n         id=\"g2903\">\n        <path\n           id=\"path2897\"\n           d=\"m 212.3,149.9 c -35.8,19.1 -58.2,-11 -80.6,-11 -22.4,0 -44.7,30.1 -80.6,11 1.2,8.7 3.8,17.2 7.7,25.1 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4 3.9,-7.9 6.5,-16.3 7.7,-25.1 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n        <path\n           id=\"path2899\"\n           d=\"m 204.6,175 c -38.7,13.5 -55.8,-8.4 -72.9,-8.4 -17.1,0 -34.1,22 -72.9,8.4 4.4,8.9 10.4,16.9 17.7,23.6 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 7.3,-6.7 13.3,-14.7 17.7,-23.6 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n        <path\n           id=\"path2901\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 -15,13.9 -34.7,21.6 -55.2,21.6 -20.4,-0.1 -40.2,-7.8 -55.2,-21.6 z\"\n           class=\"st8\"\n           \n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\" />\n      </g>\n      <g\n         style=\"stroke:#3b547c;stroke-opacity:1\"\n         id=\"g2913\">\n        <path\n           id=\"path2905\"\n           d=\"m 58.8,175 c 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2907\"\n           d=\"m 51.1,149.9 c 35.8,19.1 58.2,-11 80.6,-11 22.4,0 44.7,30.1 80.6,11\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2909\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n        <path\n           id=\"path2911\"\n           d=\"m 131.7,220.2 c 10.3,0 20.4,-1.9 29.9,-5.7 10.3,-4.1 19.7,-10.2 27.6,-18.1 7.9,-7.9 14,-17.2 18.1,-27.6 3.8,-9.5 5.7,-19.7 5.7,-29.9 0,-10.3 -1.9,-20.4 -5.7,-29.9 -4.1,-10.3 -10.2,-19.7 -18.1,-27.6 -7.9,-7.9 -17.2,-14 -27.6,-18.1 -9.5,-3.8 -19.7,-5.7 -29.9,-5.7 -10.3,0 -20.4,1.9 -29.9,5.7 -10.3,4.1 -19.7,10.2 -27.6,18.1 -7.9,7.9 -14,17.2 -18.1,27.6 -3.8,9.5 -5.7,19.7 -5.7,29.9 0,10.3 1.9,20.4 5.7,29.9 4.1,10.3 10.2,19.7 18.1,27.6 7.9,7.9 17.2,14 27.6,18.1 9.5,3.8 19.6,5.7 29.9,5.7 z\"\n           class=\"st9\"\n           \n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\" />\n      </g>\n    </g>\n    <g\n       id=\"g3308\"\n       transform=\"matrix(0.26458333,0,0,0.26458333,69.475762,109.81485)\"\n       style=\"stroke:#3b547c;stroke-opacity:1\">\n      <g\n         id=\"g3296\"\n         style=\"stroke:#3b547c;stroke-opacity:1\">\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 212.3,149.9 c -35.8,19.1 -58.2,-11 -80.6,-11 -22.4,0 -44.7,30.1 -80.6,11 1.2,8.7 3.8,17.2 7.7,25.1 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4 3.9,-7.9 6.5,-16.3 7.7,-25.1 z\"\n           id=\"path3290\" />\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 204.6,175 c -38.7,13.5 -55.8,-8.4 -72.9,-8.4 -17.1,0 -34.1,22 -72.9,8.4 4.4,8.9 10.4,16.9 17.7,23.6 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 7.3,-6.7 13.3,-14.7 17.7,-23.6 z\"\n           id=\"path3292\" />\n        <path\n           style=\"fill:#dce1f9;stroke:#3b547c;stroke-opacity:1\"\n           \n           class=\"st8\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5 -15,13.9 -34.7,21.6 -55.2,21.6 -20.4,-0.1 -40.2,-7.8 -55.2,-21.6 z\"\n           id=\"path3294\" />\n      </g>\n      <g\n         id=\"g3306\"\n         style=\"stroke:#3b547c;stroke-opacity:1\">\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 58.8,175 c 38.7,13.5 55.8,-8.4 72.9,-8.4 17.1,0 34.1,22 72.9,8.4\"\n           id=\"path3298\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 51.1,149.9 c 35.8,19.1 58.2,-11 80.6,-11 22.4,0 44.7,30.1 80.6,11\"\n           id=\"path3300\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 76.5,198.7 c 31.1,6.8 43.1,-6.5 55.2,-6.5 12.1,0 24.1,13.3 55.2,6.5\"\n           id=\"path3302\" />\n        <path\n           style=\"fill:none;stroke:#3b547c;stroke-width:4;stroke-linecap:round;stroke-linejoin:round;stroke-opacity:1\"\n           \n           class=\"st9\"\n           d=\"m 131.7,220.2 c 10.3,0 20.4,-1.9 29.9,-5.7 10.3,-4.1 19.7,-10.2 27.6,-18.1 7.9,-7.9 14,-17.2 18.1,-27.6 3.8,-9.5 5.7,-19.7 5.7,-29.9 0,-10.3 -1.9,-20.4 -5.7,-29.9 -4.1,-10.3 -10.2,-19.7 -18.1,-27.6 -7.9,-7.9 -17.2,-14 -27.6,-18.1 -9.5,-3.8 -19.7,-5.7 -29.9,-5.7 -10.3,0 -20.4,1.9 -29.9,5.7 -10.3,4.1 -19.7,10.2 -27.6,18.1 -7.9,7.9 -14,17.2 -18.1,27.6 -3.8,9.5 -5.7,19.7 -5.7,29.9 0,10.3 1.9,20.4 5.7,29.9 4.1,10.3 10.2,19.7 18.1,27.6 7.9,7.9 17.2,14 27.6,18.1 9.5,3.8 19.6,5.7 29.9,5.7 z\"\n           id=\"path3304\" />\n      </g>\n    </g>\n  </g>\n</svg>\n";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.05207cdbfaf8569aa6ae.js.map
+//# sourceMappingURL=lib_index_js.4c53e7d97d745fd9dd50.js.map
```

### Comparing `oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.adac79c2b11ab53ec7cf.js` & `oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -12,21 +12,21 @@
               !*** container entry ***!
               \***********************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
                 var moduleMap = {
                     "./index": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("style_index_css")]).then(() => (() => ((__webpack_require__( /*! ./style/index.css */ "./style/index.css")))));
+                        return __webpack_require__.e("style_index_js").then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -182,19 +182,18 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "cdb07a33d62465011526",
                 "webpack_sharing_consume_default_react": "6a93435d3217e15f3c73",
-                "lib_index_js": "05207cdbfaf8569aa6ae",
-                "style_index_css": "35da1c86a5689163d63d",
-                "vendors-node_modules_phosphor-react_dist_index_esm_js": "a2d73cddf27390da0fec"
+                "lib_index_js": "4c53e7d97d745fd9dd50",
+                "style_index_js": "089f3d25ce6bfdcec72d",
+                "vendors-node_modules_phosphor-icons_react_dist_index_mjs": "d28fe157162aff53d727"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -430,17 +429,17 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@oceanum/oceanumlab", "0.4.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("@oceanum/oceanumlab", "4.0.0", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
-                    register("phosphor-react", "1.4.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_phosphor-react_dist_index_esm_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/phosphor-react/dist/index.esm.js */ "./node_modules/phosphor-react/dist/index.esm.js"))))));
+                    register("@phosphor-icons/react", "2.1.4", () => (Promise.all([__webpack_require__.e("vendors-node_modules_phosphor-icons_react_dist_index_mjs"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/@phosphor-icons/react/dist/index.mjs */ "./node_modules/@phosphor-icons/react/dist/index.mjs"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -833,43 +832,43 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
+            "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 18, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 1, 9, 0])),
+            "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/settingregistry": () => (loadSingletonVersionCheck("default", "@jupyterlab/settingregistry", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 1, 11, 0])),
+            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/dragdrop": () => (loadSingletonVersionCheck("default", "@lumino/dragdrop", [1, 1, 13, 0])),
+            "webpack/sharing/consume/default/@lumino/dragdrop": () => (loadSingletonVersionCheck("default", "@lumino/dragdrop", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 10, 0])),
+            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/phosphor-react/phosphor-react": () => (loadStrictVersionCheckFallback("default", "phosphor-react", [1, 1, 4, 1], () => (__webpack_require__.e("vendors-node_modules_phosphor-react_dist_index_esm_js").then(() => (() => (__webpack_require__( /*! phosphor-react */ "./node_modules/phosphor-react/dist/index.esm.js")))))))
+            "webpack/sharing/consume/default/@phosphor-icons/react/@phosphor-icons/react": () => (loadStrictVersionCheckFallback("default", "@phosphor-icons/react", [1, 2, 1, 4], () => (__webpack_require__.e("vendors-node_modules_phosphor-icons_react_dist_index_mjs").then(() => (() => (__webpack_require__( /*! @phosphor-icons/react */ "./node_modules/@phosphor-icons/react/dist/index.mjs")))))))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "webpack_sharing_consume_default_react": [
@@ -902,15 +901,15 @@
                 /******/
                 "webpack/sharing/consume/default/@lumino/coreutils",
                 /******/
                 "webpack/sharing/consume/default/@lumino/dragdrop",
                 /******/
                 "webpack/sharing/consume/default/@lumino/signaling",
                 /******/
-                "webpack/sharing/consume/default/phosphor-react/phosphor-react"
+                "webpack/sharing/consume/default/@phosphor-icons/react/@phosphor-icons/react"
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1137,8 +1136,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/@oceanum/oceanumlab");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@oceanum/oceanumlab"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.adac79c2b11ab53ec7cf.js.map
+//# sourceMappingURL=remoteEntry.1c4cc02ec4ec7f0e8dba.js.map
```

### Comparing `oceanumlab-0.4.3/oceanumlab/labextension/static/remoteEntry.adac79c2b11ab53ec7cf.js.map` & `oceanumlab-4.0.0/oceanumlab/labextension/static/remoteEntry.1c4cc02ec4ec7f0e8dba.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8311688311688312%*

 * *Differences: {"'file'": "'remoteEntry.1c4cc02ec4ec7f0e8dba.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.adac79c2b11ab53ec7cf.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,2VAA2V;WACzX;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCxMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.1c4cc02ec4ec7f0e8dba.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,+NAA+N;WAC7P;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCxMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://@oceanum/oceanumlab/webpack/container-entry",
         "webpack://@oceanum/oceanumlab/webpack/bootstrap",
         "webpack://@oceanum/oceanumlab/webpack/runtime/compat get default export",
         "webpack://@oceanum/oceanumlab/webpack/runtime/define property getters",
@@ -20,27 +20,27 @@
         "webpack://@oceanum/oceanumlab/webpack/runtime/jsonp chunk loading",
         "webpack://@oceanum/oceanumlab/webpack/runtime/nonce",
         "webpack://@oceanum/oceanumlab/webpack/before-startup",
         "webpack://@oceanum/oceanumlab/webpack/startup",
         "webpack://@oceanum/oceanumlab/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_css\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.css */ \"./style/index.css\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"cdb07a33d62465011526\",\"webpack_sharing_consume_default_react\":\"6a93435d3217e15f3c73\",\"lib_index_js\":\"05207cdbfaf8569aa6ae\",\"style_index_css\":\"35da1c86a5689163d63d\",\"vendors-node_modules_phosphor-react_dist_index_esm_js\":\"a2d73cddf27390da0fec\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"webpack_sharing_consume_default_react\":\"6a93435d3217e15f3c73\",\"lib_index_js\":\"4c53e7d97d745fd9dd50\",\"style_index_js\":\"089f3d25ce6bfdcec72d\",\"vendors-node_modules_phosphor-icons_react_dist_index_mjs\":\"d28fe157162aff53d727\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"@oceanum/oceanumlab:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@oceanum/oceanumlab\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@oceanum/oceanumlab\", \"0.4.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"phosphor-react\", \"1.4.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_phosphor-react_dist_index_esm_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/phosphor-react/dist/index.esm.js */ \"./node_modules/phosphor-react/dist/index.esm.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"@oceanum/oceanumlab\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@oceanum/oceanumlab\", \"4.0.0\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"@phosphor-icons/react\", \"2.1.4\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_phosphor-icons_react_dist_index_mjs\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/@phosphor-icons/react/dist/index.mjs */ \"./node_modules/@phosphor-icons/react/dist/index.mjs\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,5])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@lumino/dragdrop\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/dragdrop\", [1,1,13,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/phosphor-react/phosphor-react\": () => (loadStrictVersionCheckFallback(\"default\", \"phosphor-react\", [1,1,4,1], () => (__webpack_require__.e(\"vendors-node_modules_phosphor-react_dist_index_esm_js\").then(() => (() => (__webpack_require__(/*! phosphor-react */ \"./node_modules/phosphor-react/dist/index.esm.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/dragdrop\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/phosphor-react/phosphor-react\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/dragdrop\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/dragdrop\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@phosphor-icons/react/@phosphor-icons/react\": () => (loadStrictVersionCheckFallback(\"default\", \"@phosphor-icons/react\", [1,2,1,4], () => (__webpack_require__.e(\"vendors-node_modules_phosphor-icons_react_dist_index_mjs\").then(() => (() => (__webpack_require__(/*! @phosphor-icons/react */ \"./node_modules/@phosphor-icons/react/dist/index.mjs\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/dragdrop\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@phosphor-icons/react/@phosphor-icons/react\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"@oceanum/oceanumlab\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunk_oceanum_oceanumlab\"] = self[\"webpackChunk_oceanum_oceanumlab\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/@oceanum/oceanumlab\");\n",
         ""
     ],
     "version": 3
```

### Comparing `oceanumlab-0.4.3/schema/plugin.json` & `oceanumlab-4.0.0/schema/datamesh-connect.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'description'": "'Oceanumlab settings.'", "'icon'": "'oceanum-io'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "additionalProperties": false,
-    "description": "oceanumlab settings.",
-    "icon": "oceanum",
+    "description": "Oceanumlab settings.",
+    "icon": "oceanum-io",
     "jupyter.lab.setting-icon": "oceanum:main",
     "jupyter.lab.setting-icon-label": "Oceanum",
     "jupyter.lab.shortcuts": [],
     "properties": {
         "datameshToken": {
             "default": "",
             "description": "Enter your Datamesh token here. You can obtain this at https://home.oceanum.io/account. You will need to reset your kernel after changing this setting.",
```

### Comparing `oceanumlab-0.4.3/src/DatameshWidget.tsx` & `oceanumlab-4.0.0/src/DatameshWidget.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,31 @@
   ReactWidget,
   UseSignal,
   showDialog
 } from '@jupyterlab/apputils';
 import { CodeCell } from '@jupyterlab/cells';
 import { CodeEditor } from '@jupyterlab/codeeditor';
 import * as nbformat from '@jupyterlab/nbformat';
-import { Notebook, NotebookModel, NotebookPanel } from '@jupyterlab/notebook';
+import { Notebook, NotebookPanel } from '@jupyterlab/notebook';
+import { CodeCellModel } from '@jupyterlab/cells';
 import { LabIcon, addIcon } from '@jupyterlab/ui-components';
 import { MimeData } from '@lumino/coreutils';
 import { Drag } from '@lumino/dragdrop';
 import { Signal } from '@lumino/signaling';
 import { Widget } from '@lumino/widgets';
 
 import React from 'react';
 
 import { DatasourceItem } from './DatasourceItem';
 
 const JUPYTER_CELL_MIME = 'application/vnd.jupyter.cells';
 
+const DRAG_IMAGE=new Image();
+DRAG_IMAGE.src='data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMiIgaGVpZ2h0PSIzMiIgZmlsbD0iIzAwMDAwMCIgdmlld0JveD0iMCAwIDI1NiAyNTYiPjxwYXRoIGQ9Ik02OS4xMiw5NC4xNSwyOC41LDEyOGw0MC42MiwzMy44NWE4LDgsMCwxLDEtMTAuMjQsMTIuMjlsLTQ4LTQwYTgsOCwwLDAsMSwwLTEyLjI5bDQ4LTQwYTgsOCwwLDAsMSwxMC4yNCwxMi4zWm0xNzYsMjcuNy00OC00MGE4LDgsMCwxLDAtMTAuMjQsMTIuM0wyMjcuNSwxMjhsLTQwLjYyLDMzLjg1YTgsOCwwLDEsMCwxMC4yNCwxMi4yOWw0OC00MGE4LDgsMCwwLDAsMC0xMi4yOVpNMTYyLjczLDMyLjQ4YTgsOCwwLDAsMC0xMC4yNSw0Ljc5bC02NCwxNzZhOCw4LDAsMCwwLDQuNzksMTAuMjZBOC4xNCw4LjE0LDAsMCwwLDk2LDIyNGE4LDgsMCwwLDAsNy41Mi01LjI3bDY0LTE3NkE4LDgsMCwwLDAsMTYyLjczLDMyLjQ4WiI+PC9wYXRoPjwvc3ZnPg==';
+
 const datameshToken = (notebook: Notebook): string => {
   const datameshTokenInjected =
     notebook &&
     notebook.widgets.find(cell => {
       if (cell.editor) {
         const line = cell.editor.getLine(0);
         if (line && line.indexOf('DATAMESH_TOKEN=') >= 0) {
@@ -126,14 +130,17 @@
     super(props);
     this._drag = null;
     this._dragData = null;
     this.handleDragMove = this.handleDragMove.bind(this);
     this._evtMouseUp = this._evtMouseUp.bind(this);
   }
 
+  private _drag: Drag | null;
+  private _dragData: { pressX: number; pressY: number; dragImage: HTMLElement } | null;
+
   render(): React.ReactElement {
     return (
       <div className={'datamesh-workspace-display'}>
         {this.props.spec && (
           <div>
             <span className="datamesh-workspace-name">
               {this.props.spec.name}
@@ -160,27 +167,31 @@
       </div>
     );
   }
 
   private injectToken = (notebookWidget: NotebookPanel): void => {
     const notebookContent = notebookWidget.content as Notebook;
     const datameshTokenInject = datameshToken(notebookContent);
+    //const codeCell=new CodeCellModel({});
     if (datameshTokenInject) {
-      const tokenCell = notebookContent.model.contentFactory.createCodeCell({
-        cell: {
-          cell_type: 'code',
-          source: datameshTokenInject,
-          metadata: { tags: ['hide_input'] }
-        }
+      // const tokenCell = notebookContent.contentFactory.createCodeCell({
+      //   model: codeCell,
+      //   rendermime: notebookContent.rendermime,
+      //   contentFactory: notebookContent.contentFactory,
+      // })
+      // tokenCell.model.sharedModel.setSource(datameshTokenInject);
+      notebookContent.model?.sharedModel.insertCell(0, {
+        cell_type:'code',
+        source: datameshTokenInject,
+        metadata: {},
       });
-      notebookContent.model.cells.insert(0, tokenCell);
-      CodeCell.execute(
-        notebookContent.widgets[0] as CodeCell,
-        notebookWidget.sessionContext
-      );
+      // CodeCell.execute(
+      //   notebookContent.widgets[0] as CodeCell,
+      //   notebookWidget.sessionContext
+      // );
     }
   };
 
   // Handle code datasource insert into an editor
   private insertDatameshConnect = async (
     datasource: IDatasource
   ): Promise<void> => {
@@ -193,47 +204,49 @@
       const notebookCellEditor = notebookCell.editor;
 
       const datasourceStr = datasourceCode(
         datasource,
         notebookContent,
         notebookCellIndex
       );
-      if (notebookCell instanceof CodeCell) {
-        this.verifyLanguageAndInsert(
-          datasourceStr,
-          'python',
-          notebookCellEditor
-        );
+      if (notebookCellEditor) {
+        if (notebookCell instanceof CodeCell) {
+          this.verifyLanguageAndInsert(
+            datasourceStr,
+            'python',
+            notebookCellEditor
+          );
+        } else {
+          notebookCellEditor.replaceSelection(datasourceStr);
+        }
+        if (window.injectToken) {
+          this.injectToken(notebookWidget);
+        }
       } else {
-        notebookCellEditor.replaceSelection(datasourceStr);
-      }
-      if (window.injectToken) {
-        this.injectToken(notebookWidget);
+        this.showErrDialog(
+          'Datamesh datasource insert failed: Please select code cell'
+        );
       }
-    } else {
-      this.showErrDialog(
-        'Datamesh datasource insert failed: Please select code cell'
-      );
     }
   };
 
   // Handle language compatibility between code datasource and editor
   private verifyLanguageAndInsert = async (
     datasourceStr: string,
     editorLanguage: string,
     editor: CodeEditor.IEditor
   ): Promise<void> => {
-    if (editorLanguage && 'python' !== editorLanguage.toLowerCase()) {
+    if (editor && editorLanguage && 'python' !== editorLanguage.toLowerCase()) {
       const result = await this.showWarnDialog(editorLanguage);
       if (result.button.accept) {
         editor.replaceSelection(datasourceStr);
       }
     } else {
       // Language match or editorLanguage is unavailable
-      editor.replaceSelection(datasourceStr);
+      editor?.replaceSelection(datasourceStr);
     }
   };
 
   // Display warning dialog when inserting a code datasource incompatible with editor's language
   private showWarnDialog = async (
     editorLanguage: string
   ): Promise<Dialog.IResult<string>> => {
@@ -264,15 +277,15 @@
     if (button !== 0) {
       return;
     }
 
     this._dragData = {
       pressX: event.clientX,
       pressY: event.clientY,
-      dragImage: null
+      dragImage: DRAG_IMAGE
     };
 
     const mouseUpListener = (event: MouseEvent): void => {
       this._evtMouseUp(event, datasource, mouseMoveListener);
     };
     const mouseMoveListener = (event: MouseEvent): void => {
       this.handleDragMove(
@@ -368,43 +381,46 @@
 
   private async startDrag(
     dragImage: HTMLElement,
     datasource: IDatasource,
     clientX: number,
     clientY: number
   ): Promise<void> {
-    const contentFactory = new NotebookModel.ContentFactory({});
-    const model = contentFactory.createCodeCell({});
-    let content = datasourceCode(datasource, null, 0);
+    const notebookPanel: NotebookPanel = this.props.getCurrentWidget() as NotebookPanel;
+    const notebookContent = notebookPanel.content as Notebook;
+    const codeCell=new CodeCellModel({});
+    const cell = notebookContent.contentFactory.createCodeCell({
+      model: codeCell,
+      rendermime: notebookContent.rendermime,
+      contentFactory: notebookContent.contentFactory
+    });
+    let content = datasourceCode(datasource, notebookContent, 0);
     if (window.injectToken) {
       const notebookPanel = this.props.getCurrentWidget() as NotebookPanel;
       content = datameshToken(notebookPanel.content) + '\n' + content;
     }
-    model.value.text = content;
+    cell.model.sharedModel.setSource(content);
 
     this._drag = new Drag({
       mimeData: new MimeData(),
       dragImage: dragImage,
       supportedActions: 'copy-move',
       proposedAction: 'copy',
       source: this
     });
 
-    const selected: nbformat.ICell[] = [model.toJSON()];
+    const selected: nbformat.ICell[] = [cell.model.toJSON()];
     this._drag.mimeData.setData(JUPYTER_CELL_MIME, selected);
     this._drag.mimeData.setData('text/plain', datasource.description);
 
     return this._drag.start(clientX, clientY).then(() => {
       this._drag = null;
       this._dragData = null;
     });
   }
-
-  private _drag: Drag;
-  private _dragData: { pressX: number; pressY: number; dragImage: HTMLElement };
 }
 
 /**
  * DatameshConnectWidget props.
  */
 export interface IDatameshWidgetProps {
   app: JupyterFrontEnd;
```

### Comparing `oceanumlab-0.4.3/src/DatasourceItem.tsx` & `oceanumlab-4.0.0/src/DatasourceItem.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import React, { useState } from 'react';
 import { caretDownIcon, caretRightIcon } from '@jupyterlab/ui-components';
-import { ArrowBendDownRight } from 'phosphor-react';
+import { ArrowBendDownRight } from '@phosphor-icons/react';
 
 import '../style/index.css';
 import { IDatasource } from './DatameshWidget';
 
 export interface IDatasourceItemProps {
   datasource: IDatasource;
   insertDatasource: (datasource: IDatasource) => void;
@@ -20,21 +20,27 @@
 
 export const DatasourceItem: React.FC<IDatasourceItemProps> = ({
   datasource,
   insertDatasource,
   onMouseDown
 }) => {
   const [expanded, setExpandedValue] = useState(false);
+  const [isDragging, setIsDragging] = useState(false);
 
   const handleToggleExpand = (): void => {
     setExpandedValue(!expanded);
   };
 
+  const startDrag=(e:React.MouseEvent<HTMLSpanElement, MouseEvent>)=>{
+    setIsDragging(true);
+    onMouseDown(e, datasource)
+  }
+
   return (
-    <div className={expanded && 'expanded'}>
+    <div className={expanded ? 'expanded' : ''}>
       <div key={datasource.id} className="datasource-item-title">
         <button
           title={expanded ? 'Hide Details' : 'Show Details'}
           onClick={handleToggleExpand}
           className="datasource-item-expand"
         >
           {expanded ? (
@@ -50,20 +56,21 @@
               width="20px"
             />
           )}
         </button>
         <span
           title={datasource.description}
           className={
-            onMouseDown
+            isDragging
               ? 'datasource-item-name'
               : 'datasource-item-name draggable'
           }
           onClick={handleToggleExpand}
-          onMouseDown={e => onMouseDown(e, datasource)}
+          onMouseDown={startDrag}
+          onMouseUp={() => setIsDragging(false)}
         >
           {datasource.description}
         </span>
 
         <button
           title="Insert code to load datasource"
           onClick={handleToggleExpand}
```

### Comparing `oceanumlab-0.4.3/src/index.ts` & `oceanumlab-4.0.0/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,26 @@
 import { IStateDB } from '@jupyterlab/statedb';
 import { DatameshConnectWidget } from './DatameshWidget';
 import { DatameshUI } from './DatameshUI';
 
 import '../style/index.css';
 
 import oceanumSvg from '../style/icons/oceanum.svg';
-
-declare global {
-  interface Window {
-    datameshToken: string;
-    injectToken: boolean;
-  }
-}
-
 const oceanumIcon = new LabIcon({
-  name: 'oceanum:main',
+  name: 'oceanum:icon',
   svgstr: oceanumSvg
 });
 
+const PLUGIN_ID = '@oceanum/oceanumlab:datamesh-connect';
+
 /**
  * Initialization data for the extension.
  */
 export const datamesh_connect_extension: JupyterFrontEndPlugin<void> = {
-  id: 'datamesh-connect',
+  id: PLUGIN_ID,
   autoStart: true,
   requires: [
     ICommandPalette,
     ILayoutRestorer,
     ILabStatus,
     ISettingRegistry,
     IStateDB
@@ -68,21 +62,30 @@
           body: JSON.stringify({ DATAMESH_TOKEN: token.user })
         }).then(res => console.log(res));
       }
       window.injectToken = set.get('injectToken').user as boolean;
     };
     //Try to get the datamesh token from the envars
 
-    settingRegistry.load('@oceanum/oceanumlab:plugin').then(set => {
-      set.changed.connect(updateSettings, this);
-      updateSettings(set);
-    });
+    Promise.all([app.restored, settingRegistry.load(PLUGIN_ID)])
+      .then(([, setting]) => {
+        // Read the settings
+        updateSettings(setting);
+
+        // Listen for your plugin setting changes using Signal
+        setting.changed.connect(updateSettings);
+      })
+      .catch(reason => {
+        console.error(
+          `Something went wrong when reading the Oceanumlab settings.\n${reason}`
+        );
+      });
 
     const getCurrentWidget = (): Widget => {
-      return app.shell.currentWidget;
+      return app.shell!.currentWidget!;
     };
 
     const openDatameshUI = (event: any): void => {
       const widgetId = 'datamesh-ui';
       const openWidget = find(
         app.shell.widgets('main'),
         (widget: Widget, index: number) => {
```

### Comparing `oceanumlab-0.4.3/style/index.css` & `oceanumlab-4.0.0/style/index.css`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/style/icons/oceanum.png` & `oceanumlab-4.0.0/style/icons/oceanum.png`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/style/icons/oceanum.svg` & `oceanumlab-4.0.0/style/icons/oceanum.svg`

 * *Files identical despite different names*

### Comparing `oceanumlab-0.4.3/PKG-INFO` & `oceanumlab-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: oceanumlab
-Version: 0.4.3
+Version: 4.0.0
+Dynamic: Keywords
 Summary: A Jupyterlab extension to interact with the Oceanum.io platform
-Project-URL: Homepage, https://github.com/oceanum-io/oceanumlab
-Project-URL: Bug Tracker, https://github.com/oceanum-io/oceanumlab/issues
+Project-URL: Homepage, https://github.com/oceanum-io/oceanumlab.git
+Project-URL: Bug Tracker, https://github.com/oceanum-io/oceanumlab.git/issues
 Project-URL: Repository, https://github.com/oceanum-io/oceanumlab.git
 Author-email: Oceanum <developers@oceanum.science>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Oceanum
         All rights reserved.
         
@@ -40,36 +41,41 @@
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Requires-Dist: jupyter-server<3,>=2.0.1
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[server]>=0.6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # oceanumlab
 
+<<<<<<< before updating
 [![Github Actions Status](https://github.com/oceanum-io/oceanumlab/workflows/Build/badge.svg)](https://github.com/oceanum-io/oceanumlab/actions/workflows/build.yml)
 A Jupyterlab extension to interact with the Oceanum.io platform
 
 This extension is composed of a Python package named `oceanumlab`
 for the server extension and a NPM package named `oceanumlab`
 for the frontend extension.
+=======
+[![Github Actions Status](https://github.com/oceanum-io/oceanumlab.git/workflows/Build/badge.svg)](https://github.com/oceanum-io/oceanumlab.git/actions/workflows/build.yml)
+
+A Jupyterlab extension to interact with the Oceanum.io platform
+>>>>>>> after updating
 
 ## Requirements
 
 - JupyterLab >= 3.0
 
 ## Install
 
@@ -83,49 +89,31 @@
 
 To remove the extension, execute:
 
 ```bash
 pip uninstall oceanumlab
 ```
 
-## Troubleshoot
-
-If you are seeing the frontend extension, but it is not working, check
-that the server extension is enabled:
-
-```bash
-jupyter server extension list
-```
-
-If the server extension is installed and enabled, but you are not seeing
-the frontend extension, check the frontend extension is installed:
-
-```bash
-jupyter labextension list
-```
-
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the oceanumlab directory
 # Install package in development mode
-pip install -e .
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
-# Server extension must be manually installed in develop mode
-jupyter server extension enable oceanumlab
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
@@ -142,16 +130,14 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-# Server extension must be manually disabled in develop mode
-jupyter server extension disable oceanumlab
 pip uninstall oceanumlab
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `oceanumlab` within that folder.
 
@@ -182,15 +168,15 @@
 ```sh
 jlpm
 jlpm test
 ```
 
 #### Integration tests
 
-This extension uses [Playwright](https://playwright.dev/docs/intro/) for the integration tests (aka user level tests).
+This extension uses [Playwright](https://playwright.dev/docs/intro) for the integration tests (aka user level tests).
 More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
 
 More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

