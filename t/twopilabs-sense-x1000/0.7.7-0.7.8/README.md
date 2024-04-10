# Comparing `tmp/twopilabs-sense-x1000-0.7.7.tar.gz` & `tmp/twopilabs-sense-x1000-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twopilabs-sense-x1000-0.7.7.tar", last modified: Wed Apr 10 10:13:35 2024, max compression
+gzip compressed data, was "twopilabs-sense-x1000-0.7.8.tar", last modified: Wed Apr 10 12:11:16 2024, max compression
```

## Comparing `twopilabs-sense-x1000-0.7.7.tar` & `twopilabs-sense-x1000-0.7.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.746068 twopilabs-sense-x1000-0.7.7/
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2889 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 10:13:35.746068 twopilabs-sense-x1000-0.7.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.719067 twopilabs-sense-x1000-0.7.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.722067 twopilabs-sense-x1000-0.7.7/docs/_images/
--rw-rw-rw-   0 root         (0) root         (0)    52074 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/_images/examples-fast-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    48716 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/_images/examples-hdf5-record-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)   425392 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/_images/examples-live-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    58587 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/_images/examples-range-doppler-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/configuring.rst
--rw-rw-rw-   0 root         (0) root         (0)     6058 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/controlling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.724068 twopilabs-sense-x1000-0.7.7/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/examples/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/examples/fast-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/examples/hdf5-recorder.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/examples/live-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/examples/range-doppler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.725067 twopilabs-sense-x1000-0.7.7/docs/extensions/
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/extensions/source.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/introduction.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.731068 twopilabs-sense-x1000-0.7.7/docs/reference/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_calc.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_control.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_core.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_initiate.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_memory.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_sense.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_system.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.scpi_trigger.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.x1000_base.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/reference/sense.x1000.x1000_scpi.rst
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.735068 twopilabs-sense-x1000-0.7.7/examples/
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/environment.yml
--rwxrwxrwx   0 root         (0) root         (0)    24515 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/fast-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/fast-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)     3180 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/fw-upgrade.py
--rwxrwxrwx   0 root         (0) root         (0)     8479 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/hdf5-record.py
--rwxrwxrwx   0 root         (0) root         (0)     7983 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/hdf5-replay.py
--rwxrwxrwx   0 root         (0) root         (0)    11766 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/live-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/live-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)    13267 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/range-doppler.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/examples/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/rth-append-path.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-10 10:13:35.747068 twopilabs-sense-x1000-0.7.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.736068 twopilabs-sense-x1000-0.7.7/spec/
--rw-rw-rw-   0 root         (0) root         (0)     4286 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/spec/logo-quadrat-2-32x32.ico
--rw-rw-rw-   0 root         (0) root         (0)     4217 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/spec/x1000-examples-win64.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.710068 twopilabs-sense-x1000-0.7.7/twopilabs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.710068 twopilabs-sense-x1000-0.7.7/twopilabs/sense/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.742068 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/
--rw-rw-rw-   0 root         (0) root         (0)      135 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3524 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_calc.py
--rw-rw-rw-   0 root         (0) root         (0)    23485 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_control.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_initiate.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_memory.py
--rw-rw-rw-   0 root         (0) root         (0)     8597 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_sense.py
--rw-rw-rw-   0 root         (0) root         (0)    11079 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_system.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000.py
--rw-rw-rw-   0 root         (0) root         (0)    49053 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2818 2024-04-10 10:12:38.000000 twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000_scpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:13:35.745068 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/
--rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 10:13:35.000000 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-10 10:13:35.000000 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:13:35.000000 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-10 10:13:35.000000 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-10 10:13:35.000000 twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.906325 twopilabs-sense-x1000-0.7.8/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 12:11:16.905325 twopilabs-sense-x1000-0.7.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.884325 twopilabs-sense-x1000-0.7.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.886325 twopilabs-sense-x1000-0.7.8/docs/_images/
+-rw-rw-rw-   0 root         (0) root         (0)    52074 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/_images/examples-fast-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    48716 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/_images/examples-hdf5-record-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)   425392 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/_images/examples-live-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    58587 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/_images/examples-range-doppler-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/configuring.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6058 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/controlling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.888325 twopilabs-sense-x1000-0.7.8/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/examples/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/examples/fast-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/examples/hdf5-recorder.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/examples/live-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/examples/range-doppler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.889325 twopilabs-sense-x1000-0.7.8/docs/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/extensions/source.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/introduction.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.893325 twopilabs-sense-x1000-0.7.8/docs/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_calc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_control.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_initiate.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_memory.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_sense.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_system.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.scpi_trigger.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.x1000_base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/reference/sense.x1000.x1000_scpi.rst
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.897325 twopilabs-sense-x1000-0.7.8/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/environment.yml
+-rwxrwxrwx   0 root         (0) root         (0)    24515 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/fast-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/fast-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)     3180 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/fw-upgrade.py
+-rwxrwxrwx   0 root         (0) root         (0)     8479 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/hdf5-record.py
+-rwxrwxrwx   0 root         (0) root         (0)     7983 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/hdf5-replay.py
+-rwxrwxrwx   0 root         (0) root         (0)    11766 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/live-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/live-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)    13267 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/range-doppler.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/examples/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/rth-append-path.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-10 12:11:16.906325 twopilabs-sense-x1000-0.7.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.898325 twopilabs-sense-x1000-0.7.8/spec/
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/spec/logo-quadrat-2-32x32.ico
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/spec/x1000-examples-win64.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.877325 twopilabs-sense-x1000-0.7.8/twopilabs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.877325 twopilabs-sense-x1000-0.7.8/twopilabs/sense/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.902325 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3524 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_calc.py
+-rw-rw-rw-   0 root         (0) root         (0)    23485 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_initiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8597 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_sense.py
+-rw-rw-rw-   0 root         (0) root         (0)    11079 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000.py
+-rw-rw-rw-   0 root         (0) root         (0)    49053 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2024-04-10 12:10:12.000000 twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000_scpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 12:11:16.905325 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 12:11:16.000000 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-10 12:11:16.000000 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 12:11:16.000000 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-10 12:11:16.000000 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-10 12:11:16.000000 twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/top_level.txt
```

### Comparing `twopilabs-sense-x1000-0.7.7/.gitlab-ci.yml` & `twopilabs-sense-x1000-0.7.8/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 variables:
+  GIT_STRATEGY: clone # Clone entire repo
+  GIT_DEPTH: 0 # No shallow copy to get version info (tags/branches)
   EXAMPLES_EXAMPLES_PACKAGE_FILE: "${CI_PROJECT_NAME}-examples-${CI_COMMIT_TAG}"
   EXAMPLES_EXAMPLES_PACKAGE_REGISTRY_URL: "${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/generic/${CI_PROJECT_NAME}/${CI_COMMIT_TAG}"
 
 image:
   name: python:3.8-slim-bullseye
   entrypoint: [ '/bin/bash', '-c', 'ln -snf /bin/bash /bin/sh && /bin/bash -c $0' ]
 
 stages:
   - build
   - deploy
-  - examples
+  - examples_build
+  - examples_deploy
 
 package:
   stage: build
   before_script:
     - apt-get update && apt-get install -y git
     - pip install --upgrade pip setuptools setuptools-scm wheel build
   script:
@@ -56,45 +59,42 @@
     - mv build/docs/ public/
   artifacts:
     paths:
     - public
 
 # Building examples binaries
 build_examples_win64:
-  stage: examples
+  stage: examples_build
   image:
     name: $PYTHON_DISTUTILS_IMAGE_WIN64
   rules:
     - if: $PYTHON_DISTUTILS_IMAGE_WIN64
   script:
     - /entrypoint.sh pyinstaller spec/x1000-examples-win64.spec
     - mkdir -p dist/x1000-examples/lib
     - mv dist/x1000-examples/*.pyd dist/x1000-examples/api-ms-*.dll dist/x1000-examples/lib/
   artifacts:
     paths:
-      - dist/x1000-examples
+      - dist/
 
 upload_examples_win64:
-  stage: examples
-  dependencies:
-      - build_examples_win64
+  stage: examples_deploy
   image: alpine:latest
   rules:
     - if: $PYTHON_DISTUTILS_IMAGE_WIN64 && $CI_COMMIT_TAG
   script:
     - |
       apk add zip curl
+      echo "${CI_COMMIT_TAG}" > dist/VERSION      
       cd dist/x1000-examples
       zip -r ${EXAMPLES_PACKAGE_FILE}-win64.zip *
       curl -k --header "JOB-TOKEN: ${CI_JOB_TOKEN}" --upload-file ${EXAMPLES_PACKAGE_FILE}-win64.zip ${EXAMPLES_PACKAGE_REGISTRY_URL}/${EXAMPLES_PACKAGE_FILE}-win64.zip
 
 release_examples:
-  stage: examples
-  dependencies:
-      - upload_examples_win64
+  stage: examples_deploy
   image: registry.gitlab.com/gitlab-org/release-cli:latest
   rules:
     - if: '$PYTHON_DISTUTILS_IMAGE_WIN64 && $CI_COMMIT_TAG =~ /^([0-9]+)\.([0-9]+)\.([0-9]+)$/'
   script:
     - echo "Running Release Job"
   release:
     tag_name: $CI_COMMIT_TAG
```

### Comparing `twopilabs-sense-x1000-0.7.7/LICENSE` & `twopilabs-sense-x1000-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/PKG-INFO` & `twopilabs-sense-x1000-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.7.7
+Version: 0.7.8
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.7.7/docs/Makefile` & `twopilabs-sense-x1000-0.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/_images/examples-fast-plot-screenshot.png` & `twopilabs-sense-x1000-0.7.8/docs/_images/examples-fast-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/_images/examples-hdf5-record-screenshot.png` & `twopilabs-sense-x1000-0.7.8/docs/_images/examples-hdf5-record-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/_images/examples-live-plot-screenshot.png` & `twopilabs-sense-x1000-0.7.8/docs/_images/examples-live-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/_images/examples-range-doppler-screenshot.png` & `twopilabs-sense-x1000-0.7.8/docs/_images/examples-range-doppler-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/conf.py` & `twopilabs-sense-x1000-0.7.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/configuring.rst` & `twopilabs-sense-x1000-0.7.8/docs/configuring.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/controlling.rst` & `twopilabs-sense-x1000-0.7.8/docs/controlling.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/examples/examples.rst` & `twopilabs-sense-x1000-0.7.8/docs/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/examples/hdf5-recorder.rst` & `twopilabs-sense-x1000-0.7.8/docs/examples/hdf5-recorder.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/examples/range-doppler.rst` & `twopilabs-sense-x1000-0.7.8/docs/examples/range-doppler.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/extensions/source.py` & `twopilabs-sense-x1000-0.7.8/docs/extensions/source.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/index.rst` & `twopilabs-sense-x1000-0.7.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/docs/introduction.rst` & `twopilabs-sense-x1000-0.7.8/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/fast-plot.py` & `twopilabs-sense-x1000-0.7.8/examples/fast-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/fast-plot.spec` & `twopilabs-sense-x1000-0.7.8/examples/fast-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/fw-upgrade.py` & `twopilabs-sense-x1000-0.7.8/examples/fw-upgrade.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/hdf5-record.py` & `twopilabs-sense-x1000-0.7.8/examples/hdf5-record.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/hdf5-replay.py` & `twopilabs-sense-x1000-0.7.8/examples/hdf5-replay.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/live-plot.py` & `twopilabs-sense-x1000-0.7.8/examples/live-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/live-plot.spec` & `twopilabs-sense-x1000-0.7.8/examples/live-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/examples/range-doppler.py` & `twopilabs-sense-x1000-0.7.8/examples/range-doppler.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/setup.cfg` & `twopilabs-sense-x1000-0.7.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/spec/logo-quadrat-2-32x32.ico` & `twopilabs-sense-x1000-0.7.8/spec/logo-quadrat-2-32x32.ico`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/spec/x1000-examples-win64.spec` & `twopilabs-sense-x1000-0.7.8/spec/x1000-examples-win64.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_calc.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_calc.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_control.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_control.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_core.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_core.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_initiate.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_initiate.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_memory.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_memory.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_sense.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_sense.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_system.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_system.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/scpi_trigger.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/scpi_trigger.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000_base.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000_base.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs/sense/x1000/x1000_scpi.py` & `twopilabs-sense-x1000-0.7.8/twopilabs/sense/x1000/x1000_scpi.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/PKG-INFO` & `twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.7.7
+Version: 0.7.8
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.7.7/twopilabs_sense_x1000.egg-info/SOURCES.txt` & `twopilabs-sense-x1000-0.7.8/twopilabs_sense_x1000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

