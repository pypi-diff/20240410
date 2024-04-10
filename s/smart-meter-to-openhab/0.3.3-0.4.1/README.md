# Comparing `tmp/smart_meter_to_openhab-0.3.3.tar.gz` & `tmp/smart_meter_to_openhab-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_to_openhab-0.3.3.tar", max compression
+gzip compressed data, was "smart_meter_to_openhab-0.4.1.tar", max compression
```

## Comparing `smart_meter_to_openhab-0.3.3.tar` & `smart_meter_to_openhab-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/LICENSE
--rw-r--r--   0        0        0     4538 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/README.md
--rw-r--r--   0        0        0      793 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      543 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/.env.example
--rw-r--r--   0        0        0      154 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/__init__.py
--rw-r--r--   0        0        0     9335 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/interfaces.py
--rw-r--r--   0        0        0     5645 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/openhab.py
--rw-r--r--   0        0        0     5694 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_iskra_mt175.py
--rw-r--r--   0        0        0     3531 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_reader.py
--rw-r--r--   0        0        0      168 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/utils.py
--rw-r--r--   0        0        0     6492 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab_scripts/main.py
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4538 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/README.md
+-rw-r--r--   0        0        0      793 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/.env.example
+-rw-r--r--   0        0        0      154 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/__init__.py
+-rw-r--r--   0        0        0     9319 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/interfaces.py
+-rw-r--r--   0        0        0     7092 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/openhab.py
+-rw-r--r--   0        0        0     8158 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_iskra_mt175.py
+-rw-r--r--   0        0        0     3531 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_reader.py
+-rw-r--r--   0        0        0      168 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/utils.py
+-rw-r--r--   0        0        0     6448 2024-04-10 10:11:54.776368 smart_meter_to_openhab-0.4.1/smart_meter_to_openhab_scripts/main.py
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.4.1/PKG-INFO
```

### Comparing `smart_meter_to_openhab-0.3.3/LICENSE` & `smart_meter_to_openhab-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.3/README.md` & `smart_meter_to_openhab-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.3/pyproject.toml` & `smart_meter_to_openhab-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smart_meter_to_openhab"
-version = "0.3.3"
+version = "0.4.1"
 description = "Pushing data of ISKRA MT175 smart meter to openhab"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smart-meter-to-openhab"
 readme = "README.md"
 packages = [
     {include = "smart_meter_to_openhab"},
     {include = "smart_meter_to_openhab_scripts"}
```

### Comparing `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/.env.example` & `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/.env.example`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/interfaces.py` & `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     
     def value_list(self) -> List[Any]:
         # consider only the values that really will be used (oh_item name not empty)
         return [oh_item_value.value for oh_item_value in self._oh_items_and_values  if oh_item_value.oh_item]
     
     def __eq__(self, other) -> bool:
         if isinstance(other, OhItemAndValueContainer):
-            return self._oh_items_and_values == other._oh_items_and_values
+            return self.value_list() == other.value_list()
         return False
     
     @staticmethod    
     def create_container(values : List[OhItemAndValue], oh_item_names : Tuple[str,...]) -> OhItemAndValueContainer:
         value_container=OhItemAndValueContainer(oh_item_names)
         value_container.assign_values(values)
         return value_container
```

### Comparing `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/openhab.py` & `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/openhab.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,52 @@
 from statistics import median
 from .interfaces import *
 
 # disable warnings about insecure requests because ssl verification is disabled
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+def _convert_list_to_smart_meter_values(oh_item_names : SmartMeterOhItemNames, 
+                                       list_values : List[List[float]]) -> List[SmartMeterValues]:
+    smart_meter_values : List[SmartMeterValues] = []
+    valid_items=[item for item in oh_item_names if item]
+    for value_index in range(len(list_values[0]) if list_values else 0):
+        item_value_list : List[OhItemAndValue] = []
+        for item_index, item in enumerate(valid_items):
+            item_value_list.append(OhItemAndValue(item, list_values[item_index][value_index]))
+        smart_meter_values.append(SmartMeterValues.create(item_value_list))
+    return smart_meter_values
+
+def _check_if_updated(values : List[SmartMeterValues], default : Union[SmartMeterValues, None] = None) -> bool:
+    valid_default=default is not None and default.is_valid()
+    valid_values=[value for value in values if value.is_valid()]
+    for value in valid_values:
+        if valid_default and value == default: # consider a valid default value as updated
+            return True
+        elif value != valid_values[0]:
+            return True
+    return False
+
+def _get_median(oh_item_names : SmartMeterOhItemNames, list_values : List[List[float]]) -> SmartMeterValues:
+    smart_meter_values : List[OhItemAndValue] = []
+    value_index=0
+    for item in oh_item_names:
+        if item:
+            avg_value = median(list_values[value_index]) if len(list_values[value_index]) > 1 else None
+            smart_meter_values.append(OhItemAndValue(item, avg_value))
+            value_index+=1
+    return SmartMeterValues.create(smart_meter_values)
+
 class OpenhabConnection():
     def __init__(self, oh_host : str, oh_user : str, oh_passwd : str, logger : Logger) -> None:
         self._oh_host=oh_host
         self._session=requests.Session()
         if oh_user:
             self._session.auth=HTTPBasicAuth(oh_user, oh_passwd)
-        retries=Retry(total=5,
+        retries=Retry(total=10,
                 backoff_factor=0.1,
                 status_forcelist=[ 500, 502, 503, 504 ])
         self._session.mount('http://', HTTPAdapter(max_retries=retries))
         self._session.mount('https://', HTTPAdapter(max_retries=retries))
         self._session.headers={'Content-Type': 'text/plain'}
         self._logger=logger
 
@@ -75,28 +106,22 @@
                         else:
                             values=[float(data['state']) for data in response.json()['data']]
                 except requests.exceptions.RequestException as e:
                     self._logger.warning("Caught Exception while getting persistence data from openHAB: " + str(e))
                 pers_values.append(values)
         return pers_values
 
-    def check_if_updated(self, oh_item_names : Tuple[str, ...], timedelta : datetime.timedelta, 
-                         default : Union[SmartMeterValues, ExtendedSmartMeterValues, None] = None) -> bool:
+    def check_if_persistence_values_updated(self, oh_item_names : SmartMeterOhItemNames, timedelta : datetime.timedelta, 
+                         default : Union[SmartMeterValues, None] = None) -> bool:
         pers_values=self._get_persistence_values(oh_item_names, timedelta)
-        for values in pers_values:
-            if default is not None and default.is_valid() and any(i == default for i in values): # consider a valid default value as updated
-                return True
-            elif any(i != values[0] for i in values):
-                return True
-        return False
+        if pers_values and any(len(values) != len(pers_values[0]) for values in pers_values):
+            # return True in case the input lists are of unequal size
+            # NOTE: This happens if the GET/POST requests to Openhab have not been completely successful.
+            return True
+        
+        smart_meter_values=_convert_list_to_smart_meter_values(oh_item_names, pers_values)
+        return _check_if_updated(smart_meter_values, default)
 
-    def get_median_from_items(self, oh_item_names : SmartMeterOhItemNames, timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
-        smart_meter_values : List[OhItemAndValue] = []
+    def get_median_from_items(self, oh_item_names : SmartMeterOhItemNames, 
+                              timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
         pers_values=self._get_persistence_values(oh_item_names, timedelta)
-        value_index=0
-        for item in oh_item_names:
-            if item:
-                avg_value = median(pers_values[value_index]) if len(pers_values[value_index]) > 10 else None
-                smart_meter_values.append(OhItemAndValue(item, avg_value))
-                value_index+=1
-        return SmartMeterValues.create(smart_meter_values)
-
+        return _get_median(oh_item_names, pers_values)
```

### Comparing `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_reader.py` & `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab/sml_reader.py`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab_scripts/main.py` & `smart_meter_to_openhab-0.4.1/smart_meter_to_openhab_scripts/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,57 +34,56 @@
     
 def create_args_parser() -> argparse.ArgumentParser:
     parser=argparse.ArgumentParser(description=f"A tool to push data of ISKRA MT175 smart meter to openHAB. Version {__version__}")
     parser.add_argument("--dotenv_path", type=Path, required=False, help=f"Provide the required environment variables in this .env file \
                         or by any other means (e.g. in your ~/.profile)")
     parser.add_argument("-c", "--smart_meter_read_count", type=int, required=False, default=5, 
                         help="Specifies the number of performed reads that are averaged per interval. Between each read is a sleep of 1 sec.")
-    parser.add_argument("--interval_in_sec", type=int, required=False, default=10, help="Interval in which the data will be read and pushed")
-    parser.add_argument("--ping_in_min", type=int, required=False, default=10, help="Reinit if no data can be found in the openHAB DB in the given timeframe")
     parser.add_argument("--max_reinit", type=int, required=False, default=5, help="Exit process with Return Code 1 when pinging stays unsuccessful.")
     parser.add_argument('--uhubctl', action='store_true', help="Use uhubctl to power off and on the usb port on reinit")
     parser.add_argument("--logfile", type=Path, required=False, help="Write logging to this file instead of to stdout")
+    parser.add_argument("--raw_data_dump_dir", type=Path, required=False, help="Dump raw data of unsuccessful reads to this folder.")
     parser.add_argument('-v', '--verbose', action='count', default=0)
     return parser
 
 def _exec_process(params : List[str]) -> None:
     result = subprocess.run(params, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     rc=result.returncode
     if rc != 0:
         raise Exception("Failed to execute command "+ ' '.join(params)+". Return code was: "+str(result.returncode))
 
-def _run(process_start_time : datetime, logger : logging.Logger, read_count : int, interval_in_sec : int, ping_in_min : int, use_uhubctl : bool) -> bool:
+def _run(process_start_time : datetime, logger : logging.Logger, read_count : int, use_uhubctl : bool, 
+         raw_data_dump_dir : Union[Path, None] = None) -> bool:
     from smart_meter_to_openhab.openhab import OpenhabConnection
     from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175OneWay
     from smart_meter_to_openhab.sml_reader import SmlReader
-    from smart_meter_to_openhab.interfaces import SmartMeterValues, ExtendedSmartMeterValues
+    from smart_meter_to_openhab.interfaces import SmartMeterValues
 
     oh_user=os.getenv('OH_USER') if 'OH_USER' in os.environ else ''
     oh_passwd=os.getenv('OH_PASSWD') if 'OH_PASSWD' in os.environ else ''
     oh_connection = OpenhabConnection(os.getenv('OH_HOST'), oh_user, oh_passwd, logger) # type: ignore
-    sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger)
+    sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger, raw_data_dump_dir)
     sml_reader = SmlReader(logger)
     logger.info("Connections established. Starting to transfer smart meter values to openhab.")
-    ping_timedelta = timedelta(minutes=ping_in_min)
+    ping_timedelta = timedelta(seconds=read_count*sml_iskra.estimated_max_read_time_in_sec*2.5)
+    logger.info(f"Calculated ping_timedelta is {ping_timedelta}. Process will be reinit if no data change is detected in the openHAB DB in the given timeframe.")
     ping_succeeded=False
     while True:
         logger.info("Reading SML data")
         ref_smart_meter_value=oh_connection.get_median_from_items(SmartMeterValues.oh_item_names())
         values, extended_values=sml_reader.read_avg_from_sml_and_compute_extended_values(sml_iskra, read_count, 
                                                                                          ref_values=ref_smart_meter_value)
         logger.info(f"current values: {values}")
         logger.info(f"current extended values: {extended_values}")
         oh_connection.post_to_items(values)
         oh_connection.post_to_items(extended_values)
         logger.info("Values posted to openHAB")
-        sleep(interval_in_sec) # TODO: rm this variable?
         # start pinging after process is running for the specified time
         if (datetime.now() - process_start_time) > ping_timedelta:
-            if not (oh_connection.check_if_updated(SmartMeterValues.oh_item_names(), ping_timedelta, default=sml_iskra.default) 
-                    and oh_connection.check_if_updated(ExtendedSmartMeterValues.oh_item_names(), ping_timedelta)):
+            if not oh_connection.check_if_persistence_values_updated(SmartMeterValues.oh_item_names(), ping_timedelta, default=sml_iskra.default):
                 break
             ping_succeeded=True
             logger.info("openHAB items ping successful.")
     
     if use_uhubctl:
         logger.error("openHAB items seem to have not been updated - Power off and on usb ports and reinit process")
         # TODO: sudo reboot seems to help a lot more. But lets try this first
@@ -101,18 +100,19 @@
     if args.dotenv_path:
         load_dotenv(dotenv_path=args.dotenv_path)
     logger=create_logger(args.logfile)
     logger.setLevel(logging.INFO)
     logger.info(f"Starting smart_meter_to_openhab version {__version__}")
     logger.setLevel(log_level_from_arg(args.verbose))
     try:
+        raw_data_dump_dir=args.raw_data_dump_dir if args.raw_data_dump_dir else None
         process_start_time=datetime.now()
         unsuccessful_reinit_count=0
         while unsuccessful_reinit_count < args.max_reinit:
-            if _run(process_start_time, logger, args.smart_meter_read_count, args.interval_in_sec, args.ping_in_min, args.uhubctl):
+            if _run(process_start_time, logger, args.smart_meter_read_count, args.uhubctl, raw_data_dump_dir):
                 unsuccessful_reinit_count=0
             else:
                 unsuccessful_reinit_count+=1
                 logger.error("No improvement after reinit. Trying again.")
 
     except Exception as e:
         logger.exception("Caught Exception: " + str(e))
```

### Comparing `smart_meter_to_openhab-0.3.3/PKG-INFO` & `smart_meter_to_openhab-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_to_openhab
-Version: 0.3.3
+Version: 0.4.1
 Summary: Pushing data of ISKRA MT175 smart meter to openhab
 Home-page: https://github.com/die-bauerei/smart-meter-to-openhab
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

