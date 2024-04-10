# Comparing `tmp/experiment_goodies-0.1.4.tar.gz` & `tmp/experiment_goodies-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment_goodies-0.1.4.tar", max compression
+gzip compressed data, was "experiment_goodies-0.2.0.tar", max compression
```

## Comparing `experiment_goodies-0.1.4.tar` & `experiment_goodies-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.1.4/experiment_goodies/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.1.4/experiment_goodies/geo/__init__.py
--rw-r--r--   0        0        0     7728 2024-03-21 18:20:53.347022 experiment_goodies-0.1.4/experiment_goodies/geo/raster.py
--rw-r--r--   0        0        0     5571 2024-03-21 18:20:53.347022 experiment_goodies-0.1.4/experiment_goodies/geo/vector.py
--rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.1.4/experiment_goodies/logger/__init__.py
--rw-r--r--   0        0        0     5193 2024-03-21 12:43:40.830253 experiment_goodies-0.1.4/experiment_goodies/logger/experiment_logger.py
--rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.1.4/experiment_goodies/logger/rainbow_logger.py
--rw-r--r--   0        0        0     1101 2024-03-21 18:24:16.020237 experiment_goodies-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1172 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/__init__.py
+-rw-r--r--   0        0        0     7728 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/raster.py
+-rw-r--r--   0        0        0     5571 2024-03-21 18:20:53.347022 experiment_goodies-0.2.0/experiment_goodies/geo/vector.py
+-rw-r--r--   0        0        0      268 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/logger/__init__.py
+-rw-r--r--   0        0        0     4189 2024-04-10 14:47:21.255719 experiment_goodies-0.2.0/experiment_goodies/logger/experiment_logger.py
+-rw-r--r--   0        0        0     5850 2024-03-21 12:43:40.830253 experiment_goodies-0.2.0/experiment_goodies/logger/rainbow_logger.py
+-rw-r--r--   0        0        0     1101 2024-04-10 14:47:21.255719 experiment_goodies-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 experiment_goodies-0.2.0/PKG-INFO
```

### Comparing `experiment_goodies-0.1.4/README.md` & `experiment_goodies-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.1.4/experiment_goodies/geo/raster.py` & `experiment_goodies-0.2.0/experiment_goodies/geo/raster.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.1.4/experiment_goodies/geo/vector.py` & `experiment_goodies-0.2.0/experiment_goodies/geo/vector.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.1.4/experiment_goodies/logger/experiment_logger.py` & `experiment_goodies-0.2.0/experiment_goodies/logger/experiment_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from experiment_goodies.logger.rainbow_logger import RainbowLoggingHandler
 
 
 class ExperimentLoggerConfig(BaseModel):
     log_level: str = "INFO"
     log_freq_steps: int = 100
     log_mlflow: bool = False
-    mlflow_experiment_id: int = None
-    mlflow_run_name: str = None
-    mlflow_run_description: str = None
-    mlflow_nested_run: bool = False
 
 
 class ExperimentLogger(Logger):
     """Extends Logger from logging library to incorporate functionalities useful during model training.
 
     Attributes:
         name (str): owner of this logger (will be printed to console)
@@ -46,40 +42,24 @@
         handler = RainbowLoggingHandler()
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         handler.setFormatter(formatter)
         self.addHandler(handler)
         self.exp_folder = exp_folder
-        if self.logger_config.log_mlflow:
-            assert (
-                self.logger_config.mlflow_experiment_id is not None
-            ), "Must provide a mlflow experiment id"
-            self.__start_mlflow_run()
 
     def __save_exp_config(self, config: dict[str, Any]):
         """Saves the configuration of this experiment"""
         with open(os.path.join(self.exp_folder, "experiment_config.json"), "w") as f:
             json.dump(config, f, indent=4)
 
-    def __start_mlflow_run(self):
-        from dotenv import load_dotenv
-
-        load_dotenv(".env")
-        mlflow.start_run(
-            experiment_id=self.logger_config.mlflow_experiment_id,
-            run_name=self.logger_config.mlflow_run_name,
-            nested=self.logger_config.mlflow_nested_run,
-            description=self.logger_config.mlflow_run_description,
-        )
-
     def log_config_to_mlflow(
         self, experiment_config: dict[str, Any], dvc_file_path: str
     ) -> mlflow.ActiveRun:
-        """Creates a new mlflow run, logging .dvc config file and experiment parameters"""
+        """Logs parameters and dvc file to mlflow"""
         mlflow.log_params(experiment_config)
         mlflow.log_artifact(dvc_file_path)
 
     def log_metrics(self, metrics: dict, epoch: int, step: int, total_step: int):
         """Logs training metrics
 
         Args:
@@ -126,13 +106,7 @@
         Args:
             exp_config (dict[str, Any]): experiment configuration to be logged
             dvc_file_path (str): path to dvc file of experiment dataset
         """
         self.__save_exp_config(exp_config)
         if self.logger_config.log_mlflow:
             self.log_config_to_mlflow(exp_config, dvc_file_path)
-
-    def end_run(self):
-        """Any clean up operations to be performed after experiment ends"""
-        self.info("Experiment ended ...")
-        if self.logger_config.log_mlflow:
-            mlflow.end_run()
```

### Comparing `experiment_goodies-0.1.4/experiment_goodies/logger/rainbow_logger.py` & `experiment_goodies-0.2.0/experiment_goodies/logger/rainbow_logger.py`

 * *Files identical despite different names*

### Comparing `experiment_goodies-0.1.4/pyproject.toml` & `experiment_goodies-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "experiment-goodies"
-version = "0.1.4"
+version = "0.2.0"
 description = "Useful helpers, callbacks and more for experimenting with ml models"
 authors = ["Javier Smith <javier.smith.dlc@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 logutils = "^0.3.5"
```

### Comparing `experiment_goodies-0.1.4/PKG-INFO` & `experiment_goodies-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-goodies
-Version: 0.1.4
+Version: 0.2.0
 Summary: Useful helpers, callbacks and more for experimenting with ml models
 Author: Javier Smith
 Author-email: javier.smith.dlc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

