# Comparing `tmp/supamodel-0.4.2.tar.gz` & `tmp/supamodel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.4.2.tar", max compression
+gzip compressed data, was "supamodel-0.4.3.tar", max compression
```

## Comparing `supamodel-0.4.2.tar` & `supamodel-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.4.2/README.md
--rw-r--r--   0        0        0      637 2024-04-09 23:56:27.844214 supamodel-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.4.2/supamodel/__init__.py
--rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.4.2/supamodel/_abc.py
--rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.4.2/supamodel/_client.py
--rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.4.2/supamodel/_core.py
--rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.4.2/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.4.2/supamodel/_types.py
--rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.2/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.2/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.2/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.4.2/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.2/supamodel/supa_model.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.2/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.2/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.2/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.2/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.2/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.4.2/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.4.2/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.4.2/supamodel/utils.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 supamodel-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3741 2024-04-10 02:14:13.207577 supamodel-0.4.3/README.md
+-rw-r--r--   0        0        0      806 2024-04-10 02:27:08.638851 supamodel-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.4.3/supamodel/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-10 01:39:15.607798 supamodel-0.4.3/supamodel/_abc.py
+-rw-r--r--   0        0        0      291 2024-04-10 00:46:46.921212 supamodel-0.4.3/supamodel/_client.py
+-rw-r--r--   0        0        0        0 2024-04-10 01:03:32.730144 supamodel-0.4.3/supamodel/_core.py
+-rw-r--r--   0        0        0      646 2024-04-10 00:56:58.984128 supamodel-0.4.3/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-10 02:17:30.714990 supamodel-0.4.3/supamodel/_types.py
+-rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.3/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.3/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.3/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-10 01:57:59.819676 supamodel-0.4.3/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.3/supamodel/supa.py
+-rw-r--r--   0        0        0     4187 2024-04-10 02:22:32.745766 supamodel-0.4.3/supamodel/supa_builder.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.3/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.3/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.3/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.3/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.3/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1865 2024-04-10 01:01:58.246531 supamodel-0.4.3/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1832 2024-04-10 01:02:12.075303 supamodel-0.4.3/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    14903 2024-04-10 02:26:32.677556 supamodel-0.4.3/supamodel/utils.py
+-rw-r--r--   0        0        0     4709 1970-01-01 00:00:00.000000 supamodel-0.4.3/PKG-INFO
```

### Comparing `supamodel-0.4.2/supamodel/_abc.py` & `supamodel-0.4.3/supamodel/_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,28 +25,28 @@
     AliasGenerator,
     BaseModel as _BaseModel,
     ConfigDict,
     EmailStr,
     alias_generators,
 )
 
-from supamodel.utils import cached_classproperty
+from supamodel.utils import cached_classattr
 
 DataT = TypeVar("DataT", bound="Data")
 InputModelT = TypeVar("InputModelT", "BaseModel", "Data")
 DataAny = DataT | Any
 
 
 class BaseModel(_BaseModel):
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         use_enum_values=True,
         extra="allow",
         populate_by_name=True,
-        ignored_types=(cached_property, cached_classproperty),
+        ignored_types=(cached_property, cached_classattr),
     )
 
     def none_dump(self) -> Dict:
         """Return the model's data in a dictionary format without incuding None values.
 
         Returns:
             Dict: A dict with the model's data without None values.
@@ -72,20 +72,20 @@
 class CamelModel(IgnoreModel):
     model_config = ConfigDict(alias_generator=alias_generators.to_camel)
 
 
 class OrmModel(BaseModel):
     model_config = ConfigDict(
         from_attributes=True,
-        ignored_types=(cached_property, cached_classproperty),
+        ignored_types=(cached_property, cached_classattr),
         arbitrary_types_allowed=True,
     )
 
 
-class Data(BaseModel):
+class Data(OrmModel):
     """
     The OpenBB Standardized Data Model.
 
     The `Data` class is a flexible Pydantic model designed to accommodate various data structures
     for OpenBB's data processing pipeline as it's structured to support dynamic field definitions.
 
     The model leverages Pydantic's powerful validation features to ensure data integrity while
```

### Comparing `supamodel-0.4.2/supamodel/config.py` & `supamodel-0.4.3/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/enums.py` & `supamodel-0.4.3/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/exceptions.py` & `supamodel-0.4.3/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/supa_model.py` & `supamodel-0.4.3/supamodel/supa.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/trading/clock.py` & `supamodel-0.4.3/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/trading/exchange.py` & `supamodel-0.4.3/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/trading/market_data.py` & `supamodel-0.4.3/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.2/supamodel/trading/order_management.py` & `supamodel-0.4.3/supamodel/trading/order_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Optional
 from uuid import UUID
 
 from pydantic import Field
 
-from supamodel._core import BaseModel
+from supamodel._abc import BaseModel
 from supamodel.enums import OrderSide, OrderStatus, OrderType
 
 
 class Trade(BaseModel):
     id: Optional[UUID] = Field(description="Unique identifier of the trade")
     position_id: UUID = Field(description="ID of the associated position")
     order_id: UUID = Field(description="ID of the associated order")
```

### Comparing `supamodel-0.4.2/supamodel/trading/portfolio.py` & `supamodel-0.4.3/supamodel/trading/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 from uuid import UUID, uuid4
 
 from pendulum import DateTime
 from pydantic import Field
 
-from supamodel._core import BaseModel
+from supamodel._abc import BaseModel
 
 
 class Portfolio(BaseModel):
     id: UUID = Field(
         default_factory=uuid4, description="Unique identifier of the portfolio"
     )
     user_id: Optional[UUID] = Field(
```

