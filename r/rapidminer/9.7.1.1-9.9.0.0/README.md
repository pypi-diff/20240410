# Comparing `tmp/rapidminer-9.7.1.1.tar.gz` & `tmp/rapidminer-9.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rapidminer-9.7.1.1.tar", last modified: Fri Jul  3 21:37:05 2020, max compression
+gzip compressed data, was "dist/rapidminer-9.9.0.0.tar", last modified: Fri Mar 19 16:41:39 2021, max compression
```

## Comparing `rapidminer-9.7.1.1.tar` & `rapidminer-9.9.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/
--rw-r--r--   0 hp         (501) staff       (20)    15323 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/PKG-INFO
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer/
--rw-r--r--   0 hp         (501) staff       (20)     1026 2020-07-03 21:23:04.000000 rapidminer-9.7.1.1/rapidminer/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer/core/
--rw-r--r--   0 hp         (501) staff       (20)      752 2020-05-31 12:46:10.000000 rapidminer-9.7.1.1/rapidminer/core/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5714 2020-05-31 12:46:10.000000 rapidminer-9.7.1.1/rapidminer/core/connector.py
--rw-r--r--   0 hp         (501) staff       (20)    14190 2020-07-03 21:22:43.000000 rapidminer-9.7.1.1/rapidminer/core/project.py
--rw-r--r--   0 hp         (501) staff       (20)     3418 2020-05-31 12:46:10.000000 rapidminer-9.7.1.1/rapidminer/core/resources.py
--rw-r--r--   0 hp         (501) staff       (20)     2141 2020-07-03 21:22:47.000000 rapidminer-9.7.1.1/rapidminer/core/scoring.py
--rw-r--r--   0 hp         (501) staff       (20)    14815 2020-06-23 12:21:24.000000 rapidminer-9.7.1.1/rapidminer/core/serdeutils.py
--rw-r--r--   0 hp         (501) staff       (20)    38837 2020-07-03 21:22:46.000000 rapidminer-9.7.1.1/rapidminer/core/server.py
--rw-r--r--   0 hp         (501) staff       (20)    22287 2020-07-03 21:22:45.000000 rapidminer-9.7.1.1/rapidminer/core/studio.py
--rw-r--r--   0 hp         (501) staff       (20)     4100 2020-06-23 12:21:24.000000 rapidminer-9.7.1.1/rapidminer/core/utilities.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)    15323 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      484 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2019-05-15 20:40:33.000000 rapidminer-9.7.1.1/rapidminer.egg-info/not-zip-safe
--rw-r--r--   0 hp         (501) staff       (20)       32 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)       11 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/rapidminer.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)       38 2020-07-03 21:37:05.000000 rapidminer-9.7.1.1/setup.cfg
--rw-r--r--   0 hp         (501) staff       (20)     2655 2020-07-03 21:24:24.000000 rapidminer-9.7.1.1/setup.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2021-03-19 16:41:39.805838 rapidminer-9.9.0.0/
+-rw-r--r--   0 hp         (501) staff       (20)    18257 2021-03-19 16:41:39.805517 rapidminer-9.9.0.0/PKG-INFO
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2021-03-19 16:41:39.797137 rapidminer-9.9.0.0/rapidminer/
+-rw-r--r--   0 hp         (501) staff       (20)     1068 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2021-03-19 16:41:39.804836 rapidminer-9.9.0.0/rapidminer/core/
+-rw-r--r--   0 hp         (501) staff       (20)      752 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/core/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)    14417 2021-03-19 16:21:37.000000 rapidminer-9.9.0.0/rapidminer/core/connections.py
+-rw-r--r--   0 hp         (501) staff       (20)     5714 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/core/connector.py
+-rw-r--r--   0 hp         (501) staff       (20)    16099 2021-03-19 16:21:33.000000 rapidminer-9.9.0.0/rapidminer/core/project.py
+-rw-r--r--   0 hp         (501) staff       (20)     3418 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/core/resources.py
+-rw-r--r--   0 hp         (501) staff       (20)     2141 2021-03-19 16:21:36.000000 rapidminer-9.9.0.0/rapidminer/core/scoring.py
+-rw-r--r--   0 hp         (501) staff       (20)    15229 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/core/serdeutils.py
+-rw-r--r--   0 hp         (501) staff       (20)    41663 2021-03-19 16:21:35.000000 rapidminer-9.9.0.0/rapidminer/core/server.py
+-rw-r--r--   0 hp         (501) staff       (20)    22287 2021-03-19 16:21:34.000000 rapidminer-9.9.0.0/rapidminer/core/studio.py
+-rw-r--r--   0 hp         (501) staff       (20)     3855 2021-03-19 15:41:34.000000 rapidminer-9.9.0.0/rapidminer/core/utilities.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2021-03-19 16:41:39.800351 rapidminer-9.9.0.0/rapidminer.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)    18257 2021-03-19 16:41:39.000000 rapidminer-9.9.0.0/rapidminer.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      515 2021-03-19 16:41:39.000000 rapidminer-9.9.0.0/rapidminer.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2021-03-19 16:41:39.000000 rapidminer-9.9.0.0/rapidminer.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2019-05-15 20:40:33.000000 rapidminer-9.9.0.0/rapidminer.egg-info/not-zip-safe
+-rw-r--r--   0 hp         (501) staff       (20)       40 2021-03-19 16:41:39.000000 rapidminer-9.9.0.0/rapidminer.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)       11 2021-03-19 16:41:39.000000 rapidminer-9.9.0.0/rapidminer.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)       38 2021-03-19 16:41:39.805945 rapidminer-9.9.0.0/setup.cfg
+-rw-r--r--   0 hp         (501) staff       (20)     2746 2021-03-19 16:17:31.000000 rapidminer-9.9.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rapidminer-9.7.1.1/PKG-INFO` & `rapidminer-9.9.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: rapidminer
-Version: 9.7.1.1
+Version: 9.9.0.0
 Summary: Tools for running RapidMiner processes and managing RapidMiner repositories.
 Home-page: https://github.com/rapidminer/python-rapidminer
 Author: RapidMiner
 License: AGPL
 Description: # RapidMiner Python package
         
-        This Python package allows you to interact with RapidMiner Studio and AI Hub. You can collaborate using the RapidMiner repository and leverage the scalable RapidMiner AI Hub infrastructure to run processes. This document shows examples on how to use the package. Additional notebook files provide more advanced examples. There is an API document for each classes: [Project](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Project.md), [Studio](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Studio.md), [Server](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Server.md), [Scoring](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Scoring.md). You can find the [changelog for the package here](CHANGES.md).
+        This Python package allows you to interact with RapidMiner Studio and AI Hub. You can collaborate using the RapidMiner repository and leverage the scalable RapidMiner AI Hub infrastructure to run processes. This document shows examples on how to use the package. Additional notebook files provide more advanced examples. There is an API document for each classes: [Project](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Project.md), [Studio](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Studio.md), [Server](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Server.md), [Connections](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Connections.md), [Scoring](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Scoring.md). You can find the [changelog for the package here](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/CHANGES.md).
         
         ## Table of contents
         
         - [Requirements](#requirements)
         - [Known current limitations](#known-current-limitations)
         - [Overview](#requirements)
         - [Installation](#installation)
         - [Project](#project)
+        - [Connections](#connections)
         - [Studio](#studio)
         - [Server](#server)
         - [Scoring](#scoring)
         
         ## Requirements
         
         * RapidMiner Studio *9.7.0* for Studio class
@@ -46,14 +47,17 @@
         Server class connects directly to a RapidMiner AI Hub instance without the need of a Studio installation. It is suitable in the following cases:
         * Collaborating with RapidMiner users, sharing data easily.
         * Calling, running, scheduling processes on the RapidMiner AI Hub platform from a local script.
         
         Project class is required to work with the git-based versioned repositories called projects. Projects can be shared using RapidMiner AI Hub. The shared data format allows Python coders and RapidMiner users to easily work on the same data. To summarize, this class is suitable in the following cases:
         * Using versioned projects to collaborate with RapidMiner users and share data easily.
         
+        Connections class can be used to access connections defined in a project. This way, Python coders can use the same external connections that are used by RapidMiner users. The connection fields are accessible, you only need an appropriate Python package to use those values.
+        * Using and sharing connections easily and securely without entering or storing any information redundantly.
+        
         ## Installation
         
         The library can be installed easily:
         
         - install in one step:
         
                 $ pip install rapidminer
@@ -81,31 +85,69 @@
         
         ```python
         df = project.read("data/mydata")
         ```
         
         The resulting `df` is a `pandas` `DataFrame` object, which you can use in the conventional way.
         
+        You can also directly read a file on an arbitrary local path by using a default Project class:
+        
+        ```python
+        df = rapidminer.Project().read("local/file/path.rmhdf5table")
+        ```
+        
         ##### Writing ExampleSet
         
         You can save any `pandas` `DataFrame` object to a project with the following command:
         
         ```python
         project.write(df, "data/mydata_modified")
         ```
         
         After writing the data set to the disk, you can use git commit and push to publish your changes to the remote project.
         
+        For more examples with projects, see the [Project examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/project_examples.ipynb).
+        
         ##### Running a process
         
         Use Studio or Server classes to run a process from a project, see examples below.
         
+        ## Connections
+        
+        Connections in RapidMiner allow you to access external systems like databases, cloud services, social media, etc. With the Connections class, you can reuse connections defined in RapidMiner in an easy and secure way. Access all connections in a project, by pointing to a local project folder:
+        
+        ```python
+        import rapidminer
+        connections = rapidminer.Connections("myproject", server=rapidminer.Server("https://myserver.mycompany.com:8080", username="myrmuser"))
+        ```
+        
+        Here, we already pointed to a [Server](#server) instance. That is only necessary if you have encrypted connection fields or use the AI Hub Vault to store certain sensitive values.
+        
+        It is also possible to use connections from an AI Hub repository. Assuming here that we have a [Server](#server) instance, you can retrieve the connections defined in its repository:
+        
+        ```python
+        connections = server.get_connections()
+        ```
+        
+        You can read the values of the connection fields by either using the connection name or an index. Use these field values to establish a connection using an appropriate Python package. The following code shows several different ways to access these values. Encryption or value injection (e.g. from AI Hub Vault) is handled transparently:
+        
+        ```python
+        myconn = connections["my_db_connection"]
+        mydb = myconn.values["database"]
+        myuser = myconn.user
+        mypass = connections[0].password
+        myhost = myconn.find_first("host")
+        myport = connections[0].values["port"]
+        ```
+        
+        Note when reading connections directly from an AI Hub repository, encrypted values are not available (values are None). You are advised to use AI Hub Vault for these values, or move those connections into projects.
+        
         ## Studio
         
-        You need to have a locally installed RapidMiner Studio instance to use this class. The only thing you need to provide is your installation path. Once that is specified, you can read from and write data or other objects to any configured repository. You can also run processes from files or from the repository. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/studio_examples.ipynb) and the [documentation of the `Studio` class](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Studio.md).
+        You need to have a locally installed RapidMiner Studio instance to use this class. The only thing you need to provide is your installation path. Once that is specified, you can read from and write data or other objects to any configured repository. You can also run processes from files or from the repository. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/studio_examples.ipynb) and the [documentation of the `Studio` class](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Studio.md).
         
         Note that each `Studio` method starts a Studio instance in the background and stops it when it is done. It is not recommended to run multiple instances in parallel, e.g. on different Notebook tabs. If you have several RapidMiner extensions installed, all of them will be loaded each time, that may lead to longer runtime. Provide multiple parameters to a read or write call, if possible, to avoid the startup overhead. 
         
         First you need a `Connector` object to interact with Studio. Once you have that, you can read and write data or run a process with a single line. To create a `Studio` `Connector` object, run the following code:
         
         ```python
         connector = rapidminer.Studio("/path/to/you/studio/installation")
@@ -138,19 +180,19 @@
         
         To run a process execute the following line:
         
         ```python
         df = connector.run_process("//Samples/processes/02_Preprocessing/01_Normalization")
         ```
         
-        You will get the results as `pandas` `DataFrames`. You can also define inputs, and many more. For more examples, see the [examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/studio_examples.ipynb)
+        You will get the results as `pandas` `DataFrames`. You can also define inputs, and many more. For more examples, see the [Studio examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/studio_examples.ipynb).
         
         ## Server
         
-        With `Server` class, you can directly connect to a local or remote RapidMiner AI Hub instance without the need for any local RapidMiner (Studio) installation. You can read data from and write data to the remote repository and you can execute processes using the scalable Job Agent architecture. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/server_examples.ipynb) and the [documentation of the `Server` class](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Server.md).
+        With `Server` class, you can directly connect to a local or remote RapidMiner AI Hub instance without the need for any local RapidMiner (Studio) installation. You can read data from and write data to the remote repository and you can execute processes using the scalable Job Agent architecture. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/server_examples.ipynb) and the [documentation of the `Server` class](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Server.md).
         
         ### Installation of Server API
         
         The `Server` class requires a web service backend to be installed on RapidMiner AI Hub. This is done automatically on the first instantiation of the Server class. The repository folder `/shared` is used by default to store the backend process. This folder exists and is accessible by anyone starting from RapidMiner Server 9.6.0.
         
         `Server` class instantiation can be fully automated (thus, no need for user input), if you specify `url`, `username` and `password` parameters.
         
@@ -198,15 +240,15 @@
         
         To run a process execute the following line:
         
         ```python
         df = connector.run_process("/home/myrmsuer/process/transform_data", inputs=df)
         ```
         
-        You will get the results as `pandas` `DataFrames`. You can also define multiple inputs, and other parameters. For more examples, see the [examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/server_examples.ipynb).
+        You will get the results as `pandas` `DataFrames`. You can also define multiple inputs, and other parameters. For more examples, see the [Server examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/server_examples.ipynb).
         
         You may want to run a process that resides in a versioned project. Note that in this case, inputs and outputs are not allowed, as the process can only directly read from the project and potentially write back using an automatic commit and push. To run the latest version of a process in project, use the following line:
         
         ```python
         df = connector.run_process("processes/myprocess", project="myproject")
         ```
         
@@ -215,14 +257,14 @@
         This class allows you to easily use a deployed [Real-Time Scoring](https://docs.rapidminer.com/server/scoring-agent/) service. You only need to provide the RapidMiner AI Hub url and the particular scoring service endpoint to create a class instance. After that, you can use the predict method to do scoring on a pandas DataFrame and get the result in a pandas DataFrame as well. For instructions on how to deploy Real-Time Scoring on RapidMiner AI Hub, please refer to its documentation.
         
         ```python
         sc = rapidminer.Scoring("http://myserver.mycompany.com:8090", "score-sales/score1")
         prediction = sc.predict(df)
         ```
         
-        where the scoring endpoint is at `"score-sales/score1"` that can be applied to the dataset `df`, and the resulting `prediction` is a `pandas` `DataFrame` object. You can find the `Scoring` class [documentation here](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Scoring.md).
+        where the scoring endpoint is at `"score-sales/score1"` that can be applied to the dataset `df`, and the resulting `prediction` is a `pandas` `DataFrame` object. You can find the `Scoring` class [documentation here](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Scoring.md).
         
         
         
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `rapidminer-9.7.1.1/rapidminer/__init__.py` & `rapidminer-9.9.0.0/rapidminer/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 #
 
-__version__ = "9.7.1.1"
+__version__ = "9.9.0.0"
 
 from .core.studio import Studio
 from .core.server import Server
 from .core.project import Project
 from .core.server import get_server
 from .core.scoring import Scoring
 from .core.resources import File
 from .core.resources import RepositoryLocation
+from .core.connections import Connections
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/__init__.py` & `rapidminer-9.9.0.0/rapidminer/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/connector.py` & `rapidminer-9.9.0.0/rapidminer/core/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/project.py` & `rapidminer-9.9.0.0/rapidminer/core/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
@@ -21,51 +21,55 @@
 import h5py
 from pathlib import Path
 from datetime import datetime
 from .serdeutils import set_metadata_without_warning
 from .utilities import ProjectException
 from .utilities import TooManyBinomialValuesError
 from .utilities import ValueConversionError
+from .connections import Connections
 
 
 
 def decode(x):
     if isinstance(x, str):
         return x
     return x.decode("utf-8")
 
 
 class Project():
     """
     Class for using a project from RapidMiner Server that has been cloned locally. Use git for cloning the repository, then read and write calls can work on local resources. You need to use git commands to push changes that you make locally.
     """
 
+    __NANOSECONDS_IN_A_DAY = 86400000000000
     _RM_HDF5_EXTENSION = ".rmhdf5table"
     _RM_RMP_EXTENSION = ".rmp"
     _METADATA_TYPES = {"NOMINAL": np.int8(1),
                        "INTEGER": np.int8(3),
                        "REAL": np.int8(4),
                        "TEXT": np.int8(5),
                        "BINOMINAL": np.int8(6),
                        "POLYNOMINAL": np.int8(7),
                        "FILE_PATH": np.int8(8),
                        "DATE_TIME": np.int8(9),
                        "DATE": np.int8(10),
                        "TIME": np.int8(11)}
-    _LEGACY_TYPES = ["TEXT", "BINOMINAL", "FILE_PATH", "DATE", "TIME"] # POLYNOMIAL handled separatly
+    _LEGACY_TYPES = ["TEXT", "BINOMINAL", "FILE_PATH", "DATE"] # POLYNOMIAL handled separatly
     _METADATA_ROLES = ["BATCH", "CLUSTER", "ID", "LABEL", "OUTLIER", "PREDICTION", "WEIGHT"]
 
+    __RM_MISSING_DATETIME_OR_TIME = 9223372036854775807 # constant value is coming from com.rapidminer.storage.hdf5.ExampleSetHdf5Writer.java#writeDateData/writeTimeData as of Long.MAX_VALUE/TimeColumn.MISSING_VALUE
+    __PANDAS_MISSING_DATE = pd.to_numeric(pd.Series([datetime.utcfromtimestamp(0), None]), downcast="integer")[1]
+
     def __init__(self, path="."):
         """
         Initializes a reference to a locally cloned project. You need to clone a project from RapidMiner Server first (e.g. via git commands) to be able to use the methods of this instance.
         
         :param path: path to the local project repository root folder. It can be a relative path from the current working directory or an absolute path, . The default value points to the working directory.
         """
         if not os.path.exists(path):
-            dirname = os.path.dirname(path)
             if path == "":
                 msg_dir_part = "in the current directory"
             else:
                 msg_dir_part = "at the specified path '%s'" % (os.path.dirname(path))
             raise ProjectException("Project '%s' does not exist %s. Please make sure you have a local copy of the project." % (os.path.basename(path), msg_dir_part))
         self.path = os.path.abspath(path)
 
@@ -91,43 +95,51 @@
         :param path: relative path inside the project (e.g. subfolder and file name) specifying the target location or an absolute path. The RapidMiner-specific HDF5 file extension is automatically added to the filename, if it is missing.
         """
         path = os.path.join(self.path, path)
         if len(Path(path).suffix) == 0:
             path = path + Project._RM_HDF5_EXTENSION
         Project.__write_data_safe(df, path)
 
+    def get_connections(self):
+        """
+        Returns the connection in that this project contains.
+        """
+        return Connections(self.path)
         
 #####################
 # Private functions #
 #####################
 
-    __from_ts = np.vectorize(datetime.utcfromtimestamp)
+    __from_ts_nanos = np.vectorize(lambda x: datetime.utcfromtimestamp(x/1e9) if x != Project.__RM_MISSING_DATETIME_OR_TIME else None)
+    __from_ts_seconds_and_nanos = np.vectorize(lambda x,y: datetime.utcfromtimestamp(x+y/1e9) if x != Project.__RM_MISSING_DATETIME_OR_TIME else None)
     __hyp5_string_dtype = h5py.string_dtype()
     __h5py_reference_dtype = h5py.special_dtype(ref=h5py.Reference)
     
     def __get_numerical(x, typestr):
         if typestr == 'Integer':
             # NaN values are not allowed in int64
             if not np.isnan(np.min(x[:])):
                 with x.astype('int64'):
                     return x[:]
             else:
                 return x
         elif typestr in ('Date-Time', 'Date'):
-            return Project.__from_ts(x[:])
+            return Project.__from_ts_seconds_and_nanos(x[:],0)
+        elif typestr == "Time":
+            return Project.__from_ts_nanos(x[:])
         else:
             return x
 
     def __get_data(f, x):
         r = f[x]
         mapping = r.attrs.get('dictionary')
         if "additional" in r.attrs and r.attrs.get("type") == "Date-Time":
             additional = r.attrs.get('additional')
             additional = f[additional]
-            return Project.__from_ts(r[:] + additional[:] / 1e9)
+            return Project.__from_ts_seconds_and_nanos(r[:], additional[:])
         if mapping is None:
             return Project.__get_numerical(r, decode(r.attrs.get('type')))
         if isinstance(mapping,h5py.Reference):
             mapping = f[mapping]
         mapping = mapping[1:]
         g = lambda x:x-1
         return pd.Categorical.from_codes(g(r[()]), [decode(s) if not isinstance(s, str) else s for s in mapping], ordered=False)
@@ -137,16 +149,18 @@
         Decides type based on the pandas DataFrame type, the explicit HDF5 type and whether there is a positive nominal type that indicates binominal.
         """
         if "legacy_type" in hdf_attrs:
             for k in Project._METADATA_TYPES.keys():
                 if Project._METADATA_TYPES[k] == hdf_attrs.get("legacy_type"):
                     return k.lower()
         hdf_type = decode(hdf_attrs.get("type"))
-        if hdf_type in ("Date-Time", "Date", "Time"):
+        if hdf_type in ("Date-Time", "Date"):
             meta_type = "date_time"
+        elif hdf_type == "Time":
+            meta_type = "time"
         elif df_kind_char in ('i', 'u'):
             meta_type = 'integer'
         elif df_kind_char in ('f'):
             meta_type = 'real'
         elif df_kind_char in ('M'):
             meta_type = 'date_time'
         elif df_kind_char in ('b') or "positive_index" in hdf_attrs:
@@ -207,42 +221,56 @@
 
     def __create_dataset(f, column, desired_type, index):
         shortname = 'a'+str(index)
         if desired_type in ["NOMINAL", "BINOMINAL", "POLYNOMINAL", "TEXT", "FILE_PATH"]:
             cat = column.astype("category").cat
             dset = f.create_dataset(shortname, data = pd.to_numeric(cat.codes.apply(lambda x:x+1), downcast='integer'))
             mappingname = 'd'+str(index)
-            mappingvals = cat.categories.values.astype(np.object)
+            mappingvals = cat.categories.values.astype(object)
             replacement = "NULL"
             while replacement in mappingvals:
                 replacement = "\x00" + replacement
-            mappingvals = np.concatenate([[replacement],mappingvals])
+            mappingvals = np.concatenate([[replacement], mappingvals])
             if desired_type == "BINOMINAL" and len(mappingvals) > 3:
                 raise TooManyBinomialValuesError("Column '%s' marked as binomial column in rm_metadata attribute, but has more there is more then two distinct values present.", )
             if len(mappingvals) <= 3:
                 dset.attrs["dictionary"] = [str(v) for v in mappingvals]
-                # positive index may change after read and write
-                dset.attrs['positive_index'] = np.int8(len(mappingvals) - 1)
+                if desired_type == "BINOMINAL":
+                    # positive index may change after read and write
+                    dset.attrs['positive_index'] = np.int8(len(mappingvals) - 1)
             else:
-                mset = f.create_dataset(mappingname, data=mappingvals, dtype=Project.__hyp5_string_dtype)
+                mset = f.create_dataset(mappingname, (len(mappingvals), ), dtype=Project.__hyp5_string_dtype)
+                try:
+                    mset[()] = mappingvals
+                except TypeError:
+                    # fixes error: TypeError: Can't implicitly convert non-string objects to strings (caused by some Python environments)
+                    mset[()] = [str(v) for v in mappingvals]
                 dset.attrs.create("dictionary", mset.ref, dtype=Project.__h5py_reference_dtype)
             dset.attrs['type'] = "Nominal"
         elif desired_type == "INTEGER":
             dset = f.create_dataset(shortname, data = column.astype("int64"))
             dset.attrs['type'] = "Integer"
         elif desired_type in ["DATE", "TIME", "DATE_TIME"]:
             if column.dtype.kind == "M":
-                nanoseconds = column.dt.tz_localize(None).astype("int64")
+                nanoseconds = pd.to_numeric(column.dt.tz_localize(None), downcast="integer")
+            else:
+                nanoseconds = pd.to_numeric(column, downcast="integer")
+            if desired_type == "TIME":
+                missing = nanoseconds==Project.__PANDAS_MISSING_DATE
+                nanoseconds.loc[missing] = Project.__RM_MISSING_DATETIME_OR_TIME
+                nanoseconds.loc[~missing] = nanoseconds.loc[~missing] % int(Project.__NANOSECONDS_IN_A_DAY)
+                dset = f.create_dataset(shortname, data = nanoseconds)
+                dset.attrs['type'] = "Time"
             else:
-                nanoseconds = column.astype("int64")
-            dset = f.create_dataset(shortname, data = nanoseconds // int(1e9))
-            additionalname = shortname+"a"
-            aset = f.create_dataset(additionalname, data = nanoseconds % int(1e9))
-            dset.attrs.create("additional", aset.ref, dtype=Project.__h5py_reference_dtype)
-            dset.attrs['type'] = "Date-Time"
+                seconds = nanoseconds.apply(lambda x: x // int(1e9) if x != Project.__PANDAS_MISSING_DATE else Project.__RM_MISSING_DATETIME_OR_TIME)
+                dset = f.create_dataset(shortname, data = seconds )
+                additionalname = shortname+"a"
+                aset = f.create_dataset(additionalname, data = (nanoseconds % int(1e9)).astype("int32"))
+                dset.attrs.create("additional", aset.ref, dtype=Project.__h5py_reference_dtype)
+                dset.attrs['type'] = "Date-Time"
         else:
             dset = f.create_dataset(shortname, data = column.astype("float64"))
             dset.attrs['type'] = "Real"
         return dset
 
     def __to_column_role(role):
         if role.startswith("confidence"):
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/resources.py` & `rapidminer-9.9.0.0/rapidminer/core/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/scoring.py` & `rapidminer-9.9.0.0/rapidminer/core/scoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/serdeutils.py` & `rapidminer-9.9.0.0/rapidminer/core/serdeutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
@@ -280,15 +280,15 @@
                 new_name = 'att'+str(name)
                 original_names[new_name] = name
             new_columns.append(new_name)
         dataframe.columns = new_columns
     return original_names
 
 # base64 encode all nominals and convert dates to epoch
-def convert_to_output_format(df, metadata):
+def convert_to_output_format(df, metadata, hdf5_compliant_date_and_time_conversion):
     def b64(x):
         if isinstance(x, basestring):
             return b64encode(x)
         # avoid lists, numpy array, etc. in isnull check
         elif not hasattr(x, "__len__") and pandas.isnull(x):
             return "null"
         return b64encode(str(x))
@@ -322,34 +322,39 @@
                         sample = df.loc[index, name].iloc[0]
                         if __is_integer_number(sample):
                             # // operator is necessary to keep type int in all python, pandas versions
                             df.loc[index, name] = df.loc[index,name]//1000
                         else:
                             df[name] = df[name].astype("object")
                             df.loc[index, name] = ((df.loc[index, name] - pandas.to_datetime(0, unit="ns")).dt.total_seconds()*1e6).round().astype("int64")
+                    if hdf5_compliant_date_and_time_conversion:
+                        if meta_type == "time":
+                            df[name] = df[name] % 86400000000
+                        elif meta_type == "date":
+                            df[name] = df[name] // 1e6 * 1e6
                 except ValueError:
                     raise DateConversionError("Error while serializing dataframe: some values in column '" + str(name) + "' are not valid dates.")
             elif __nominal_meta_type(meta_type):
                 df[name] = df[name].apply(b64)
     df.rm_converted_for_writing = True
 
 # writes the data and metadata to files
 # SIDE EFFECT: the method may modify the original data
-def write_example_set(data, output_csv, output_pmd):
+def write_example_set(data, output_csv, output_pmd, hdf5_compliant_date_and_time_conversion=False):
     original_names = rename_columns(data)
     # metadata
     metadata = get_metadata(data, original_names)
     write_file(output_pmd, "{\n")
     write_file(output_pmd, "  \"source\": \"RapidMiner Python Scripting Extension and Library\",\n")
     write_file(output_pmd, "  \"module\": \"Python\",\n")
     write_file(output_pmd, "  \"version\": \"" + __version__ + "\",\n")
     write_file(output_pmd, "  \"metadata\":\n" + json.dumps(metadata))
     write_file(output_pmd, "\n}")
     # data
-    convert_to_output_format(data, metadata)
+    convert_to_output_format(data, metadata, hdf5_compliant_date_and_time_conversion)
     data.to_csv(output_csv, encoding="utf-8", header=False, index=False)
 
 def set_metadata_without_warning(df, metadata):
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", UserWarning)
         df.rm_metadata = metadata
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/server.py` & `rapidminer-9.9.0.0/rapidminer/core/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
@@ -21,20 +21,22 @@
 import pandas as pd
 import getpass
 try:
     import cPickle as pickle
 except:
     import pickle
 from time import sleep
+from .connections import Connections
 from .connector import Connector
 from .utilities import ServerException
 from .utilities import GeneralException
 from .utilities import extract_json
 from .utilities import Version
 from .utilities import VersionException
+from .utilities import _is_docker_based_deployment
 from .resources import RepositoryLocation, ProjectLocation
 from .serdeutils import read_example_set, write_example_set, is_file_object
 from .project import Project
 from functools import partial
 import warnings
 import io
 import logging
@@ -132,14 +134,16 @@
         :param install: boolean. If set to false, web service installation step is completely skipped. Default value is True.
         :param verifySSL: either a boolean, in which case it controls whether we verify the server's TLS certificate, or a string, in which case it must be a path to a CA bundle to use. Default value is True.
         :param logger: a Logger object to use. By default a very simple logger is used, with INFO level, logging to stdout.
         :param loglevel: the loglevel, as an int value. Common values are defined in the standard logging module. Only used, if logger is not defined.
         """
         super(Server, self).__init__(logger, loglevel)
         # URL of the Rapidminer Server
+        if url.endswith("/"):
+            url = url[:-1]
         self.server_url = url
         if not _is_docker_based_deployment():
             # RapidMiner Server Username
             if username is None:
                 username = input('Username: ')
             self.username = username
             # RapidMiner Server Password
@@ -193,15 +197,15 @@
             this_project = project
             if isinstance(inp, RepositoryLocation):
                 inp = inp.to_string(with_prefix=False)
             elif isinstance(inp, ProjectLocation):
                 this_project = inp.project
                 inp = inp.path
             elif not isinstance(inp, str):
-                raise ServerException("Input path should be 'str' or 'rapidminer.RepositoryLocation object, not '" + str(type(inp)) + "'.")
+                raise ServerException("Input path should be 'str' or 'rapidminer.RepositoryLocation or 'rapidminer.ProjectLocation object, not '" + str(type(inp)) + "'.")
             if this_project:
                 resources.append(self.__read_project(this_project, inp))
             else:
                 resources.append(self.__read_repository(inp))
         if single_input:
             return resources[0]
         else:
@@ -339,28 +343,82 @@
         get_url = self.server_url + "/executions/queues?"
         r = self.__send_request(partial(requests.get, get_url),
                                 lambda s: "Failed to get queues, status: " + str(s))
         return r.json()
 
     def get_projects(self):
         """
-        Gets information of the available projects in the Server instance.
+        Gets information of the available projects in the AI Hub instance.
 
         :return: a JSON array of objects representing each repository with its properties
         """
         get_url = self.server_url + "/executions/repositories?"
         r = self.__send_request(partial(requests.get, get_url),
                                 lambda s: "Failed to get projects, status: " + str(s))
         return r.json()
+    
+    def get_connections(self):
+        """
+        Read the connections from the AI Hub repository.
+        
+        :return: Connections object listing connections from the AI Hub repository. Note that values of encrypted fields are not available (values will be None). Use AI Hub Vault to securely store and retrieve these values instead  
+        """
+        return Connections(path=None, server=self)
         
         
 #####################
 # Private functions #
 #####################
 
+    def _get_vault_info(self, location):
+        """
+        Load all server vault entries for a repository location.
+        
+        :param location: the location to read the vault information for. Note that there is a different syntax depending on the target repository type. For Projects, use git://reponame.git/Connections/My Connection.conninfo. For AI Hub repository, use /Connections/My Connection
+        """
+        if isinstance(location, ProjectLocation):
+            location = location.to_string(with_prefix=True)
+        elif not isinstance(location, str):
+            raise ServerException("Location must be a 'str' or 'rapidminer.ProjectLocation object, not '" + str(type(inp)) + "'.")
+        get_url = self.server_url + "/executions/connections/vault?location=" + location
+        r = self.__send_request(partial(requests.get, get_url),
+                                lambda s: "Failed to get vault info, status: " + str(s))
+        return r.json()
+
+    def _get_project_info(self, project_name):
+        """
+        Read the information for a project from AI Hub.
+        
+        :param project_name: specifies the project
+        :return: info in JSON format for the project
+        """
+        get_url = self.server_url + "/executions/repositories/" + project_name
+        r = self.__send_request(partial(requests.get, get_url),
+                                lambda s: "Failed to get project info" 
+                                + (": No project exists with the name '" + project_name + "', provide a valid project name" 
+                                   if s == 404 else ", status: " + str(s)))
+        return r.json()
+
+    def _get_connections_info(self):
+        """
+        Read the connections from the AI Hub repository.
+        
+        :return: connections in JSON format
+        """
+        get_url = self.server_url + "/api/rest/repository/connections"
+        r = self.__send_request(partial(requests.get, get_url),
+                                lambda s: "Failed to get connections list, status: " + str(s))
+        return r.json()
+
+    def _read_connection_info(self, location):
+        get_url = self.server_url + "/executions/connections/detail?location=" + location
+        r = self.__send_request(partial(requests.get, get_url),
+                                lambda s: "Failed to get connection details, status: " + str(s))
+        return r.json()
+
     def __username(self):
         if _is_docker_based_deployment():
             if "JUPYTERHUB_USER" in os.environ:
                 return os.environ["JUPYTERHUB_USER"]
             else:
                 raise ServerException("Internal exception: JUPYTERHUB_USER environment variable not set.")
         else:
@@ -662,15 +720,15 @@
                 elif ext == "pmd-encoded":
                     metadata = io.StringIO(content)
                 elif ext == "bin":
                     try:
                         obj = pickle.load(io.BytesIO(base64.b64decode(content)))
                     except Exception as exc:
                         raise GeneralException("Error while trying to load pickled object (note that Python 2 objects may not be readable): " + str(exc))
-                    resources.append(obj)
+                    return obj
                 elif ext == 'fo':
                     return io.BytesIO(base64.b64decode(content.encode("utf-8"))) # reads the file to memory
             except KeyError as e:
                 raise ServerException("The response from the server differs from the expected.") from e
         if csv_data is not None:
             if metadata is None:
                 raise ServerException("No metadata found.")
@@ -688,10 +746,7 @@
             # re-try with rmp file extension if it has not been specified
             if str(e).endswith("404") and len(Path(path).suffix) == 0:
                 r = self.__send_request(partial(requests.get, get_url + Project._RM_RMP_EXTENSION),
                                         lambda s: "Failed to find process at " + project + "/" + path + ", status: " + str(s))
             else:
                 raise e
         return r.text
-
-def _is_docker_based_deployment():
-    return all([var in os.environ for var in ["JUPYTERHUB_API_TOKEN", "JUPYTERHUB_API_URL", "JUPYTERHUB_USER"]])
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/studio.py` & `rapidminer-9.9.0.0/rapidminer/core/studio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
```

### Comparing `rapidminer-9.7.1.1/rapidminer/core/utilities.py` & `rapidminer-9.9.0.0/rapidminer/core/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License along with this program.
 # If not, see https://www.gnu.org/licenses/.
 #
 import os
 import sys
-import pkgutil
 
 if sys.version_info.major > 2:
     def __open__(file, mode):
         return open(file, mode, encoding="utf-8")
 else:
     raise GeneralException("Python 2 is not supported. Use Python 3.")
 
@@ -78,22 +77,14 @@
                 str += error["message"]
             if str == "":
                 str = "Unkown error: " + str(response)
             raise ServerException(str)
     return response
 
 
-def put_docker_notebook_start(path, template_type="long"):
-    if template_type not in ["short", "long"]:
-        raise ValueError("Template_type should be 'long' or 'short' (" + str(template_type) + " is provided).")
-    data = pkgutil.get_data(__name__, "notebooks/server_docker_start_" + template_type + ".ipynb")
-    with open(path, "wb") as outf:
-        outf.write(data)
-
-
 class Version:
     def __init__(self, version):
         v = version.split(".")
         # cut -BETA, -SNAPSHOT from last component, etc.
         [self.major, self.minor, self.patch] = [int(v[0]), int(v[1]), int(v[2].rsplit('-', 1)[0])]
  
     def is_at_least(self, other):
@@ -101,7 +92,10 @@
         otherlist = [other.major, other.minor, other.patch]
         for i in range(len(selflist)):
             if selflist[i] > otherlist[i]:
                 return True
             elif selflist[i] < otherlist[i]:
                 return False
         return True
+
+def _is_docker_based_deployment():
+    return all([var in os.environ for var in ["JUPYTERHUB_API_TOKEN", "JUPYTERHUB_API_URL", "JUPYTERHUB_USER"]])
```

### Comparing `rapidminer-9.7.1.1/rapidminer.egg-info/PKG-INFO` & `rapidminer-9.9.0.0/rapidminer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: rapidminer
-Version: 9.7.1.1
+Version: 9.9.0.0
 Summary: Tools for running RapidMiner processes and managing RapidMiner repositories.
 Home-page: https://github.com/rapidminer/python-rapidminer
 Author: RapidMiner
 License: AGPL
 Description: # RapidMiner Python package
         
-        This Python package allows you to interact with RapidMiner Studio and AI Hub. You can collaborate using the RapidMiner repository and leverage the scalable RapidMiner AI Hub infrastructure to run processes. This document shows examples on how to use the package. Additional notebook files provide more advanced examples. There is an API document for each classes: [Project](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Project.md), [Studio](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Studio.md), [Server](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Server.md), [Scoring](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Scoring.md). You can find the [changelog for the package here](CHANGES.md).
+        This Python package allows you to interact with RapidMiner Studio and AI Hub. You can collaborate using the RapidMiner repository and leverage the scalable RapidMiner AI Hub infrastructure to run processes. This document shows examples on how to use the package. Additional notebook files provide more advanced examples. There is an API document for each classes: [Project](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Project.md), [Studio](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Studio.md), [Server](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Server.md), [Connections](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Connections.md), [Scoring](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Scoring.md). You can find the [changelog for the package here](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/CHANGES.md).
         
         ## Table of contents
         
         - [Requirements](#requirements)
         - [Known current limitations](#known-current-limitations)
         - [Overview](#requirements)
         - [Installation](#installation)
         - [Project](#project)
+        - [Connections](#connections)
         - [Studio](#studio)
         - [Server](#server)
         - [Scoring](#scoring)
         
         ## Requirements
         
         * RapidMiner Studio *9.7.0* for Studio class
@@ -46,14 +47,17 @@
         Server class connects directly to a RapidMiner AI Hub instance without the need of a Studio installation. It is suitable in the following cases:
         * Collaborating with RapidMiner users, sharing data easily.
         * Calling, running, scheduling processes on the RapidMiner AI Hub platform from a local script.
         
         Project class is required to work with the git-based versioned repositories called projects. Projects can be shared using RapidMiner AI Hub. The shared data format allows Python coders and RapidMiner users to easily work on the same data. To summarize, this class is suitable in the following cases:
         * Using versioned projects to collaborate with RapidMiner users and share data easily.
         
+        Connections class can be used to access connections defined in a project. This way, Python coders can use the same external connections that are used by RapidMiner users. The connection fields are accessible, you only need an appropriate Python package to use those values.
+        * Using and sharing connections easily and securely without entering or storing any information redundantly.
+        
         ## Installation
         
         The library can be installed easily:
         
         - install in one step:
         
                 $ pip install rapidminer
@@ -81,31 +85,69 @@
         
         ```python
         df = project.read("data/mydata")
         ```
         
         The resulting `df` is a `pandas` `DataFrame` object, which you can use in the conventional way.
         
+        You can also directly read a file on an arbitrary local path by using a default Project class:
+        
+        ```python
+        df = rapidminer.Project().read("local/file/path.rmhdf5table")
+        ```
+        
         ##### Writing ExampleSet
         
         You can save any `pandas` `DataFrame` object to a project with the following command:
         
         ```python
         project.write(df, "data/mydata_modified")
         ```
         
         After writing the data set to the disk, you can use git commit and push to publish your changes to the remote project.
         
+        For more examples with projects, see the [Project examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/project_examples.ipynb).
+        
         ##### Running a process
         
         Use Studio or Server classes to run a process from a project, see examples below.
         
+        ## Connections
+        
+        Connections in RapidMiner allow you to access external systems like databases, cloud services, social media, etc. With the Connections class, you can reuse connections defined in RapidMiner in an easy and secure way. Access all connections in a project, by pointing to a local project folder:
+        
+        ```python
+        import rapidminer
+        connections = rapidminer.Connections("myproject", server=rapidminer.Server("https://myserver.mycompany.com:8080", username="myrmuser"))
+        ```
+        
+        Here, we already pointed to a [Server](#server) instance. That is only necessary if you have encrypted connection fields or use the AI Hub Vault to store certain sensitive values.
+        
+        It is also possible to use connections from an AI Hub repository. Assuming here that we have a [Server](#server) instance, you can retrieve the connections defined in its repository:
+        
+        ```python
+        connections = server.get_connections()
+        ```
+        
+        You can read the values of the connection fields by either using the connection name or an index. Use these field values to establish a connection using an appropriate Python package. The following code shows several different ways to access these values. Encryption or value injection (e.g. from AI Hub Vault) is handled transparently:
+        
+        ```python
+        myconn = connections["my_db_connection"]
+        mydb = myconn.values["database"]
+        myuser = myconn.user
+        mypass = connections[0].password
+        myhost = myconn.find_first("host")
+        myport = connections[0].values["port"]
+        ```
+        
+        Note when reading connections directly from an AI Hub repository, encrypted values are not available (values are None). You are advised to use AI Hub Vault for these values, or move those connections into projects.
+        
         ## Studio
         
-        You need to have a locally installed RapidMiner Studio instance to use this class. The only thing you need to provide is your installation path. Once that is specified, you can read from and write data or other objects to any configured repository. You can also run processes from files or from the repository. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/studio_examples.ipynb) and the [documentation of the `Studio` class](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Studio.md).
+        You need to have a locally installed RapidMiner Studio instance to use this class. The only thing you need to provide is your installation path. Once that is specified, you can read from and write data or other objects to any configured repository. You can also run processes from files or from the repository. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/studio_examples.ipynb) and the [documentation of the `Studio` class](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Studio.md).
         
         Note that each `Studio` method starts a Studio instance in the background and stops it when it is done. It is not recommended to run multiple instances in parallel, e.g. on different Notebook tabs. If you have several RapidMiner extensions installed, all of them will be loaded each time, that may lead to longer runtime. Provide multiple parameters to a read or write call, if possible, to avoid the startup overhead. 
         
         First you need a `Connector` object to interact with Studio. Once you have that, you can read and write data or run a process with a single line. To create a `Studio` `Connector` object, run the following code:
         
         ```python
         connector = rapidminer.Studio("/path/to/you/studio/installation")
@@ -138,19 +180,19 @@
         
         To run a process execute the following line:
         
         ```python
         df = connector.run_process("//Samples/processes/02_Preprocessing/01_Normalization")
         ```
         
-        You will get the results as `pandas` `DataFrames`. You can also define inputs, and many more. For more examples, see the [examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/studio_examples.ipynb)
+        You will get the results as `pandas` `DataFrames`. You can also define inputs, and many more. For more examples, see the [Studio examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/studio_examples.ipynb).
         
         ## Server
         
-        With `Server` class, you can directly connect to a local or remote RapidMiner AI Hub instance without the need for any local RapidMiner (Studio) installation. You can read data from and write data to the remote repository and you can execute processes using the scalable Job Agent architecture. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/server_examples.ipynb) and the [documentation of the `Server` class](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Server.md).
+        With `Server` class, you can directly connect to a local or remote RapidMiner AI Hub instance without the need for any local RapidMiner (Studio) installation. You can read data from and write data to the remote repository and you can execute processes using the scalable Job Agent architecture. In this section, we show you some examples on how to read and write repository data and run processes. For more advanced scenarios see the included [IPython notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/server_examples.ipynb) and the [documentation of the `Server` class](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Server.md).
         
         ### Installation of Server API
         
         The `Server` class requires a web service backend to be installed on RapidMiner AI Hub. This is done automatically on the first instantiation of the Server class. The repository folder `/shared` is used by default to store the backend process. This folder exists and is accessible by anyone starting from RapidMiner Server 9.6.0.
         
         `Server` class instantiation can be fully automated (thus, no need for user input), if you specify `url`, `username` and `password` parameters.
         
@@ -198,15 +240,15 @@
         
         To run a process execute the following line:
         
         ```python
         df = connector.run_process("/home/myrmsuer/process/transform_data", inputs=df)
         ```
         
-        You will get the results as `pandas` `DataFrames`. You can also define multiple inputs, and other parameters. For more examples, see the [examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/examples/server_examples.ipynb).
+        You will get the results as `pandas` `DataFrames`. You can also define multiple inputs, and other parameters. For more examples, see the [Server examples notebook](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/examples/server_examples.ipynb).
         
         You may want to run a process that resides in a versioned project. Note that in this case, inputs and outputs are not allowed, as the process can only directly read from the project and potentially write back using an automatic commit and push. To run the latest version of a process in project, use the following line:
         
         ```python
         df = connector.run_process("processes/myprocess", project="myproject")
         ```
         
@@ -215,14 +257,14 @@
         This class allows you to easily use a deployed [Real-Time Scoring](https://docs.rapidminer.com/server/scoring-agent/) service. You only need to provide the RapidMiner AI Hub url and the particular scoring service endpoint to create a class instance. After that, you can use the predict method to do scoring on a pandas DataFrame and get the result in a pandas DataFrame as well. For instructions on how to deploy Real-Time Scoring on RapidMiner AI Hub, please refer to its documentation.
         
         ```python
         sc = rapidminer.Scoring("http://myserver.mycompany.com:8090", "score-sales/score1")
         prediction = sc.predict(df)
         ```
         
-        where the scoring endpoint is at `"score-sales/score1"` that can be applied to the dataset `df`, and the resulting `prediction` is a `pandas` `DataFrame` object. You can find the `Scoring` class [documentation here](https://github.com/rapidminer/python-rapidminer/blob/9.7.1.1/docs/api/Scoring.md).
+        where the scoring endpoint is at `"score-sales/score1"` that can be applied to the dataset `df`, and the resulting `prediction` is a `pandas` `DataFrame` object. You can find the `Scoring` class [documentation here](https://github.com/rapidminer/python-rapidminer/blob/9.9.0.0/docs/api/Scoring.md).
         
         
         
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `rapidminer-9.7.1.1/setup.py` & `rapidminer-9.9.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of the RapidMiner Python package.
 #
-# Copyright (C) 2018-2020 RapidMiner GmbH
+# Copyright (C) 2018-2021 RapidMiner GmbH
 #
 # This program is free software: you can redistribute it and/or modify it under the terms of the
 # GNU Affero General Public License as published by the Free Software Foundation, either version 3
 # of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
@@ -15,15 +15,15 @@
 # If not, see https://www.gnu.org/licenses/.
 #
 from setuptools import setup, find_packages
 import os
 import codecs
 import re
 
-requirements = ["pandas", "requests", "numpy", "zeep", "h5py"]
+requirements = ["pandas>=1", "requests", "numpy", "zeep", "h5py", "tink"]
 name = "rapidminer"
 here = os.path.abspath(os.path.dirname(__file__))
 
 def read(*parts):
     with codecs.open(os.path.join(here, *parts), 'r') as fp:
         return fp.read()
 
@@ -45,25 +45,25 @@
         readme = read("README.md")
     except FileNotFoundError:
         # ignore
         pass
 
 # Replaces links to other markdown files with github links to make them work on PyPi
 github_baseurl = "https://github.com/rapidminer/python-rapidminer/blob/" + version + "/"
-for cname in "Studio.md", "Server.md", "Scoring.md", "Project.md":
+for cname in "Studio.md", "Server.md", "Scoring.md", "Project.md", "Connections.md":
     readme = readme.replace("docs/api/" + cname, github_baseurl + "docs/api/" + cname)
-for pyname in "studio_examples.ipynb", "server_examples.ipynb":
+for pyname in "studio_examples.ipynb", "server_examples.ipynb", "project_examples.ipynb":
     readme = readme.replace("examples/" + pyname, github_baseurl + "examples/" + pyname)
+readme = readme.replace("CHANGES.md", github_baseurl + "CHANGES.md")
     
 setup(name=name,
       version=version,
       description='Tools for running RapidMiner processes and managing RapidMiner repositories.',
       url='https://github.com/rapidminer/python-rapidminer',
       author='RapidMiner',
       license='AGPL',
       long_description=readme,
       long_description_content_type="text/markdown",
       packages=find_packages(),
-      include_package_data=True,
       zip_safe=False,
       install_requires=requirements,
       python_requires='>=3')
```

