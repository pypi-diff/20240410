# Comparing `tmp/processing-pypelines-0.0.55.tar.gz` & `tmp/processing_pypelines-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.55.tar", last modified: Fri Apr  5 00:03:32 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.56.tar", last modified: Wed Apr 10 21:23:23 2024, max compression
```

## Comparing `processing-pypelines-0.0.55.tar` & `processing_pypelines-0.0.56.tar`

### file list

```diff
@@ -1,34 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:03:32.091239 processing-pypelines-0.0.55/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-05 00:03:32.000000 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-05 00:03:32.000000 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 00:03:32.000000 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-05 00:03:32.000000 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-05 00:03:32.000000 processing-pypelines-0.0.55/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    22296 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 00:03:32.095239 processing-pypelines-0.0.55/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-05 00:03:21.000000 processing-pypelines-0.0.55/tests/tests.py
+-rw-r--r--   0        0        0     1073 2024-04-10 21:23:11.892750 processing_pypelines-0.0.56/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-10 21:23:11.892750 processing_pypelines-0.0.56/README.md
+-rw-r--r--   0        0        0     1152 2024-04-10 21:23:23.196619 processing_pypelines-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4633 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34226 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-04-10 21:23:11.896750 processing_pypelines-0.0.56/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17038 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6559 2024-04-10 21:23:11.900750 processing_pypelines-0.0.56/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     8676 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    36877 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-04-10 21:23:11.980749 processing_pypelines-0.0.56/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-04-10 21:23:11.904750 processing_pypelines-0.0.56/tests/versions_example.json
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 processing_pypelines-0.0.56/PKG-INFO
```

### Comparing `processing-pypelines-0.0.55/LICENSE` & `processing_pypelines-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.55/pyproject.toml` & `processing_pypelines-0.0.56/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 [build-system]
-requires = ["setuptools >= 66.0"]
-build-backend = "setuptools.build_meta"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
 
 [project]
 name = "processing-pypelines"
+dependencies = [
+    "coloredlogs>=15.0.1",
+    "dynaconf>=3.2.4",
+    "natsort>=8.4.0",
+    "networkx>=3.1",
+    "numpy",
+    "matplotlib",
+    "pandas>=2.1.4",
+]
 authors = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
-license = { text = "MIT" }
-dynamic = ["version", "dependencies", "optional-dependencies"]
+dynamic = []
+version = "0.0.56"
+
+[project.license]
+text = "MIT"
+
+[project.optional-dependencies]
+celery = [
+    "celery>=5.3.5",
+    "alyx_connector>=2.1.5",
+]
 
 [project.urls]
 homepage = "https://gitlab.pasteur.fr/haisslab/data-management/pypelines"
 repository = "https://gitlab.pasteur.fr/haisslab/data-management/pypelines"
 documentation = "https://gitlab.pasteur.fr/haisslab/data-management/pypelines"
 
-[tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-optional-dependencies = { celery = { file = [
-    "requirements.txt",
-    "requirements-celery.txt",
-] } }
-version = { attr = "pypelines.__version__" }
-
-[tool.setuptools.packages.find]
-where = ["src"]
+[tool.pdm.version]
+source = "file"
+path = "src/pypelines/__init__.py"
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/arguments.py` & `processing_pypelines-0.0.56/src/pypelines/arguments.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,27 @@
     json_no_comments = re.sub(pattern, "", json_string, flags=re.DOTALL)
 
     # loading the json format string without comments as a python dict
     return json.loads(json_no_comments)
 
 
 def read_session_arguments_file(session, step, file_suffix="_arguments.json"):
+    """Reads the arguments file for a specific session and step.
+
+    Args:
+        session: The session object containing the path information.
+        step: The step object for which the arguments file needs to be read.
+        file_suffix: The suffix to be appended to the arguments file name (default is "_arguments.json").
+
+    Returns:
+        The contents of the arguments file as a dictionary.
+
+    Raises:
+        FileNotFoundError: If the arguments file for the specified session and step is not found.
+    """
     file_name = step.pipeline.pipeline_name + file_suffix
     try:
         path = os.path.join(session.path, file_name)
         return read_json_file(path)
     except FileNotFoundError:
         raise FileNotFoundError(f"Could not open the config file {file_name} for the session {session.alias}")
 
@@ -42,15 +55,26 @@
         step (_type_): the step instance from wich to get name information.
 
     Returns:
         function: the wrapped function
     """
 
     @wraps(wrapped_function)
-    def wraper(session, *args, **kwargs):
+    def wrapper(session, *args, **kwargs):
+        """Wrapper function that automatically loads arguments from pipelines_arguments.json
+        and overrides them with current call arguments.
+
+        Args:
+            session: The session object.
+            *args: Variable length argument list.
+            **kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            The result of the wrapped function with updated arguments.
+        """
         local_log = getLogger("autoload_arguments")
 
         config_kwargs = get_step_arguments(session, step)
         if config_kwargs:  # new_kwargs is not empty
             local_log.note(
                 f"Using the arguments for the function {step.relative_name} found in pipelines_arguments.json."
             )
@@ -66,18 +90,32 @@
                 f"Values of pipelines_arguments.json arguments : {', '.join(overrides_names)}, are overrided by the"
                 f" current call arguments to {step.relative_name}"
             )
 
         config_kwargs.update(kwargs)
         return wrapped_function(session, *args, **config_kwargs)
 
-    return wraper
+    return wrapper
 
 
 def get_step_arguments(session, step):
+    """Get the arguments for a specific step from the session's arguments file.
+
+    Args:
+        session (str): The name of the session.
+        step (Step): The step object for which arguments need to be retrieved.
+
+    Returns:
+        dict: The arguments for the specified step.
+
+    Raises:
+        FileNotFoundError: If the session arguments file is not found.
+        KeyError: If the 'functions' key or the key corresponding to step.relative_name
+            is not found in the arguments file.
+    """
     local_log = getLogger("autoload_arguments")
 
     try:
         config_args = read_session_arguments_file(session, step)["functions"][step.relative_name]
     except FileNotFoundError as e:
         local_log.debug(f"{type(e).__name__} : {e}. Skipping")
         return {}
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.56/src/pypelines/celery_tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,28 +21,59 @@
 
 class CeleryAlyxTaskManager(BaseStepTaskManager):
 
     backend: "CeleryTaskBackend"
     step: "BaseStep"
 
     def register_step(self):
+        """Register a step in the backend.
+
+        This method registers a task in the backend using the runner obtained from get_runner() method.
+
+        Returns:
+            None
+        """
         if self.backend:
             # self.backend.app.task(CeleryRunner, name=self.step.complete_name)
             self.backend.app.register_task(self.get_runner())
 
     def start(self, session, extra=None, **kwargs):
+        """Starts a task on a celery cluster.
+
+        Args:
+            session: The session to use for the task.
+            extra: Extra information to pass to the task (default is None).
+            **kwargs: Additional keyword arguments to pass to the task.
+
+        Raises:
+            NotImplementedError: If the pipeline does not have a working celery backend.
+
+        Returns:
+            The created CeleryTaskRecord.
+        """
 
         if not self.backend:
             raise NotImplementedError(
                 "Cannot start a task on a celery cluster as this pipeline " "doesn't have a working celery backend"
             )
 
         return CeleryTaskRecord.create(self, session, extra, **kwargs)
 
     def get_runner(superself):  # type: ignore
+        """Return a CeleryRunner task for executing a step in a pipeline.
+
+        Args:
+            superself: The parent object that contains the step information.
+
+        Returns:
+            CeleryRunner: A Celery Task object that runs the specified step.
+
+        Raises:
+            Any exceptions that occur during the execution of the task.
+        """
         from celery import Task
 
         class CeleryRunner(Task):
             name = superself.step.complete_name
 
             def run(self, task_id, extra=None):
 
@@ -83,26 +114,43 @@
 
 
 class CeleryTaskRecord(dict):
     session: Series
 
     # a class to make dictionnary keys accessible with attribute syntax
     def __init__(self, task_id, task_infos_dict={}, response_handle=None, session=None):
+        """Initialize the Task object.
+
+        Args:
+            task_id (str): The unique identifier for the task.
+            task_infos_dict (dict, optional): A dictionary containing information about the task.
+                If not provided, it will be fetched using the task_id. Defaults to {}.
+            response_handle (Any, optional): A handle for the response. Defaults to None.
+            session (Any, optional): A session object. Defaults to None.
+        """
 
         if not task_infos_dict:
             from one import ONE
 
             connector = ONE(mode="remote", data_access_mode="remote")
             task_infos_dict = connector.alyx.rest("tasks", "read", id=task_id)
 
         super().__init__(task_infos_dict)
         self.session = session  # type: ignore
         self.response = response_handle
 
     def status_from_logs(self, log_object):
+        """Update the status based on the content of the log file.
+
+        Args:
+            log_object: Log object containing the full path to the log file.
+
+        Returns:
+            None
+        """
         with open(log_object.fullpath, "r") as f:
             content = f.read()
 
         if len(content) == 0:
             status = "No_Info"
         elif "CRITICAL" in content:
             status = "Failed"
@@ -112,61 +160,104 @@
             status = "Warnings"
         else:
             status = "Complete"
 
         self["status"] = status
 
     def partial_update(self):
+        """Partially updates a task using the ONE API.
+
+        This function connects to the ONE database in remote mode and performs a partial update on a task
+        using the export data from the current instance.
+
+        Returns:
+            None
+        """
         from one import ONE
 
         connector = ONE(mode="remote", data_access_mode="remote")
         connector.alyx.rest("tasks", "partial_update", **self.export())
 
     def get_session(self):
+        """Retrieve the session object associated with the current instance.
+
+        Returns:
+            The session object.
+        """
         if self.session is None:
             from one import ONE
 
             connector = ONE(mode="remote", data_access_mode="remote")
             session = connector.search(id=self["session"], no_cache=True, details=True)
             self.session = session  # type: ignore
 
         return self.session
 
     def get_application(self):
+        """Return the application associated with the executable stored in the instance.
+
+        Returns:
+            str: The application associated with the executable.
+
+        Raises:
+            KeyError: If the application associated with the executable is not found in the APPLICATIONS_STORE.
+        """
         try:
             return APPLICATIONS_STORE[self["executable"]]
         except KeyError:
             raise KeyError(f"Unable to retrieve the application {self['executable']}")
 
     @property
     def pipeline_name(self):
+        """Return the name of the pipeline by splitting the name attribute at '.' and returning the first part."""
         return self["name"].split(".")[0]
 
     @property
     def pipe_name(self):
+        """Return the name of the pipe by splitting the name attribute using '.' and returning the second element.
+
+        Returns:
+            str: The name of the pipe.
+        """
         return self["name"].split(".")[1]
 
     @property
     def step_name(self):
+        """Return the third element after splitting the 'name' attribute of the object with '.'."""
         return self["name"].split(".")[2]
 
     @property
     def arguments(self):
+        """Retrieve and filter arguments for the current step.
+
+        Returns:
+            dict: Filtered arguments for the current step.
+        """
         # once step arguments control will be done via file, these should take prio over the main step ran's file args
         args = self.get("arguments", {})
         args = args if args else {}
         management_args = self.management_arguments
         filtered_args = {}
         for key, value in args.items():
             if key not in management_args.keys():
                 filtered_args[key] = value
         return filtered_args
 
     @property
     def management_arguments(self):
+        """Returns a dictionary of management arguments based on the default values and any provided arguments.
+
+        Returns:
+            dict: A dictionary containing the management arguments with keys:
+                - "skip": A boolean indicating whether to skip management.
+                - "refresh": A boolean indicating whether to refresh.
+                - "refresh_requirements": A boolean indicating whether to refresh requirements.
+                - "check_requirements": A boolean indicating whether to check requirements.
+                - "save_output": A boolean indicating whether to save output.
+        """
         default_management_args = {
             "skip": True,
             "refresh": False,
             "refresh_requirements": False,
             "check_requirements": True,
             "save_output": True,
         }
@@ -178,25 +269,43 @@
         if management_args["refresh"] == True:
             management_args["skip"] = False
 
         return management_args
 
     @property
     def session_path(self) -> str:
+        """Returns the path of the session."""
         return self.session["path"]
 
     @property
     def task_id(self):
+        """Return the task ID."""
         return self["id"]
 
     def export(self):
+        """Export the object as a dictionary with specific keys removed.
+
+        Returns:
+            dict: A dictionary containing the object's id and data with certain keys removed.
+        """
         return {"id": self["id"], "data": {k: v for k, v in self.items() if k not in ["id", "session_path"]}}
 
     @staticmethod
     def create(task_manager: CeleryAlyxTaskManager, session, extra=None, **kwargs):
+        """Creates a new task using the given CeleryAlyxTaskManager and session.
+
+        Args:
+            task_manager (CeleryAlyxTaskManager): The CeleryAlyxTaskManager instance to use.
+            session: The session to associate with the task.
+            extra (optional): Any extra information to include in the task.
+            **kwargs: Additional keyword arguments to pass to the task.
+
+        Returns:
+            CeleryTaskRecord: A CeleryTaskRecord object representing the created task.
+        """
         from one import ONE
 
         connector = ONE(mode="remote", data_access_mode="remote")
 
         data = {
             "session": session.name,
             "name": task_manager.step.complete_name,
@@ -212,14 +321,27 @@
 
         return CeleryTaskRecord(
             task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
         )
 
     @staticmethod
     def create_from_task_name(app: "Celery", task_name: str, pipeline_name: str, session, extra=None, **kwargs):
+        """Create a new task from the given task name and pipeline name.
+
+        Args:
+            app (Celery): The Celery application.
+            task_name (str): The name of the task to be created.
+            pipeline_name (str): The name of the pipeline.
+            session: The session object.
+            extra (optional): Extra information for the task.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            CeleryTaskRecord: A record of the created Celery task.
+        """
         from one import ONE
 
         connector = ONE(mode="remote", data_access_mode="remote")
 
         data = {
             "session": session.name if isinstance(session, Series) else session,
             "name": task_name,
@@ -236,14 +358,29 @@
             task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
         )
 
     @staticmethod
     def create_from_model(
         app: "Celery", task_model: type, task_name: str, pipeline_name: str, session: object, extra=None, **kwargs
     ):
+        """Create a new task from a given task model and send it to a Celery app.
+
+        Args:
+            app (Celery): The Celery app instance.
+            task_model (type): The task model class to create a new task instance.
+            task_name (str): The name of the task.
+            pipeline_name (str): The name of the pipeline.
+            session (object): The session object.
+            extra (optional): Extra information to pass to the task.
+            **kwargs: Additional keyword arguments to pass to the task.
+
+        Returns:
+            CeleryTaskRecord: A record of the created task with task ID, task information dictionary,
+                response handle, and session.
+        """
 
         new_task = task_model(name=task_name, session=session, arguments=kwargs, status=25, executable=pipeline_name)
         new_task.save()
 
         task_dict = new_task.__dict__.copy()
         task_dict.pop("_state", None)
 
@@ -255,56 +392,104 @@
 
 
 class CeleryTaskBackend(BaseTaskBackend):
     app: "Celery"
     task_manager_class = CeleryAlyxTaskManager
 
     def __init__(self, parent: Pipeline, app: "Celery | None" = None):
+        """Initialize the PipelineApp object.
+
+        Args:
+            parent (Pipeline): The parent Pipeline object.
+            app (str): The Celery app associated with the Pipeline, or None if not provided.
+
+        Attributes:
+            parent (Pipeline): The parent Pipeline object.
+            success (bool): Flag indicating if the initialization was successful.
+            app (str): The Celery app associated with the Pipeline.
+        """
         super().__init__(parent)
         self.parent = parent
 
         if app is not None:
             self.success = True
             self.app = app
 
             pipelines = getattr(self.app, "pipelines", {})
             pipelines[parent.pipeline_name] = parent
             self.app.pipelines = pipelines
 
     def start(self):
+        """Starts the application."""
         self.app.start()
 
     def create_task_manager(self, step):
+        """Create a task manager for the given step.
+
+        Args:
+            step: The step to be associated with the task manager.
+
+        Returns:
+            Task manager object initialized with the given step.
+        """
         task_manager = self.task_manager_class(step, self)
         task_manager.register_step()
         return task_manager
 
 
 class CeleryPipeline(Pipeline):
     runner_backend_class = CeleryTaskBackend
 
 
 class LogTask:
     def __init__(self, task_record: CeleryTaskRecord, username=None, level="LOAD"):
+        """Initialize the TaskLogger object.
+
+        Args:
+            task_record (CeleryTaskRecord): The Celery task record.
+            username (str, optional): The username associated with the task. Defaults to None.
+            level (str, optional): The logging level for the task. Defaults to "LOAD".
+        """
         self.path = Path(task_record.session_path) / "logs"
         self.username = username if username is not None else (node() if node() else "unknown")
         self.worker_pk = task_record.task_id
         self.task_name = task_record["name"]
         self.level = getattr(logging, level.upper())
 
     def __enter__(self):
+        """Perform necessary setup tasks when entering a context manager.
+
+        Returns:
+            self: The current instance of the context manager.
+        """
         self.path.mkdir(exist_ok=True)
         self.logger = getLogger()
         self.set_handler()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        """Clean up resources when exiting a context manager.
+
+        Args:
+            exc_type: The type of the exception that caused the exit, or None if no exception occurred.
+            exc_val: The exception instance that caused the exit, or None if no exception occurred.
+            exc_tb: The traceback of the exception that caused the exit, or None if no exception occurred.
+        """
         self.remove_handler()
 
     def set_handler(self):
+        """Set up logging handler for the current task.
+
+        This method sets up a logging handler for the current task by creating a log file
+        with a specific filename based on task details.
+        It then configures the file handler with appropriate formatters and filters for colored logging.
+
+        Returns:
+            None
+        """
         self.filename = f"task_log.{self.task_name}.{self.worker_pk}.log"
         self.fullpath = self.path / self.filename
         fh = logging.FileHandler(self.fullpath)
         f_formater = FileFormatter()
         coloredlogs.HostNameFilter.install(
             fmt=f_formater.FORMAT,
             handler=fh,
@@ -325,18 +510,30 @@
         )
 
         fh.setLevel(self.level)
         fh.setFormatter(f_formater)
         self.logger.addHandler(fh)
 
     def remove_handler(self):
+        """Removes the last handler from the logger."""
         self.logger.removeHandler(self.logger.handlers[-1])
 
 
 def create_celery_app(conf_path, app_name="pypelines", v_host=None) -> "Celery | None":
+    """Create a Celery app with the given configuration.
+
+    Args:
+        conf_path (str): The path to the configuration file.
+        app_name (str): The name of the Celery app. Default is "pypelines".
+        v_host (str): The virtual host for the Celery app.
+
+    Returns:
+        Celery | None: The created Celery app instance or None if creation failed.
+
+    """
 
     failure_message = (
         f"Celery app : {app_name} failed to be created."
         "Don't worry, about this alert, "
         "this is not be an issue if you didn't explicitely planned on using celery. Issue was : "
     )
 
@@ -351,31 +548,55 @@
     except ImportError as e:
         logger.warning(f"{failure_message} Could not import celery app. {e}")
         return None
 
     from types import MethodType
 
     def get_setting_files_path(conf_path) -> List[Path]:
+        """Get the paths of setting files for the given configuration path.
+
+        Args:
+            conf_path (str): The path to the configuration file.
+
+        Returns:
+            List[Path]: A list of Path objects representing the setting files found.
+        """
         conf_path = Path(conf_path)
         if conf_path.is_file():
             conf_path = conf_path.parent
         files = []
         for prefix, suffix in zip(["", "."], ["", "_secrets"]):
             file_loc = conf_path / f"{prefix}celery_{app_name}{suffix}.toml"
             if file_loc.is_file():
                 files.append(file_loc)
         return files
 
     def get_signature_as_string(signature):
+        """Return the function signature as a string without the 'session' parameter.
+
+        Args:
+            signature: The signature of the function.
+
+        Returns:
+            str: The function signature as a string without the 'session' parameter.
+        """
         params = [
             param_value for param_name, param_value in signature.parameters.items() if param_name not in ["session"]
         ]
         return str(signature.replace(parameters=params))[1:-1].replace(" *,", "")
 
     def get_type_name(annotation):
+        """Returns the name of the type hint for a given annotation.
+
+        Args:
+            annotation: The annotation for which to determine the type name.
+
+        Returns:
+            str: The name of the type hint.
+        """
         from inspect import Parameter
         from typing import get_args, get_origin
         from types import UnionType
 
         if isinstance(annotation, str):
             annotation = string_to_typehint(annotation, globals(), locals())
 
@@ -390,22 +611,45 @@
             if typ is Parameter.empty:
                 return "__unknown__"
             else:
                 return typ.__name__
         return "__unknown__"
 
     def string_to_typehint(string_hint, globalns=None, localns=None):
+        """Converts a string type hint to a valid type hint object.
+
+        Args:
+            string_hint (str): The string representation of the type hint.
+            globalns (dict, optional): Global namespace dictionary. Defaults to None.
+            localns (dict, optional): Local namespace dictionary. Defaults to None.
+
+        Returns:
+            type: The type hint object corresponding to the input string hint,
+                or "__unknown__" if the type hint is not valid.
+        """
         from typing import ForwardRef, _eval_type
 
         try:
             return _eval_type(ForwardRef(string_hint), globalns, localns)
         except NameError:
             return "__unknown__"
 
     def get_signature_as_dict(signature):
+        """Return a dictionary containing information about the parameters of a function signature.
+
+        Args:
+            signature: A function signature object.
+
+        Returns:
+            dict: A dictionary where keys are parameter names and values
+                are dictionaries containing the following information:
+                - "typehint": The type hint of the parameter.
+                - "default_value": The default value of the parameter (or "__empty__" if no default value is specified).
+                - "kind": The kind of the parameter (e.g., POSITIONAL_ONLY, KEYWORD_ONLY, etc.).
+        """
         from inspect import Parameter
 
         parameters = signature.parameters
         parsed_args = {}
         for name, param in parameters.items():
 
             parsed_args[name] = {
@@ -422,14 +666,23 @@
         def run(self):
             return f"{node()} is happy to shake your hand and says hello !"
 
     class TasksInfos(Task):
         name = f"{app_name}.tasks_infos"
 
         def run(self, app_name, selfish=False):
+            """Run the specified app to gather tasks information.
+
+            Args:
+                app_name (str): The name of the app to run.
+                selfish (bool, optional): Flag to indicate whether to include selfish tasks. Defaults to False.
+
+            Returns:
+                dict: A dictionary containing tasks information for the specified app.
+            """
             app = APPLICATIONS_STORE[app_name]
             tasks_dynamic_data = {}
             pipelines = getattr(app, "pipelines", {})
             if len(pipelines) == 0:
                 logger.warning(
                     "No pipeline is registered on this app instance. "
                     "Are you trying to read tasks infos from a non worker app ? (web server side ?)"
@@ -453,28 +706,46 @@
                                 "requires": [item.complete_name for item in step.requires],
                                 "step_level_in_pipe": step.get_level(selfish=selfish),
                             }
                             tasks_dynamic_data[step.complete_name] = task_data
             return tasks_dynamic_data
 
     def get_remote_tasks(self):
+        """Retrieve information about remote tasks.
+
+        Returns:
+            dict: A dictionary containing information about remote tasks, including workers and task names.
+        """
         registered_tasks = self.control.inspect().registered_tasks()
         workers = []
         task_names = []
         if registered_tasks:
             for worker, tasks in registered_tasks.items():
                 workers.append(worker)
                 for task in tasks:
                     task_names.append(task)
 
         return {"workers": workers, "task_names": task_names}
 
     def get_celery_app_tasks(
         self, refresh=False, auto_refresh=3600 * 24, failed_refresh=60 * 5, initial_timeout=10, refresh_timeout=2
     ):
+        """Get the celery app tasks data with optional refresh mechanism.
+
+        Args:
+            refresh (bool): Flag to force refresh the tasks data. Default is False.
+            auto_refresh (int): Time interval in seconds for auto refresh. Default is 3600 seconds (1 hour).
+            failed_refresh (int): Time interval in seconds for retrying refresh after failure.
+                Default is 300 seconds (5 minutes).
+            initial_timeout (int): Timeout in seconds for initial task data retrieval. Default is 10 seconds.
+            refresh_timeout (int): Timeout in seconds for refreshing task data. Default is 2 seconds.
+
+        Returns:
+            dict: The task data of the celery app if available, otherwise None.
+        """
 
         from datetime import datetime, timedelta
 
         auto_refresh_time = timedelta(0, seconds=auto_refresh)  # a full day (24 hours of 3600 seconds)
         failed_refresh_retry_time = timedelta(0, failed_refresh)  # try to refresh after 5 minutes
 
         app_task_data = getattr(self, "task_data", None)
@@ -516,27 +787,44 @@
                 setattr(self, "task_data", app_task_data)
             else:
                 delta = (app_task_data["refresh_time"] - now).total_seconds()
                 logger.warning(f"Returned cached task_data. Next refresh will happen in at least {delta} seconds")
         return app_task_data["task_data"] if app_task_data is not None else None
 
     def launch_named_task_remotely(self, session_id, task_name, task_model=None, extra=None, kwargs={}):
+        """Launches a named task remotely.
+
+        Args:
+            session_id (str): The session ID for the task.
+            task_name (str): The name of the task to be launched.
+            task_model (object, optional): The task model object. Defaults to None.
+            extra (dict, optional): Extra data to be passed to the task. Defaults to None.
+            kwargs (dict, optional): Additional keyword arguments to be passed to the task. Defaults to {}.
+
+        Returns:
+            CeleryTaskRecord: The task record created for the launched task.
+        """
 
         if task_model is None:
             task_record = CeleryTaskRecord.create_from_task_name(
                 self, task_name, app_name, session_id, extra=extra, **kwargs
             )
         else:
             task_record = CeleryTaskRecord.create_from_model(
                 self, task_model, task_name, app_name, session_id, extra=extra, **kwargs
             )
 
         return task_record
 
     def is_hand_shaken(self):
+        """Check if a handshake is successful.
+
+        Returns:
+            bool: True if handshake is successful, False otherwise.
+        """
         try:
             result = self.tasks[f"{app_name}.handshake"].delay().get(timeout=1)
             logger.warning(f"Handshake result : {result}")
             return True
         except Exception as e:
             logger.error(f"No handshake result. All workers are busy ? {e}")
             return False
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/loggs.py` & `processing_pypelines-0.0.56/src/pypelines/loggs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 import logging
 import sys
 import re
-import os
 from functools import wraps
-import coloredlogs
-
-NAMELENGTH = 33  # global variable for fromatting the length of the padding dedicated to name part in a logging record
-LEVELLENGTH = 8  # global variable for fromatting the length of the padding dedicated to levelname part in a record
-
-
-def enable_logging(terminal_level="NOTE", file_level="LOAD", programname="", username=""):
-    """_summary_
+from coloredlogs import (
+    coerce_string,
+    ansi_wrap,
+    Empty,
+    ColoredFormatter,
+    UserNameFilter,
+    ProgramNameFilter,
+    HostNameFilter,
+)
+from pathlib import Path
+
+NAMELENGTH = 33  # global variable for formatting the length of the padding dedicated to name part in a logging record
+LEVELLENGTH = 8  # global variable for formatting the length of the padding dedicated to levelname part in a record
+
+
+def enable_logging(
+    filename: str | None = None,
+    terminal_level: str = "NOTE",
+    file_level: str = "LOAD",
+    programname: str = "",
+    username: str = "",
+):
+    """Enable logging with specified configurations.
 
     Args:
-        terminal_level (str, optional): _description_. Defaults to "INFO".
-        file_level (str, optional): _description_. Defaults to "LOAD".
-        programname (str, optional): _description_. Defaults to "".
-        username (str, optional): _description_. Defaults to "".
+        filename (str, optional): Path to the log file. Defaults to None.
+        terminal_level (str, optional): Logging level for terminal output. Defaults to "INFO".
+        file_level (str, optional): Logging level for file output. Defaults to "LOAD".
+        programname (str, optional): Name of the program. Defaults to "".
+        username (str, optional): Username for logging. Defaults to "".
     """
     # Create a filehandler object for file
-    fh = logging.FileHandler("test.log", "w", "utf-8")
+    if filename is None:
+        logs_folder = Path.home() / ".python" / "pypelines_logs"
+        logs_folder.mkdir(parents=True, exist_ok=True)
+        filename = str(logs_folder / "logs.log")
+
+    fh = logging.FileHandler(filename, mode="a", encoding="utf-8")
     f_formater = FileFormatter()
     fh.setFormatter(f_formater)
 
-    coloredlogs.HostNameFilter.install(
-        fmt=f_formater.FORMAT,
-        handler=fh,
-        style=f_formater.STYLE,
-        use_chroot=True,
-    )
-    coloredlogs.ProgramNameFilter.install(
-        fmt=f_formater.FORMAT,
-        handler=fh,
-        programname=programname,
-        style=f_formater.STYLE,
-    )
-    coloredlogs.UserNameFilter.install(
-        fmt=f_formater.FORMAT,
-        handler=fh,
-        username=username,
-        style=f_formater.STYLE,
-    )
-
     # Create a filehandler object for terminal
     ch = logging.StreamHandler(sys.stdout)
     c_formater = TerminalFormatter()
     ch.setFormatter(c_formater)
 
-    coloredlogs.HostNameFilter.install(
-        fmt=c_formater.FORMAT,
-        handler=fh,
-        style=c_formater.STYLE,
-        use_chroot=True,
-    )
-    coloredlogs.ProgramNameFilter.install(
-        fmt=c_formater.FORMAT,
-        handler=fh,
-        programname=programname,
-        style=c_formater.STYLE,
-    )
-    coloredlogs.UserNameFilter.install(
-        fmt=c_formater.FORMAT,
-        handler=fh,
-        username=username,
-        style=c_formater.STYLE,
-    )
+    for handler, formater in zip([fh, ch], [f_formater, c_formater]):
+
+        HostNameFilter.install(
+            fmt=formater.FORMAT,
+            handler=handler,
+            style=f_formater.STYLE,
+            use_chroot=True,
+        )
+        ProgramNameFilter.install(
+            fmt=formater.FORMAT,
+            handler=handler,
+            programname=programname,
+            style=formater.STYLE,
+        )
+        UserNameFilter.install(
+            fmt=formater.FORMAT,
+            handler=handler,
+            username=username,
+            style=formater.STYLE,
+        )
 
     logger = logging.getLogger()  # root logger
 
     while logger.hasHandlers():
         # make sure we start fresh from any previous handlers when we enable
         handler = logger.handlers[0]
         logger.removeHandler(handler)
@@ -80,90 +83,90 @@
 
     logger = logging.getLogger()
 
     logger.setLevel(
         min(terminal_level, file_level)
     )  # set logger level to the lowest usefull, to be sure we can capture messages necessary in handlers
 
-    fh.setLevel(file_level)
-    logger.addHandler(fh)
-    ch.setLevel(terminal_level)
-    logger.addHandler(ch)
+    for handler in [fh, ch]:
+
+        handler.setLevel(file_level)
+        logger.addHandler(handler)
 
 
-class DynamicColoredFormatter(coloredlogs.ColoredFormatter):
+class DynamicColoredFormatter(ColoredFormatter):
     """_summary_"""
 
     # note that only message, name, levelname, pathname, process, thread, lineno, levelno and filename can be dynamic.
     # asctime of hostname for example, can't. This is limitation for implementation simplicity reasons only,
     # as it would be more complex to implement otherwise, and for a small benefit.
 
     def __init__(self, fmt=None, datefmt=None, style="%", level_styles=None, field_styles=None, dynamic_levels=None):
-        """_summary_
+        """Initialize the logging formatter with custom formatting options.
 
         Args:
-            fmt (_type_, optional): _description_. Defaults to None.
-            datefmt (_type_, optional): _description_. Defaults to None.
-            style (str, optional): _description_. Defaults to "%".
-            level_styles (_type_, optional): _description_. Defaults to None.
-            field_styles (_type_, optional): _description_. Defaults to None.
-            dynamic_levels (_type_, optional): _description_. Defaults to None.
+            fmt (str, optional): A format string for the log message. Defaults to None.
+            datefmt (str, optional): A format string for the date/time portion of the log message. Defaults to None.
+            style (str, optional): The style of formatting to use. Defaults to "%".
+            level_styles (dict, optional): A dictionary mapping log levels to custom styles. Defaults to None.
+            field_styles (dict, optional): A dictionary mapping log fields to custom styles. Defaults to None.
+            dynamic_levels (dict, optional): A dictionary mapping dynamic log levels. Defaults to None.
         """
         self.dynamic_levels = dynamic_levels
         self.lenght_pre_formaters = self.get_length_pre_formaters(fmt)
         super().__init__(
             fmt=fmt,
             datefmt=datefmt,
             style=style,
             level_styles=level_styles,
             field_styles=field_styles,
         )
 
     def get_length_pre_formaters(self, fmt):
-        """_summary_
+        """Get the length of pre-formatters in the given format string.
 
         Args:
-            fmt (_type_): _description_
+            fmt (str): The format string containing pre-formatters.
 
         Returns:
-            _type_: _description_
+            dict: A dictionary containing the length of each pre-formatter.
         """
         pattern = r"%\((?P<part_name>\w+)\)-?(?P<length>\d+)?[sd]?"
         result = re.findall(pattern, fmt)
         padding_dict = {name: int(padding) if padding else 0 for name, padding in result}
 
         return padding_dict
 
     def format(self, record: logging.LogRecord):
-        """_summary_
+        """Format the log record for display.
 
         Args:
-            record (_type_): _description_
+            record (logging.LogRecord): The log record to be formatted.
 
         Returns:
-            _type_: _description_
+            str: The formatted log message.
         """
         style = self.nn.get(self.level_styles, record.levelname)
         # print(repr(humanfriendly.terminal.ansi_style(**style)))
         record.message = record.getMessage()
         if self.usesTime():
             record.asctime = self.formatTime(record, self.datefmt)
-        if style and coloredlogs.Empty is not None:
-            copy = coloredlogs.Empty()
+        if style and Empty is not None:
+            copy = Empty()
             copy.__class__ = record.__class__
             copy.__dict__.update(record.__dict__)
             for part_name, length in self.lenght_pre_formaters.items():
                 part = getattr(copy, part_name)  # .ljust(length, " ")
                 real_length = len(part)
                 missing_length = length - real_length
                 missing_length = 0 if missing_length < 0 else missing_length
                 if part_name in self.dynamic_levels.keys():
                     dyn_keys = self.dynamic_levels[part_name]
                     dynamic_style = {k: v for k, v in style.items() if k in dyn_keys or dyn_keys == "all"}
-                    part = coloredlogs.ansi_wrap(coloredlogs.coerce_string(part), **dynamic_style)
+                    part = ansi_wrap(coerce_string(part), **dynamic_style)
                 part = part + (" " * missing_length)
                 setattr(copy, part_name, part)
             record = copy  # type: ignore
 
         s = self.formatMessage(record)
         if record.exc_info:
             # Cache the traceback text to avoid converting it multiple times
@@ -207,14 +210,27 @@
     DYNAMIC_LEVELS = {
         "message": ["color", "bold", "background"],
         "levelname": "all",
         "name": "all",
     }
 
     def __init__(self, fmt=None, datefmt=None, style=None, level_styles=None, field_styles=None, dynamic_levels=None):
+        """Initializes a custom logging formatter with specified parameters.
+
+        Args:
+            fmt (str): The log message format string.
+            datefmt (str): The date format string.
+            style (str): The log message style.
+            level_styles (dict): Dictionary mapping log levels to custom styles.
+            field_styles (dict): Dictionary mapping log fields to custom styles.
+            dynamic_levels (bool): Flag indicating whether dynamic levels are enabled.
+
+        Returns:
+            None
+        """
         self.STYLE = style if style is not None else self.STYLE
         self.FORMAT = fmt if fmt is not None else self.FORMAT
         self.DATE_FORMAT = datefmt if datefmt is not None else self.DATE_FORMAT
         self.LEVEL_STYLES = level_styles if level_styles is not None else self.LEVEL_STYLES
         self.FIELD_STYLES = field_styles if field_styles is not None else self.FIELD_STYLES
 
         self.DYNAMIC_LEVELS = dynamic_levels if dynamic_levels is not None else self.DYNAMIC_LEVELS
@@ -363,14 +379,25 @@
         with LogSession(session):
             return func(session, *args, **kwargs)
 
     return wrapper
 
 
 def add_all_custom_headers():
+    """Adds custom logging levels to the logging module.
+
+    This function adds custom logging levels "NOTE", "LOAD", "SAVE", "HEADER", "START",
+    and "END" to the logging module with specific integer values relative to existing levels.
+
+    Example:
+        add_all_custom_headers()
+
+    Note:
+        This function should be called before using the custom logging levels in the application.
+    """
     addLoggingLevel("NOTE", logging.INFO - 1, if_exists="keep")
     addLoggingLevel("LOAD", logging.DEBUG + 1, if_exists="keep")
     addLoggingLevel("SAVE", logging.DEBUG + 2, if_exists="keep")
     addLoggingLevel("HEADER", logging.INFO + 1, if_exists="keep")
     addLoggingLevel("START", logging.INFO + 2, if_exists="keep")
     addLoggingLevel("END", logging.INFO + 3, if_exists="keep")
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.56/src/pypelines/pickle_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,33 @@
     current_suffixes = ""
     remove = True
     current_disk_file = None
     update_file_format = True
     is_legacy_format = False
 
     def __init__(self, session, step, extra=""):
+        """Initialize the StepTask object.
+
+        Args:
+            session: The session object for the task.
+            step: The step object for the task.
+            extra: Additional information for the task (default is an empty string).
+        """
         self.file_prefix = step.pipeline.pipeline_name
         super().__init__(session, step, extra)
 
     def version_deprecated(self) -> bool:
+        """Check if the current version is deprecated.
+
+        This method compares the current version with the disk version and returns True if they are different,
+        indicating that the current version is deprecated. Otherwise, it returns False.
+
+        Returns:
+            bool: True if the current version is deprecated, False otherwise.
+        """
         logger = logging.getLogger("pickle.version_deprecated")
 
         # if we didn't found the disk version, we return False.
         # it's not labeled as "deprecated" for retro-compatibility
         if self.disk_version is None or self.disk_version == "":
             return False
 
@@ -35,14 +50,19 @@
 
         logger.debug(
             f"Disk version {self.disk_version} was identicall to current version {self.version}. Returning False"
         )
         return False
 
     def step_level_too_low(self) -> bool:
+        """Check if the level of the disk step is lower than the current step level.
+
+        Returns:
+            bool: True if the disk step level is lower than the current step level, False otherwise.
+        """
         logger = logging.getLogger("pickle.step_level_too_low")
 
         # we get the step instance that corresponds to the one on the disk
         disk_step = self.disk_step_instance()
 
         # if we didn't found the disk step, we return False.
         # it's not labeled as "too low" for retro-compatibility
@@ -60,26 +80,41 @@
         logger.debug(
             f"Disk step {disk_step.relative_name} was higher or equal than {self.step.relative_name}. Returning False"
         )
         return False
 
     @property
     def version(self):
+        """Return the version of the pipeline."""
         return self.step.pipe.version
 
     def parse_extra(self, extra, regexp=False):
+        """Parses the extra string by optionally applying a regular expression pattern.
+
+        Args:
+            extra (str): The extra string to be parsed.
+            regexp (bool): A flag indicating whether to apply regular expression pattern (default is False).
+
+        Returns:
+            str: The parsed extra string.
+        """
         extra = extra.strip(".")
         if regexp:
             extra = extra.replace(".", r"\.")
             extra = r"\." + extra if extra else ""
         else:
             extra = r"." + extra if extra else ""
         return extra
 
     def make_file_name_pattern(self):
+        """Generate a file name pattern based on the steps in the pipeline.
+
+        Returns:
+            str: A regular expression pattern for creating file names based on the steps in the pipeline.
+        """
         steps_patterns = []
 
         for key in sorted(self.step.pipe.steps.keys()):
             step = self.step.pipe.steps[key]
             steps_patterns.append(rf"(?:{step.step_name})")
 
         steps_patterns = "|".join(steps_patterns)
@@ -89,14 +124,19 @@
 
         extra = self.parse_extra(self.extra, regexp=True)
 
         pattern = self.file_prefix + r"\." + self.step.pipe_name + step_pattern + extra + r"\." + self.extension
         return pattern
 
     def get_file_name(self):
+        """Return the file name based on the object attributes.
+
+        Returns:
+            str: The generated file name.
+        """
         extra = self.parse_extra(self.extra, regexp=False)
         version_string = "." + self.version if self.version else ""
         filename = (
             self.file_prefix
             + "."
             + self.step.pipe_name
             + "."
@@ -105,14 +145,19 @@
             + extra
             + "."
             + self.extension
         )
         return filename
 
     def check_disk(self):
+        """Check disk for matching files based on specified pattern and expected values.
+
+        Returns:
+            bool: True if a matching file is found, False otherwise.
+        """
         logger = logging.getLogger("pickle.check_disk")
 
         search_path = os.path.join(self.session.path, os.path.sep.join(self.collection))
         pattern = self.make_file_name_pattern()
 
         os.makedirs(search_path, exist_ok=True)
 
@@ -163,21 +208,36 @@
             logger.load(
                 f"More than one partial match was found for {self.step.relative_name}. Cannot auto select. Expected :"
                 f" {expected_values}, Found : {match_datas}"
             )
             return False
 
     def get_found_disk_object_description(self):
+        """Return the description of the found disk object."""
         return str(self.current_disk_file)
 
     def get_full_path(self):
+        """Return the full path of the file by joining the session path, collection, and file name.
+
+        Returns:
+            str: The full path of the file.
+        """
         full_path = os.path.join(self.session.path, os.path.sep.join(self.collection), self.get_file_name())
         return full_path
 
     def save(self, data):
+        """Save data to disk.
+
+        Args:
+            data: Data to be saved to disk. If data is a pandas DataFrame, it will be saved as a pickle file.
+                Otherwise, it will be pickled and saved.
+
+        Returns:
+            None
+        """
         logger = logging.getLogger("PickleDiskObject.save")
         new_full_path = self.get_full_path()
         logger.debug(f"Saving to path : {new_full_path}")
 
         if isinstance(data, pd.DataFrame):
             data.to_pickle(new_full_path)
         else:
@@ -188,14 +248,22 @@
             try:
                 os.remove(self.current_disk_file)
             except FileNotFoundError:
                 logger.error(f"The file {self.current_disk_file} that should have been removed don't exist anymore")
         self.current_disk_file = new_full_path
 
     def load(self):
+        """Load data from the current disk file.
+
+        Raises:
+            IOError: If no file was found on disk or 'check_disk()' was not run.
+
+        Returns:
+            The loaded data from the disk file.
+        """
         logger = logging.getLogger("PickleDiskObject.load")
         logger.debug(f"Current disk file status : {self.current_disk_file=}")
         if self.current_disk_file is None:
             raise IOError(
                 "Could not find a file to load. Either no file was found on disk, or you forgot to run 'check_disk()'"
             )
 
@@ -215,25 +283,45 @@
             self.save(data)
             self.is_legacy_format = False
 
         return data
 
     @staticmethod
     def multisession_packer(sessions, session_result_dict: dict) -> pd.DataFrame | dict:
+        """Packs the results of multiple sessions into a DataFrame
+            if all values in the session_result_dict are DataFrames.
+
+        Args:
+            sessions: List of sessions.
+            session_result_dict (dict): Dictionary containing the results of each session.
+
+        Returns:
+            pd.DataFrame or dict: Returns a DataFrame if all values in session_result_dict are DataFrames,
+                otherwise returns the original session_result_dict.
+        """
         session_result_dict = BaseDiskObject.multisession_packer(sessions, session_result_dict)
 
         are_dataframe = [isinstance(item, pd.core.frame.DataFrame) for item in session_result_dict.values()]
 
         if not all(are_dataframe):
             return session_result_dict
 
         return PickleDiskObject.get_multi_session_df(session_result_dict, add_session_level=False)
 
     @staticmethod
     def get_multi_session_df(multisession_data_dict: dict, add_session_level: bool = False) -> pd.DataFrame:
+        """Return a pandas DataFrame by combining multiple session dataframes.
+
+        Args:
+            multisession_data_dict (dict): A dictionary containing session names as keys and dataframes as values.
+            add_session_level (bool, optional): Whether to add session level to the index. Defaults to False.
+
+        Returns:
+            pd.DataFrame: A combined dataframe containing data from all sessions.
+        """
         dataframes = []
         for session_name, dataframe in multisession_data_dict.items():
             level_names = list(dataframe.index.names)
 
             dataframe = dataframe.reset_index()
 
             if add_session_level:
@@ -253,14 +341,23 @@
             dataframes.append(dataframe)
 
         multisession_dataframe = pd.concat(dataframes)
         return multisession_dataframe
 
     @staticmethod
     def merge_index_element(values: tuple | str | float | int, session_name: str) -> tuple:
+        """Merge the elements of the input values with the session name.
+
+        Args:
+            values (tuple | str | float | int): The values to be merged with the session name.
+            session_name (str): The name of the session to be merged with the values.
+
+        Returns:
+            tuple: A tuple containing the merged values with the session name.
+        """
         if not isinstance(values, tuple):
             values = (values,)
 
         new_values = []
         for value in values:
             value = str(value) + "_" + session_name
             new_values.append(value)
@@ -301,14 +398,22 @@
 
     if levels == -1:
         levels = 32767
     current_level = 0
     output_list = []
 
     def _recursive_search(_input_path):
+        """Recursively search for files and directories in the given input path.
+
+        Args:
+            _input_path (str): The input path to start the recursive search from.
+
+        Returns:
+            None
+        """
         nonlocal current_level
         for subdir in os.listdir(_input_path):
             fullpath = os.path.join(_input_path, subdir)
             if os.path.isfile(fullpath):
                 if (get == "all" or get == "files") and (re_pattern is None or qregexp(re_pattern, fullpath)):
                     output_list.append(os.path.normpath(fullpath))
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/pipelines.py` & `processing_pypelines-0.0.56/src/pypelines/pipelines.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,39 @@
 
 
 class Pipeline:
     pipes: Dict[str, "BasePipe"]
     runner_backend_class = BaseTaskBackend
 
     def __init__(self, name: str, **runner_args):
+        """Initialize the pipeline with the given name and runner arguments.
+
+        Args:
+            name (str): The name of the pipeline.
+            **runner_args: Additional keyword arguments for the runner backend.
+
+        Attributes:
+            pipeline_name (str): The name of the pipeline.
+            pipes (dict): Dictionary to store pipeline components.
+            resolved (bool): Flag to indicate if the pipeline is resolved.
+            runner_backend: The runner backend object created with the provided arguments.
+                If creation fails, it evaluates to False as a boolean.
+        """
         self.pipeline_name = name
         self.pipes = {}
         self.resolved = False
 
         # create a runner backend, if fails, the runner_backend object evaluates to False as a boolean
         # (to be checked and used througout the pipeline wrappers creation)
         self.runner_backend = self.runner_backend_class(self, **runner_args)
 
     def register_pipe(self, pipe_class: Type["BasePipe"]) -> Type["BasePipe"]:
         """Wrapper to instanciate and attache a a class inheriting from BasePipe it to the Pipeline instance.
-        The Wraper returns the class without changing it."""
+        The Wraper returns the class without changing it.
+        """
         instance = pipe_class(self)
 
         # attaches the instance itself to the pipeline, and to the dictionnary 'pipes' of the current pipeline
         # if instance.single_step:
         #     # in case it's a single_step instance (speficied by the user, not auto detected)
         #     # then we attach the step to the pipeline directly as a pipe, for ease of use.
         #     step = list(instance.steps.values())[0]
@@ -43,14 +57,25 @@
         self.pipes[instance.pipe_name] = instance
         setattr(self, instance.pipe_name, instance)
 
         self.resolved = False
         return pipe_class
 
     def resolve_instance(self, instance_name: str) -> "BaseStep":
+        """Resolve the specified instance name to a BaseStep object.
+
+        Args:
+            instance_name (str): The name of the instance in the format 'pipe_name.step_name'.
+
+        Returns:
+            BaseStep: The BaseStep object corresponding to the instance name.
+
+        Raises:
+            KeyError: If the specified instance name is not found in the pipeline.
+        """
         pipe_name, step_name = instance_name.split(".")
         try:
             pipe = self.pipes[pipe_name]
             # if pipe.single_step:
             #    return pipe
             return pipe.steps[step_name]
         except KeyError as exc:
@@ -135,10 +160,11 @@
         recurse_requirement_stack(instance)
         if names:
             required_steps = [req.relative_name for req in required_steps]
         return required_steps
 
     @property
     def graph(self) -> "PipelineGraph":
+        """Return a PipelineGraph object representing the graph of the pipeline."""
         from .graphs import PipelineGraph
 
         return PipelineGraph(self)
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/pipes.py` & `processing_pypelines-0.0.56/src/pypelines/pipes.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,14 +25,42 @@
     step_class: Type[BaseStep] = BaseStep
     disk_class: Type[BaseDiskObject] = BaseDiskObject
     multisession_class: Type[BaseMultisessionAccessor] = BaseMultisessionAccessor
 
     steps: Dict[str, BaseStep]
 
     def __init__(self, parent_pipeline: "Pipeline") -> None:
+        """Initialize the Pipeline object with the parent pipeline and set up the steps based on the methods decorated
+        with @stepmethod.
+
+        Args:
+            parent_pipeline (Pipeline): The parent pipeline object.
+
+        Raises:
+            ValueError: If no step class is registered with @stepmethod decorator, or if single_step is set to
+                True with more than one step, or if steps are not linked in hierarchical order.
+
+        Notes:
+            - The step methods must inherit from BaseStep.
+            - The steps should be linked in hierarchical order with `requires` specification for at least N-1 steps
+                in a single pipe.
+
+        Syntaxic sugar:
+            - If the pipe is a single step, accessing any pipe instance in the pipeline can be done by iterating on
+                pipeline.pipes.pipe.
+
+        Attributes:
+            pipeline (Pipeline): The parent pipeline object.
+            pipe_name (str): The name of the pipeline.
+            steps (Dict[str, BaseStep]): Dictionary containing the step objects.
+            pipe: A reference to the pipeline object.
+
+        Returns:
+            None
+        """
         self.pipeline = parent_pipeline
         self.pipe_name = self.__class__.__name__
 
         _steps: Dict[str, MethodType] = {}
         # this loop populates self.steps dictionnary from the instanciated (bound) step methods.
         for step_name, step in inspect.getmembers(self, predicate=inspect.ismethod):
             if getattr(step, "is_step", False):
@@ -72,27 +100,44 @@
         # below is just a syntaxic sugar to help in case the pipe is "single_step"
         # so that we can access any pipe instance in pipeline with simple iteration on
         # pipeline.pipes.pipe, whatever if the object in pipelines.pipes is a step or a pipe
         self.pipe = self
 
     @property
     def version(self):
+        """Return a hash representing the versions of all steps in the object.
+
+        Returns:
+            str: A 7-character hexadecimal hash representing the versions of all steps.
+        """
         versions = []
         for step in self.steps.values():
             versions.append(str(step.version))
         versions_string = "/".join(versions)
 
         m = hashlib.sha256()
         r = versions_string.encode()
         m.update(r)
         version_hash = m.hexdigest()[0:7]
 
         return version_hash
 
     def get_levels(self, selfish=True):
+        """Get the levels of each step in the pipeline.
+
+        Args:
+            selfish (bool, optional): Flag to indicate if the levels should be calculated selfishly. Defaults to True.
+
+        Returns:
+            dict: A dictionary containing the steps as keys and their corresponding levels as values.
+
+        Raises:
+            ValueError: If there are multiple steps with the same level and the saving backend doesn't
+                support multi-step version identification.
+        """
         levels = {}
         for step in self.steps.values():
             levels[step] = step.get_level(selfish=selfish)
 
         # if checking step levels internal to a single pipe,
         # we disallow several steps having identical level if the saving backend doesn't allow
         # for multi-step version identification
@@ -104,31 +149,60 @@
                     f"The disk backend {self.disk_class} does not support multi step (step_traceback attribute). All"
                     f" steps of the pipe {self.pipe_name} must then be hierarchically organized"
                 )
 
         return levels
 
     def __repr__(self) -> str:
+        """Return a string representation of the PipeObject in the format: "<BaseClassName.pipe_name PipeObject>".
+
+        Returns:
+            str: A string representation of the PipeObject.
+        """
         return f"<{self.__class__.__bases__[0].__name__}.{self.pipe_name} PipeObject>"
 
     # @abstractmethod
     # def disk_step(self, session : Session, extra = "") -> BaseStep :
     #     #simply returns the pipe's (most recent in the step requirement order)
     # step instance that corrresponds to the step that is found on the disk
     #     return None
 
     def dispatcher(self, function: Callable, dispatcher_type):
+        """Dispatches the given function based on the dispatcher type.
+
+        Args:
+            function (Callable): The function to be dispatched.
+            dispatcher_type: The type of dispatcher to be used.
+
+        Returns:
+            Callable: A wrapped function based on the dispatcher type.
+        """
         # the dispatcher must be return a wrapped function
         return function
 
     def pre_run_wrapper(self, function: Callable):
+        """Return a wrapped function by the dispatcher."""
         # the dispatcher must be return a wrapped function
         return function
 
     def load(self, session, extra="", which: Literal["lowest", "highest"] = "highest"):
+        """Load a step object for a session with optional extra data.
+
+        Args:
+            session: The session object to load the step for.
+            extra (str, optional): Additional data to pass to the step object. Defaults to "".
+            which (Literal["lowest", "highest"], optional): Determines whether to load the lowest or highest step.
+                Defaults to "highest".
+
+        Returns:
+            The loaded step object.
+
+        Raises:
+            ValueError: If no matching step object is found for the session.
+        """
         if which == "lowest":
             reverse = False
         else:
             reverse = True
 
         ordered_steps = sorted(
             list(self.steps.values()), key=lambda item: item.get_level(selfish=True), reverse=reverse
```

### Comparing `processing-pypelines-0.0.55/src/pypelines/steps.py` & `processing_pypelines-0.0.56/src/pypelines/steps.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,14 +38,23 @@
         callable : the callable with extra attributes attached
     """
 
     # This  allows method  to register class methods inheriting of BasePipe as steps.
     # It basically just step an "is_step" stamp on the method that are defined as steps.
     # This stamp will later be used in the metaclass __new__ to set additionnal usefull attributes to those methods
     def registrate(function: Callable):
+        """Registers a function as a step in a process.
+
+        Args:
+            function (Callable): The function to be registered as a step.
+
+        Returns:
+            Callable: The registered function with additional attributes such as 'requires', 'is_step', 'version',
+                'do_dispatch', 'step_name', and 'callbacks'.
+        """
         function.requires = [requires] if not isinstance(requires, list) else requires
         function.is_step = True
         function.version = version
         function.do_dispatch = do_dispatch
         function.step_name = function.__name__
         function.callbacks = [on_save_callbacks] if not isinstance(on_save_callbacks, list) else on_save_callbacks
         return function
@@ -69,14 +78,33 @@
 
     def __init__(
         self,
         pipeline: "Pipeline",
         pipe: "BasePipe",
         worker: MethodType,
     ):
+        """Initialize a BaseStep object.
+
+        Args:
+            pipeline (Pipeline): The parent pipeline object.
+            pipe (BasePipe): The parent pipe object.
+            worker (MethodType): The worker method associated with this step.
+
+        Attributes:
+            pipeline (Pipeline): An instance of the parent pipeline.
+            pipe (BasePipe): An instance of the parent pipe.
+            worker (MethodType): An instance of the worker method.
+            do_dispatch: The do_dispatch attribute of the worker method.
+            version: The version attribute of the worker method.
+            requires: The requires attribute of the worker method.
+            step_name: The step_name attribute of the worker method.
+            callbacks: The callbacks attribute of the worker method.
+            multisession: An instance of the multisession class associated with the pipe.
+            task: The task manager created by the runner backend of the pipeline.
+        """
         # save an instanciated access to the pipeline parent
         self.pipeline = pipeline
         # save an instanciated access to the pipe parent
         self.pipe = pipe
         # save an instanciated access to the step function (undecorated)
         self.worker = worker
 
@@ -98,75 +126,141 @@
 
         self.multisession = self.pipe.multisession_class(self)
 
         self.task = self.pipeline.runner_backend.create_task_manager(self)
 
     @property
     def requirement_stack(self) -> Callable:
+        """Return a partial function that calls the get_requirement_stack method of the pipeline
+        attribute with the instance set to self.
+        """
         return partial(self.pipeline.get_requirement_stack, instance=self)
 
     @property
     def pipe_name(self) -> str:
+        """Return the name of the pipe."""
         return self.pipe.pipe_name
 
     @property
     def relative_name(self) -> str:
+        """Return the relative name of the object by concatenating the pipe name and step name."""
         return f"{self.pipe_name}.{self.step_name}"
 
     @property
     def pipeline_name(self) -> str:
+        """Return the name of the pipeline."""
         return self.pipe.pipeline.pipeline_name
 
     @property
     def complete_name(self) -> str:
+        """Return the complete name by combining the pipeline name and relative name."""
         return f"{self.pipeline_name}.{self.relative_name}"
 
     def disk_step(self, session, extra=""):
+        """Retrieve the disk object and return the disk step instance."""
         disk_object = self.get_disk_object(session, extra)
         return disk_object.disk_step_instance()
 
     def __call__(self, *args, **kwargs):
+        """Call the worker method with the given arguments and keyword arguments."""
         return self.worker(*args, **kwargs)
 
     def __repr__(self):
+        """Return a string representation of the StepObject in the format: "<pipe_name.step_name StepObject>"."""
         return f"<{self.pipe_name}.{self.step_name} StepObject>"
 
     @property
     def load(self):
+        """Load data using the get_load_wrapped method."""
         return self.get_load_wrapped()
 
     @property
     def save(self):
+        """Save the current state of the object.
+
+        Returns:
+            The saved state of the object.
+        """
         return self.get_save_wrapped()
 
     @property
     def generate(self):
+        """Return the result of calling the get_generate_wrapped method."""
         return self.get_generate_wrapped()
 
     # def make_wrapped_functions(self):
     #     self.save = self.make_wrapped_save()
     #     self.load = self.make_wrapped_load()
     #     self.generate = self.make_wrapped_generate()
 
     def get_save_wrapped(self):
+        """Returns a wrapped function that saves data using the disk class.
+
+        This function wraps the save method of the disk class with additional functionality.
+
+        Args:
+            session: The session to use for saving the data.
+            data: The data to be saved.
+            extra: Additional information to be used during saving (default is None).
+
+        Returns:
+            The wrapped function that saves the data using the disk class.
+        """
+
         @wraps(self.pipe.disk_class.save)
         def wrapper(session, data, extra=None):
+            """Wrapper function to save data to disk.
+
+            Args:
+                session: The session object.
+                data: The data to be saved.
+                extra: Additional information (default is None).
+
+            Returns:
+                The result of saving the data to disk.
+            """
             if extra is None:
                 extra = self.get_default_extra()
             self.pipeline.resolve()
             disk_object = self.get_disk_object(session, extra)
             return disk_object.save(data)
 
         if self.do_dispatch:
             return self.pipe.dispatcher(wrapper, "saver")
         return wrapper
 
     def get_load_wrapped(self):
+        """Get a wrapped function for loading disk objects.
+
+        This function wraps the load method of the disk class with the provided session, extra, and strict parameters.
+
+        Args:
+            session: The session to use for loading the disk object.
+            extra: Additional parameters for loading the disk object (default is None).
+            strict: A boolean flag indicating whether to strictly load the disk object (default is False).
+
+        Returns:
+            The wrapped function for loading disk objects.
+        """
+
         @wraps(self.pipe.disk_class.load)
         def wrapper(session, extra=None, strict=False):
+            """Wrapper function to load disk object with session and optional extra parameters.
+
+            Args:
+                session: The session to use for loading the disk object.
+                extra (optional): Extra parameters to be passed for loading the disk object. Defaults to None.
+                strict (bool, optional): Flag to indicate strict loading. Defaults to False.
+
+            Returns:
+                The loaded disk object.
+
+            Raises:
+                ValueError: If the disk object does not match and has a status message.
+            """
             # print("extra in load wrapper : ", extra)
             if extra is None:
                 extra = self.get_default_extra()
             # print("extra in load wrapper after None : ", extra)
             self.pipeline.resolve()
             disk_object = self.get_disk_object(session, extra)
             if not disk_object.is_matching():
@@ -174,32 +268,73 @@
             return disk_object.load()
 
         if self.do_dispatch:
             return self.pipe.dispatcher(wrapper, "loader")
         return wrapper
 
     def get_generate_wrapped(self):
+        """Return the wrapped generation mechanism with optional dispatching.
+
+        Returns:
+            The wrapped generation mechanism with optional dispatching.
+        """
         if self.do_dispatch:
             return autoload_arguments(
                 self.pipe.dispatcher(loggedmethod(self.generation_mechanism), "generator"),
                 self,
             )
         return autoload_arguments(loggedmethod(self.generation_mechanism), self)
 
     def get_level(self, selfish=False) -> int:
+        """Get the level of the step.
+
+        Args:
+            selfish (bool): Whether to calculate the level selfishly. Defaults to False.
+
+        Returns:
+            int: The level of the step.
+        """
         self.pipeline.resolve()
         return StepLevel(self).resolve_level(selfish=selfish)
 
     def get_disk_object(self, session, extra=None):
+        """Return a disk object based on the provided session and optional extra parameters.
+
+        Args:
+            session: The session to use for creating the disk object.
+            extra (optional): Additional parameters to be passed to the disk object. Defaults to None.
+
+        Returns:
+            Disk: A disk object created using the provided session and extra parameters.
+        """
         if extra is None:
             extra = self.get_default_extra()
         return self.pipe.disk_class(session, self, extra)
 
     @property
     def generation_mechanism(self):
+        """Generates a wrapper function for the given worker function with additional functionality such as skipping,
+        refreshing, checking requirements, and saving output to file.
+
+        Args:
+            session: The session object.
+            *args: Positional arguments for the worker function.
+            extra: Additional argument for the worker function (default is None).
+            skip: If True, the step doesn't get loaded if found on the drive (default is False).
+            refresh: If True, the step's value gets refreshed instead of used from a file (default is False).
+            refresh_requirements: If True, refreshes all requirements; if list of strings, refreshes specific
+                steps/pipes (default is False).
+            check_requirements: If True, checks requirements with skip=True (default is False).
+            save_output: If False, doesn't save the output to file after calculation (default is True).
+            **kwargs: Additional keyword arguments for the worker function.
+
+        Returns:
+            The wrapper function with extended functionality.
+        """
+
         @wraps(self.worker)
         def wrapper(
             session,
             *args,
             extra=None,
             skip=False,
             refresh=False,
@@ -431,14 +566,20 @@
         # Replace the wrapper function's signature with the new one
         wrapper.__signature__ = original_signature.replace(parameters=original_params)
         wrapper.__doc__ = self.generate_doc()
 
         return wrapper
 
     def generate_doc(self) -> str:
+        """Generate a new docstring by inserting a chapter about Pipeline Args before the existing
+        docstring of the function.
+        If the existing docstring contains 'Raises' or 'Returns', the new chapter will be inserted before that.
+        If not, it will be inserted at the end of the existing docstring.
+        """
+
         new_doc = ""
         doc = self.worker.__doc__
         if doc is None:
             return new_doc
         lines = doc.split("\n")
         lines_count = len(lines)
         inserted_chapter = False
@@ -499,34 +640,70 @@
         if param is None:
             raise ValueError(f"Parameter extra not found in function {self.relative_name}")
         if param.default is param.empty:
             raise ValueError("Parameter extra does not have a default value")
         return param.default
 
     def is_refresh_in_kwargs(self):
+        """Check if the 'refresh' parameter is present in the keyword arguments of the function.
+
+        Returns:
+            bool: True if the 'refresh' parameter is present, False otherwise.
+        """
         sig = inspect.signature(self.worker)
         param = sig.parameters.get("refresh")
         if param is None:
             return False
         return True
 
     def load_requirement(self, pipe_name, session, extra=None):
+        """Load the specified requirement step for the given pipe name.
+
+        Args:
+            pipe_name (str): The name of the pipe for which the requirement step needs to be loaded.
+            session: The session to be used for loading the requirement step.
+            extra (optional): Any extra information to be passed while loading the requirement step.
+
+        Returns:
+            The loaded requirement step.
+
+        Raises:
+            IndexError: If the required step with the specified pipe name is not found in the requirement stack.
+        """
         try:
             req_step = [step for step in self.requirement_stack() if step.pipe_name == pipe_name][-1]
         except IndexError as e:
             raise IndexError(
                 f"Could not find a required step with the pipe_name {pipe_name} for the step {self.relative_name}. "
                 "Are you sure it figures in the requirement stack ?"
             ) from e
         return req_step.load(session, extra=extra)
 
     def set_arguments(self, session, **arguments):
+        """Set the arguments for the session.
+
+        Args:
+            session: The session to set the arguments for.
+            **arguments: Additional keyword arguments to set.
+
+        Raises:
+            NotImplementedError: This method is not implemented and should be overridden in a subclass.
+        """
         raise NotImplementedError
 
     def get_arguments(self, session):
+        """Get the arguments for the specified session.
+
+        Args:
+            self: The object instance.
+            session: The session for which arguments need to be retrieved.
+
+        Raises:
+            NotImplementedError: This method must be implemented in a subclass.
+        """
         raise NotImplementedError
 
 
 @dataclass
 class StepLevel:
     """A class used to represent the level of a Step.
     This class helps track and manage step dependencies in a pipeline.
```

### Comparing `processing-pypelines-0.0.55/tests/tests.py` & `processing_pypelines-0.0.56/tests/tests.py`

 * *Files identical despite different names*

