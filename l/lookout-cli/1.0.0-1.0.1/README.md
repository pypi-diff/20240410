# Comparing `tmp/lookout_cli-1.0.0.tar.gz` & `tmp/lookout_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookout_cli-1.0.0.tar", last modified: Tue Apr  9 05:20:04 2024, max compression
+gzip compressed data, was "lookout_cli-1.0.1.tar", last modified: Tue Apr  9 23:21:50 2024, max compression
```

## Comparing `lookout_cli-1.0.0.tar` & `lookout_cli-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      700 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/lookout_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      424 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1102 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/lookout_cli/docker/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2649 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/docker/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      261 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/docker/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      221 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/docker/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      428 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/docker/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      946 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/docker/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/lookout_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     7935 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      832 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3604 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/lookout_cli/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/lookout_cli/test/lookout_cli_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/lookout_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      712 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       48 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       76 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-09 05:20:04.000000 lookout_cli-1.0.0/lookout_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-09 05:19:56.000000 lookout_cli-1.0.0/lookout_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      997 2024-04-09 05:20:04.673092 lookout_cli-1.0.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-09 05:18:46.000000 lookout_cli-1.0.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      700 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/lookout_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      424 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1102 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/lookout_cli/docker/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2649 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/docker/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      212 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/docker/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      221 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/docker/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      428 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/docker/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      990 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/docker/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/lookout_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     8509 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/groups/base.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      832 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3600 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/lookout_cli/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/lookout_cli/test/lookout_cli_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-09 23:21:50.314518 lookout_cli-1.0.1/lookout_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1511 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      712 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       48 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       76 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-09 23:21:50.000000 lookout_cli-1.0.1/lookout_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-09 23:21:38.000000 lookout_cli-1.0.1/lookout_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      997 2024-04-09 23:21:50.318518 lookout_cli-1.0.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-09 23:20:18.000000 lookout_cli-1.0.1/setup.py
```

### Comparing `lookout_cli-1.0.0/PKG-INFO` & `lookout_cli-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CLI for interacting with Lookout+
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_cli-1.0.0/README.md` & `lookout_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.0.0/lookout_cli/docker/docker-compose.dev.yaml` & `lookout_cli-1.0.1/lookout_cli/docker/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.0.0/lookout_cli/docker/docker-compose.yaml` & `lookout_cli-1.0.1/lookout_cli/docker/docker-compose.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 services:
   lookout_core:
     container_name: lookout_core
     image: ghcr.io/greenroom-robotics/lookout_core:${LOOKOUT_VERSION:-latest}
     volumes:
       - /dev:/dev
       - ~/.config/greenroom:/home/ros/.config/greenroom
+      - ~/lookout/rosbags:/home/ros/rosbags
     command: ${LOOKOUT_CORE_COMMAND:-tail -f /dev/null}
     privileged: true
     ipc: host
     pid: host
     environment:
       - ROS_DOMAIN_ID
```

### Comparing `lookout_cli-1.0.0/lookout_cli/groups/misc.py` & `lookout_cli-1.0.1/lookout_cli/groups/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,35 @@
 
 from python_on_whales.docker_client import DockerClient
 from python_on_whales.utils import ValidPath
 import lookout_config
 from lookout_config import LookoutConfig, LogLevel, Mode, Network
 import os
 
-DOCKER_GS = docker_compose_path("./docker-compose.yaml")
-DOCKER_GS_DEV = docker_compose_path("./docker-compose.dev.yaml")
+DOCKER = docker_compose_path("./docker-compose.yaml")
+DOCKER_DEV = docker_compose_path("./docker-compose.dev.yaml")
 DOCKER_NETWORK_SHARED = docker_compose_path("./docker-compose.network-shared.yaml")
 DOCKER_NETWORK_HOST = docker_compose_path("./docker-compose.network-host.yaml")
 DOCKER_GPU = docker_compose_path("./docker-compose.gpu.yaml")
 
+SERVICES = [
+    "lookout_core",
+    "lookout_ui",
+    "lookout_greenstream",
+    "lookout_docs",
+]
+
 
 def _get_compose_files(
     prod: bool = False, network: Network = Network.HOST, gpu=False
 ) -> List[ValidPath]:
-    compose_files: List[ValidPath] = [DOCKER_GS]
+    compose_files: List[ValidPath] = [DOCKER]
 
     if not prod:
-        compose_files.append(DOCKER_GS_DEV)
+        compose_files.append(DOCKER_DEV)
 
     if network == Network.SHARED:
         compose_files.append(DOCKER_NETWORK_SHARED)
 
     if network == Network.HOST:
         compose_files.append(DOCKER_NETWORK_HOST)
 
@@ -53,38 +60,52 @@
 @click.option(
     "--build",
     type=bool,
     default=False,
     is_flag=True,
     help="Should we rebuild the docker containers? Default: False",
 )
-@click.argument("args", nargs=-1)
+@click.option(
+    "--pull",
+    help="Should we do a docker pull",
+    is_flag=True,
+)
+@click.argument(
+    "services",
+    required=False,
+    nargs=-1,
+    type=click.Choice(SERVICES),
+)
 def up(
     build: bool,
-    args: List[str],
+    pull: bool,
+    services: List[str],
 ):
     """Starts lookout"""
     config = lookout_config.read()
+    version = get_version()
+    prod = version != "latest"
     log_config(config)
 
     os.environ["ROS_DOMAIN_ID"] = str(config.ros_domain_id)
     os.environ["LOOKOUT_NAMESPACE_VESSEL"] = config.namespace_vessel
+    os.environ["LOOKOUT_VERSION"] = version
     os.environ[
         "LOOKOUT_CORE_COMMAND"
     ] = "platform ros launch lookout_bringup lookout.launch.py --build --watch"
-    if not args:
-        services = ["lookout_docs", "lookout_core", "lookout_ui", "lookout_greenstream"]
-    else:
-        services = [arg for arg in args]
+
+    services_list = list(services) if services else None
 
     docker = DockerClient(
-        compose_files=_get_compose_files(False, config.network, config.gpu),
+        compose_files=_get_compose_files(prod, config.network, config.gpu),
         compose_project_directory=get_project_root(),
     )
-    docker.compose.up(services, detach=True, build=build)
+    docker.compose.up(
+        services_list, detach=True, build=build, pull="always" if pull else "missing"
+    )
 
     click.echo(click.style("UI started: http://localhost:4000", fg="green"))
 
 
 @click.command(name="down")
 @click.argument("args", nargs=-1)
 def down(args: List[str]):
@@ -101,25 +122,33 @@
 @click.option(
     "--no-cache",
     type=bool,
     default=False,
     is_flag=True,
     help="Should we rebuild without the docker cache?",
 )
-@click.argument("services", nargs=-1)
+@click.argument(
+    "services",
+    required=False,
+    nargs=-1,
+    type=click.Choice(SERVICES),
+)
 def build(no_cache: bool, services: List[str]):
     """Builds the Lookout docker containers"""
     config = lookout_config.read()
     os.environ["LOOKOUT_NAMESPACE_VESSEL"] = config.namespace_vessel
+    os.environ["GPU"] = "true" if config.gpu else "false"
 
     docker = DockerClient(
         compose_files=_get_compose_files(gpu=config.gpu),
         compose_project_directory=get_project_root(),
     )
-    docker.compose.build(services=services, cache=not no_cache)
+    services_list = list(services) if services else None
+
+    docker.compose.build(services=services_list, cache=not no_cache)
 
 
 @click.command(name="bake")
 @click.option(
     "--version",
     type=str,
     required=True,
@@ -128,15 +157,20 @@
 @click.option(
     "--push",
     type=bool,
     default=False,
     is_flag=True,
     help="Should we push the images to the registry? Default: False",
 )
-@click.argument("services", nargs=-1)
+@click.argument(
+    "services",
+    required=False,
+    nargs=-1,
+    type=click.Choice(SERVICES),
+)
 def bake(version: str, push: bool, services: List[str]):  # type: ignore
     """Bakes the docker containers"""
     compose_files = _get_compose_files()
     docker_bake(
         version=version,
         services=services,
         push=push,
```

### Comparing `lookout_cli-1.0.0/lookout_cli/groups/setup.py` & `lookout_cli-1.0.1/lookout_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `lookout_cli-1.0.0/lookout_cli/helpers.py` & `lookout_cli-1.0.1/lookout_cli/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,12 +106,9 @@
             " ".join(bake_args),
             " ".join(services_actual),
         ]
     )
 
     print("Running bake command: ", bake_command)
     subprocess.run(
-        bake_command,
-        shell=True,
-        check=True,
-        cwd=get_project_root(),
+        bake_command, shell=True, check=True, cwd=get_project_root(), env={"GPU": "true"}
     )
```

### Comparing `lookout_cli-1.0.0/lookout_cli.egg-info/PKG-INFO` & `lookout_cli-1.0.1/lookout_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: A CLI for interacting with Lookout+
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_cli-1.0.0/lookout_cli.egg-info/SOURCES.txt` & `lookout_cli-1.0.1/lookout_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 lookout_cli.egg-info/zip-safe
 lookout_cli/docker/docker-compose.dev.yaml
 lookout_cli/docker/docker-compose.gpu.yaml
 lookout_cli/docker/docker-compose.network-host.yaml
 lookout_cli/docker/docker-compose.network-shared.yaml
 lookout_cli/docker/docker-compose.yaml
 lookout_cli/groups/__init__.py
-lookout_cli/groups/misc.py
+lookout_cli/groups/base.py
 lookout_cli/groups/setup.py
 lookout_cli/test/lookout_cli_test.py
```

### Comparing `lookout_cli-1.0.0/setup.cfg` & `lookout_cli-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lookout_cli
-version = 1.0.0
+version = 1.0.1
 url = https://github.com/Greenroom-Robotics/lookout
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

