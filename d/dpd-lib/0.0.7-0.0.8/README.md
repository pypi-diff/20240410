# Comparing `tmp/dpd_lib-0.0.7.tar.gz` & `tmp/dpd_lib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.0.7.tar", last modified: Mon Apr  8 23:42:24 2024, max compression
+gzip compressed data, was "dpd_lib-0.0.8.tar", last modified: Tue Apr  9 23:49:38 2024, max compression
```

## Comparing `dpd_lib-0.0.7.tar` & `dpd_lib-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 23:42:24.981812 dpd_lib-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 23:42:24.981812 dpd_lib-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/PYPI.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 23:42:24.977812 dpd_lib-0.0.7/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 23:42:17.000000 dpd_lib-0.0.7/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 23:42:24.981812 dpd_lib-0.0.7/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 23:42:17.000000 dpd_lib-0.0.7/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5713 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 23:42:24.981812 dpd_lib-0.0.7/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 23:42:24.000000 dpd_lib-0.0.7/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-08 23:42:24.000000 dpd_lib-0.0.7/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 23:42:24.000000 dpd_lib-0.0.7/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-08 23:42:24.000000 dpd_lib-0.0.7/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 23:42:24.000000 dpd_lib-0.0.7/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      968 2024-04-08 23:41:43.000000 dpd_lib-0.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 23:42:24.981812 dpd_lib-0.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/PYPI.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 23:49:31.000000 dpd_lib-0.0.8/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 23:49:31.000000 dpd_lib-0.0.8/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5895 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-09 23:49:38.000000 dpd_lib-0.0.8/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-09 23:49:38.000000 dpd_lib-0.0.8/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 23:49:38.000000 dpd_lib-0.0.8/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-09 23:49:38.000000 dpd_lib-0.0.8/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 23:49:38.000000 dpd_lib-0.0.8/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-09 23:49:30.000000 dpd_lib-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 23:49:38.510970 dpd_lib-0.0.8/setup.cfg
```

### Comparing `dpd_lib-0.0.7/PKG-INFO` & `dpd_lib-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: influxdb-client
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: pydantic_settings
 Requires-Dist: uvicorn
 Requires-Dist: datetime
 Requires-Dist: loguru
+Requires-Dist: httpx
 
 # Derived Project Database Library
 
 ## Overview
 
 This libary contains several functions that enable the processing, storage, and retrieve of seismic and infrasound signal data. The underlying storage mechanism that sits under each respective component is an [InfluxDB](https://docs.influxdata.com/influxdb/v2/) database that we call the Derived Product Database (DPD).
```

### Comparing `dpd_lib-0.0.7/PYPI.md` & `dpd_lib-0.0.8/PYPI.md`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.7/dpd_lib/client/influx.py` & `dpd_lib-0.0.8/dpd_lib/client/influx.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,36 +60,42 @@
         self,
         type: str = "",
         stations: List[str] = [],
         t0: datetime = datetime.now(timezone.utc) - timedelta(seconds=15),
         t1: datetime = datetime.now(timezone.utc),
     ) -> List[InfluxInfrasoundRecord]:
         """
-        Reads a infrasound record given a type and timestamp
+        Reads infrasound records for a given type, station list, and timestamp
 
         Arguments:
             type (str): The type of infrasound record
             station (List(str)): The station of infrasound record
             t0 (datetime): the beginning of the timerange
             t1 (datetime): The end of the timerange
 
         Returns:
             res(List[InfluxInfrasoundRecord]): All records of a
             certain type for a given range.
         """
         query = """from(bucket:"{0}")
-        |> range(start: {1}, stop: {2})
-        |> filter(fn:(r) => r._measurement == "{3}")
-        |> filter(fn:(r) => contains(value: r.station, set: {4}))""".format(
+        |> range(start: {1}, stop: {2})""".format(
             self.bucket,
             t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
             t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
-            type,
-            json.dumps(stations),
         )
+        if type != "":
+            query += '|> filter(fn:(r) => r._measurement == "{0}")'.format(
+                type
+            )
+        if len(stations) != 0:
+            query += """
+            |> filter(fn:(r) => contains(value: r.station, set: {0}))
+            """.format(
+                json.dumps(stations)
+            )
         return await self._query(query)
 
     async def list_infrasound(
         self,
         t0: datetime = datetime.now(timezone.utc) - timedelta(seconds=15),
         t1: datetime = datetime.now(timezone.utc),
     ) -> List[InfluxInfrasoundRecord]:
```

### Comparing `dpd_lib-0.0.7/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.0.8/dpd_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: influxdb-client
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: pydantic_settings
 Requires-Dist: uvicorn
 Requires-Dist: datetime
 Requires-Dist: loguru
+Requires-Dist: httpx
 
 # Derived Project Database Library
 
 ## Overview
 
 This libary contains several functions that enable the processing, storage, and retrieve of seismic and infrasound signal data. The underlying storage mechanism that sits under each respective component is an [InfluxDB](https://docs.influxdata.com/influxdb/v2/) database that we call the Derived Product Database (DPD).
```

### Comparing `dpd_lib-0.0.7/pyproject.toml` & `dpd_lib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "PYPI.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
@@ -24,14 +24,15 @@
   "influxdb-client",
   "fastapi",
   "pydantic",
   "pydantic_settings",
   "uvicorn",
   "datetime",
   "loguru",
+  "httpx",
 ]
 
 [tool.setuptools.packages.find]
 include = ["dpd_lib*"]
 exclude = ["dpd_agent*", "dpd_service*", "docs*", "tests*"]
 
 [project.urls]
```

