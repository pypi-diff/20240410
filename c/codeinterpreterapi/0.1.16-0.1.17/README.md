# Comparing `tmp/codeinterpreterapi-0.1.16.tar.gz` & `tmp/codeinterpreterapi-0.1.17.tar.gz`

## Comparing `codeinterpreterapi-0.1.16.tar` & `codeinterpreterapi-0.1.17.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.env.example
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.python-version
--rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/dev-setup.sh
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/mkdocs.yml
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/requirements-dev.lock
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/roadmap.todo
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/FUNDING.yml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/dependabot.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/workflows/ci.yml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/bitcoin_chart.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/code_interpreter_response.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/code_interpreter_session.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/codebox.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/concepts_overview.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/deploy.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/file.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/index.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/installation.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/iris_dataset.md
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/settings.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/streamlit_webapp.md
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/usage.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/docs/user_request.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/analyze_dataset.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/anthropic_claude.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/chat_cli.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/chat_history_backend.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/convert_file.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/plot_sin_wave.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/show_bitcoin_chart.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/use_additional_tools.py
--rw-r--r--   0        0        0    62087 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/bitcoin_chart.png
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/iris.csv
--rw-r--r--   0        0        0   138297 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/assets/iris_analysis.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/__init__.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/app.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/chainlitui.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/examples/frontend/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/_patch_parser.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chat_history.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/config.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/schema.py
--rw-r--r--   0        0        0    20167 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/extract_code.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/rm_dl_link.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/modifications_check.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/chain_test.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/general_test.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/tests/run_examples.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/LICENSE
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/README.md
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/pyproject.toml
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.env.example
+-rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/dev-setup.sh
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/mkdocs.yml
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/requirements-dev.lock
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/roadmap.todo
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.github/FUNDING.yml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.github/dependabot.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/bitcoin_chart.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/code_interpreter_response.md
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/code_interpreter_session.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/codebox.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/concepts_overview.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/deploy.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/file.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/index.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/installation.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/iris_dataset.md
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/settings.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/streamlit_webapp.md
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/usage.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/docs/user_request.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/analyze_dataset.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/anthropic_claude.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/chat_cli.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/chat_history_backend.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/convert_file.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/plot_sin_wave.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/show_bitcoin_chart.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/use_additional_tools.py
+-rw-r--r--   0        0        0    62087 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/assets/bitcoin_chart.png
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/assets/iris.csv
+-rw-r--r--   0        0        0   138297 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/assets/iris_analysis.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/frontend/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/frontend/app.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/frontend/chainlitui.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/examples/frontend/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/_patch_parser.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/chat_history.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/schema.py
+-rw-r--r--   0        0        0    20167 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/extract_code.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/rm_dl_link.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/tests/chain_test.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/tests/general_test.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/tests/run_examples.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/LICENSE
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/README.md
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/pyproject.toml
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 codeinterpreterapi-0.1.17/PKG-INFO
```

### Comparing `codeinterpreterapi-0.1.16/mkdocs.yml` & `codeinterpreterapi-0.1.17/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/requirements-dev.lock` & `codeinterpreterapi-0.1.17/requirements-dev.lock`

 * *Files 15% similar despite different names*

```diff
@@ -4,55 +4,55 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-aiohttp==3.9.1
+aiohttp==3.9.3
     # via codeboxapi
     # via langchain
     # via langchain-community
 aiosignal==1.3.1
     # via aiohttp
-altair==5.2.0
+altair==5.3.0
     # via streamlit
 annotated-types==0.6.0
     # via pydantic
-anyio==4.1.0
+anyio==4.3.0
     # via httpx
     # via jupyter-server
     # via openai
-appnope==0.1.3
+appnope==0.1.4
     # via ipykernel
 argon2-cffi==23.1.0
     # via jupyter-server
     # via nbclassic
     # via notebook
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 asttokens==2.4.1
     # via stack-data
-attrs==23.1.0
+attrs==23.2.0
     # via aiohttp
     # via jsonschema
     # via referencing
-babel==2.13.1
+babel==2.14.0
     # via mkdocs-material
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via nbconvert
 bleach==6.1.0
     # via nbconvert
 blinker==1.7.0
     # via streamlit
-cachetools==5.3.2
+cachetools==5.3.3
     # via streamlit
-certifi==2023.11.17
+certifi==2024.2.2
     # via httpcore
     # via httpx
     # via requests
 cffi==1.16.0
     # via argon2-cffi-bindings
 cfgv==3.4.0
     # via pre-commit
@@ -61,152 +61,150 @@
 click==8.1.7
     # via mkdocs
     # via streamlit
 codeboxapi==0.1.19
     # via codeinterpreterapi
 colorama==0.4.6
     # via mkdocs-material
-comm==0.2.0
+comm==0.2.2
     # via ipykernel
 dataclasses-json==0.6.4
     # via langchain
     # via langchain-community
-debugpy==1.8.0
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
 distlib==0.3.8
     # via virtualenv
-distro==1.8.0
+distro==1.9.0
     # via openai
 entrypoints==0.4
     # via jupyter-client
 executing==2.0.1
     # via stack-data
-fastjsonschema==2.19.0
+fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via virtualenv
 fqdn==1.5.1
     # via jsonschema
-frozenlist==1.4.0
+frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 ghp-import==2.1.0
     # via mkdocs
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.40
+gitpython==3.1.43
     # via streamlit
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
-httpx==0.25.2
+httpx==0.27.0
     # via openai
-identify==2.5.33
+identify==2.5.35
     # via pre-commit
 idna==3.6
     # via anyio
     # via httpx
     # via jsonschema
     # via requests
     # via yarl
-importlib-metadata==6.11.0
-    # via streamlit
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.27.1
+ipykernel==6.29.4
     # via nbclassic
     # via notebook
-ipython==8.18.1
+ipython==8.23.0
     # via ipykernel
 ipython-genutils==0.2.0
     # via nbclassic
     # via notebook
 isoduration==20.11.0
     # via jsonschema
-isort==5.13.1
+isort==5.13.2
 jedi==0.19.1
     # via ipython
-jinja2==3.1.2
+jinja2==3.1.3
     # via altair
     # via jupyter-server
     # via mkdocs
     # via mkdocs-material
     # via nbclassic
     # via nbconvert
     # via notebook
     # via pydeck
 jsonpatch==1.33
     # via langchain
     # via langchain-core
 jsonpointer==2.4
     # via jsonpatch
     # via jsonschema
-jsonschema==4.20.0
+jsonschema==4.21.1
     # via altair
     # via jupyter-events
     # via nbformat
-jsonschema-specifications==2023.11.2
+jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-client==7.4.9
     # via ipykernel
     # via jupyter-kernel-gateway
     # via jupyter-server
     # via nbclassic
     # via nbclient
     # via notebook
-jupyter-core==5.5.0
+jupyter-core==5.7.2
     # via ipykernel
     # via jupyter-client
     # via jupyter-kernel-gateway
     # via jupyter-server
     # via nbclassic
     # via nbclient
     # via nbconvert
     # via nbformat
     # via notebook
-jupyter-events==0.9.0
+jupyter-events==0.10.0
     # via jupyter-server
 jupyter-kernel-gateway==2.5.2
     # via codeboxapi
-jupyter-server==2.12.1
+jupyter-server==2.13.0
     # via nbclassic
     # via notebook-shim
-jupyter-server-terminals==0.5.0
+jupyter-server-terminals==0.5.3
     # via jupyter-server
 jupyterlab-pygments==0.3.0
     # via nbconvert
-langchain==0.1.14
+langchain==0.1.15
     # via codeinterpreterapi
-langchain-community==0.0.31
+langchain-community==0.0.32
     # via langchain
-langchain-core==0.1.40
+langchain-core==0.1.41
     # via langchain
     # via langchain-community
     # via langchain-openai
     # via langchain-text-splitters
-langchain-openai==0.1.1
+langchain-openai==0.1.2
     # via codeinterpreterapi
 langchain-text-splitters==0.0.1
     # via langchain
-langsmith==0.1.40
+langsmith==0.1.43
     # via langchain
     # via langchain-community
     # via langchain-core
-markdown==3.5.1
+markdown==3.6
     # via mkdocs
     # via mkdocs-material
     # via pymdown-extensions
 markdown-it-py==3.0.0
     # via rich
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via jinja2
     # via mkdocs
     # via nbconvert
 marshmallow==3.21.1
     # via dataclasses-json
 matplotlib-inline==0.1.6
     # via ipykernel
@@ -215,169 +213,170 @@
     # via markdown-it-py
 mergedeep==1.3.4
     # via mkdocs
 mistune==3.0.2
     # via nbconvert
 mkdocs==1.5.3
     # via mkdocs-material
-mkdocs-material==9.5.2
+mkdocs-material==9.5.17
 mkdocs-material-extensions==1.3.1
     # via mkdocs-material
-multidict==6.0.4
+multidict==6.0.5
     # via aiohttp
     # via yarl
-mypy==1.7.1
+mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
     # via typing-inspect
 nbclassic==1.0.0
     # via notebook
-nbclient==0.9.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.12.0
+nbconvert==7.16.3
     # via jupyter-server
     # via nbclassic
     # via notebook
-nbformat==5.9.2
+nbformat==5.10.4
     # via jupyter-server
     # via nbclassic
     # via nbclient
     # via nbconvert
     # via notebook
-nest-asyncio==1.5.8
+nest-asyncio==1.6.0
     # via ipykernel
     # via jupyter-client
     # via nbclassic
     # via notebook
 nodeenv==1.8.0
     # via pre-commit
-notebook==6.5.6
+notebook==6.5.4
     # via jupyter-kernel-gateway
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via nbclassic
-numpy==1.26.2
+numpy==1.26.4
     # via altair
     # via langchain
     # via langchain-community
+    # via pandas
     # via pyarrow
     # via pydeck
     # via streamlit
-openai==1.16.1
+openai==1.16.2
     # via langchain-openai
 orjson==3.10.0
     # via langsmith
-overrides==7.4.0
+overrides==7.7.0
     # via jupyter-server
 packaging==23.2
     # via altair
     # via ipykernel
     # via jupyter-server
     # via langchain-core
     # via marshmallow
     # via mkdocs
     # via nbconvert
     # via pytest
     # via streamlit
 paginate==0.5.6
     # via mkdocs-material
-pandas==2.1.4
+pandas==2.2.1
     # via altair
     # via streamlit
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pathspec==0.12.1
     # via mkdocs
 pexpect==4.9.0
     # via ipython
-pillow==10.1.0
+pillow==10.3.0
     # via codeboxapi
     # via streamlit
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via jupyter-core
     # via mkdocs
     # via virtualenv
-pluggy==1.3.0
+pluggy==1.4.0
     # via pytest
-pre-commit==3.6.0
-prometheus-client==0.19.0
+pre-commit==3.7.0
+prometheus-client==0.20.0
     # via jupyter-server
     # via nbclassic
     # via notebook
-prompt-toolkit==3.0.41
+prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.1
+protobuf==4.25.3
     # via streamlit
-psutil==5.9.6
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
     # via terminado
 pure-eval==0.2.2
     # via stack-data
-pyarrow==14.0.1
+pyarrow==15.0.2
     # via streamlit
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==2.5.2
+pydantic==2.6.4
     # via codeboxapi
     # via langchain
     # via langchain-core
     # via langsmith
     # via openai
     # via pydantic-settings
-pydantic-core==2.14.5
+pydantic-core==2.16.3
     # via pydantic
-pydantic-settings==2.1.0
+pydantic-settings==2.2.1
     # via codeboxapi
-pydeck==0.8.1b0
+pydeck==0.8.0
     # via streamlit
 pygments==2.17.2
     # via ipython
     # via mkdocs-material
     # via nbconvert
     # via rich
-pymdown-extensions==10.5
+pymdown-extensions==10.7.1
     # via mkdocs-material
-pytest==7.4.3
-python-dateutil==2.8.2
+pytest==8.1.1
+python-dateutil==2.9.0.post0
     # via arrow
     # via ghp-import
     # via jupyter-client
     # via pandas
-    # via streamlit
-python-dotenv==1.0.0
+python-dotenv==1.0.1
     # via pydantic-settings
 python-json-logger==2.0.7
     # via jupyter-events
-pytz==2023.3.post1
+pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via jupyter-events
     # via langchain
     # via langchain-community
     # via langchain-core
     # via mkdocs
     # via pre-commit
     # via pymdown-extensions
     # via pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-pyzmq==24.0.1
+pyzmq==25.1.2
+    # via codeinterpreterapi
     # via ipykernel
     # via jupyter-client
     # via jupyter-server
     # via nbclassic
     # via notebook
-referencing==0.32.0
+referencing==0.34.0
     # via jsonschema
     # via jsonschema-specifications
     # via jupyter-events
-regex==2023.10.3
+regex==2023.12.25
     # via mkdocs-material
     # via tiktoken
 requests==2.31.0
     # via codeboxapi
     # via jupyter-kernel-gateway
     # via langchain
     # via langchain-community
@@ -387,124 +386,118 @@
     # via tiktoken
 rfc3339-validator==0.1.4
     # via jsonschema
     # via jupyter-events
 rfc3986-validator==0.1.1
     # via jsonschema
     # via jupyter-events
-rich==13.7.0
+rich==13.7.1
     # via streamlit
-rpds-py==0.13.2
+rpds-py==0.18.0
     # via jsonschema
     # via referencing
-ruff==0.1.7
-send2trash==1.8.2
+ruff==0.3.5
+send2trash==1.8.3
     # via jupyter-server
     # via nbclassic
     # via notebook
-setuptools==69.0.2
+setuptools==69.2.0
     # via nodeenv
 six==1.16.0
     # via asttokens
     # via bleach
     # via python-dateutil
     # via rfc3339-validator
 smmap==5.0.1
     # via gitdb
-sniffio==1.3.0
+sniffio==1.3.1
     # via anyio
     # via httpx
     # via openai
 soupsieve==2.5
     # via beautifulsoup4
 sqlalchemy==2.0.29
     # via langchain
     # via langchain-community
 stack-data==0.6.3
     # via ipython
-streamlit==1.29.0
+streamlit==1.33.0
     # via codeinterpreterapi
 tenacity==8.2.3
     # via langchain
     # via langchain-community
     # via langchain-core
     # via streamlit
-terminado==0.18.0
+terminado==0.18.1
     # via jupyter-server
     # via jupyter-server-terminals
     # via nbclassic
     # via notebook
 tiktoken==0.6.0
     # via langchain-openai
 tinycss2==1.2.1
     # via nbconvert
 toml==0.10.2
     # via streamlit
-toolz==0.12.0
+toolz==0.12.1
     # via altair
 tornado==6.4
     # via ipykernel
     # via jupyter-client
     # via jupyter-kernel-gateway
     # via jupyter-server
     # via nbclassic
     # via notebook
     # via streamlit
     # via terminado
-tqdm==4.66.1
+tqdm==4.66.2
     # via openai
-traitlets==5.14.0
+traitlets==5.14.2
     # via comm
     # via ipykernel
     # via ipython
     # via jupyter-client
     # via jupyter-core
     # via jupyter-events
     # via jupyter-kernel-gateway
     # via jupyter-server
     # via matplotlib-inline
     # via nbclassic
     # via nbclient
     # via nbconvert
     # via nbformat
     # via notebook
-types-python-dateutil==2.8.19.14
+types-python-dateutil==2.9.0.20240316
     # via arrow
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via mypy
     # via openai
     # via pydantic
     # via pydantic-core
     # via sqlalchemy
     # via streamlit
     # via typing-inspect
 typing-inspect==0.9.0
     # via dataclasses-json
-tzdata==2023.3
+tzdata==2024.1
     # via pandas
-tzlocal==5.2
-    # via streamlit
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
-validators==0.22.0
-    # via streamlit
-virtualenv==20.25.0
+virtualenv==20.25.1
     # via pre-commit
-watchdog==3.0.0
+watchdog==4.0.0
     # via mkdocs
-wcwidth==0.2.12
+wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via bleach
     # via tinycss2
 websocket-client==1.7.0
     # via jupyter-server
 websockets==12.0
     # via codeboxapi
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
```

### Comparing `codeinterpreterapi-0.1.16/requirements.lock` & `codeinterpreterapi-0.1.17/requirements.lock`

 * *Files 5% similar despite different names*

```diff
@@ -4,140 +4,142 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-aiohttp==3.9.1
+aiohttp==3.9.3
     # via codeboxapi
     # via langchain
     # via langchain-community
 aiosignal==1.3.1
     # via aiohttp
 annotated-types==0.6.0
     # via pydantic
-anyio==4.1.0
+anyio==4.3.0
     # via httpx
     # via openai
-attrs==23.1.0
+attrs==23.2.0
     # via aiohttp
-certifi==2023.11.17
+certifi==2024.2.2
     # via httpcore
     # via httpx
     # via requests
 charset-normalizer==3.3.2
     # via requests
 codeboxapi==0.1.19
     # via codeinterpreterapi
 dataclasses-json==0.6.4
     # via langchain
     # via langchain-community
-distro==1.8.0
+distro==1.9.0
     # via openai
-frozenlist==1.4.0
+frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
-httpx==0.25.2
+httpx==0.27.0
     # via openai
 idna==3.6
     # via anyio
     # via httpx
     # via requests
     # via yarl
 jsonpatch==1.33
     # via langchain
     # via langchain-core
 jsonpointer==2.4
     # via jsonpatch
-langchain==0.1.14
+langchain==0.1.15
     # via codeinterpreterapi
-langchain-community==0.0.31
+langchain-community==0.0.32
     # via langchain
-langchain-core==0.1.40
+langchain-core==0.1.41
     # via langchain
     # via langchain-community
     # via langchain-openai
     # via langchain-text-splitters
-langchain-openai==0.1.1
+langchain-openai==0.1.2
     # via codeinterpreterapi
 langchain-text-splitters==0.0.1
     # via langchain
-langsmith==0.1.40
+langsmith==0.1.43
     # via langchain
     # via langchain-community
     # via langchain-core
 marshmallow==3.21.1
     # via dataclasses-json
-multidict==6.0.4
+multidict==6.0.5
     # via aiohttp
     # via yarl
 mypy-extensions==1.0.0
     # via typing-inspect
 numpy==1.26.4
     # via langchain
     # via langchain-community
-openai==1.16.1
+openai==1.16.2
     # via langchain-openai
 orjson==3.10.0
     # via langsmith
 packaging==23.2
     # via langchain-core
     # via marshmallow
-pydantic==2.5.2
+pydantic==2.6.4
     # via codeboxapi
     # via langchain
     # via langchain-core
     # via langsmith
     # via openai
     # via pydantic-settings
-pydantic-core==2.14.5
+pydantic-core==2.16.3
     # via pydantic
-pydantic-settings==2.1.0
+pydantic-settings==2.2.1
     # via codeboxapi
-python-dotenv==1.0.0
+python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via langchain
     # via langchain-community
     # via langchain-core
+pyzmq==25.1.2
+    # via codeinterpreterapi
 regex==2023.12.25
     # via tiktoken
 requests==2.31.0
     # via codeboxapi
     # via langchain
     # via langchain-community
     # via langsmith
     # via tiktoken
-sniffio==1.3.0
+sniffio==1.3.1
     # via anyio
     # via httpx
     # via openai
 sqlalchemy==2.0.29
     # via langchain
     # via langchain-community
 tenacity==8.2.3
     # via langchain
     # via langchain-community
     # via langchain-core
 tiktoken==0.6.0
     # via langchain-openai
-tqdm==4.66.1
+tqdm==4.66.2
     # via openai
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via openai
     # via pydantic
     # via pydantic-core
     # via sqlalchemy
     # via typing-inspect
 typing-inspect==0.9.0
     # via dataclasses-json
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
 websockets==12.0
     # via codeboxapi
 yarl==1.9.4
     # via aiohttp
```

### Comparing `codeinterpreterapi-0.1.16/.github/FUNDING.yml` & `codeinterpreterapi-0.1.17/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/.github/workflows/ci.yml` & `codeinterpreterapi-0.1.17/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/.github/workflows/python-publish.yml` & `codeinterpreterapi-0.1.17/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/bitcoin_chart.md` & `codeinterpreterapi-0.1.17/docs/bitcoin_chart.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/code_interpreter_session.md` & `codeinterpreterapi-0.1.17/docs/code_interpreter_session.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/codebox.md` & `codeinterpreterapi-0.1.17/docs/codebox.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/deploy.md` & `codeinterpreterapi-0.1.17/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/file.md` & `codeinterpreterapi-0.1.17/docs/file.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/index.md` & `codeinterpreterapi-0.1.17/docs/index.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/installation.md` & `codeinterpreterapi-0.1.17/docs/installation.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/iris_dataset.md` & `codeinterpreterapi-0.1.17/docs/iris_dataset.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/docs/settings.md` & `codeinterpreterapi-0.1.17/docs/settings.md`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/analyze_dataset.py` & `codeinterpreterapi-0.1.17/examples/analyze_dataset.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/chat_history_backend.py` & `codeinterpreterapi-0.1.17/examples/chat_history_backend.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/use_additional_tools.py` & `codeinterpreterapi-0.1.17/examples/use_additional_tools.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/assets/bitcoin_chart.png` & `codeinterpreterapi-0.1.17/examples/assets/bitcoin_chart.png`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/assets/iris.csv` & `codeinterpreterapi-0.1.17/examples/assets/iris.csv`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/assets/iris_analysis.png` & `codeinterpreterapi-0.1.17/examples/assets/iris_analysis.png`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/frontend/app.py` & `codeinterpreterapi-0.1.17/examples/frontend/app.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/frontend/chainlitui.py` & `codeinterpreterapi-0.1.17/examples/frontend/chainlitui.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/examples/frontend/utils.py` & `codeinterpreterapi-0.1.17/examples/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/_patch_parser.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/_patch_parser.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chat_history.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/chat_history.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/config.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/config.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/schema.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/schema.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/session.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/session.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/extract_code.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/extract_code.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/chains/rm_dl_link.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/chains/rm_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/modifications_check.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/remove_dl_link.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/remove_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/src/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.1.17/src/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/tests/chain_test.py` & `codeinterpreterapi-0.1.17/tests/chain_test.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/tests/general_test.py` & `codeinterpreterapi-0.1.17/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/.gitignore` & `codeinterpreterapi-0.1.17/.gitignore`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/LICENSE` & `codeinterpreterapi-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.1.16/README.md` & `codeinterpreterapi-0.1.17/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # 👾 Code Interpreter API
 
 [![Version](https://badge.fury.io/py/codeinterpreterapi.svg)](https://badge.fury.io/py/codeinterpreterapi)
-[![code-check](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml/badge.svg)](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml)
 ![Downloads](https://img.shields.io/pypi/dm/codeinterpreterapi)
 ![License](https://img.shields.io/pypi/l/codeinterpreterapi)
 ![PyVersion](https://img.shields.io/pypi/pyversions/codeinterpreterapi)
 
 A [LangChain](https://github.com/langchain-ai/langchain) implementation of the ChatGPT Code Interpreter.
 Using CodeBoxes as backend for sandboxed python code execution.
 [CodeBox](https://github.com/shroominic/codebox-api/tree/main) is the simplest cloud infrastructure for your LLM Apps.
```

### Comparing `codeinterpreterapi-0.1.16/pyproject.toml` & `codeinterpreterapi-0.1.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "codeinterpreterapi"
-version = "0.1.16"
+version = "0.1.17"
 description = "CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter."
 authors = [{ name = "Shroominic", email = "contact@shroominic.com" }]
 dependencies = [
     "langchain-openai>=0.1.1",
     "codeboxapi>=0.1.19",
     "langchain>=0.1.14",
+    "pyzmq==25.1.2",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">= 3.9.7, <3.12"
+requires-python = ">= 3.9.7, <3.13"
 keywords = [
     "codeinterpreter",
     "chatgpt",
     "codeinterpreterapi",
     "api",
     "langchain",
     "codeboxapi",
```

### Comparing `codeinterpreterapi-0.1.16/PKG-INFO` & `codeinterpreterapi-0.1.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: codeinterpreterapi
-Version: 0.1.16
+Version: 0.1.17
 Summary: CodeInterpreterAPI is an (unofficial) open source python interface for the ChatGPT CodeInterpreter.
 Project-URL: Code, https://github.com/shroominic/codeinterpreter-api
 Project-URL: Docs, https://shroominic.github.io/codeinterpreter-api
 Author-email: Shroominic <contact@shroominic.com>
 License: # MIT License
         
         Copyright (c) 2023 Dominic Bäumer
@@ -30,33 +30,33 @@
 Keywords: api,chatgpt,codeboxapi,codeinterpreter,codeinterpreterapi,langchain
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.12,>=3.9.7
+Requires-Python: <3.13,>=3.9.7
 Requires-Dist: codeboxapi>=0.1.19
 Requires-Dist: langchain-openai>=0.1.1
 Requires-Dist: langchain>=0.1.14
+Requires-Dist: pyzmq==25.1.2
 Provides-Extra: all
 Requires-Dist: codeboxapi[all]; extra == 'all'
 Requires-Dist: codeinterpreterapi[frontend]; extra == 'all'
 Provides-Extra: frontend
 Requires-Dist: streamlit; extra == 'frontend'
 Provides-Extra: image-support
 Requires-Dist: codeboxapi[image-support]; extra == 'image-support'
 Provides-Extra: localbox
 Requires-Dist: codeboxapi[local-support]; extra == 'localbox'
 Description-Content-Type: text/markdown
 
 # 👾 Code Interpreter API
 
 [![Version](https://badge.fury.io/py/codeinterpreterapi.svg)](https://badge.fury.io/py/codeinterpreterapi)
-[![code-check](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml/badge.svg)](https://github.com/shroominic/codeinterpreter-api/actions/workflows/code-check.yml)
 ![Downloads](https://img.shields.io/pypi/dm/codeinterpreterapi)
 ![License](https://img.shields.io/pypi/l/codeinterpreterapi)
 ![PyVersion](https://img.shields.io/pypi/pyversions/codeinterpreterapi)
 
 A [LangChain](https://github.com/langchain-ai/langchain) implementation of the ChatGPT Code Interpreter.
 Using CodeBoxes as backend for sandboxed python code execution.
 [CodeBox](https://github.com/shroominic/codebox-api/tree/main) is the simplest cloud infrastructure for your LLM Apps.
```

