# Comparing `tmp/pytest_container-0.4.1.tar.gz` & `tmp/pytest_container-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_container-0.4.1.tar", max compression
+gzip compressed data, was "pytest_container-0.4.2.tar", max compression
```

## Comparing `pytest_container-0.4.1.tar` & `pytest_container-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26529 2024-04-03 11:39:43.392852 pytest_container-0.4.1/LICENSE
--rw-r--r--   0        0        0     3098 2024-04-03 11:39:43.392852 pytest_container-0.4.1/README.rst
--rw-r--r--   0        0        0     2075 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      946 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/__init__.py
--rw-r--r--   0        0        0    10564 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/build.py
--rw-r--r--   0        0        0    42407 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/container.py
--rw-r--r--   0        0        0     5725 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/helpers.py
--rw-r--r--   0        0        0     8932 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/inspect.py
--rw-r--r--   0        0        0      362 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/logging.py
--rw-r--r--   0        0        0     7754 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/plugin.py
--rw-r--r--   0        0        0     7973 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/pod.py
--rw-r--r--   0        0        0    21722 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/runtime.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 pytest_container-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    26529 2024-04-10 10:06:09.293092 pytest_container-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3098 2024-04-10 10:06:09.293092 pytest_container-0.4.2/README.rst
+-rw-r--r--   0        0        0     2075 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1497 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/__init__.py
+-rw-r--r--   0        0        0    10564 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/build.py
+-rw-r--r--   0        0        0    42407 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/container.py
+-rw-r--r--   0        0        0     5725 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/helpers.py
+-rw-r--r--   0        0        0     8932 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/inspect.py
+-rw-r--r--   0        0        0      362 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/logging.py
+-rw-r--r--   0        0        0     7754 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/plugin.py
+-rw-r--r--   0        0        0     8344 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/pod.py
+-rw-r--r--   0        0        0    21936 2024-04-10 10:06:09.293092 pytest_container-0.4.2/pytest_container/runtime.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 pytest_container-0.4.2/PKG-INFO
```

### Comparing `pytest_container-0.4.1/LICENSE` & `pytest_container-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/README.rst` & `pytest_container-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pyproject.toml` & `pytest_container-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_container"
-version = "0.4.1"
+version = "0.4.2"
 description = "Pytest fixtures for writing container based tests"
 authors = ["Dan Čermák <dcermak@suse.com>"]
 homepage = "https://dcermak.github.io/pytest_container/"
 repository = "https://github.com/dcermak/pytest_container/"
 readme = "README.rst"
 license = "LGPL-2.1-or-later"
 classifiers = [
```

### Comparing `pytest_container-0.4.1/pytest_container/build.py` & `pytest_container-0.4.2/pytest_container/build.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pytest_container/container.py` & `pytest_container-0.4.2/pytest_container/container.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pytest_container/helpers.py` & `pytest_container-0.4.2/pytest_container/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pytest_container/inspect.py` & `pytest_container-0.4.2/pytest_container/inspect.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pytest_container/plugin.py` & `pytest_container-0.4.2/pytest_container/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.1/pytest_container/pod.py` & `pytest_container-0.4.2/pytest_container/pod.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,39 @@
     #: unique id/hash of the infra container of the pod
     infra_container_id: str
 
     #: ports exposed by this pod
     forwarded_ports: List[PortForwarding]
 
 
+def infra_container_id_from_pod_inspect(inspect_output: bytes) -> str:
+    """Given the output of :command:`podman pod inspect $id`, return the id of
+    the infra container.
+
+    """
+    # we don't want to directly query the infra container id via
+    # podman pod inspect -f "{{.InfraContainerID}}"
+    # as that doesn't work on ancient podman versions
+    #
+    # But both new and old podman versions have the Containers field with
+    # (at this stage), just the infra container.
+    # So we just grab the id from the full inspect
+    pod_inspect = json.loads(inspect_output.decode().strip())
+
+    # for $reasons, since podman 5, the output of `podman pod inspect $id`
+    # is no longer a dict, but a list of a dict 😡
+    infra_container = (
+        pod_inspect[0] if isinstance(pod_inspect, list) else pod_inspect
+    )["Containers"][0]
+
+    # old podman had the id of the containers with lowercase, new podman has
+    # uppercase => have to check for both :-(
+    return str(infra_container.get("Id", infra_container.get("id")))
+
+
 @dataclass
 class PodLauncher:
     """A context manager that creates, starts and destroys a pod with all of its
     containers.
 
     """
 
@@ -143,37 +168,23 @@
                     [runtime.runner_binary, "pod", "rm", "-f", self._pod_id]
                 )
             else:
                 _logger.debug("Not removing pod, not created")
 
         self._stack.callback(_delete_pod)
 
-        # we don't want to directly query the infra container id via
-        # podman pod inspect -f "{{.InfraContainerID}}"
-        # as that doesn't work on ancient podman versions
-        # But both new and old podman versions have the Containers field with
-        # (at this stage), just the infra container.
-        # So we just grab the id from the full inspect
-        pod_inspect = json.loads(
+        self._infra_container_id = infra_container_id_from_pod_inspect(
             check_output(
                 [
                     runtime.runner_binary,
                     "pod",
                     "inspect",
                     self._pod_id,
                 ]
             )
-            .decode()
-            .strip()
-        )
-        infra_container = pod_inspect["Containers"][0]
-        # old podman had the id of the containers with lowercase, new podman has
-        # uppercase => have to check for both :-(
-        self._infra_container_id = infra_container.get(
-            "Id", infra_container.get("id")
         )
 
         for container in self.pod.containers:
             self._launchers.append(
                 self._stack.enter_context(
                     ContainerLauncher(
                         container=container,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest_container-0.4.1/pytest_container/runtime.py` & `pytest_container-0.4.2/pytest_container/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -498,30 +498,36 @@
         return podman_recent_enough and _get_buildah_version() >= Version(
             1, 25, 0
         )
 
     def inspect_container(self, container_id: str) -> ContainerInspect:
         inspect = self._get_container_inspect(container_id)
 
-        Conf = inspect["Config"]
+        config = inspect["Config"]
         healthcheck = None
-        if "Healthcheck" in Conf:
+        if "Healthcheck" in config:
             healthcheck = HealthCheck.from_container_inspect(
-                Conf["Healthcheck"]
+                config["Healthcheck"]
             )
 
+        entrypoint = config.get("Entrypoint")
+        if isinstance(entrypoint, str):
+            entrypoint = entrypoint.split()
+        if not entrypoint:
+            entrypoint = []
+
         conf = Config(
-            user=Conf["User"],
-            tty=Conf["Tty"],
-            cmd=Conf["Cmd"],
-            image=Conf["Image"],
-            entrypoint=Conf["Entrypoint"].split(),
-            labels=Conf["Labels"],
-            env=dict([env.split("=", maxsplit=1) for env in Conf["Env"]]),
-            stop_signal=self._stop_signal_from_inspect_conf(Conf),
+            user=config["User"],
+            tty=config["Tty"],
+            cmd=config["Cmd"],
+            image=config["Image"],
+            entrypoint=entrypoint,
+            labels=config["Labels"],
+            env=dict([env.split("=", maxsplit=1) for env in config["Env"]]),
+            stop_signal=self._stop_signal_from_inspect_conf(config),
             healthcheck=healthcheck,
         )
 
         state = self._state_from_inspect(inspect)
 
         return ContainerInspect(
             config=conf,
@@ -578,33 +584,33 @@
     @property
     def supports_healthcheck_inherit_from_base(self) -> bool:
         return True
 
     def inspect_container(self, container_id: str) -> ContainerInspect:
         inspect = self._get_container_inspect(container_id)
 
-        Conf = inspect["Config"]
-        if Conf.get("Env"):
-            env = dict([env.split("=", maxsplit=1) for env in Conf["Env"]])
+        config = inspect["Config"]
+        if config.get("Env"):
+            env = dict([env.split("=", maxsplit=1) for env in config["Env"]])
         else:
             env = {}
         healthcheck = None
-        if "Healthcheck" in Conf:
+        if "Healthcheck" in config:
             healthcheck = HealthCheck.from_container_inspect(
-                Conf["Healthcheck"]
+                config["Healthcheck"]
             )
 
         conf = Config(
-            user=Conf["User"],
-            tty=Conf["Tty"],
-            cmd=Conf["Cmd"],
-            image=Conf["Image"],
-            entrypoint=Conf["Entrypoint"],
-            labels=Conf["Labels"],
-            stop_signal=self._stop_signal_from_inspect_conf(Conf),
+            user=config["User"],
+            tty=config["Tty"],
+            cmd=config["Cmd"],
+            image=config["Image"],
+            entrypoint=config["Entrypoint"],
+            labels=config["Labels"],
+            stop_signal=self._stop_signal_from_inspect_conf(config),
             env=env,
             healthcheck=healthcheck,
         )
 
         state = self._state_from_inspect(inspect)
 
         return ContainerInspect(
```

### Comparing `pytest_container-0.4.1/PKG-INFO` & `pytest_container-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_container
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pytest fixtures for writing container based tests
 Home-page: https://dcermak.github.io/pytest_container/
 License: LGPL-2.1-or-later
 Author: Dan Čermák
 Author-email: dcermak@suse.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 4 - Beta
```

