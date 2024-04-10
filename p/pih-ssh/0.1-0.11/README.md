# Comparing `tmp/pih-ssh-0.1.tar.gz` & `tmp/pih-ssh-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ssh-0.1.tar", last modified: Mon Feb 26 10:13:42 2024, max compression
+gzip compressed data, was "pih-ssh-0.11.tar", last modified: Wed Apr 10 02:30:16 2024, max compression
```

## Comparing `pih-ssh-0.1.tar` & `pih-ssh-0.11.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 10:13:42.468864 pih-ssh-0.1/
--rw-rw-rw-   0        0        0      241 2024-02-26 10:13:42.968841 pih-ssh-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 10:13:42.531355 pih-ssh-0.1/SSHService/
--rw-rw-rw-   0        0        0        0 2022-07-23 04:31:56.000000 pih-ssh-0.1/SSHService/__init__.py
--rw-rw-rw-   0        0        0      145 2024-02-14 10:50:22.000000 pih-ssh-0.1/SSHService/__main__.py
--rw-rw-rw-   0        0        0     4108 2024-02-25 01:07:12.000000 pih-ssh-0.1/SSHService/api.py
--rw-rw-rw-   0        0        0      343 2023-08-05 09:47:04.000000 pih-ssh-0.1/SSHService/api_test.py
--rw-rw-rw-   0        0        0     1030 2024-02-26 10:13:28.000000 pih-ssh-0.1/SSHService/const.py
--rw-rw-rw-   0        0        0     2638 2024-02-17 15:29:43.000000 pih-ssh-0.1/SSHService/service.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:13:42.718848 pih-ssh-0.1/pih_ssh.egg-info/
--rw-rw-rw-   0        0        0      241 2024-02-26 10:13:41.000000 pih-ssh-0.1/pih_ssh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-02-26 10:13:42.000000 pih-ssh-0.1/pih_ssh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 10:13:41.000000 pih-ssh-0.1/pih_ssh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-02-26 10:13:41.000000 pih-ssh-0.1/pih_ssh.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-02-26 10:13:41.000000 pih-ssh-0.1/pih_ssh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-26 10:13:41.000000 pih-ssh-0.1/pih_ssh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 10:13:42.968841 pih-ssh-0.1/setup.cfg
--rw-rw-rw-   0        0        0       90 2024-02-15 06:33:54.000000 pih-ssh-0.1/ssh_build.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:30:17.018956 pih-ssh-0.11/
+-rw-rw-rw-   0        0        0      288 2024-04-10 02:30:16.972063 pih-ssh-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 02:30:16.592923 pih-ssh-0.11/SSHService/
+-rw-rw-rw-   0        0        0        0 2022-07-23 04:31:56.000000 pih-ssh-0.11/SSHService/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-02-14 10:50:22.000000 pih-ssh-0.11/SSHService/__main__.py
+-rw-rw-rw-   0        0        0     4108 2024-02-25 01:07:12.000000 pih-ssh-0.11/SSHService/api.py
+-rw-rw-rw-   0        0        0      343 2023-08-05 09:47:04.000000 pih-ssh-0.11/SSHService/api_test.py
+-rw-rw-rw-   0        0        0     1031 2024-04-10 01:18:16.000000 pih-ssh-0.11/SSHService/const.py
+-rw-rw-rw-   0        0        0     2632 2024-04-10 00:54:37.000000 pih-ssh-0.11/SSHService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:30:16.923126 pih-ssh-0.11/pih_ssh.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 02:30:16.000000 pih-ssh-0.11/pih_ssh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:30:17.018956 pih-ssh-0.11/setup.cfg
```

### Comparing `pih-ssh-0.1/SSHService/api.py` & `pih-ssh-0.11/SSHService/api.py`

 * *Files identical despite different names*

### Comparing `pih-ssh-0.1/SSHService/const.py` & `pih-ssh-0.11/SSHService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.ssh_hosts import SSHHosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "SSH"
 
 HOST = A.CT_H.BACKUP_WORKER
 
-VERSION: str ="0.1"
+VERSION: str ="0.11"
 
 PACKAGES: tuple[str, ...] = ("paramiko",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="SSH service",
     host=HOST.NAME,
```

### Comparing `pih-ssh-0.1/SSHService/service.py` & `pih-ssh-0.11/SSHService/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import ipih
 
 from pih import A
 from SSHService.const import SD
 
-# version 1.0
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
     if A.U.for_service(SD, as_standalone=as_standalone):
-        from typing import Any
-        from pih.tools import ParameterList, js, j, escs
+        
         from SSHService.api import SSHApi as Api
+        from pih.tools import ParameterList, js, j, escs
+        
+        from typing import Any
 
         api: Api = Api()
 
         def service_call_handler(sc: SC, pl: ParameterList) -> Any:
             if sc == SC.mount_facade_for_linux_host:
                 host: str = pl.next()
                 api.execute_command(
                     js(("mkdir", A.PTH.FACADE.LINUX_MOUNT_POINT_PATH)), host, use_sudo=True
                 )
                 api.execute_command(
                     js(
                         (
                             "mount -t cifs",
-                            escs(A.PTH.adapt_for_windows(A.PTH.FACADE.STORAGE_PATH())),
+                            escs(A.PTH.for_windows(A.PTH.FACADE.STORAGE())),
                             A.PTH.FACADE.LINUX_MOUNT_POINT_PATH,
                             j(
                                 (
                                     "-o username=",
                                     A.D_V.value(A.CT_LNK.ADMINISTRATOR_LOGIN, True),
                                     ",",
                                     "password=",
```

