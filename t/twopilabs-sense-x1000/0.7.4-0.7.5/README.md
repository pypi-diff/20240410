# Comparing `tmp/twopilabs-sense-x1000-0.7.4.tar.gz` & `tmp/twopilabs-sense-x1000-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twopilabs-sense-x1000-0.7.4.tar", last modified: Mon Nov 27 15:25:49 2023, max compression
+gzip compressed data, was "twopilabs-sense-x1000-0.7.5.tar", last modified: Wed Apr 10 09:55:52 2024, max compression
```

## Comparing `twopilabs-sense-x1000-0.7.4.tar` & `twopilabs-sense-x1000-0.7.5.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.533234 twopilabs-sense-x1000-0.7.4/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1050 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      895 2023-11-27 15:25:49.533234 twopilabs-sense-x1000-0.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.391234 twopilabs-sense-x1000-0.7.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.460234 twopilabs-sense-x1000-0.7.4/docs/_images/
--rw-rw-rw-   0 root         (0) root         (0)    52074 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/_images/examples-fast-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    48716 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/_images/examples-hdf5-record-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)   425392 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/_images/examples-live-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    58587 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/_images/examples-range-doppler-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/configuring.rst
--rw-rw-rw-   0 root         (0) root         (0)     6058 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/controlling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.464234 twopilabs-sense-x1000-0.7.4/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/examples/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/examples/fast-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/examples/hdf5-recorder.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/examples/live-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/examples/range-doppler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.465234 twopilabs-sense-x1000-0.7.4/docs/extensions/
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/extensions/source.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/introduction.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.513234 twopilabs-sense-x1000-0.7.4/docs/reference/
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_calc.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_control.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_core.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_initiate.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_memory.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_sense.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_system.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.scpi_trigger.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.x1000_base.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/reference/sense.x1000.x1000_scpi.rst
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.520234 twopilabs-sense-x1000-0.7.4/examples/
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/environment.yml
--rwxrwxrwx   0 root         (0) root         (0)    24515 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/fast-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/fast-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)     3180 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/fw-upgrade.py
--rwxrwxrwx   0 root         (0) root         (0)     8479 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/hdf5-record.py
--rwxrwxrwx   0 root         (0) root         (0)     7983 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/hdf5-replay.py
--rwxrwxrwx   0 root         (0) root         (0)    11766 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/live-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/live-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)    13267 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/range-doppler.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/examples/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-11-27 15:25:49.534234 twopilabs-sense-x1000-0.7.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.357234 twopilabs-sense-x1000-0.7.4/twopilabs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.357234 twopilabs-sense-x1000-0.7.4/twopilabs/sense/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.528234 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3524 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_calc.py
--rw-rw-rw-   0 root         (0) root         (0)    23485 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_control.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_initiate.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_memory.py
--rw-rw-rw-   0 root         (0) root         (0)     8597 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_sense.py
--rw-rw-rw-   0 root         (0) root         (0)    11079 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_system.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000.py
--rw-rw-rw-   0 root         (0) root         (0)    49053 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2818 2023-11-27 15:24:28.000000 twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000_scpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-27 15:25:49.531234 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/
--rw-r--r--   0 root         (0) root         (0)      895 2023-11-27 15:25:49.000000 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1963 2023-11-27 15:25:49.000000 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-27 15:25:49.000000 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-11-27 15:25:49.000000 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-27 15:25:49.000000 twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.599120 twopilabs-sense-x1000-0.7.5/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 09:55:52.599120 twopilabs-sense-x1000-0.7.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.573120 twopilabs-sense-x1000-0.7.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.576120 twopilabs-sense-x1000-0.7.5/docs/_images/
+-rw-rw-rw-   0 root         (0) root         (0)    52074 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/_images/examples-fast-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    48716 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/_images/examples-hdf5-record-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)   425392 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/_images/examples-live-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    58587 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/_images/examples-range-doppler-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/configuring.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6058 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/controlling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.579120 twopilabs-sense-x1000-0.7.5/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/examples/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/examples/fast-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/examples/hdf5-recorder.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/examples/live-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/examples/range-doppler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.579120 twopilabs-sense-x1000-0.7.5/docs/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/extensions/source.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/introduction.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.585120 twopilabs-sense-x1000-0.7.5/docs/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_calc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_control.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_initiate.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_memory.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_sense.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_system.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.scpi_trigger.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.x1000_base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/reference/sense.x1000.x1000_scpi.rst
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.589120 twopilabs-sense-x1000-0.7.5/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/environment.yml
+-rwxrwxrwx   0 root         (0) root         (0)    24515 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/fast-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/fast-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)     3180 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/fw-upgrade.py
+-rwxrwxrwx   0 root         (0) root         (0)     8479 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/hdf5-record.py
+-rwxrwxrwx   0 root         (0) root         (0)     7983 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/hdf5-replay.py
+-rwxrwxrwx   0 root         (0) root         (0)    11766 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/live-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/live-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)    13267 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/range-doppler.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/examples/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/rth-append-path.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-10 09:55:52.600120 twopilabs-sense-x1000-0.7.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.590120 twopilabs-sense-x1000-0.7.5/spec/
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/spec/logo-quadrat-2-32x32.ico
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/spec/x1000-examples-win64.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.565120 twopilabs-sense-x1000-0.7.5/twopilabs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.565120 twopilabs-sense-x1000-0.7.5/twopilabs/sense/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.596120 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3524 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_calc.py
+-rw-rw-rw-   0 root         (0) root         (0)    23485 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_initiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8597 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_sense.py
+-rw-rw-rw-   0 root         (0) root         (0)    11079 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000.py
+-rw-rw-rw-   0 root         (0) root         (0)    49053 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2024-04-10 09:54:55.000000 twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000_scpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 09:55:52.598120 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-10 09:55:52.000000 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-10 09:55:52.000000 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 09:55:52.000000 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-10 09:55:52.000000 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-10 09:55:52.000000 twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/top_level.txt
```

### Comparing `twopilabs-sense-x1000-0.7.4/LICENSE` & `twopilabs-sense-x1000-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/PKG-INFO` & `twopilabs-sense-x1000-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.7.4
+Version: 0.7.5
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.7.4/docs/Makefile` & `twopilabs-sense-x1000-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/_images/examples-fast-plot-screenshot.png` & `twopilabs-sense-x1000-0.7.5/docs/_images/examples-fast-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/_images/examples-hdf5-record-screenshot.png` & `twopilabs-sense-x1000-0.7.5/docs/_images/examples-hdf5-record-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/_images/examples-live-plot-screenshot.png` & `twopilabs-sense-x1000-0.7.5/docs/_images/examples-live-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/_images/examples-range-doppler-screenshot.png` & `twopilabs-sense-x1000-0.7.5/docs/_images/examples-range-doppler-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/conf.py` & `twopilabs-sense-x1000-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/configuring.rst` & `twopilabs-sense-x1000-0.7.5/docs/configuring.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/controlling.rst` & `twopilabs-sense-x1000-0.7.5/docs/controlling.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/examples/examples.rst` & `twopilabs-sense-x1000-0.7.5/docs/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/examples/hdf5-recorder.rst` & `twopilabs-sense-x1000-0.7.5/docs/examples/hdf5-recorder.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/examples/range-doppler.rst` & `twopilabs-sense-x1000-0.7.5/docs/examples/range-doppler.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/extensions/source.py` & `twopilabs-sense-x1000-0.7.5/docs/extensions/source.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/index.rst` & `twopilabs-sense-x1000-0.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/docs/introduction.rst` & `twopilabs-sense-x1000-0.7.5/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/fast-plot.py` & `twopilabs-sense-x1000-0.7.5/examples/fast-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/fast-plot.spec` & `twopilabs-sense-x1000-0.7.5/examples/fast-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/fw-upgrade.py` & `twopilabs-sense-x1000-0.7.5/examples/fw-upgrade.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/hdf5-record.py` & `twopilabs-sense-x1000-0.7.5/examples/hdf5-record.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/hdf5-replay.py` & `twopilabs-sense-x1000-0.7.5/examples/hdf5-replay.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/live-plot.py` & `twopilabs-sense-x1000-0.7.5/examples/live-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/live-plot.spec` & `twopilabs-sense-x1000-0.7.5/examples/live-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/examples/range-doppler.py` & `twopilabs-sense-x1000-0.7.5/examples/range-doppler.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/setup.cfg` & `twopilabs-sense-x1000-0.7.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_calc.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_calc.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_control.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_control.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_core.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_core.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_initiate.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_initiate.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_memory.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_memory.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_sense.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_sense.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_system.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_system.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/scpi_trigger.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/scpi_trigger.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000_base.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000_base.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs/sense/x1000/x1000_scpi.py` & `twopilabs-sense-x1000-0.7.5/twopilabs/sense/x1000/x1000_scpi.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/PKG-INFO` & `twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.7.4
+Version: 0.7.5
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.7.4/twopilabs_sense_x1000.egg-info/SOURCES.txt` & `twopilabs-sense-x1000-0.7.5/twopilabs_sense_x1000.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 .gitlab-ci.yml
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
+rth-append-path.py
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
 docs/configuring.rst
 docs/controlling.rst
 docs/index.rst
@@ -40,14 +42,16 @@
 examples/fw-upgrade.py
 examples/hdf5-record.py
 examples/hdf5-replay.py
 examples/live-plot.py
 examples/live-plot.spec
 examples/range-doppler.py
 examples/requirements.txt
+spec/logo-quadrat-2-32x32.ico
+spec/x1000-examples-win64.spec
 twopilabs/sense/x1000/__init__.py
 twopilabs/sense/x1000/scpi_calc.py
 twopilabs/sense/x1000/scpi_control.py
 twopilabs/sense/x1000/scpi_core.py
 twopilabs/sense/x1000/scpi_initiate.py
 twopilabs/sense/x1000/scpi_memory.py
 twopilabs/sense/x1000/scpi_sense.py
```

