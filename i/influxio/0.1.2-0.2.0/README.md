# Comparing `tmp/influxio-0.1.2.tar.gz` & `tmp/influxio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxio-0.1.2.tar", last modified: Fri Mar 22 22:45:02 2024, max compression
+gzip compressed data, was "influxio-0.2.0.tar", last modified: Wed Apr 10 01:31:15 2024, max compression
```

## Comparing `influxio-0.1.2.tar` & `influxio-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-22 22:45:02.240015 influxio-0.1.2/
--rw-r--r--   0 amo        (501) staff       (20)      617 2024-03-22 22:44:19.000000 influxio-0.1.2/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)     1097 2023-03-11 00:48:15.000000 influxio-0.1.2/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)       79 2023-03-11 00:48:15.000000 influxio-0.1.2/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    11384 2024-03-22 22:45:02.239479 influxio-0.1.2/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     8016 2024-03-22 22:34:52.000000 influxio-0.1.2/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-22 22:45:02.226293 influxio-0.1.2/doc/
--rw-r--r--   0 amo        (501) staff       (20)     2203 2024-01-30 20:18:01.000000 influxio-0.1.2/doc/backlog.rst
--rw-r--r--   0 amo        (501) staff       (20)     2326 2024-02-15 00:19:17.000000 influxio-0.1.2/doc/development.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-22 22:45:02.230865 influxio-0.1.2/influxio/
--rw-r--r--   0 amo        (501) staff       (20)      110 2023-03-13 01:28:31.000000 influxio-0.1.2/influxio/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     2950 2023-03-15 23:52:07.000000 influxio-0.1.2/influxio/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     2247 2024-02-14 23:51:01.000000 influxio-0.1.2/influxio/core.py
--rw-r--r--   0 amo        (501) staff       (20)     3207 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/io.py
--rw-r--r--   0 amo        (501) staff       (20)    11343 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/model.py
--rw-r--r--   0 amo        (501) staff       (20)     2048 2024-02-14 23:51:01.000000 influxio-0.1.2/influxio/testdata.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-22 22:45:02.236593 influxio-0.1.2/influxio/util/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-10 22:36:39.000000 influxio-0.1.2/influxio/util/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1548 2023-03-11 00:20:47.000000 influxio-0.1.2/influxio/util/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     1302 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/util/common.py
--rw-r--r--   0 amo        (501) staff       (20)      328 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/util/compat.py
--rw-r--r--   0 amo        (501) staff       (20)      414 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/util/db.py
--rw-r--r--   0 amo        (501) staff       (20)     2605 2023-11-12 01:46:47.000000 influxio-0.1.2/influxio/util/report.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-22 22:45:02.237355 influxio-0.1.2/influxio.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    11384 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      534 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       46 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      411 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       15 2024-03-22 22:45:02.000000 influxio-0.1.2/influxio.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     5128 2024-03-22 22:43:14.000000 influxio-0.1.2/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-03-22 22:45:02.240115 influxio-0.1.2/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.291934 influxio-0.2.0/
+-rw-r--r--   0 amo        (501) staff       (20)      731 2024-04-10 01:30:29.000000 influxio-0.2.0/CHANGES.rst
+-rw-r--r--   0 amo        (501) staff       (20)     1097 2023-03-11 00:48:15.000000 influxio-0.2.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)       79 2023-03-11 00:48:15.000000 influxio-0.2.0/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    12388 2024-04-10 01:31:15.291425 influxio-0.2.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     8997 2024-04-10 01:29:43.000000 influxio-0.2.0/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.278186 influxio-0.2.0/doc/
+-rw-r--r--   0 amo        (501) staff       (20)     2781 2024-04-10 01:29:43.000000 influxio-0.2.0/doc/backlog.rst
+-rw-r--r--   0 amo        (501) staff       (20)     2338 2024-04-07 22:18:58.000000 influxio-0.2.0/doc/development.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.282279 influxio-0.2.0/influxio/
+-rw-r--r--   0 amo        (501) staff       (20)      110 2023-03-13 01:28:31.000000 influxio-0.2.0/influxio/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)    15584 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/adapter.py
+-rw-r--r--   0 amo        (501) staff       (20)     4514 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     3354 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     4084 2024-04-07 22:18:58.000000 influxio-0.2.0/influxio/io.py
+-rw-r--r--   0 amo        (501) staff       (20)     2325 2024-04-10 00:09:59.000000 influxio-0.2.0/influxio/model.py
+-rw-r--r--   0 amo        (501) staff       (20)     2048 2024-02-14 23:51:01.000000 influxio-0.2.0/influxio/testdata.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.289047 influxio-0.2.0/influxio/util/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-10 22:36:39.000000 influxio-0.2.0/influxio/util/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1548 2023-03-11 00:20:47.000000 influxio-0.2.0/influxio/util/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     2101 2024-04-10 01:29:43.000000 influxio-0.2.0/influxio/util/common.py
+-rw-r--r--   0 amo        (501) staff       (20)      328 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/compat.py
+-rw-r--r--   0 amo        (501) staff       (20)      414 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/db.py
+-rw-r--r--   0 amo        (501) staff       (20)     2605 2023-11-12 01:46:47.000000 influxio-0.2.0/influxio/util/report.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-10 01:31:15.289622 influxio-0.2.0/influxio.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    12388 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      554 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       46 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      419 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       15 2024-04-10 01:31:15.000000 influxio-0.2.0/influxio.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     5168 2024-04-09 23:21:05.000000 influxio-0.2.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-10 01:31:15.292020 influxio-0.2.0/setup.cfg
```

### Comparing `influxio-0.1.2/CHANGES.rst` & `influxio-0.2.0/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 influxio changelog
 ##################
 
 
 in progress
 ===========
 
+2024-04-10 v0.2.0
+=================
+- Export data from InfluxDB API and data directory into line protocol format
+
 2024-03-22 v0.1.2
 =================
 - Add support for Python 3.12
 - Dependencies: Use ``dask[dataframe]``
 
 2023-11-12 v0.1.1
 =================
```

### Comparing `influxio-0.1.2/LICENSE` & `influxio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxio-0.1.2/PKG-INFO` & `influxio-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxio
-Version: 0.1.2
+Version: 0.2.0
 Summary: Import and export data into/from InfluxDB
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: changelog, https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/daq-tools/influxio
 Project-URL: homepage, https://github.com/daq-tools/influxio
 Project-URL: repository, https://github.com/daq-tools/influxio
@@ -48,129 +48,135 @@
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click<9
 Requires-Dist: colorama<1
 Requires-Dist: crate[sqlalchemy]
 Requires-Dist: cratedb-toolkit
-Requires-Dist: dask[dataframe]<=2024.3.1,>=2020
+Requires-Dist: dask[dataframe]>=2020
 Requires-Dist: importlib-metadata; python_version <= "3.9"
+Requires-Dist: influx-line==1.0.0
 Requires-Dist: influxdb-client[ciso]<2
 Requires-Dist: line-protocol-parser<2
 Requires-Dist: pandas<2.3
 Requires-Dist: psycopg2-binary<3
 Requires-Dist: pueblo>=0.0.7
 Requires-Dist: SQLAlchemy-Utils<0.42
 Requires-Dist: yarl<2
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: mypy==1.9.0; extra == "develop"
 Requires-Dist: poethepoet<0.26; extra == "develop"
 Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff==0.3.4; extra == "develop"
+Requires-Dist: ruff==0.3.5; extra == "develop"
 Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
 Requires-Dist: pytest<9; extra == "test"
-Requires-Dist: pytest-cov<5; extra == "test"
+Requires-Dist: pytest-cov<6; extra == "test"
 
 ########
 influxio
 ########
 
-.. image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/daq-tools/influxio/actions/workflows/tests.yml
     :alt: Build status
 
-.. image:: https://codecov.io/gh/daq-tools/influxio/branch/master/graph/badge.svg
+.. |ci-coverage| image:: https://codecov.io/gh/daq-tools/influxio/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/daq-tools/influxio
     :alt: Coverage
 
-.. image:: https://img.shields.io/pypi/v/influxio.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/pyversions/influxio.svg
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Python Version
 
-.. image:: https://img.shields.io/pypi/dw/influxio.svg
-    :target: https://pypi.org/project/influxio/
-    :alt: PyPI Downloads
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/influxio/month
+    :target: https://www.pepy.tech/projects/influxio
+    :alt: PyPI Downloads per month
 
-.. image:: https://img.shields.io/pypi/status/influxio.svg
+.. |status| image:: https://img.shields.io/pypi/status/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Status
 
-.. image:: https://img.shields.io/pypi/l/influxio.svg
+.. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
+.. end-badges
+
 
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
 ``influxio`` is, amongst others, based on the excellent `dask`_, `fsspec`_,
-`influxdb-client`_, `line-protocol-parser`_, `pandas`_, and `SQLAlchemy`_
-packages.
+`influxdb-client`_, `influx-line`_, `line-protocol-parser`_, `pandas`_,
+and `SQLAlchemy`_ packages.
 
 Please note that ``influxio`` is alpha-quality software, and a work in progress.
 Contributions of all kinds are very welcome, in order to make it more solid.
 Breaking changes should be expected until a 1.0 release, so version pinning
 is recommended, especially when you use it as a library.
 
-**Caveat**: Only a few features sketched out in the README have actually been
-implemented right now.
-
 
 ********
 Synopsis
 ********
 
-.. code-block:: sh
-
-    # Export from data directory to line protocol format.
-    influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
-        "file://export.lp"
+.. code-block:: shell
 
     # Export from API to database.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "sqlite://export.sqlite?table=demo"
 
+    # Export from data directory to line protocol format.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp"
+
 
 **********
 Quickstart
 **********
 
 If you are in a hurry, and want to run ``influxio`` without any installation,
 just use the OCI image on Podman or Docker.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive/demo"
 
 
 *****
 Setup
 *****
 
 Install ``influxio`` from PyPI.
 
-.. code-block:: sh
+.. code-block:: shell
 
     pip install influxio
 
 
 *****
 Usage
 *****
@@ -191,24 +197,24 @@
 
 Command line use
 ================
 
 Help
 ----
 
-.. code-block:: sh
+.. code-block:: shell
 
     influxio --help
     influxio info
     influxio copy --help
 
 Import
 ------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From test data to API.
     # Choose one of dummy, mixed, dateindex, wide.
     influxio copy \
         "testdata://dateindex/" \
         "http://example:token@localhost:8086/testdrive/demo"
 
@@ -218,86 +224,109 @@
         "http://example:token@localhost:8086/testdrive/demo"
 
     # With selected amount of rows and columns (only supported by certain test data sources).
     influxio copy \
         "testdata://wide/?rows=42&columns=42" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "file://tests/testdata/basic.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "https://github.com/influxdata/influxdb2-sample-data/raw/master/air-sensor-data/air-sensor-data.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-Export
-------
+    # From line protocol file to any database supported by SQLAlchemy.
+    influxio copy \
+        "file://export.lp" \
+        "sqlite://export.sqlite?table=export"
+
+
+Export from API
+---------------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From API to database file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
-        "sqlite://export.sqlite?table=demo"
+        "sqlite:///export.sqlite?table=demo"
 
     # From API to database server.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive?table=demo"
 
     # From API to line protocol file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://export.lp"
 
-    # From data directory to line protocol file.
+    # From API to line protocol on stdout.
+    influxio copy \
+        "http://example:token@localhost:8086/testdrive/demo" \
+        "file://-?format=lp"
+
+
+Export from data directory
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB data directory to line protocol file.
     influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
         "file://export.lp"
 
-    # From line protocol file to database.
+    # From InfluxDB data directory to line protocol file, compressed with gzip.
     influxio copy \
-        "file://export.lp" \
-        "sqlite://export.sqlite?table=export"
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp.gz"
+
+    # From InfluxDB data directory to line protocol on stdout.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        ""file://-?format=lp"
+
 
 OCI
 ---
 
 OCI images are available on the GitHub Container Registry (GHCR). In order to
 run them on Podman or Docker, invoke:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "stdout://export.lp"
 
 If you want to work with files on your filesystem, you will need to either
 mount the working directory into the container using the ``--volume`` option,
 or use the ``--interactive`` option to consume STDIN, like:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --volume=$(pwd):/data ghcr.io/daq-tools/influxio \
         influxio copy "file:///data/export.lp" "sqlite:///data/export.sqlite?table=export"
 
     cat export.lp | \
     docker run --rm --interactive --network=host ghcr.io/daq-tools/influxio \
         influxio copy "stdin://?format=lp" "crate://crate@localhost:4200/testdrive/export"
 
 In order to always run the latest ``nightly`` development version, and to use a
 shortcut for that, this section outlines how to use an alias for ``influxio``,
 and a variable for storing the input URL. It may be useful to save a few
 keystrokes on subsequent invocations.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker pull ghcr.io/daq-tools/influxio:nightly
     alias influxio="docker run --rm --interactive ghcr.io/daq-tools/influxio:nightly influxio"
     SOURCE=https://github.com/daq-tools/influxio/raw/main/tests/testdata/basic.lp
     TARGET=crate://crate@localhost:4200/testdrive/basic
 
     influxio copy "${SOURCE}" "${TARGET}"
@@ -321,14 +350,15 @@
 - `Outflux`_
 
 
 .. _dask: https://www.dask.org/
 .. _development: doc/development.rst
 .. _fsspec: https://pypi.org/project/fsspec/
 .. _influx: https://docs.influxdata.com/influxdb/latest/reference/cli/influx/
+.. _influx-line: https://github.com/functionoffunction/influx-line
 .. _influxd: https://docs.influxdata.com/influxdb/latest/reference/cli/influxd/
 .. _InfluxDB Fetcher: https://github.com/hgomez/influxdb
 .. _InfluxDB line protocol: https://docs.influxdata.com/influxdb/latest/reference/syntax/line-protocol/
 .. _influxdb-client: https://github.com/influxdata/influxdb-client-python
 .. _influxdb-write-to-postgresql: https://github.com/eras/influxdb-write-to-postgresql
 .. _line-protocol-parser: https://github.com/Penlect/line-protocol-parser
 .. _list of other projects: doc/prior-art.rst
```

### Comparing `influxio-0.1.2/README.rst` & `influxio-0.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 ########
 influxio
 ########
 
-.. image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/daq-tools/influxio/actions/workflows/tests.yml
     :alt: Build status
 
-.. image:: https://codecov.io/gh/daq-tools/influxio/branch/master/graph/badge.svg
+.. |ci-coverage| image:: https://codecov.io/gh/daq-tools/influxio/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/daq-tools/influxio
     :alt: Coverage
 
-.. image:: https://img.shields.io/pypi/v/influxio.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/pyversions/influxio.svg
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Python Version
 
-.. image:: https://img.shields.io/pypi/dw/influxio.svg
-    :target: https://pypi.org/project/influxio/
-    :alt: PyPI Downloads
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/influxio/month
+    :target: https://www.pepy.tech/projects/influxio
+    :alt: PyPI Downloads per month
 
-.. image:: https://img.shields.io/pypi/status/influxio.svg
+.. |status| image:: https://img.shields.io/pypi/status/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Status
 
-.. image:: https://img.shields.io/pypi/l/influxio.svg
+.. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
+.. end-badges
+
 
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
 ``influxio`` is, amongst others, based on the excellent `dask`_, `fsspec`_,
-`influxdb-client`_, `line-protocol-parser`_, `pandas`_, and `SQLAlchemy`_
-packages.
+`influxdb-client`_, `influx-line`_, `line-protocol-parser`_, `pandas`_,
+and `SQLAlchemy`_ packages.
 
 Please note that ``influxio`` is alpha-quality software, and a work in progress.
 Contributions of all kinds are very welcome, in order to make it more solid.
 Breaking changes should be expected until a 1.0 release, so version pinning
 is recommended, especially when you use it as a library.
 
-**Caveat**: Only a few features sketched out in the README have actually been
-implemented right now.
-
 
 ********
 Synopsis
 ********
 
-.. code-block:: sh
-
-    # Export from data directory to line protocol format.
-    influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
-        "file://export.lp"
+.. code-block:: shell
 
     # Export from API to database.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "sqlite://export.sqlite?table=demo"
 
+    # Export from data directory to line protocol format.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp"
+
 
 **********
 Quickstart
 **********
 
 If you are in a hurry, and want to run ``influxio`` without any installation,
 just use the OCI image on Podman or Docker.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive/demo"
 
 
 *****
 Setup
 *****
 
 Install ``influxio`` from PyPI.
 
-.. code-block:: sh
+.. code-block:: shell
 
     pip install influxio
 
 
 *****
 Usage
 *****
@@ -114,24 +119,24 @@
 
 Command line use
 ================
 
 Help
 ----
 
-.. code-block:: sh
+.. code-block:: shell
 
     influxio --help
     influxio info
     influxio copy --help
 
 Import
 ------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From test data to API.
     # Choose one of dummy, mixed, dateindex, wide.
     influxio copy \
         "testdata://dateindex/" \
         "http://example:token@localhost:8086/testdrive/demo"
 
@@ -141,86 +146,109 @@
         "http://example:token@localhost:8086/testdrive/demo"
 
     # With selected amount of rows and columns (only supported by certain test data sources).
     influxio copy \
         "testdata://wide/?rows=42&columns=42" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "file://tests/testdata/basic.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "https://github.com/influxdata/influxdb2-sample-data/raw/master/air-sensor-data/air-sensor-data.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-Export
-------
+    # From line protocol file to any database supported by SQLAlchemy.
+    influxio copy \
+        "file://export.lp" \
+        "sqlite://export.sqlite?table=export"
+
+
+Export from API
+---------------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From API to database file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
-        "sqlite://export.sqlite?table=demo"
+        "sqlite:///export.sqlite?table=demo"
 
     # From API to database server.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive?table=demo"
 
     # From API to line protocol file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://export.lp"
 
-    # From data directory to line protocol file.
+    # From API to line protocol on stdout.
+    influxio copy \
+        "http://example:token@localhost:8086/testdrive/demo" \
+        "file://-?format=lp"
+
+
+Export from data directory
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB data directory to line protocol file.
     influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
         "file://export.lp"
 
-    # From line protocol file to database.
+    # From InfluxDB data directory to line protocol file, compressed with gzip.
     influxio copy \
-        "file://export.lp" \
-        "sqlite://export.sqlite?table=export"
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp.gz"
+
+    # From InfluxDB data directory to line protocol on stdout.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        ""file://-?format=lp"
+
 
 OCI
 ---
 
 OCI images are available on the GitHub Container Registry (GHCR). In order to
 run them on Podman or Docker, invoke:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "stdout://export.lp"
 
 If you want to work with files on your filesystem, you will need to either
 mount the working directory into the container using the ``--volume`` option,
 or use the ``--interactive`` option to consume STDIN, like:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --volume=$(pwd):/data ghcr.io/daq-tools/influxio \
         influxio copy "file:///data/export.lp" "sqlite:///data/export.sqlite?table=export"
 
     cat export.lp | \
     docker run --rm --interactive --network=host ghcr.io/daq-tools/influxio \
         influxio copy "stdin://?format=lp" "crate://crate@localhost:4200/testdrive/export"
 
 In order to always run the latest ``nightly`` development version, and to use a
 shortcut for that, this section outlines how to use an alias for ``influxio``,
 and a variable for storing the input URL. It may be useful to save a few
 keystrokes on subsequent invocations.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker pull ghcr.io/daq-tools/influxio:nightly
     alias influxio="docker run --rm --interactive ghcr.io/daq-tools/influxio:nightly influxio"
     SOURCE=https://github.com/daq-tools/influxio/raw/main/tests/testdata/basic.lp
     TARGET=crate://crate@localhost:4200/testdrive/basic
 
     influxio copy "${SOURCE}" "${TARGET}"
@@ -244,14 +272,15 @@
 - `Outflux`_
 
 
 .. _dask: https://www.dask.org/
 .. _development: doc/development.rst
 .. _fsspec: https://pypi.org/project/fsspec/
 .. _influx: https://docs.influxdata.com/influxdb/latest/reference/cli/influx/
+.. _influx-line: https://github.com/functionoffunction/influx-line
 .. _influxd: https://docs.influxdata.com/influxdb/latest/reference/cli/influxd/
 .. _InfluxDB Fetcher: https://github.com/hgomez/influxdb
 .. _InfluxDB line protocol: https://docs.influxdata.com/influxdb/latest/reference/syntax/line-protocol/
 .. _influxdb-client: https://github.com/influxdata/influxdb-client-python
 .. _influxdb-write-to-postgresql: https://github.com/eras/influxdb-write-to-postgresql
 .. _line-protocol-parser: https://github.com/Penlect/line-protocol-parser
 .. _list of other projects: doc/prior-art.rst
```

### Comparing `influxio-0.1.2/doc/backlog.rst` & `influxio-0.2.0/doc/backlog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,50 +2,52 @@
 influxio backlog
 ################
 
 
 ************
 Iteration +1
 ************
-- [x] Add project boilerplate
-- [x] Make it work
-- [x] Export to SQLite, PostgreSQL, and CrateDB
-- [x] Fix documentation about crate:// target
-- [x] Check if using a CrateDB schema works well
-- [x] Release 0.1.0
+- [o] README: Demonstrate "library use"
+- [o] README: Caveat about overwrite protection
+- [o] README: How to export from data directory using Docker?
+- [o] README: Add examples using InfluxDB Cloud
+- [o] README: Caveat when exporting unknown measurement from data directory:
+  It can not be detected.
+- [o] README: Inform about ``--verbose`` flag
+- [o] Publish documentation on RTD
+- [o] Add annotated CSV export/import
+- [o] Address "TODO" items
+- [o] Verify documentation. ``influxio.cli.help_copy``
+- [o] More refinements
+- [o] ``list-buckets`` subcommand, for both API and data directory
+- [o] Progress bars for non-Dask tasks
 
 
 ************
 Iteration +2
 ************
-- [o] Fix ``.from_lineprotocol``
-- [o] Tests using ``assert_dataframe_equal``? Maybe in ``cratedb-toolkit``?
-- [o] Support InfluxDB 1.x
-- [o] Verify connecting to InfluxDB Cloud works well
 - [o] Fix ``cratedb_toolkit.sqlalchemy.patch_inspector()`` re. reflection of ``?schema=`` URL parameter
 - [o] Fix ``crate.client.sqlalchemy.dialect.DateTime`` re. ``TimezoneUnawareException``
+- [o] Support InfluxDB 1.x
 - [o] Add Docker Compose file for auxiliary services
-- [o] Refinements
-- [o] Verify documentation. ``influxio.cli.help_copy``
 - [o] Refactor general purpose code to ``pueblo`` package
 - [o] Verify import and export of ILP and CSV files works well
+- [o] Tests using ``assert_dataframe_equal``? Maybe in ``cratedb-toolkit``?
 
 
 ************
 Iteration +3
 ************
-- [o] Unlock more parameters in InfluxDbAdapter.write_df
+- [o] Unlock more parameters in InfluxDbApiAdapter.write_df
 - [o] Format: Compressed line protocol
 - [o] Format: Annotated CSV
   - https://docs.influxdata.com/influxdb/v2.6/reference/syntax/annotated-csv/
   - https://docs.influxdata.com/influxdb/v2.6/reference/syntax/annotated-csv/extended/
 - [o] Backends: python, cmdline, flux
 - [o] InfluxDB 1.x subscriptions?
-- [o] Line protocol builder
-  https://github.com/functionoffunction/influx-line
 - [o] cloud-to-cloud copy
 - [o] influxio list testdata://
 - [o] "SQLAlchemy » Dialects built-in" is broken
 - [o] ``DBURI = "crate+psycopg://localhost:4200"``
 - [o] Use Podman instead of Docker
 
 References
@@ -53,7 +55,22 @@
 - https://docs.influxdata.com/influxdb/v2.6/migrate-data/
 - https://docs.influxdata.com/influxdb/v2.6/reference/cli/influx/write/
 - https://docs.influxdata.com/influxdb/v2.6/reference/cli/influx/backup/
 - https://docs.influxdata.com/influxdb/v2.6/reference/cli/influx/export/
 - https://github.com/influxdata/flux/blob/e513f1483/stdlib/sql/sql_test.flux#L119-L173
 - https://github.com/influxdata/flux/blob/e513f1483/stdlib/universe/universe.flux#L1159-L1176
 - https://github.com/influxdata/flux/blob/e513f1483/stdlib/sql/to.go#L525
+
+
+****
+Done
+****
+- [x] Add project boilerplate
+- [x] Make it work
+- [x] Export to SQLite, PostgreSQL, and CrateDB
+- [x] Fix documentation about crate:// target
+- [x] Check if using a CrateDB schema works well
+- [x] Release 0.1.0
+- [x] Fix ``.from_lineprotocol``
+- [x] Parameters bucket-id and measurement are obligatory on data
+  directory export. Verify that.
+- [x] Be ``--verbose`` by default
```

### Comparing `influxio-0.1.2/doc/development.rst` & `influxio-0.2.0/doc/development.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 For properly running the test cases, you will need running instances of InfluxDB,
 PostgreSQL, and CrateDB. The easiest way to spin up those instances is to use
 Docker or Podman.
 
 InfluxDB
 --------
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm -it --publish=8086:8086 \
         --env=DOCKER_INFLUXDB_INIT_MODE=setup \
         --env=DOCKER_INFLUXDB_INIT_USERNAME=admin \
         --env=DOCKER_INFLUXDB_INIT_PASSWORD=secret1234 \
         --env=DOCKER_INFLUXDB_INIT_ORG=example \
         --env=DOCKER_INFLUXDB_INIT_BUCKET=default \
@@ -40,25 +40,25 @@
         --volume="$PWD/var/lib/influxdb2:/var/lib/influxdb2" \
         influxdb:2.7
 
 - https://github.com/docker-library/docs/blob/master/influxdb/README.md
 
 CrateDB
 -------
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm -it --publish=4200:4200 \
         --volume="$PWD/var/lib/cratedb:/data" \
-        crate:5.6 -Cdiscovery.type=single-node
+        crate:latest -Cdiscovery.type=single-node
 
 - https://github.com/docker-library/docs/blob/master/crate/README.md
 
 PostgreSQL
 ----------
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm -it --publish=5432:5432 \
         --env "POSTGRES_HOST_AUTH_METHOD=trust" postgres:16 \
         postgres -c log_statement=all
 
 Software Tests
 ==============
```

### Comparing `influxio-0.1.2/influxio/core.py` & `influxio-0.2.0/influxio/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
+import typing as t
 from pathlib import Path
 
 from yarl import URL
 
-from influxio.model import InfluxDbAdapter, SqlAlchemyAdapter
+from influxio.adapter import FileAdapter, InfluxDbApiAdapter, InfluxDbEngineAdapter, SqlAlchemyAdapter
+from influxio.model import CommandResult
+from influxio.util.common import url_fullpath
 from influxio.util.db import get_sqlalchemy_dialects
 
 logger = logging.getLogger(__name__)
 
 
-def copy(source: str, target: str, progress: bool = False):
+def copy(source: str, target: str, progress: bool = False) -> t.Union[CommandResult, None]:
     """
     Copy/transfer data from/to InfluxDB API / InfluxDB line protocol / RDBMS.
 
     RDBMS is any SQLAlchemy-supported database.
 
     `source` and `target` are resource identifiers in URL format.
 
@@ -39,35 +42,56 @@
     sqlalchemy_dialects = get_sqlalchemy_dialects()
 
     logger.info(f"Copying from {source} to {target}")
 
     scheme_primary = target_url.scheme.split("+")[0]
 
     if target_url.scheme.startswith("http"):
-        sink = InfluxDbAdapter.from_url(target)
+        sink = InfluxDbApiAdapter.from_url(target)
     elif scheme_primary in sqlalchemy_dialects:
         sink = SqlAlchemyAdapter.from_url(target, progress=True)
+    elif target_url.scheme == "file":
+        sink = FileAdapter.from_url(target, progress=True)
     else:
         raise NotImplementedError(f"Data sink not implemented: {target_url}")
 
     if source_url.scheme == "testdata":
         from influxio.testdata import DataFrameFactory
 
         dff = DataFrameFactory(**source_url.query)
         df = dff.make(source_url.host)
         sink.write_df(df)
 
     elif source_url.scheme == "file":
-        path = Path(source_url.host).joinpath(Path(source_url.path).relative_to("/"))
-        # TODO: Determine file type by suffix.
-        # TODO: Make `precision` configurable.
-        sink.from_lineprotocol(path)
+
+        # Export
+        if target_url.scheme == "file":
+            path = url_fullpath(source_url)
+            source_path_dir = [path.name for path in Path(path).iterdir()]
+            if "data" in source_path_dir and "wal" in source_path_dir:
+                source_element = InfluxDbEngineAdapter.from_url(source)
+                if not source_element.bucket_id:
+                    raise ValueError("Parameter missing or empty: bucket-id")
+                if not source_element.measurement:
+                    raise ValueError("Parameter missing or empty: measurement")
+                return source_element.to_lineprotocol(url=target_url)
+            else:
+                raise FileNotFoundError(f"No InfluxDB data directory: {path}")
+
+        # Import
+        else:
+            path = Path(source_url.host).joinpath(Path(source_url.path).relative_to("/"))
+            # TODO: Determine file type by suffix.
+            # TODO: Make `precision` configurable.
+            sink.from_lineprotocol(path)
 
     elif source_url.scheme.startswith("http"):
-        if isinstance(sink, SqlAlchemyAdapter):
-            source_node = InfluxDbAdapter.from_url(source)
+        if isinstance(sink, (FileAdapter, SqlAlchemyAdapter)):
+            source_node = InfluxDbApiAdapter.from_url(source)
             sink.write(source_node)
         else:
             sink.from_lineprotocol(str(source_url))
 
     else:
         raise NotImplementedError(f"Data source not implemented: {source_url}")
+
+    return None
```

### Comparing `influxio-0.1.2/influxio/io.py` & `influxio-0.2.0/influxio/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import typing as t
 from collections import OrderedDict
 from pathlib import Path
 
 import fsspec
 import pandas as pd
+from influx_line import InfluxLine
 
 logger = logging.getLogger(__name__)
 
 
 BytesString = t.Union[bytes, str]
 BytesStringList = t.List[BytesString]
 
@@ -65,14 +66,35 @@
     """
     Read stream of InfluxDB line protocol into pandas DataFrame.
     """
     records = records_from_lineprotocol(data)
     return pd.DataFrame(records)
 
 
+def dataframe_to_lineprotocol(df: pd.DataFrame, progress: bool = False) -> t.Generator[str, None, None]:
+    """
+    Convert DataFrame to InfluxDB Line Protocol.
+
+    TODO: Needs a test verifying dispatching of tags.
+    TODO: Needs configurability to manually dispatch columns to either fields or tags.
+    TODO: Needs heuristics if timestamp field is called differently than `time`.
+    """
+    for record in df.to_dict(orient="records"):
+        line = InfluxLine(record["measurement"])
+        line.set_timestamp(record["time"].to_datetime64().view("int64"))
+        del record["measurement"]
+        del record["time"]
+        for key, value in record.items():
+            if isinstance(value, (int, float)):
+                line.add_field(key, value)
+            else:
+                line.add_tag(key, value)
+        yield str(line)
+
+
 def dataframe_to_sql(
     df: pd.DataFrame,
     dburi: str,
     tablename: str,
     index=False,
     chunksize=None,
     if_exists="replace",
```

### Comparing `influxio-0.1.2/influxio/model.py` & `influxio-0.2.0/influxio/adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+import io
 import json
 import logging
+import sys
 import typing as t
 from pathlib import Path
 
 import influxdb_client.rest
 import pandas as pd
 import psycopg2
 import sqlalchemy
 import sqlalchemy as sa
 from influxdb_client import InfluxDBClient
 from sqlalchemy_utils import create_database
 from yarl import URL
 
-from influxio.io import dataframe_to_sql
-from influxio.util.common import run_command
+from influxio.io import dataframe_to_lineprotocol, dataframe_to_sql
+from influxio.model import CommandResult, DataFormat, OutputFile
+from influxio.util.common import run_command, url_fullpath
 
 logger = logging.getLogger(__name__)
 
 
-class InfluxDbAdapter:
+class InfluxDbApiAdapter:
     def __init__(self, url: str, token: str, org: str, bucket: str, measurement: str, debug: bool = False):
         self.url = url
         self.token = token
         self.org = org
         self.bucket = bucket
         self.measurement = measurement
         self.debug = debug
         self.client = InfluxDBClient(url=self.url, org=self.org, token=self.token, debug=self.debug)
 
     @classmethod
-    def from_url(cls, url: t.Union[URL, str], **kwargs) -> "InfluxDbAdapter":
+    def from_url(cls, url: t.Union[URL, str], **kwargs) -> "InfluxDbApiAdapter":
         if isinstance(url, str):
             url: URL = URL(url)
         token = url.password
         org = url.user
         bucket, measurement = url.path.strip("/").split("/")
         bare_url = f"{url.scheme}://{url.host}:{url.port}"
         return cls(url=bare_url, token=token, org=org, bucket=bucket, measurement=measurement, **kwargs)
@@ -165,85 +168,114 @@
             --precision={precision} \
             --format=lp \
             {source_option}
         """
         # print("command:", command)  # noqa: ERA001
         run_command(command)
 
-    def get_bucket_id(self):
+    @property
+    def bucket_id(self) -> str:
+        return self.get_bucket_id()
+
+    def get_bucket_id(self) -> str:
         """
         Resolve bucket name to bucket id.
         """
         bucket: influxdb_client.Bucket = self.client.buckets_api().find_bucket_by_name(bucket_name=self.bucket)
         if bucket is None:
             raise KeyError(f"Bucket not found: {self.bucket}")
         return bucket.id
 
-    def to_lineprotocol(self, engine_path: str, output_path: t.Union[str, Path]):
+
+class InfluxDbEngineAdapter:
+    def __init__(self, path: t.Union[Path, str], bucket_id: str, measurement: str, debug: bool = False):
+
+        if isinstance(path, str):
+            path: Path = Path(path)
+
+        self.path = path
+        self.bucket_id = bucket_id
+        self.measurement = measurement
+        self.debug = debug
+
+    @classmethod
+    def from_url(cls, url: t.Union[URL, str], **kwargs) -> "InfluxDbEngineAdapter":
+        if isinstance(url, str):
+            url: URL = URL(url)
+        return cls(
+            path=url_fullpath(url),
+            bucket_id=url.query.get("bucket-id"),
+            measurement=url.query.get("measurement"),
+            **kwargs,
+        )
+
+    def to_lineprotocol(self, url: t.Union[URL, str]) -> CommandResult:
         """
         Export data into lineprotocol format (ILP) by invoking `influxd inspect export-lp`.
 
+        TODO: Unify with `FileAdapter` sink and expand with `InfluxDbApiAdapter`'s API connectivity.
         TODO: Using a hyphen `-` for `--output-path` works well now, so export can also go to stdout.
         TODO: By default, it will *append* to the .lp file.
               Make it configurable to "replace" data.
         TODO: Make it configurable to use compression, or not.
         TODO: Propagate `--start` and `--end` parameters.
         TODO: Capture stderr messages, and forward user admonition.
               »detected deletes in WAL file, some deleted data may be brought back by replaying this export«
               -- https://github.com/influxdata/influxdb/issues/24456
 
         https://docs.influxdata.com/influxdb/v2.6/migrate-data/migrate-oss/
         """
-        logger.info("Exporting data to InfluxDB line protocol format (ILP)")
-        bucket_id = self.get_bucket_id()
+        if isinstance(url, str):
+            url: URL = URL(url)
+        format_ = DataFormat.from_url(url)
+        logger.info(f"Exporting data to InfluxDB line protocol format (ILP): {format_}")
         command = f"""
         influxd inspect export-lp \
-            --engine-path '{engine_path}' \
-            --bucket-id '{bucket_id}' \
+            --engine-path '{self.path}' \
+            --bucket-id '{self.bucket_id}' \
             --measurement '{self.measurement}' \
-            --output-path '{output_path}' \
-            --compress
-        """
-        run_command(command)
-
-
-def decode_database_table(url: URL):
-    """
-    Decode database and table names from database URI path and/or query string.
-
-    Variants:
-
-        /<database>/<table>
-        ?database=<database>&table=<table>
-        ?schema=<database>&table=<table>
-    """
-    try:
-        database, table = url.path.strip("/").split("/")
-    except ValueError as ex:
-        if "too many values to unpack" not in str(ex) and "not enough values to unpack" not in str(ex):
-            raise
-        database = url.query.get("database")
-        table = url.query.get("table")
-        if url.scheme == "crate" and not database:
-            database = url.query.get("schema")
-    return database, table
+            --output-path '{url_fullpath(url)}'
+        """.rstrip()
+        if format_ is DataFormat.LINE_PROTOCOL_COMPRESSED:
+            command += " --compress"
+        out = run_command(command)
+
+        stderr = out.stderr.decode("utf-8")
+
+        # Decode output of `influxd inspect export-lp`.
+        """
+        {"level":"info","ts":1712536769.359062,"caller":"export_lp/export_lp.go:219","msg":"exporting TSM files","tsm_dir":"var/lib/influxdb2/engine/data/372d1908eab801a6","file_count":3}
+        {"level":"info","ts":1712536769.3782709,"caller":"export_lp/export_lp.go:315","msg":"exporting WAL files","wal_dir":"var/lib/influxdb2/engine/wal/372d1908eab801a6","file_count":3}
+        {"level":"info","ts":1712536769.3783438,"caller":"export_lp/export_lp.go:204","msg":"export complete"}
+        """  # noqa: E501
+        if format_ in [DataFormat.LINE_PROTOCOL_UNCOMPRESSED, DataFormat.LINE_PROTOCOL_COMPRESSED]:
+            report = pd.read_json(path_or_buf=io.StringIO(stderr), lines=True).to_dict(orient="records")
+            tsm_file_count = report[0]["file_count"]
+            wal_file_count = report[1]["file_count"]
+            if tsm_file_count == 0 and wal_file_count == 0:
+                raise FileNotFoundError(r"Export yielded zero records. Make sure to use a valid bucket-id.")
+        else:
+            raise NotImplementedError(f"Format is not supported: {format_}")
+        if out.stdout:
+            sys.stdout.buffer.write(out.stdout)
+        return CommandResult(stderr=stderr, exitcode=out.returncode)
 
 
 class SqlAlchemyAdapter:
     """
     Adapter to talk to SQLAlchemy-compatible databases.
     """
 
     def __init__(self, url: t.Union[URL, str], progress: bool = False, debug: bool = False):
         self.progress = progress
 
         if isinstance(url, str):
             url: URL = URL(url)
 
-        self.database, self.table = decode_database_table(url)
+        self.database, self.table = SqlAlchemyAdapter.decode_database_table(url)
 
         # Special handling for SQLite and CrateDB databases.
         self.dburi = str(url.with_query(None))
         if url.scheme == "crate":
             url = url.with_path("")
             if self.database:
                 url = url.with_query({"schema": self.database})
@@ -256,17 +288,17 @@
 
         logger.info(f"SQLAlchemy DB URI: {self.dburi}")
 
     @classmethod
     def from_url(cls, url: t.Union[URL, str], **kwargs) -> "SqlAlchemyAdapter":
         return cls(url=url, **kwargs)
 
-    def write(self, source: t.Union[pd.DataFrame, InfluxDbAdapter]):
+    def write(self, source: t.Union[pd.DataFrame, InfluxDbApiAdapter]):
         logger.info("Loading dataframes into RDBMS/SQL database using pandas/Dask")
-        if isinstance(source, InfluxDbAdapter):
+        if isinstance(source, InfluxDbApiAdapter):
             for df in source.read_df():
                 dataframe_to_sql(df, dburi=self.dburi, tablename=self.table, progress=self.progress)
         elif isinstance(source, pd.DataFrame):
             dataframe_to_sql(source, dburi=self.dburi, tablename=self.table, progress=self.progress)
         else:
             raise NotImplementedError(f"Failed handling source: {source}")
 
@@ -301,7 +333,69 @@
         connection.set_isolation_level(psycopg2.extensions.ISOLATION_LEVEL_AUTOCOMMIT)
         cursor = connection.cursor()
         cursor.execute(sql)
         result = cursor.fetchall()
         cursor.close()
         connection.close()
         return result
+
+    @staticmethod
+    def decode_database_table(url: URL):
+        """
+        Decode database and table names from database URI path and/or query string.
+
+        Variants:
+
+            /<database>/<table>
+            ?database=<database>&table=<table>
+            ?schema=<database>&table=<table>
+        """
+        try:
+            database, table = url.path.strip("/").split("/")
+        except ValueError as ex:
+            if "too many values to unpack" not in str(ex) and "not enough values to unpack" not in str(ex):
+                raise
+            database = url.query.get("database")
+            table = url.query.get("table")
+            if url.scheme == "crate" and not database:
+                database = url.query.get("schema")
+        return database, table
+
+
+class FileAdapter:
+    """
+    Adapter for pipelining data in and out of files.
+    """
+
+    def __init__(self, url: t.Union[URL, str], progress: bool = False, debug: bool = False):
+        self.progress = progress
+
+        if isinstance(url, str):
+            url: URL = URL(url)
+
+        self.output = OutputFile.from_url(url)
+
+    @classmethod
+    def from_url(cls, url: t.Union[URL, str], **kwargs) -> "FileAdapter":
+        """
+        Factory to create a `FileAdapter` instance from a URL.
+        """
+        return cls(url=url, **kwargs)
+
+    def write(self, source: t.Union[pd.DataFrame, InfluxDbApiAdapter]):
+        """
+        Export data from a pandas DataFrame or from an API-connected InfluxDB database into lineprotocol format (ILP).
+        """
+        logger.info(f"Exporting dataframes in {self.output.format.value} format to {self.output.path}")
+        generators = []
+        if self.output.format is DataFormat.LINE_PROTOCOL_UNCOMPRESSED:
+            if isinstance(source, InfluxDbApiAdapter):
+                for df in source.read_df():
+                    generators.append(dataframe_to_lineprotocol(df, progress=self.progress))
+            elif isinstance(source, pd.DataFrame):
+                generators.append(dataframe_to_lineprotocol(source, progress=self.progress))
+            else:
+                raise NotImplementedError(f"Unknown data source: {source}")
+        else:
+            raise NotImplementedError(f"File output format not implemented: {self.output.format}")
+        for generator in generators:
+            print("\n".join(generator), file=self.output.stream)
```

### Comparing `influxio-0.1.2/influxio/testdata.py` & `influxio-0.2.0/influxio/testdata.py`

 * *Files identical despite different names*

### Comparing `influxio-0.1.2/influxio/util/cli.py` & `influxio-0.2.0/influxio/util/cli.py`

 * *Files identical despite different names*

### Comparing `influxio-0.1.2/influxio/util/report.py` & `influxio-0.2.0/influxio/util/report.py`

 * *Files identical despite different names*

### Comparing `influxio-0.1.2/influxio.egg-info/PKG-INFO` & `influxio-0.2.0/influxio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxio
-Version: 0.1.2
+Version: 0.2.0
 Summary: Import and export data into/from InfluxDB
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: changelog, https://github.com/daq-tools/influxio/blob/main/CHANGES.rst
 Project-URL: documentation, https://github.com/daq-tools/influxio
 Project-URL: homepage, https://github.com/daq-tools/influxio
 Project-URL: repository, https://github.com/daq-tools/influxio
@@ -48,129 +48,135 @@
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click<9
 Requires-Dist: colorama<1
 Requires-Dist: crate[sqlalchemy]
 Requires-Dist: cratedb-toolkit
-Requires-Dist: dask[dataframe]<=2024.3.1,>=2020
+Requires-Dist: dask[dataframe]>=2020
 Requires-Dist: importlib-metadata; python_version <= "3.9"
+Requires-Dist: influx-line==1.0.0
 Requires-Dist: influxdb-client[ciso]<2
 Requires-Dist: line-protocol-parser<2
 Requires-Dist: pandas<2.3
 Requires-Dist: psycopg2-binary<3
 Requires-Dist: pueblo>=0.0.7
 Requires-Dist: SQLAlchemy-Utils<0.42
 Requires-Dist: yarl<2
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: mypy==1.9.0; extra == "develop"
 Requires-Dist: poethepoet<0.26; extra == "develop"
 Requires-Dist: pyproject-fmt<1.8; extra == "develop"
-Requires-Dist: ruff==0.3.4; extra == "develop"
+Requires-Dist: ruff==0.3.5; extra == "develop"
 Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
 Requires-Dist: pytest<9; extra == "test"
-Requires-Dist: pytest-cov<5; extra == "test"
+Requires-Dist: pytest-cov<6; extra == "test"
 
 ########
 influxio
 ########
 
-.. image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
+.. start-badges
+
+|ci-tests| |ci-coverage| |license| |pypi-downloads|
+
+|python-versions| |status| |pypi-version|
+
+.. |ci-tests| image:: https://github.com/daq-tools/influxio/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/daq-tools/influxio/actions/workflows/tests.yml
     :alt: Build status
 
-.. image:: https://codecov.io/gh/daq-tools/influxio/branch/master/graph/badge.svg
+.. |ci-coverage| image:: https://codecov.io/gh/daq-tools/influxio/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/daq-tools/influxio
     :alt: Coverage
 
-.. image:: https://img.shields.io/pypi/v/influxio.svg
+.. |pypi-version| image:: https://img.shields.io/pypi/v/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: PyPI Version
 
-.. image:: https://img.shields.io/pypi/pyversions/influxio.svg
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Python Version
 
-.. image:: https://img.shields.io/pypi/dw/influxio.svg
-    :target: https://pypi.org/project/influxio/
-    :alt: PyPI Downloads
+.. |pypi-downloads| image:: https://static.pepy.tech/badge/influxio/month
+    :target: https://www.pepy.tech/projects/influxio
+    :alt: PyPI Downloads per month
 
-.. image:: https://img.shields.io/pypi/status/influxio.svg
+.. |status| image:: https://img.shields.io/pypi/status/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: Status
 
-.. image:: https://img.shields.io/pypi/l/influxio.svg
+.. |license| image:: https://img.shields.io/pypi/l/influxio.svg
     :target: https://pypi.org/project/influxio/
     :alt: License
 
+.. end-badges
+
 
 *****
 About
 *****
 
 You can use ``influxio`` to import and export data into/from InfluxDB.
 It can be used both as a standalone program, and as a library.
 
 ``influxio`` is, amongst others, based on the excellent `dask`_, `fsspec`_,
-`influxdb-client`_, `line-protocol-parser`_, `pandas`_, and `SQLAlchemy`_
-packages.
+`influxdb-client`_, `influx-line`_, `line-protocol-parser`_, `pandas`_,
+and `SQLAlchemy`_ packages.
 
 Please note that ``influxio`` is alpha-quality software, and a work in progress.
 Contributions of all kinds are very welcome, in order to make it more solid.
 Breaking changes should be expected until a 1.0 release, so version pinning
 is recommended, especially when you use it as a library.
 
-**Caveat**: Only a few features sketched out in the README have actually been
-implemented right now.
-
 
 ********
 Synopsis
 ********
 
-.. code-block:: sh
-
-    # Export from data directory to line protocol format.
-    influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
-        "file://export.lp"
+.. code-block:: shell
 
     # Export from API to database.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "sqlite://export.sqlite?table=demo"
 
+    # Export from data directory to line protocol format.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp"
+
 
 **********
 Quickstart
 **********
 
 If you are in a hurry, and want to run ``influxio`` without any installation,
 just use the OCI image on Podman or Docker.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive/demo"
 
 
 *****
 Setup
 *****
 
 Install ``influxio`` from PyPI.
 
-.. code-block:: sh
+.. code-block:: shell
 
     pip install influxio
 
 
 *****
 Usage
 *****
@@ -191,24 +197,24 @@
 
 Command line use
 ================
 
 Help
 ----
 
-.. code-block:: sh
+.. code-block:: shell
 
     influxio --help
     influxio info
     influxio copy --help
 
 Import
 ------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From test data to API.
     # Choose one of dummy, mixed, dateindex, wide.
     influxio copy \
         "testdata://dateindex/" \
         "http://example:token@localhost:8086/testdrive/demo"
 
@@ -218,86 +224,109 @@
         "http://example:token@localhost:8086/testdrive/demo"
 
     # With selected amount of rows and columns (only supported by certain test data sources).
     influxio copy \
         "testdata://wide/?rows=42&columns=42" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "file://tests/testdata/basic.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-    # From line protocol file to API.
+    # From line protocol file to InfluxDB API.
     influxio copy \
         "https://github.com/influxdata/influxdb2-sample-data/raw/master/air-sensor-data/air-sensor-data.lp" \
         "http://example:token@localhost:8086/testdrive/demo"
 
-Export
-------
+    # From line protocol file to any database supported by SQLAlchemy.
+    influxio copy \
+        "file://export.lp" \
+        "sqlite://export.sqlite?table=export"
+
+
+Export from API
+---------------
 
-.. code-block:: sh
+.. code-block:: shell
 
     # From API to database file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
-        "sqlite://export.sqlite?table=demo"
+        "sqlite:///export.sqlite?table=demo"
 
     # From API to database server.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "crate://crate@localhost:4200/testdrive?table=demo"
 
     # From API to line protocol file.
     influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "file://export.lp"
 
-    # From data directory to line protocol file.
+    # From API to line protocol on stdout.
+    influxio copy \
+        "http://example:token@localhost:8086/testdrive/demo" \
+        "file://-?format=lp"
+
+
+Export from data directory
+--------------------------
+
+.. code-block:: shell
+
+    # From InfluxDB data directory to line protocol file.
     influxio copy \
-        "file:///path/to/data/engine?org=example&bucket=testdrive&measurement=demo" \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
         "file://export.lp"
 
-    # From line protocol file to database.
+    # From InfluxDB data directory to line protocol file, compressed with gzip.
     influxio copy \
-        "file://export.lp" \
-        "sqlite://export.sqlite?table=export"
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        "file://export.lp.gz"
+
+    # From InfluxDB data directory to line protocol on stdout.
+    influxio copy \
+        "file:///path/to/influxdb/engine?bucket-id=372d1908eab801a6&measurement=demo" \
+        ""file://-?format=lp"
+
 
 OCI
 ---
 
 OCI images are available on the GitHub Container Registry (GHCR). In order to
 run them on Podman or Docker, invoke:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --network=host ghcr.io/daq-tools/influxio \
         influxio copy \
         "http://example:token@localhost:8086/testdrive/demo" \
         "stdout://export.lp"
 
 If you want to work with files on your filesystem, you will need to either
 mount the working directory into the container using the ``--volume`` option,
 or use the ``--interactive`` option to consume STDIN, like:
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker run --rm --volume=$(pwd):/data ghcr.io/daq-tools/influxio \
         influxio copy "file:///data/export.lp" "sqlite:///data/export.sqlite?table=export"
 
     cat export.lp | \
     docker run --rm --interactive --network=host ghcr.io/daq-tools/influxio \
         influxio copy "stdin://?format=lp" "crate://crate@localhost:4200/testdrive/export"
 
 In order to always run the latest ``nightly`` development version, and to use a
 shortcut for that, this section outlines how to use an alias for ``influxio``,
 and a variable for storing the input URL. It may be useful to save a few
 keystrokes on subsequent invocations.
 
-.. code-block:: sh
+.. code-block:: shell
 
     docker pull ghcr.io/daq-tools/influxio:nightly
     alias influxio="docker run --rm --interactive ghcr.io/daq-tools/influxio:nightly influxio"
     SOURCE=https://github.com/daq-tools/influxio/raw/main/tests/testdata/basic.lp
     TARGET=crate://crate@localhost:4200/testdrive/basic
 
     influxio copy "${SOURCE}" "${TARGET}"
@@ -321,14 +350,15 @@
 - `Outflux`_
 
 
 .. _dask: https://www.dask.org/
 .. _development: doc/development.rst
 .. _fsspec: https://pypi.org/project/fsspec/
 .. _influx: https://docs.influxdata.com/influxdb/latest/reference/cli/influx/
+.. _influx-line: https://github.com/functionoffunction/influx-line
 .. _influxd: https://docs.influxdata.com/influxdb/latest/reference/cli/influxd/
 .. _InfluxDB Fetcher: https://github.com/hgomez/influxdb
 .. _InfluxDB line protocol: https://docs.influxdata.com/influxdb/latest/reference/syntax/line-protocol/
 .. _influxdb-client: https://github.com/influxdata/influxdb-client-python
 .. _influxdb-write-to-postgresql: https://github.com/eras/influxdb-write-to-postgresql
 .. _line-protocol-parser: https://github.com/Penlect/line-protocol-parser
 .. _list of other projects: doc/prior-art.rst
```

### Comparing `influxio-0.1.2/influxio.egg-info/SOURCES.txt` & `influxio-0.2.0/influxio.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 doc/backlog.rst
 doc/development.rst
 influxio/__init__.py
+influxio/adapter.py
 influxio/cli.py
 influxio/core.py
 influxio/io.py
 influxio/model.py
 influxio/testdata.py
 influxio.egg-info/PKG-INFO
 influxio.egg-info/SOURCES.txt
```

### Comparing `influxio-0.1.2/pyproject.toml` & `influxio-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -76,40 +76,41 @@
   "version",
 ]
 dependencies = [
   "click<9",
   "colorama<1",
   "crate[sqlalchemy]",
   "cratedb-toolkit",
-  "dask[dataframe]>=2020,<=2024.3.1",
+  "dask[dataframe]>=2020",
   'importlib-metadata; python_version <= "3.9"',
+  "influx-line==1.0.0",
   "influxdb-client[ciso]<2",
   "line-protocol-parser<2",
   "pandas<2.3",
   "psycopg2-binary<3",
   "pueblo>=0.0.7",
   "SQLAlchemy-Utils<0.42",
   "yarl<2",
 ]
 [project.optional-dependencies]
 develop = [
   "black<25",
   "mypy==1.9.0",
   "poethepoet<0.26",
   "pyproject-fmt<1.8",
-  "ruff==0.3.4",
+  "ruff==0.3.5",
   "validate-pyproject<0.17",
 ]
 release = [
   "build<2",
   "twine<6",
 ]
 test = [
   "pytest<9",
-  "pytest-cov<5",
+  "pytest-cov<6",
 ]
 [project.urls]
 changelog = "https://github.com/daq-tools/influxio/blob/main/CHANGES.rst"
 documentation = "https://github.com/daq-tools/influxio"
 homepage = "https://github.com/daq-tools/influxio"
 repository = "https://github.com/daq-tools/influxio"
 [project.scripts]
@@ -151,15 +152,15 @@
   "examples",
   "slow",
 ]
 
 [tool.ruff]
 line-length = 120
 
-select = [
+lint.select = [
   # Bandit
   "S",
   # Bugbear
   "B",
   # Builtins
   "A",
   # comprehensions
@@ -179,26 +180,26 @@
   "W",
   # Pyflakes
   "F",
   # return
   "RET",
 ]
 
-extend-ignore = [
+lint.extend-ignore = [
   # zip() without an explicit strict= parameter
   "B905",
   # df is a bad variable name. Be kinder to your future self.
   "PD901",
   # Unnecessary variable assignment before `return` statement
   "RET504",
   # Unnecessary `elif` after `return` statement
   "RET505",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101"]  # Use of `assert` detected
 "influxio/util/report.py" = ["T201"]
 
 [tool.setuptools.packages.find]
 namespaces = false
 
 
@@ -212,20 +213,20 @@
   "lint",
   "test",
 ]
 
 format = [
   { cmd = "black ." },
   # Configure Ruff not to auto-fix (remove!) unused variables (F841) and `print` statements (T201).
-  { cmd = "ruff --fix --ignore=ERA --ignore=F401 --ignore=F841 --ignore=T20 ." },
+  { cmd = "ruff check --fix --ignore=ERA --ignore=F401 --ignore=F841 --ignore=T20 ." },
   { cmd = "pyproject-fmt --keep-full-version pyproject.toml" },
 ]
 
 lint = [
-  { cmd = "ruff ." },
+  { cmd = "ruff check ." },
   { cmd = "black --check ." },
   { cmd = "validate-pyproject pyproject.toml" },
   # { cmd = "mypy" },
 ]
 
 release = [
   { cmd = "python -m build" },
```

