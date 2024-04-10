# Comparing `tmp/pih-auto-0.18.tar.gz` & `tmp/pih-auto-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-auto-0.18.tar", last modified: Fri Mar 29 03:55:05 2024, max compression
+gzip compressed data, was "pih-auto-0.19.tar", last modified: Wed Apr 10 01:31:28 2024, max compression
```

## Comparing `pih-auto-0.18.tar` & `pih-auto-0.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 03:55:06.061819 pih-auto-0.18/
-drwxrwxrwx   0        0        0        0 2024-03-29 03:55:05.622338 pih-auto-0.18/AutomationService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.18/AutomationService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.18/AutomationService/__main__.py
--rw-rw-rw-   0        0        0      559 2024-03-29 03:54:21.000000 pih-auto-0.18/AutomationService/const.py
--rw-rw-rw-   0        0        0    14739 2024-03-29 03:54:13.000000 pih-auto-0.18/AutomationService/service.py
--rw-rw-rw-   0        0        0      295 2024-03-29 03:55:06.029509 pih-auto-0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 03:55:05.997214 pih-auto-0.18/pih_auto.egg-info/
--rw-rw-rw-   0        0        0      295 2024-03-29 03:55:04.000000 pih-auto-0.18/pih_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-03-29 03:55:05.000000 pih-auto-0.18/pih_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 03:55:04.000000 pih-auto-0.18/pih_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-29 03:55:04.000000 pih-auto-0.18/pih_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-03-29 03:55:05.000000 pih-auto-0.18/pih_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-29 03:55:05.000000 pih-auto-0.18/pih_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 03:55:06.077445 pih-auto-0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 01:31:28.443618 pih-auto-0.19/
+drwxrwxrwx   0        0        0        0 2024-04-10 01:31:27.990510 pih-auto-0.19/AutomationService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.19/AutomationService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.19/AutomationService/__main__.py
+-rw-rw-rw-   0        0        0      559 2024-04-09 23:52:18.000000 pih-auto-0.19/AutomationService/const.py
+-rw-rw-rw-   0        0        0    14806 2024-04-09 22:56:43.000000 pih-auto-0.19/AutomationService/service.py
+-rw-rw-rw-   0        0        0      295 2024-04-10 01:31:28.396758 pih-auto-0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 01:31:28.365482 pih-auto-0.19/pih_auto.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 01:31:28.459228 pih-auto-0.19/setup.cfg
```

### Comparing `pih-auto-0.18/AutomationService/const.py` & `pih-auto-0.19/AutomationService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Automation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.18"
+VERSION: str = "0.19"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Automation service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="auto",
```

### Comparing `pih-auto-0.18/AutomationService/service.py` & `pih-auto-0.19/AutomationService/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,16 @@
         PolibasePerson,
         ResourceStatus,
         EmailInformation,
         ChillerIndicationsValueContainer,
     )
     from pih.collections.service import SubscribtionResult
 
-
-
     class DH:
-        resource_problem_status_map: dict[str, ProblemState] = defaultdict()
+        resource_problem_status_map: dict[str, ProblemState] = defaultdict(ProblemState)
         hr_user: str | None = None
 
     def get_resource_status_address(resource_status: ResourceStatus) -> str:
         resource_status_address: str = resource_status.address # type: ignore
         address_list: list[str] = [
             A.CT_R_D.VPN_PACS_SPB.address,
             A.CT_R_D.PACS_SPB.address,
@@ -276,18 +274,19 @@
                         params=params,
                     )
 
                 if event == A.E_B.action_was_done():
                     action_data: ActionWasDone = A.D_Ex_E.action(event_parameters)
                     action: A.CT_ACT = action_data.action
                     PIHThread(
-                        lambda: A.R_F.execute(
+                        lambda: print(A.R_F.execute(
                             "@on_action",
                             {"action": action, "action_data": action_data, "pl" : pl},
-                        )
+                            stdout_redirect = True
+                        ))
                     )
                     return
         return True
 
     def send_message_to_control_service(
         value: str, on_workstation: bool = False
     ) -> None:
```

