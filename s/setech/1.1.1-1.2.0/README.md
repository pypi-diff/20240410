# Comparing `tmp/setech-1.1.1.tar.gz` & `tmp/setech-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.1.1.tar", last modified: Thu Apr  4 13:29:48 2024, max compression
+gzip compressed data, was "setech-1.2.0.tar", last modified: Wed Apr 10 13:58:28 2024, max compression
```

## Comparing `setech-1.1.1.tar` & `setech-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.083649 setech-1.1.1/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.1.1/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-04 13:29:48.080316 setech-1.1.1/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.1.1/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-04 13:29:41.000000 setech-1.1.1/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-04 13:29:48.083649 setech-1.1.1/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-04 13:29:41.000000 setech-1.1.1/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.1.1/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4832 2024-04-03 09:38:51.000000 setech-1.1.1/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2258 2024-04-03 09:38:51.000000 setech-1.1.1/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2163 2024-04-03 09:38:59.000000 setech-1.1.1/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.1.1/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.1.1/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      137 2024-04-04 13:28:43.000000 setech-1.1.1/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.1.1/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.1.1/src/setech/logging/handlers.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.1.1/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      933 2024-04-03 21:49:44.000000 setech-1.1.1/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      848 2024-04-03 22:46:33.000000 setech-1.1.1/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2133 2024-04-03 21:49:42.000000 setech-1.1.1/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5555 2024-04-03 14:57:53.000000 setech-1.1.1/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.1.1/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-03 15:03:11.000000 setech-1.1.1/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      874 2024-04-03 20:52:45.000000 setech-1.1.1/src/setech/utils/various.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:29:48.080316 setech-1.1.1/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-04 13:29:48.000000 setech-1.1.1/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      732 2024-04-04 13:29:48.000000 setech-1.1.1/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-04 13:29:48.000000 setech-1.1.1/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-04 13:29:48.000000 setech-1.1.1/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-04 13:29:48.000000 setech-1.1.1/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.2.0/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-10 13:58:28.427983 setech-1.2.0/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.2.0/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-10 13:58:19.000000 setech-1.2.0/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-10 13:58:28.427983 setech-1.2.0/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.424650 setech-1.2.0/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-10 13:58:19.000000 setech-1.2.0/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.2.0/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4832 2024-04-03 09:38:51.000000 setech-1.2.0/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2258 2024-04-03 09:38:51.000000 setech-1.2.0/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2163 2024-04-03 09:38:59.000000 setech-1.2.0/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.2.0/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.2.0/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.2.0/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.2.0/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.2.0/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      921 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      849 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2013 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5598 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.2.0/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-03 15:03:11.000000 setech-1.2.0/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1453 2024-04-10 13:57:32.000000 setech-1.2.0/src/setech/utils/various.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-10 13:58:28.427983 setech-1.2.0/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      732 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-10 13:58:28.000000 setech-1.2.0/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.1.1/LICENCE` & `setech-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/PKG-INFO` & `setech-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.1.1
+Version: 1.2.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.1.1/README.md` & `setech-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/pyproject.toml` & `setech-1.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.1.1"
+current_version = "1.2.0"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.1.1/src/setech/api_client/_base.py` & `setech-1.2.0/src/setech/api_client/_base.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/api_client/async_client.py` & `setech-1.2.0/src/setech/api_client/async_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/api_client/sync_client.py` & `setech-1.2.0/src/setech/api_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/constants/date.py` & `setech-1.2.0/src/setech/constants/date.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/logging/formatters.py` & `setech-1.2.0/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/logging/handlers.py` & `setech-1.2.0/src/setech/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/utils/__init__.py` & `setech-1.2.0/src/setech/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .numeric import round_decimal
 from .parse import SetechJSONEncoder, as_decimal, as_decimal_or_none, str_as_date, str_as_date_or_none
 from .ssn import generate_aged_latvian_personal_code, generate_random_latvian_personal_code
 from .text import convert_datetime_to_latvian_words, convert_number_to_latvian_words
 from .validators import validate_iban, validate_latvian_personal_code
-from .various import get_logger, get_nonce, shorten_dict_values, shortify_log_dict
+from .various import get_logger, get_nonce, shorten_value, shortify_log_dict
 
 __all__ = [
     "round_decimal",
     "SetechJSONEncoder",
     "str_as_date",
     "str_as_date_or_none",
     "as_decimal",
@@ -16,10 +16,10 @@
     "convert_number_to_latvian_words",
     "generate_aged_latvian_personal_code",
     "generate_random_latvian_personal_code",
     "validate_iban",
     "validate_latvian_personal_code",
     "get_logger",
     "get_nonce",
-    "shorten_dict_values",
+    "shorten_value",
     "shortify_log_dict",
 ]
```

### Comparing `setech-1.1.1/src/setech/utils/numeric.py` & `setech-1.2.0/src/setech/utils/numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 def round_decimal(dec: decimal.Decimal, precision: int = 4) -> decimal.Decimal:
     """Round decimal value to a predefined precision from the start of the value. Examples:
         - dec=123.456, precision=7 -> 123.4560,
         - dec=123.456, precision=5 -> 123.46,
         - dec=123.456, precision=3 -> 123,
         - dec=123.456, precision=2 -> 120;
+
     :param dec: Decimal value to round
     :param precision: how many digits since the start of the value to keep
     :return: rounded Decimal
     """
     with decimal.localcontext() as ctx:
         ctx.rounding = decimal.ROUND_HALF_UP
         value = decimal.Decimal(dec)
```

### Comparing `setech-1.1.1/src/setech/utils/parse.py` & `setech-1.2.0/src/setech/utils/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,25 +38,23 @@
     def default(self, obj: Any) -> Any:
         try:
             if isinstance(obj, decimal.Decimal):
                 return str(obj)
             if isinstance(obj, (datetime.datetime, datetime.date)):
                 return obj.isoformat()
             if isinstance(obj, BaseModel):
-                return obj.model_dump_json()
+                return obj.model_dump()
             if isinstance(obj, datetime.timedelta):
                 return dict(__type__="timedelta", total_seconds=obj.total_seconds())
+            if isinstance(obj, set):
+                return sorted(obj, key=str)
             if hasattr(obj, "as_dict"):
-                if callable(getattr(obj, "as_dict")):
-                    return super().default(obj.as_dict())
-                return super().default(obj.as_dict)
+                return obj.as_dict
             if dataclasses.is_dataclass(obj):
-                return super().default(dataclasses.asdict(obj))
-            if isinstance(obj, set):
-                return list(obj)
+                return dataclasses.asdict(obj)
             if hasattr(obj, "__dict__"):
                 return obj.__dict__
             return super().default(obj)
         except TypeError as exc:
             if "not JSON serializable" in str(exc):
                 return str(obj)
-            raise exc
+            raise exc  # pragma: no cover
```

### Comparing `setech-1.1.1/src/setech/utils/ssn.py` & `setech-1.2.0/src/setech/utils/ssn.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,19 +51,21 @@
             if years < (datetime.date.today() - FINAL_LEGACY_DATE).days // 365:
                 raise ValueError(
                     "Too young for legacy Personal Code! years < "
                     f"{(datetime.date.today() - FINAL_LEGACY_DATE).days // 365}"
                 )
             min_age_in_days = abs(years) * 365
             max_age_in_days = abs(years + 1) * 365
-            birthdate = datetime.date.today() - datetime.timedelta(days=randint(min_age_in_days, max_age_in_days))
+            birthdate = datetime.date.today() - datetime.timedelta(
+                days=randint(min_age_in_days + 1, max_age_in_days - 1)
+            )
         else:
             max_age_in_days = (FINAL_LEGACY_DATE - START_LEGACY_DATE).days
             min_age_in_days = 1
-            birthdate = FINAL_LEGACY_DATE - datetime.timedelta(days=randint(min_age_in_days, max_age_in_days))
+            birthdate = FINAL_LEGACY_DATE - datetime.timedelta(days=randint(min_age_in_days + 1, max_age_in_days - 1))
         return cls._create_from_birthday(birthdate)
 
     @classmethod
     def generate_legacy_for_birthday(cls, *args: datetime.date | int) -> "PersonalCode":
         if len(args) == 1:
             if not isinstance(args[0], datetime.date):
                 raise ValueError(
@@ -96,15 +98,15 @@
     def _create_from_birthday(cls, birthday: datetime.date) -> "PersonalCode":
         first_part = f"{birthday.day:02d}{birthday.month:02d}{str(birthday.year)[2:]}"
         century_digit = 2 if birthday.year // 2000 else 1 if birthday.year // 1900 else 0
         second_part = f"{century_digit}{randint(0, 999):03}"
         tmp = cls(first_part, second_part)
         check_digit = tmp._get_checksum_digit()
         if check_digit == 10:
-            return cls.generate_legacy_with_check_digit()
+            return cls._create_from_birthday(birthday)
         second_part = f"{second_part}{check_digit}"
         return cls(first_part, second_part, True)
 
     def as_tuple(self) -> tuple[str, str]:
         return self.first_part, self.second_part
 
     def __str__(self) -> str:
```

### Comparing `setech-1.1.1/src/setech/utils/text.py` & `setech-1.2.0/src/setech/utils/text.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech/utils/validators.py` & `setech-1.2.0/src/setech/utils/validators.py`

 * *Files identical despite different names*

### Comparing `setech-1.1.1/src/setech.egg-info/PKG-INFO` & `setech-1.2.0/src/setech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.1.1
+Version: 1.2.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.1.1/src/setech.egg-info/SOURCES.txt` & `setech-1.2.0/src/setech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

