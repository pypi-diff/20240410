# Comparing `tmp/agentops-0.1.1.tar.gz` & `tmp/agentops-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.1.tar", last modified: Fri Apr  5 22:40:57 2024, max compression
+gzip compressed data, was "agentops-0.1.2.tar", last modified: Tue Apr  9 23:00:47 2024, max compression
```

## Comparing `agentops-0.1.1.tar` & `agentops-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 22:40:52.000000 agentops-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-05 22:40:57.348312 agentops-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-05 22:40:52.000000 agentops-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2866 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-05 22:40:52.000000 agentops-0.1.1/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 22:40:57.000000 agentops-0.1.1/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 22:40:52.000000 agentops-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:40:57.348312 agentops-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:40:57.348312 agentops-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-05 22:40:52.000000 agentops-0.1.1/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:00:47.359114 agentops-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 23:00:40.000000 agentops-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-09 23:00:47.359114 agentops-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-09 23:00:40.000000 agentops-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:00:47.355114 agentops-0.1.2/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2879 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-09 23:00:40.000000 agentops-0.1.2/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:00:47.359114 agentops-0.1.2/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-09 23:00:47.000000 agentops-0.1.2/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 23:00:47.000000 agentops-0.1.2/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:00:47.000000 agentops-0.1.2/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 23:00:47.000000 agentops-0.1.2/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 23:00:47.000000 agentops-0.1.2/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 23:00:40.000000 agentops-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:00:47.359114 agentops-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:00:47.359114 agentops-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-09 23:00:40.000000 agentops-0.1.2/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-09 23:00:40.000000 agentops-0.1.2/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-09 23:00:40.000000 agentops-0.1.2/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-09 23:00:40.000000 agentops-0.1.2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-09 23:00:40.000000 agentops-0.1.2/tests/test_teardown.py
```

### Comparing `agentops-0.1.1/LICENSE` & `agentops-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/PKG-INFO` & `agentops-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
+Requires-Dist: packaging==24.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.2 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Provides-Extra: dev Requires-
-Dist: pytest==7.4.0; extra == "dev" Requires-Dist: requests_mock==1.11.0; extra
-== "dev" Provides-Extra: langchain Requires-Dist: langchain>=0.0.354; extra ==
-"langchain"
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==24.0
+Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
+requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
+langchain>=0.0.354; extra == "langchain"
                                     [Logo]
                             _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
                      AI agents suck. Weâre fixing that.
 Build your next agent with benchmarks, observability, and replay analytics.
 AgentOps is the toolkit for evaluating and developing robust and reliable AI
 agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
 app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
```

### Comparing `agentops-0.1.1/README.md` & `agentops-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/__init__.py` & `agentops-0.1.2/agentops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     Client().end_session(end_state, end_state_reason, video)
 
 
 def start_session(tags: Optional[List[str]] = None, config: Optional[Configuration] = None):
     Client().start_session(tags, config)
 
 
-def record(event: Event):
+def record(event: Event | ErrorEvent):
     Client().record(event)
 
 
 def add_tags(tags: List[str]):
     Client().add_tags(tags)
```

### Comparing `agentops-0.1.1/agentops/agent.py` & `agentops-0.1.2/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/client.py` & `agentops-0.1.2/agentops/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             event (Event): The event to record.
         """
 
         if self._session is not None and not self._session.has_ended:
             self._worker.add_event(event.__dict__)
         else:
             logging.warning(
-                "AgentOps: Cannot record event - no current session")
+                "🖇 AgentOps: Cannot record event - no current session")
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
         # Get default values
         arg_values = {name: func_args[name].default
@@ -201,25 +201,25 @@
 
         Args:
             tags (List[str], optional): Tags that can be used for grouping or sorting later.
                 e.g. ["test_run"].
             config: (Configuration, optional): Client configuration object
         """
         if self._session is not None:
-            return logging.warning("AgentOps: Cannot start session - session already started")
+            return logging.warning("🖇 AgentOps: Cannot start session - session already started")
 
         if not config and not self.config:
-            return logging.warning("AgentOps: Cannot start session - missing configuration")
+            return logging.warning("🖇 AgentOps: Cannot start session - missing configuration")
 
         self._session = Session(uuid4(), tags or self._tags, host_env=get_host_env())
         self._worker = Worker(config or self.config)
         start_session_result = self._worker.start_session(self._session)
         if not start_session_result:
             self._session = None
-            return logging.warning("AgentOps: Cannot start session")
+            return logging.warning("🖇 AgentOps: Cannot start session")
 
         logging.info('View info on this session at https://app.agentops.ai/drilldown?session_id={}'
                      .format(self._session.session_id))
 
     def end_session(self,
                     end_state: str,
                     end_state_reason: Optional[str] = None,
@@ -229,22 +229,23 @@
 
         Args:
             end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
             end_state_reason (str, optional): The reason for ending the session.
             video (str, optional): The video screen recording of the session
         """
         if self._session is None or self._session.has_ended:
-            return logging.warning("AgentOps: Cannot end session - no current session")
+            return logging.warning("🖇 AgentOps: Cannot end session - no current session")
 
         if not any(end_state == state.value for state in EndState):
-            return logging.warning("AgentOps: Invalid end_state. Please use one of the EndState enums")
+            return logging.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
-        self._worker.end_session(self._session)
+        token_cost = float(self._worker.end_session(self._session))
+        print('🖇 AgentOps: This run cost ${:.6f}'.format(token_cost))
         self._session = None
         self._worker = None
 
     def create_agent(self, agent_id: str, name: str):
         if self._worker:
             self._worker.create_agent(agent_id, name)
 
@@ -261,15 +262,15 @@
 
             Args:
                 signum (int): The signal number.
                 frame: The current stack frame.
             """
             signal_name = 'SIGINT' if signum == signal.SIGINT else 'SIGTERM'
             logging.info(
-                f'AgentOps: {signal_name} detected. Ending session...')
+                f'🖇 AgentOps: {signal_name} detected. Ending session...')
             self.end_session(end_state='Fail',
                              end_state_reason=f'Signal {signal_name} detected')
             sys.exit(0)
 
         def handle_exception(exc_type, exc_value, exc_traceback):
             """
             Handle uncaught exceptions before they result in program termination.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agentops-0.1.1/agentops/config.py` & `agentops-0.1.2/agentops/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                  endpoint: Optional[str] = None,
                  max_wait_time: Optional[int] = None,
                  max_queue_size: Optional[int] = None):
 
         if not api_key:
             api_key = environ.get('AGENTOPS_API_KEY', None)
             if not api_key:
-                raise ConfigurationError("AgentOps: No API key provided - no data will be recorded.")
+                raise ConfigurationError("🖇 AgentOps: No API key provided - no data will be recorded.")
 
         if not parent_key:
             parent_key = environ.get('AGENTOPS_PARENT_KEY', None)
 
         if not endpoint:
             endpoint = environ.get('AGENTOPS_API_ENDPOINT', 'https://api.agentops.ai')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agentops-0.1.1/agentops/decorators.py` & `agentops-0.1.2/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/enums.py` & `agentops-0.1.2/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/event.py` & `agentops-0.1.2/agentops/event.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/helpers.py` & `agentops-0.1.2/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/host_env.py` & `agentops-0.1.2/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/http_client.py` & `agentops-0.1.2/agentops/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,29 +79,29 @@
                                        headers=JSON_HEADER, timeout=20)
 
             result.parse(res)
         except requests.exceptions.Timeout:
             result.code = 408
             result.status = HttpStatus.TIMEOUT
             logging.warning(
-                'AgentOps: Could not post data - connection timed out')
+                '🖇 AgentOps: Could not post data - connection timed out')
         except requests.exceptions.HTTPError as e:
             try:
                 result.parse(e.response)
             except:
                 result = Response()
                 result.code = e.response.status_code
                 result.status = Response.get_status(e.response.status_code)
                 result.body = {'error': str(e)}
         except requests.exceptions.RequestException as e:
             result.body = {'error': str(e)}
 
         if result.code == 401:
             logging.warning(
-                f'AgentOps: Could not post data - API server rejected your API key: {api_key}')
+                f'🖇 AgentOps: Could not post data - API server rejected your API key: {api_key}')
         if result.code == 400:
-            logging.warning(f'AgentOps: Could not post data - {result.body}')
+            logging.warning(f'🖇 AgentOps: Could not post data - {result.body}')
         if result.code == 500:
             logging.warning(
-                f'AgentOps: Could not post data - internal server error')
+                f'🖇 AgentOps: Could not post data - internal server error')
 
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agentops-0.1.1/agentops/langchain_callback_handler.py` & `agentops-0.1.2/agentops/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/llm_tracker.py` & `agentops-0.1.2/agentops/llm_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
-                    f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                    f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if inspect.isasyncgen(response):
             async def async_generator():
                 async for chunk in response:
                     handle_stream_chunk(chunk)
 
@@ -96,15 +96,15 @@
             self.llm_event.end_timestamp = get_ISO_time()
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
-                f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def _handle_response_v1_openai(self, response, kwargs, init_timestamp):
         """Handle responses for OpenAI versions >v1.0.0"""
         from openai import Stream, AsyncStream
         from openai.types.chat import ChatCompletionChunk
@@ -142,15 +142,15 @@
                     self.llm_event.end_timestamp = get_ISO_time()
 
                     self.client.record(self.llm_event)
             except Exception as e:
                 self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
                 # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
                 logging.warning(
-                    f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                    f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         # if the response is a generator, decorate the generator
         if isinstance(response, Stream):
             def generator():
                 for chunk in response:
                     handle_stream_chunk(chunk)
                     yield chunk
@@ -187,15 +187,15 @@
             self.llm_event.model = response.model
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
             # TODO: This error is specific to only one path of failure. Should be more generic or have different logging for different paths
             logging.warning(
-                f"AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
+                f"🖇 AgentOps: Unable to parse a chunk for LLM call {kwargs} - skipping upload to AgentOps")
 
         return response
 
     def override_openai_v1_completion(self):
         from openai.resources.chat import completions
 
         # Store the original method
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agentops-0.1.1/agentops/meta_client.py` & `agentops-0.1.2/agentops/meta_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 def handle_exceptions(method):
     """Decorator within the metaclass to wrap method execution in try-except block."""
 
     def wrapper(self, *args, **kwargs):
         try:
             return method(self, *args, **kwargs)
         except Exception as e:
-            logging.warning(f"AgentOps: Error: {e}")
+            logging.warning(f"🖇 AgentOps: Error: {e}")
             config = getattr(self, 'config', None)
             if config is not None:
                 type(self).send_exception_to_server(e, self.config._api_key)
             raise e
 
     return wrapper
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `agentops-0.1.1/agentops/session.py` & `agentops-0.1.2/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/agentops/worker.py` & `agentops-0.1.2/agentops/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,31 +55,33 @@
                                   self.config.parent_key)
 
             if res.code != 200:
                 return False
 
             return True
 
-    def end_session(self, session: Session) -> None:
+    def end_session(self, session: Session) -> str:
         self.stop_flag.set()
         self.thread.join(timeout=1)
         self.flush_queue()
         self._session = None
 
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
 
-            HttpClient.post(f'{self.config.endpoint}/sessions',
+            res = HttpClient.post(f'{self.config.endpoint}/sessions',
                             json.dumps(filter_unjsonable(
                                 payload)).encode("utf-8"),
                             self.config.api_key,
                             self.config.parent_key)
 
+            return res.body.get('token_cost', "unknown")
+
     def update_session(self, session: Session) -> None:
         with self.lock:
             payload = {
                 "session": session.__dict__
             }
 
             HttpClient.post(f'{self.config.endpoint}/sessions',
```

### Comparing `agentops-0.1.1/agentops.egg-info/PKG-INFO` & `agentops-0.1.2/agentops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
+Requires-Dist: packaging==24.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
 Requires-Dist: langchain>=0.0.354; extra == "langchain"
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.2 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Provides-Extra: dev Requires-
-Dist: pytest==7.4.0; extra == "dev" Requires-Dist: requests_mock==1.11.0; extra
-== "dev" Provides-Extra: langchain Requires-Dist: langchain>=0.0.354; extra ==
-"langchain"
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==24.0
+Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
+requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
+langchain>=0.0.354; extra == "langchain"
                                     [Logo]
                             _D_o_c_u_m_e_n_t_a_t_i_o_n | _D_i_s_c_o_r_d
                      AI agents suck. Weâre fixing that.
 Build your next agent with benchmarks, observability, and replay analytics.
 AgentOps is the toolkit for evaluating and developing robust and reliable AI
 agents. AgentOps is open beta. You can sign up for AgentOps [here](https://
 app.agentops.ai). [![License: MIT](https://img.shields.io/badge/License-MIT-
```

### Comparing `agentops-0.1.1/agentops.egg-info/SOURCES.txt` & `agentops-0.1.2/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/pyproject.toml` & `agentops-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
@@ -17,15 +17,16 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
-    "psutil==5.9.8"
+    "psutil==5.9.8",
+    "packaging==24.0"
 ]
 [project.optional-dependencies]
 dev = [
     "pytest==7.4.0",
     "requests_mock==1.11.0"
 ]
 langchain = [
```

### Comparing `agentops-0.1.1/tests/test_canary.py` & `agentops-0.1.2/tests/test_canary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import pytest
+import requests
 import requests_mock
 import time
 import agentops
 from agentops import ActionEvent
 
 
 @pytest.fixture
 def mock_req():
     with requests_mock.Mocker() as m:
         url = 'https://api.agentops.ai'
         m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', text='ok')
+        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
         yield m
 
-
 class TestCanary:
     def setup_method(self):
         self.url = 'https://api.agentops.ai'
         self.api_key = "random_api_key"
         agentops.init(api_key=self.api_key, max_wait_time=5, auto_start_session=False)
 
-    def teardown_method(self):
-        agentops.end_session(end_state='Success')
-
     def test_agent_ops_record(self, mock_req):
         # Arrange
         event_type = 'test_event_type'
         agentops.start_session()
         
         # Act
         agentops.record(ActionEvent(event_type))
         time.sleep(0.1)
 
         # Assert
         assert len(mock_req.request_history) == 2
         request_json = mock_req.last_request.json()
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         assert request_json['events'][0]['event_type'] == event_type
+
+        agentops.end_session('Success')
```

### Comparing `agentops-0.1.1/tests/test_patcher.py` & `agentops-0.1.2/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.1/tests/test_record_function.py` & `agentops-0.1.2/tests/test_record_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,85 +6,92 @@
 from datetime import datetime
 
 @pytest.fixture
 def mock_req():
     with requests_mock.Mocker() as m:
         url = 'https://api.agentops.ai'
         m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', text='ok')
+        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
         yield m
 
 class TestRecordAction:
     def setup_method(self):
         self.url = 'https://api.agentops.ai'
         self.api_key = "random_api_key"
         self.event_type = 'test_event_type'
         agentops.init(self.api_key, max_wait_time=5, auto_start_session=False)
-        agentops.start_session()
-
-    def teardown_method(self):
-        agentops.end_session(end_state='Success')
 
     def test_record_function_decorator(self, mock_req):
+        agentops.start_session()
+
         @record_function(event_name=self.event_type)
         def add_two(x, y):
             return x + y
 
         # Act
         add_two(3, 4)
         time.sleep(0.1)
 
         # Assert
-        assert len(mock_req.request_history) == 1
+        assert len(mock_req.request_history) == 2
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['events'][0]['action_type'] == self.event_type
         assert request_json['events'][0]['params'] == {'x': 3, 'y': 4}
         assert request_json['events'][0]['returns'] == 7
 
+        agentops.end_session(end_state='Success')
+
     def test_record_function_decorator_multiple(self, mock_req):
+        agentops.start_session()
+
         # Arrange
         @record_function(event_name=self.event_type)
         def add_three(x, y, z=3):
             return x + y + z
 
         # Act
         add_three(1, 2)
         time.sleep(0.1)
         add_three(1, 2)
         time.sleep(0.1)
 
         # Assert
-        assert len(mock_req.request_history) == 2
+        assert len(mock_req.request_history) == 3
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['events'][0]['action_type'] == self.event_type
         assert request_json['events'][0]['params'] == {'x': 1, 'y': 2, 'z': 3}
         assert request_json['events'][0]['returns'] == 6
 
+        agentops.end_session(end_state='Success')
+
     @pytest.mark.asyncio
     async def test_async_function_call(self, mock_req):
+        agentops.start_session()
 
         @record_function(self.event_type)
         async def async_add(x, y):
             time.sleep(0.1)
             return x + y
 
         # Act
         result = await async_add(3, 4)
         time.sleep(0.1)
 
         # Assert
         assert result == 7
         # Assert
-        assert len(mock_req.request_history) == 1
+        assert len(mock_req.request_history) == 2
         assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
         request_json = mock_req.last_request.json()
         assert request_json['events'][0]['action_type'] == self.event_type
         assert request_json['events'][0]['params'] == {'x': 3, 'y': 4}
         assert request_json['events'][0]['returns'] == 7
         init = datetime.fromisoformat(
             request_json['events'][0]['init_timestamp'].replace('Z', '+00:00'))
         end = datetime.fromisoformat(
             request_json['events'][0]['end_timestamp'].replace('Z', '+00:00'))
 
-        assert (end - init).total_seconds() >= 0.1
+        assert (end - init).total_seconds() >= 0.1
+
+        agentops.end_session(end_state='Success')
```

### Comparing `agentops-0.1.1/tests/test_session.py` & `agentops-0.1.2/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @pytest.fixture
 def mock_req():
     with requests_mock.Mocker() as m:
         url = 'https://api.agentops.ai'
         m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', text='ok')
+        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
         yield m
 
 
 class TestSessions:
     def setup_method(self):
         self.api_key = "random_api_key"
         self.event_type = 'test_event_type'
```

### Comparing `agentops-0.1.1/tests/test_teardown.py` & `agentops-0.1.2/tests/test_teardown.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @pytest.fixture
 def mock_req():
     with requests_mock.Mocker() as m:
         url = 'https://api.agentops.ai'
         m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', text='ok')
+        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
         yield m
 
 
 class TestSessions:
     def setup_method(self):
         self.api_key = "random_api_key"
         self.event_type = 'test_event_type'
```

