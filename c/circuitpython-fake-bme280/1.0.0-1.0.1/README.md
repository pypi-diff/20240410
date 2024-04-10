# Comparing `tmp/circuitpython-fake-bme280-1.0.0.tar.gz` & `tmp/circuitpython-fake-bme280-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-fake-bme280-1.0.0.tar", last modified: Tue Apr  2 19:19:40 2024, max compression
+gzip compressed data, was "circuitpython-fake-bme280-1.0.1.tar", last modified: Wed Apr 10 16:03:48 2024, max compression
```

## Comparing `circuitpython-fake-bme280-1.0.0.tar` & `circuitpython-fake-bme280-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.403219 circuitpython-fake-bme280-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.407219 circuitpython-fake-bme280-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.407219 circuitpython-fake-bme280-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.407219 circuitpython-fake-bme280-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-02 19:19:40.000000 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-02 19:19:40.000000 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:19:40.000000 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 19:19:40.000000 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:19:40.000000 circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.407219 circuitpython-fake-bme280-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-02 19:19:37.000000 circuitpython-fake-bme280-1.0.0/examples/fake_bme280_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/fake_bme280/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:37.000000 circuitpython-fake-bme280-1.0.0/fake_bme280/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-04-02 19:19:37.000000 circuitpython-fake-bme280-1.0.0/fake_bme280/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-02 19:19:37.000000 circuitpython-fake-bme280-1.0.0/fake_bme280/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 19:19:37.000000 circuitpython-fake-bme280-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 19:19:30.000000 circuitpython-fake-bme280-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:19:40.411219 circuitpython-fake-bme280-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.426512 circuitpython-fake-bme280-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.430512 circuitpython-fake-bme280-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.430512 circuitpython-fake-bme280-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.430512 circuitpython-fake-bme280-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-10 16:03:48.000000 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-10 16:03:48.000000 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:03:48.000000 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 16:03:48.000000 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 16:03:48.000000 circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-10 16:03:46.000000 circuitpython-fake-bme280-1.0.1/examples/fake_bme280_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/fake_bme280/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:03:46.000000 circuitpython-fake-bme280-1.0.1/fake_bme280/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-10 16:03:46.000000 circuitpython-fake-bme280-1.0.1/fake_bme280/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 16:03:46.000000 circuitpython-fake-bme280-1.0.1/fake_bme280/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 16:03:46.000000 circuitpython-fake-bme280-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 16:03:39.000000 circuitpython-fake-bme280-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:03:48.434512 circuitpython-fake-bme280-1.0.1/setup.cfg
```

### Comparing `circuitpython-fake-bme280-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-fake-bme280-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/.github/workflows/release_gh.yml` & `circuitpython-fake-bme280-1.0.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/.gitignore` & `circuitpython-fake-bme280-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/.pre-commit-config.yaml` & `circuitpython-fake-bme280-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/.pylintrc` & `circuitpython-fake-bme280-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/LICENSE` & `circuitpython-fake-bme280-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-fake-bme280-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/LICENSES/MIT.txt` & `circuitpython-fake-bme280-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-fake-bme280-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/PKG-INFO` & `circuitpython-fake-bme280-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-fake-bme280
-Version: 1.0.0
+Version: 1.0.1
 Summary: BME280 Driver for CircuitPython used for testing functionality with no hardware attached
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brentru/CircuitPython_Fake_BME280
 Keywords: adafruit,blinka,circuitpython,micropython,fake_bme280,bme280,,test,,fake,,mock,,stub
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-fake-bme280-1.0.0/README.rst` & `circuitpython-fake-bme280-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/PKG-INFO` & `circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-fake-bme280
-Version: 1.0.0
+Version: 1.0.1
 Summary: BME280 Driver for CircuitPython used for testing functionality with no hardware attached
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brentru/CircuitPython_Fake_BME280
 Keywords: adafruit,blinka,circuitpython,micropython,fake_bme280,bme280,,test,,fake,,mock,,stub
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-fake-bme280-1.0.0/circuitpython_fake_bme280.egg-info/SOURCES.txt` & `circuitpython-fake-bme280-1.0.1/circuitpython_fake_bme280.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/docs/_static/favicon.ico` & `circuitpython-fake-bme280-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/docs/conf.py` & `circuitpython-fake-bme280-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/docs/index.rst` & `circuitpython-fake-bme280-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/examples/fake_bme280_simpletest.py` & `circuitpython-fake-bme280-1.0.1/examples/fake_bme280_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-fake-bme280-1.0.0/fake_bme280/basic.py` & `circuitpython-fake-bme280-1.0.1/fake_bme280/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 """
 import math
-import os
 import socket as pool
 import ssl
 import typing  # pylint: disable=unused-import
+import toml
 from micropython import const
 import adafruit_requests
 from fake_bme280.protocol import I2C_Impl, SPI_Impl
 
 try:
     from busio import I2C, SPI
     from digitalio import DigitalInOut
@@ -71,25 +71,27 @@
 _BME280_REGISTER_CTRL_HUM = const(0xF2)
 _BME280_REGISTER_STATUS = const(0xF3)
 _BME280_REGISTER_CTRL_MEAS = const(0xF4)
 _BME280_REGISTER_CONFIG = const(0xF5)
 _BME280_REGISTER_TEMPDATA = const(0xFA)
 _BME280_REGISTER_HUMIDDATA = const(0xFD)
 
+# Load the settings.toml file
+toml_config = toml.load("settings.toml")
+
 # OpenWeatherMap API
 # GET weather data for a specific location
-# TODO: this could be cleaned up a bit..
 DATA_SOURCE = (
     "http://api.openweathermap.org/data/2.5/weather?q="
-    + os.getenv("openweather_location")
+    + toml_config["openweather_location"]
     + "&units="
-    + os.getenv("openweather_units")
+    + toml_config["openweather_units"]
     + "&mode=json"
     + "&appid="
-    + os.getenv("openweather_token")
+    + toml_config["openweather_token"]
 )
 
 
 class Adafruit_BME280:
     """Driver from BME280 Temperature, Humidity and Barometric Pressure sensor
 
     .. note::
@@ -109,19 +111,14 @@
         self.overscan_temperature = OVERSCAN_X1
         self.overscan_pressure = OVERSCAN_X16
         self._t_standby = STANDBY_TC_125
         self._mode = MODE_SLEEP
         self.sea_level_pressure = 1013.25
         """Pressure in hectoPascals at sea level. Used to calibrate `altitude`."""
         self._t_fine = None
-        # Configure OpenWeather for mock data
-        self.openweather_token = os.getenv("OPENWEATHER_TOKEN", "default_token")
-        self.openweather_location = os.getenv(
-            "OPENWEATHER_LOCATION", "default_location"
-        )
         # Configure a CPython adafruit_requests session
         self.requests = adafruit_requests.Session(pool, ssl.create_default_context())
         self._current_forcast = None
         # Test call get_forecast
         self.get_forecast()
 
     def get_forecast(self):
```

### Comparing `circuitpython-fake-bme280-1.0.0/fake_bme280/protocol.py` & `circuitpython-fake-bme280-1.0.1/fake_bme280/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from busio import I2C, SPI
 from digitalio import DigitalInOut
 
 
 class I2C_Impl:
     "Protocol implementation for the I2C bus."
 
-    # pylint: disable=too-few-public-methods
+    # pylint: disable=too-few-public-methods, unused-argument, unused-import
     def __init__(self, i2c: I2C, address: int) -> None:
         from adafruit_bus_device import (  # pylint: disable=import-outside-toplevel
             i2c_device,
         )
 
-        self._i2c = i2c_device.I2CDevice(i2c, address)
+        # self._i2c = i2c_device.I2CDevice(i2c, address)
 
 
 class SPI_Impl:
     """Protocol implemenation for the SPI bus."""
 
     # pylint: disable=too-few-public-methods
     def __init__(
```

### Comparing `circuitpython-fake-bme280-1.0.0/pyproject.toml` & `circuitpython-fake-bme280-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-fake-bme280"
 description = "BME280 Driver for CircuitPython used for testing functionality with no hardware attached"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/brentru/CircuitPython_Fake_BME280"}
 keywords = [
     "adafruit",
```

