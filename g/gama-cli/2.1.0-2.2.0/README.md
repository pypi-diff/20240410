# Comparing `tmp/gama_cli-2.1.0.tar.gz` & `tmp/gama_cli-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-2.1.0.tar", last modified: Mon Oct  9 10:18:53 2023, max compression
+gzip compressed data, was "gama_cli-2.2.0.tar", last modified: Wed Apr 10 12:27:42 2024, max compression
```

## Comparing `gama_cli-2.1.0.tar` & `gama_cli-2.2.0.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.503806 gama_cli-2.1.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     2468 2023-10-09 10:18:53.503806 gama_cli-2.1.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1656 2023-10-09 10:17:35.000000 gama_cli-2.1.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.499806 gama_cli-2.1.0/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2373 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.499806 gama_cli-2.1.0/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.503806 gama_cli-2.1.0/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      517 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       60 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      501 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.503806 gama_cli-2.1.0/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2353 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      109 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      517 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      935 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      276 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      417 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.variant.educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      429 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.variant.oracle_22.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      433 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.variant.oracle_2_2.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      520 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.variant.whiskey_bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1788 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.503806 gama_cli-2.1.0/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     7031 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2062 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    12313 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4345 2023-10-09 10:17:35.000000 gama_cli-2.1.0/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:53.503806 gama_cli-2.1.0/gama_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     2468 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1414 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       42 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-10-09 10:18:53.000000 gama_cli-2.1.0/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-10-09 10:18:26.000000 gama_cli-2.1.0/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      988 2023-10-09 10:18:53.503806 gama_cli-2.1.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-10-09 10:17:35.000000 gama_cli-2.1.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-10 12:27:42.628624 gama_cli-2.2.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1656 2024-04-10 12:26:35.000000 gama_cli-2.2.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2430 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.624623 gama_cli-2.2.0/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      402 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       60 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2397 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      109 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      517 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      247 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      296 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.armidale.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      290 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      299 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.oracle_22.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      387 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.oracle_2_2.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.variant.whiskey_bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1851 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      839 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      327 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      249 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6993 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2062 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    14953 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4345 2024-04-10 12:26:35.000000 gama_cli-2.2.0/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.628624 gama_cli-2.2.0/gama_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     2468 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1368 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       70 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2024-04-10 12:27:42.000000 gama_cli-2.2.0/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:28.000000 gama_cli-2.2.0/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1017 2024-04-10 12:27:42.628624 gama_cli-2.2.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 12:26:35.000000 gama_cli-2.2.0/setup.py
```

### Comparing `gama_cli-2.1.0/PKG-INFO` & `gama_cli-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 2.1.0
+Version: 2.2.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-2.1.0/README.md` & `gama_cli-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/banner.py` & `gama_cli-2.2.0/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/cli.py` & `gama_cli-2.2.0/gama_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         vessel.vessel.add_command(vessel.build)
         vessel.vessel.add_command(vessel.bake)
         vessel.vessel.add_command(vessel.test)
         vessel.vessel.add_command(vessel.type_generate)
         vessel.vessel.add_command(vessel.test_ui)
         vessel.vessel.add_command(vessel.test_e2e)
         vessel.vessel.add_command(vessel.test_ros)
+        vessel.vessel.add_command(vessel.test_scenarios)
 
         gs.gs.add_command(gs.build)
         gs.gs.add_command(gs.bake)
         gs.gs.add_command(gs.test)
 
     gama_cli()
```

### Comparing `gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,27 @@
       - ./projects/gama_ui/tsconfig.json:/app/tsconfig.json
       - ./projects/gama_ui/typings:/app/typings
       - ./projects/gama_ui/vite.config.ts:/app/vite.config.ts
       - ./projects/gama_ui/yarn.lock:/app/yarn.lock
     command: yarn dev
 
   gama_vessel:
-    entrypoint: ./scripts/watch.sh ./scripts/build.sh
     build:
       dockerfile: projects/gama_vessel/Dockerfile
       secrets:
         - apt_conf
         - API_TOKEN_GITHUB
     volumes:
+      - ./.secrets/apt.conf:/etc/apt/auth.conf.d/greenroom-robotics.conf
+      - ./log:/home/ros/.ros/log
       - ./projects/gama_ui/src/generated/ros:/home/ros/gama_vessel/generated/ros
       - ./projects/gama_vessel/src:/home/ros/gama_vessel/src
-      - ./projects/gama_vessel/scripts:/home/ros/gama_vessel/scripts
       - ./projects/gama_vessel/ros-ts-generator-config.json:/home/ros/gama_vessel/ros-ts-generator-config.json
       - ./data/frame_saver:/data/frame_saver
-      - ./log:/home/ros/log
+      # - ../missim/packages/missim_scenarios:/home/ros/gama_vessel/src/missim_scenarios
 
   gama_docs:
     build:
       context: ./
       dockerfile: projects/gama_docs/Dockerfile
     volumes:
       - ./projects/gama_docs/src:/app/src
```

### Comparing `gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml` & `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-2.2.0/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,18 @@
   gama_ui:
     container_name: gama_ui
     image: ghcr.io/greenroom-robotics/gama_ui:${GAMA_VERSION:-latest}
     ports:
       - "3000:3000"
       - "3100:3100"
     environment:
-      GAMA_VARIANT: $GAMA_VARIANT
-      GAMA_NAMESPACE_VESSEL: $GAMA_NAMESPACE_VESSEL
-      GAMA_NAMESPACE_GROUNDSTATION: $GAMA_NAMESPACE_GROUNDSTATION
+      GAMA_MODE: ${GAMA_MODE:-simulator}
+      GAMA_VARIANT: ${GAMA_VARIANT:-whiskey_bravo}
+      GAMA_NAMESPACE_VESSEL: ${GAMA_NAMESPACE_VESSEL:-vessel_1}
+      GAMA_NAMESPACE_GROUNDSTATION: ${GAMA_NAMESPACE_GROUNDSTATION:-vessel_1}
     networks:
       - vessel
 
   gama_chart_tiler:
     container_name: gama_chart_tiler
     image: ghcr.io/greenroom-robotics/gr_chart_tiler:1.1.0
     ports:
@@ -39,33 +40,34 @@
       - vessel
 
   gama_vessel:
     container_name: gama_vessel
     environment:
       - DISPLAY
       - ROS_DOMAIN_ID
+      - SCENARIO_TEST
+      - ROS_STATIC_PEERS
+      - GAMA_VESSEL_CONFIG
     ipc: host
     volumes:
-      - /dev/shm:/dev/shm
-      - ./log:/home/ros/.ros/log
-      - ~/.config/greenroom:/home/ros/.config/greenroom
-      - /tmp/.X11-unix:/tmp/.X11-unix:rw
       - /dev:/dev
+      - /tmp/.X11-unix:/tmp/.X11-unix:rw
     privileged: true
+    command: ${GAMA_VESSEL_COMMAND:-tail -f /dev/null}
 
   gama_greenstream:
     container_name: gama_greenstream
     image: ghcr.io/greenroom-robotics/gama_greenstream:${GAMA_VERSION:-latest}
     ipc: host
     volumes:
-      - /dev/shm:/dev/shm
-      - ~/.config/greenroom:/root/.config/greenroom
+      - /dev:/dev
     privileged: true
     environment:
       - ROS_DOMAIN_ID
+      - GAMA_VESSEL_CONFIG
 
   gama_docs:
     container_name: gama_docs
     image: ghcr.io/greenroom-robotics/gama_docs:${GAMA_VERSION:-latest}
     ports:
       - "3003:3000"
```

### Comparing `gama_cli-2.1.0/gama_cli/groups/attach.py` & `gama_cli-2.2.0/gama_cli/groups/attach.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/groups/gs.py` & `gama_cli-2.2.0/gama_cli/groups/gs.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Network,
     Mode,
     LogLevel,
     read_gs_config,
     GamaGsConfig,
     get_gs_config_path,
     write_gs_config,
+    serialise_gs_config,
 )
 from gama_cli.helpers import (
     docker_compose_path,
     get_project_root,
     docker_bake,
     maybe_ignore_build,
     maybe_ignore_prod,
@@ -22,31 +23,28 @@
 from python_on_whales.docker_client import DockerClient
 from python_on_whales.utils import ValidPath
 
 DOCKER_GS = docker_compose_path("./gs/docker-compose.yaml")
 DOCKER_GS_DEV = docker_compose_path("./gs/docker-compose.dev.yaml")
 DOCKER_GS_NETWORK_SHARED = docker_compose_path("./gs/docker-compose.network-shared.yaml")
 DOCKER_GS_NETWORK_HOST = docker_compose_path("./gs/docker-compose.network-host.yaml")
-DOCKER_GS_NETWORK_VPN = docker_compose_path("./gs/docker-compose.network-vpn.yaml")
 DOCKER_GS_WARTHOG_COMBO = docker_compose_path("./gs/docker-compose.warthog-combo.yaml")
 
 
 def _get_compose_files(
     mode: Optional[Mode] = None, network: Network = Network.SHARED, prod: bool = False
 ) -> List[ValidPath]:
     compose_files: List[ValidPath] = [DOCKER_GS]
 
     if not prod:
         compose_files.append(DOCKER_GS_DEV)
     if mode == Mode.WARTHOG_COMBO:
         compose_files.append(DOCKER_GS_WARTHOG_COMBO)
     if network == Network.SHARED:
         compose_files.append(DOCKER_GS_NETWORK_SHARED)
-    if network == Network.VPN:
-        compose_files.append(DOCKER_GS_NETWORK_VPN)
     if network == Network.HOST:
         compose_files.append(DOCKER_GS_NETWORK_HOST)
 
     return compose_files
 
 
 def log_config(config: GamaGsConfig):
@@ -76,15 +74,23 @@
 ):
     """Starts the ground-station"""
     dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
 
     config = read_gs_config()
     build = maybe_ignore_build(dev_mode, build)
     prod = maybe_ignore_prod(dev_mode, config.prod)
+
+    gama_gs_command = "platform ros launch gama_gs_bringup gs.launch.py"
+    if not prod:
+        gama_gs_command += " --watch --build"
+
+    os.environ["GAMA_GS_CONFIG"] = serialise_gs_config(config)
+    os.environ["GAMA_GS_COMMAND"] = gama_gs_command
     os.environ["ROS_DOMAIN_ID"] = str(config.ros_domain_id)
+    os.environ["ROS_STATIC_PEERS"] = str(config.static_peers)
 
     log_config(config)
 
     docker = DockerClient(
         compose_files=_get_compose_files(mode=config.mode, network=config.network, prod=prod),
         compose_project_directory=get_project_root(),
     )
@@ -151,41 +157,38 @@
     except Exception:
         config_current = GamaGsConfig()
 
     config = GamaGsConfig(
         ros_domain_id=click.prompt(
             "ROS Domain ID", type=int, default=config_current.ros_domain_id
         ),
+        static_peers=click.prompt(
+            "Static Peer IPs (';' separated)",
+            type=str,
+            default=config_current.static_peers,
+            value_proc=lambda x: x if len(x) else None,
+        ),
         namespace_vessel=click.prompt("Namespace Vessel", default=config_current.namespace_vessel),
         namespace_groundstation=click.prompt(
             "Namespace Groundstation", default=config_current.namespace_groundstation
         ),
         mode=click.prompt(
             "Mode", type=click.Choice([mode.value for mode in Mode]), default=config_current.mode
         ),
         network=click.prompt(
             "Network",
             type=click.Choice([network.value for network in Network]),
             default=config_current.network,
         ),
         prod=click.prompt("Prod", type=bool, default=config_current.prod),
-        remote_cmd_override=click.prompt(
-            "Remote Command Override", type=bool, default=config_current.remote_cmd_override
-        ),
         log_level=click.prompt(
             "Log Level",
             type=click.Choice([log_level.value for log_level in LogLevel]),
             default=config_current.log_level,
         ),
-        ddsrouter_vessel_ip=click.prompt(
-            "DDS Router Vessel IP", default=config_current.ddsrouter_vessel_ip
-        ),
-        ddsrouter_groundstation_ip=click.prompt(
-            "DDS Router Groundstation IP", default=config_current.ddsrouter_groundstation_ip
-        ),
     )
     write_gs_config(config)
 
 
 @click.command(name="build")
 def build():
     """Builds the ground-station"""
```

### Comparing `gama_cli-2.1.0/gama_cli/groups/misc.py` & `gama_cli-2.2.0/gama_cli/groups/misc.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/groups/setup.py` & `gama_cli-2.2.0/gama_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli/groups/vessel.py` & `gama_cli-2.2.0/gama_cli/groups/vessel.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import click
 
 from gama_config.gama_vessel import (
     Variant,
     Network,
     Mode,
     read_vessel_config,
+    serialise_vessel_config,
     get_vessel_config_path,
     LogLevel,
     write_vessel_config,
     GamaVesselConfig,
 )
 from gama_cli.helpers import (
     call,
@@ -25,15 +26,14 @@
 from python_on_whales.utils import ValidPath
 
 
 DOCKER_VESSEL = docker_compose_path("vessel/docker-compose.yaml")
 DOCKER_VESSEL_PROD = docker_compose_path("vessel/docker-compose.prod.yaml")
 DOCKER_VESSEL_DEV = docker_compose_path("vessel/docker-compose.dev.yaml")
 DOCKER_VESSEL_NETWORK_SHARED = docker_compose_path("vessel/docker-compose.network-shared.yaml")
-DOCKER_VESSEL_NETWORK_VPN = docker_compose_path("vessel/docker-compose.network-vpn.yaml")
 DOCKER_VESSEL_NETWORK_HOST = docker_compose_path("vessel/docker-compose.network-host.yaml")
 
 SERVICES = [
     "gama_ui",
     "gama_chart_tiler",
     "gama_chart_api",
     "gama_vessel",
@@ -53,16 +53,14 @@
 
     compose_files.append(
         docker_compose_path(f"vessel/docker-compose.variant.{variant.value}.yaml")
     )
 
     if network == Network.SHARED:
         compose_files.append(DOCKER_VESSEL_NETWORK_SHARED)
-    if network == Network.VPN:
-        compose_files.append(DOCKER_VESSEL_NETWORK_VPN)
     if network == Network.HOST:
         compose_files.append(DOCKER_VESSEL_NETWORK_HOST)
     if prod:
         compose_files.append(DOCKER_VESSEL_PROD)
 
     return compose_files
 
@@ -94,23 +92,24 @@
     docker = DockerClient(
         compose_files=_get_compose_files(
             variant=config.variant,
         ),
         compose_project_directory=get_project_root(),
     )
 
+    os.environ["GAMA_MODE"] = config.mode.value
     os.environ["GAMA_VARIANT"] = config.variant.value
     os.environ["GAMA_NAMESPACE_VESSEL"] = config.namespace_vessel
     os.environ["GAMA_NAMESPACE_GROUNDSTATION"] = config.namespace_groundstation
 
     if service:
         docker.compose.build([service])
         return
 
-    docker.compose.build(["gama_ui", "gama_chart_tiler", "gama_chart_api", "gama_vessel"])
+    docker.compose.build()
 
 
 @click.command(name="bake")
 @click.option(
     "--variant",
     type=click.Choice(Variant),  # type: ignore
     required=True,
@@ -156,15 +155,63 @@
     """Runs test for the ros nodes"""
     docker = DockerClient(
         compose_files=_get_compose_files(),
         compose_project_directory=get_project_root(),
     )
     docker.compose.run(
         "gama_vessel",
-        ["/bin/bash", "-c", "source /home/ros/.profile && platform ros test"],
+        ["platform", "ros", "test"],
+    )
+
+
+@click.command(name="test-scenarios")
+@click.option(
+    "--restart",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Should we restart the containers? Default: False",
+)
+@click.option(
+    "--sim-speed",
+    type=float,
+    default=25.0,
+    help="What speed should the scenarios be run at? Default: 25",
+)
+@click.argument("name", required=False, type=str)
+def test_scenarios(restart: bool, sim_speed: float, name: Optional[str]):
+    """Runs the scenario tests"""
+
+    if restart:
+        call("missim down")
+        call("gama vessel down")
+
+    call("missim up")
+    call("gama vessel up --scenario-test")
+
+    config = read_vessel_config()
+    log_config(config)
+
+    docker = DockerClient(
+        compose_files=_get_compose_files(
+            network=config.network,
+            variant=config.variant,
+            prod=False,
+        ),
+        compose_project_directory=get_project_root(),
+    )
+
+    docker.compose.execute(
+        "gama_vessel",
+        [
+            "bash",
+            "-l",
+            "-c",
+            f"SCENARIO_NAME='{name or ''}' SCENARIO_SIM_SPEED={sim_speed} python3 -m pytest ./src/gama_scenarios/gama_scenarios/test_scenarios_armidale.py -s -v",
+        ],
     )
 
 
 @click.command(name="test-e2e")
 def test_e2e():  # type: ignore
     """Runs UI e2e tests (assuming all the containers are up)"""
     call("cd ./projects/gama_ui && yarn test:e2e")
@@ -187,37 +234,56 @@
     )
     docker.compose.run("gama_ui", ["yarn", "lint", *args])
 
 
 @click.command(name="type-generate")
 def type_generate():  # type: ignore
     """Generates typescript types for all ros messages"""
+    config = read_vessel_config()
     docker = DockerClient(
-        compose_files=_get_compose_files(),
+        compose_files=_get_compose_files(
+            network=config.network, variant=config.variant, prod=False
+        ),
         compose_project_directory=get_project_root(),
     )
     docker.compose.run("gama_vessel", ["npx", "ros-typescript-generator"])
 
 
 @click.command(name="up")
 @click.option(
     "--build",
     type=bool,
     default=False,
     is_flag=True,
     help="Should we rebuild the docker containers? Default: False",
 )
+@click.option(
+    "--nowatch",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Should we prevent gama_vessel from watching for changes? Default: False",
+)
+@click.option(
+    "--scenario-test",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Are we starting GAMA for scenario tests? Default: False",
+)
 @click.argument(
     "service",
     required=False,
     type=click.Choice(SERVICES),
 )
 @click.argument("args", nargs=-1)
 def up(
     build: bool,
+    nowatch: bool,
+    scenario_test: bool,
     service: str,
     args: List[str],
 ):
     """Starts the vessel"""
     dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
 
     config = read_vessel_config()
@@ -230,19 +296,35 @@
             network=config.network,
             variant=config.variant,
             prod=prod,
         ),
         compose_project_directory=get_project_root(),
     )
 
+    gama_vessel_command_args = ""
+    if not prod:
+        gama_vessel_command_args += "--build"
+        if not nowatch:
+            gama_vessel_command_args += " --watch"
+
+    gama_vessel_command = f"platform ros run {gama_vessel_command_args} ros2 launch ./src/variants/{config.variant.value}_bringup/launch/vessel.launch.py"
+    if scenario_test:
+        gama_vessel_command = "platform ros build --watch"
+
+    os.environ["GAMA_VESSEL_CONFIG"] = serialise_vessel_config(config)
     os.environ["GAMA_VERSION"] = get_gama_version()
+    os.environ["GAMA_MODE"] = config.mode.value
     os.environ["GAMA_VARIANT"] = config.variant.value
     os.environ["GAMA_NAMESPACE_VESSEL"] = config.namespace_vessel
     os.environ["GAMA_NAMESPACE_GROUNDSTATION"] = config.namespace_groundstation
+    os.environ["GAMA_VESSEL_COMMAND"] = gama_vessel_command
+    os.environ["SCENARIO_TEST"] = "true" if scenario_test else "false"
     os.environ["ROS_DOMAIN_ID"] = str(config.ros_domain_id)
+    if config.static_peers:
+        os.environ["ROS_STATIC_PEERS"] = str(config.static_peers)
 
     services = (
         [service]
         if service
         else [
             "gama_ui",
             "gama_chart_tiler",
@@ -255,21 +337,14 @@
 
     docker.compose.up(
         services,
         detach=True,
         build=build,
     )
 
-    if config.extensions.lookout:
-        docker.compose.up(
-            ["lookout"],
-            detach=True,
-            build=build,
-        )
-
 
 @click.command(name="down")
 @click.argument("args", nargs=-1)
 def down(args: List[str]):  # type: ignore
     """Stops the vessel"""
     docker = DockerClient(
         compose_files=_get_compose_files(),
@@ -335,15 +410,22 @@
     help="The Network",
 )
 @click.option(
     "--prod",
     type=bool,
     help="Whether to run in production mode",
 )
-def configure(variant: Optional[Variant], mode: Optional[Mode], log_level: Optional[LogLevel], network: Optional[Network], prod: Optional[bool]):  # type: ignore
+@click.option(
+    "--ubiquity",
+    type=bool,
+    flag_value=True,
+    default=False,
+    help="Whether to run in ubiquity mode",
+)
+def configure(variant: Optional[Variant], mode: Optional[Mode], log_level: Optional[LogLevel], network: Optional[Network], prod: Optional[bool], ubiquity: bool):  # type: ignore
     """Configure GAMA Vessel"""
     # Prompt the user only if no arguments are passed
     prompt_user = all(v is None for v in [variant, mode, log_level, network, prod])
     if not prompt_user:
         config = GamaVesselConfig()
         if variant is not None:
             config.variant = variant
@@ -378,30 +460,42 @@
 
         config = GamaVesselConfig(
             ros_domain_id=click.prompt(
                 "ROS Domain ID",
                 default=config_current.ros_domain_id,
                 type=int,
             ),
+            static_peers=click.prompt(
+                "Static Peer IPs (';' separated)",
+                type=str,
+                default=config_current.static_peers,
+                value_proc=lambda x: x if len(x) else None,
+            ),
             namespace_vessel=click.prompt(
                 "Namespace Vessel",
                 default=config_current.namespace_vessel,
             ),
             namespace_groundstation=click.prompt(
                 "Namespace Groundstation",
                 default=config_current.namespace_groundstation,
             ),
             variant=click.prompt(
                 "Variant",
                 default=config_current.variant,
                 type=click.Choice([item.value for item in Variant]),
             ),
-            ubiquity_user=click.prompt("Ubiquity username", default=config_current.ubiquity_user),
-            ubiquity_pass=click.prompt("Ubiquity password", default=config_current.ubiquity_pass),
-            ubiquity_ip=click.prompt("Ubiquity ip", default=config_current.ubiquity_ip),
+            ubiquity_user=click.prompt("Ubiquity username", default=config_current.ubiquity_user)
+            if ubiquity
+            else None,
+            ubiquity_pass=click.prompt("Ubiquity password", default=config_current.ubiquity_pass)
+            if ubiquity
+            else None,
+            ubiquity_ip=click.prompt("Ubiquity ip", default=config_current.ubiquity_ip)
+            if ubiquity
+            else None,
             mode=click.prompt(
                 "Mode",
                 default=config_current.mode,
                 type=click.Choice([item.value for item in Mode]),
             ),
             prod=click.prompt("Prod", default=config_current.prod, type=bool),
             network=click.prompt(
```

### Comparing `gama_cli-2.1.0/gama_cli/helpers.py` & `gama_cli-2.2.0/gama_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `gama_cli-2.1.0/gama_cli.egg-info/PKG-INFO` & `gama_cli-2.2.0/gama_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama-cli
-Version: 2.1.0
+Name: gama_cli
+Version: 2.2.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-2.1.0/gama_cli.egg-info/SOURCES.txt` & `gama_cli-2.2.0/gama_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 gama_cli.egg-info/entry_points.txt
 gama_cli.egg-info/requires.txt
 gama_cli.egg-info/top_level.txt
 gama_cli.egg-info/zip-safe
 gama_cli/docker/gs/docker-compose.dev.yaml
 gama_cli/docker/gs/docker-compose.network-host.yaml
 gama_cli/docker/gs/docker-compose.network-shared.yaml
-gama_cli/docker/gs/docker-compose.network-vpn.yaml
 gama_cli/docker/gs/docker-compose.prod.yaml
 gama_cli/docker/gs/docker-compose.warthog-combo.yaml
 gama_cli/docker/gs/docker-compose.yaml
 gama_cli/docker/vessel/docker-compose.dev.yaml
 gama_cli/docker/vessel/docker-compose.network-host.yaml
 gama_cli/docker/vessel/docker-compose.network-shared.yaml
-gama_cli/docker/vessel/docker-compose.network-vpn.yaml
 gama_cli/docker/vessel/docker-compose.prod.yaml
+gama_cli/docker/vessel/docker-compose.variant.armidale.yaml
 gama_cli/docker/vessel/docker-compose.variant.educat.yaml
 gama_cli/docker/vessel/docker-compose.variant.oracle_22.yaml
 gama_cli/docker/vessel/docker-compose.variant.oracle_2_2.yaml
 gama_cli/docker/vessel/docker-compose.variant.whiskey_bravo.yaml
 gama_cli/docker/vessel/docker-compose.yaml
 gama_cli/groups/__init__.py
 gama_cli/groups/attach.py
```

### Comparing `gama_cli-2.1.0/setup.cfg` & `gama_cli-2.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_cli
-version = 2.1.0
+version = 2.2.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -37,12 +37,13 @@
 	**/*.py
 	**/**/*.yaml
 	**/**/*.yml
 
 [options.entry_points]
 console_scripts = 
 	gama = gama_cli.cli:cli
+	gama_cli = gama_cli.cli:cli
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

