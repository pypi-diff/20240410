# Comparing `tmp/supamodel-0.3.0.tar.gz` & `tmp/supamodel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.3.0.tar", max compression
+gzip compressed data, was "supamodel-0.3.1.tar", max compression
```

## Comparing `supamodel-0.3.0.tar` & `supamodel-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.3.0/README.md
--rw-r--r--   0        0        0      523 2024-04-09 22:47:45.369423 supamodel-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.3.0/supamodel/__init__.py
--rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.3.0/supamodel/_abc.py
--rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.3.0/supamodel/_client.py
--rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.3.0/supamodel/_core.py
--rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.3.0/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.3.0/supamodel/_types.py
--rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.3.0/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.3.0/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.3.0/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.3.0/supamodel/exceptions.py
--rw-r--r--   0        0        0     7911 2024-04-09 21:41:30.442305 supamodel-0.3.0/supamodel/supa_model.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.3.0/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.3.0/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.3.0/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.3.0/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.3.0/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.3.0/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.3.0/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.3.0/supamodel/utils.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 supamodel-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.3.1/README.md
+-rw-r--r--   0        0        0      554 2024-04-09 23:44:08.836481 supamodel-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.3.1/supamodel/__init__.py
+-rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.3.1/supamodel/_abc.py
+-rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.3.1/supamodel/_client.py
+-rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.3.1/supamodel/_core.py
+-rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.3.1/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.3.1/supamodel/_types.py
+-rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.3.1/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.3.1/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.3.1/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.3.1/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.3.1/supamodel/supa_model.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.3.1/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.3.1/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.3.1/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.3.1/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.3.1/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.3.1/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.3.1/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.3.1/supamodel/utils.py
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 supamodel-0.3.1/PKG-INFO
```

### Comparing `supamodel-0.3.0/README.md` & `supamodel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/_abc.py` & `supamodel-0.3.1/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/_core.py` & `supamodel-0.3.1/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/config.py` & `supamodel-0.3.1/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/enums.py` & `supamodel-0.3.1/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/exceptions.py` & `supamodel-0.3.1/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/supa_model.py` & `supamodel-0.3.1/supamodel/supa_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-"""Get it SupaModel, because it's like a SuperModel, but Supa!"""
+# """Get it SupaModel, because it's like a SuperModel, but Supa!"""
 
-import contextlib
-import uuid
-from functools import cached_property
-from typing import Any, Optional, Type, TypeVar
-
-from loguru import logger
-from postgrest._sync.request_builder import SyncQueryRequestBuilder
-from pydantic import ConfigDict, field_serializer, model_validator
-
-# from pydantic.dataclasses import dataclass
-from rich import print
-
-from galapy.app.utils.formatting import tableize
-from galapy.config import supa_client as supabase
-from galapy.models.abstracts.data import Data
-from galapy.models.abstracts.dataset import Dataset
-from galapy.utils.decorators import cached_classproperty
-from galapy.utils.fn_tools import in_all_dicts, serialize_dict
-
-# from galapy.models.supas.core import Exchange
-
-SupaModelT = TypeVar("SupaModelT", bound=Data)
-ReqBuilderT = TypeVar("ReqBuilderT", bound=SyncQueryRequestBuilder)
-# PartT = TypeVar("PartT")
-SupaItem = TypeVar("SupaItem")
-
-
-class ResponseModel(Data):
-    model_config = ConfigDict(from_attributes=True)
-    data: list[dict[str, Any]] | None = []
-    count: int | None = None
-    error: str | None = None
-
-    def is_error(self):
-        return self.error is not None
-
-    def is_success(self) -> bool:
-        return self.error is None and self.data is not None
-
-    def empty(self) -> bool:
-        return self.data is None or len(self.data) == 0
-
-
-class SupaModel(Data):
-
-    id: uuid.UUID | None = None
-
-    # Like Super Model, but Supa
-    @field_serializer("id")
-    def serialize_courses_in_order(exchange_id: uuid.UUID | None):
-        if exchange_id is None:
-            return None
-        return str(exchange_id)
-
-    @classmethod
-    def table_name(cls) -> str:
-        return tableize(cls.__name__)
-
-    @cached_classproperty
-    def table(cls) -> SyncQueryRequestBuilder:
-        return supabase.table(cls.table_name())
-
-    @cached_classproperty
-    def class_type(cls):
-        """
-        Returns the class type of an instance created from the model. It must be an instance so tha we don't get the parent class type.
-        It would get ModelMetaClass instead of the current model normally instead.
-        """
-        instance = cls.model_construct({})
-        return type(instance)
-
-    @cached_classproperty
-    def dataset(cls):
-        """
-        Returns the dataset associated with the class.
-        """
-        return Dataset[cls.class_type]
-
-    @classmethod
-    def sync_by_id(cls, id: str) -> SupaModelT:
-        return cls.find_one(query_params={"id": id})
-
-    @classmethod
-    def rpc(cls, method: str, data: dict[str, Any]) -> ReqBuilderT:
-        query: ReqBuilderT = supabase.rpc(method, params=data)
-        # self.execute_dataset(query)
-        return query
-        # return self.execute_dataset(query)
-
-    @classmethod
-    def select(cls, columns: list[str] = ["*"]) -> ReqBuilderT:
-        return cls.table.select(*columns)
-
-    @classmethod
-    def select_eq(
-        cls, columns: list[str] = ["*"], inputs: dict[str, Any] = {}
-    ) -> ReqBuilderT:
-        # Looks for exact matches in the table
-        builder = cls.select(columns)
-        if not inputs:
-            return builder
-        for key, value in inputs.items():
-            builder = builder.eq(key, value)
-        return builder
-
-    @classmethod
-    def extract(
-        cls, query: ReqBuilderT, type_var: Optional[Type[SupaModelT]] = None
-    ) -> Dataset[SupaModelT]:
-        # Since most supabase queries return an object with a data attribute, and count attribute, this method will parse that information and the containing model's data attribute (subclasses of SupaModel).
-        response = query.execute()
-        response = ResponseModel.model_validate(response)
-        if response.is_error():
-            raise Exception(response.error)
-        resp_data = response.data
-        if type_var is not None:
-            return Dataset[type_var](data=resp_data)
-        return cls.dataset(data=resp_data)
-
-    def sync(self) -> SupaModelT:
-        dump = self.model_dump(exclude_none=True, round_trip=True)
-        found = self.find_one(query_params=dump)
-
-        if found is None:
-            return None
-        # for key, value in found:
-        #     print((key, value))
-        for key, value in found:
-            with contextlib.suppress(AttributeError):
-                setattr(self, key, value)
-        return found
-        # logger.success(found)
-
-    def save_current(self, record: dict = {}) -> Dataset[SupaModelT]:
-        try:
-            dump = (
-                record if record else self.model_dump(exclude_none=True, by_alias=True)
-            )
-            saved = self.save_one(dump)
-            if saved.data:
-                self.id = saved[0].id
-            else:
-                return saved
-        except Exception:
-            raise
-
-    @classmethod
-    def save_one(cls, record: dict = {}) -> Dataset[SupaModelT]:
-        if not record:
-            raise ValueError(
-                "No data to save. Please provide a record with something in the dictionary."
-            )
-        dump_id = record.pop("id", None)
-        if dump_id:
-            query_fn = cls.table.upsert
-            record = {**record, "id": str(dump_id)}
-        else:
-            query_fn = cls.table.insert
-
-        serialize_dict(record)
-        query = query_fn(record)
-        # logger.debug(query)
-        # logger.warning(cls.table_name())
-        return cls.extract(query)
-
-    @classmethod
-    def save_many(cls, records: list[dict] = []) -> Dataset[SupaModelT]:
-        if not records:
-            raise ValueError(
-                "No data to save. Please provide a record with something in the dictionary."
-            )
-        if not isinstance(records, list) or not all(
-            isinstance(record, dict) for record in records
-        ):
-            raise ValueError("Please provide a list of records to save.")
-        all_ids = in_all_dicts(records, "id")
-        query_fn = cls.table.insert if not all_ids else cls.table().upsert
-
-        query = query_fn(records)
-        return cls.extract(query)
-
-    def delete(self, id: str | None = None) -> Dataset[SupaModelT]:
-        try:
-            delete_id = id if id is not None else self.id
-            return self.delete_one(delete_id)
-        except Exception as e:
-            raise e
-
-    @classmethod
-    def delete_one(cls, id: str | None = None) -> SupaModelT:
-
-        query = cls.table.delete().eq("id", id)
-        return cls.extract(query)
-
-    # Delete many records by id
-    @classmethod
-    def delete_many(cls, ids: list[str] = []) -> Dataset[SupaModelT]:
-        if not ids or not isinstance(ids, list):
-            raise ValueError("No ids to delete. Please provide a list of ids.")
-        query = cls.table.delete().in_("id", ids)
-        return cls.extract(query)
-
-    @classmethod
-    def list_all(cls) -> Dataset[SupaModelT]:
-
-        with contextlib.suppress(Exception):
-            builder = cls.table.select("*")
-            return cls.extract(builder)
-        return cls.dataset(data=[])
-
-    @classmethod
-    def list_paginated(cls, page: int = 0, per_page: int = 50) -> Dataset[SupaModelT]:
-        with contextlib.suppress(Exception):
-            response = cls.table.select("*").range(page, per_page).execute()
-            return cls.dataset(data=response.data)
-        return cls.dataset(data=[])
-        # except Exception as e:
-        #     raise e
-
-    @model_validator(mode="before")
-    @classmethod
-    def validate_model(cls, values: Any) -> Any:
-        return values
-
-    @classmethod
-    def find_one(cls, query_params: dict = {}, ordering=True) -> SupaModelT | None:
-
-        query = cls.select_eq(inputs=query_params)
-        query = query.limit(1)
-        dataset = cls.extract(query)
-        if not dataset.empty():
-            return dataset[0]
-        return None
+# import contextlib
+# import uuid
+# from functools import cached_property
+# from typing import Any, Optional, Type, TypeVar
+
+# from loguru import logger
+# from postgrest._sync.request_builder import SyncQueryRequestBuilder
+# from pydantic import ConfigDict, field_serializer, model_validator
+
+# # from pydantic.dataclasses import dataclass
+# from rich import print
+
+# from galapy.app.utils.formatting import tableize
+# from galapy.config import supa_client as supabase
+# from galapy.models.abstracts.data import Data
+# from galapy.models.abstracts.dataset import Dataset
+# from galapy.utils.decorators import cached_classproperty
+# from galapy.utils.fn_tools import in_all_dicts, serialize_dict
+
+# # from galapy.models.supas.core import Exchange
+
+# SupaModelT = TypeVar("SupaModelT", bound=Data)
+# ReqBuilderT = TypeVar("ReqBuilderT", bound=SyncQueryRequestBuilder)
+# # PartT = TypeVar("PartT")
+# SupaItem = TypeVar("SupaItem")
+
+
+# class ResponseModel(Data):
+#     model_config = ConfigDict(from_attributes=True)
+#     data: list[dict[str, Any]] | None = []
+#     count: int | None = None
+#     error: str | None = None
+
+#     def is_error(self):
+#         return self.error is not None
+
+#     def is_success(self) -> bool:
+#         return self.error is None and self.data is not None
+
+#     def empty(self) -> bool:
+#         return self.data is None or len(self.data) == 0
+
+
+# class SupaModel(Data):
+
+#     id: uuid.UUID | None = None
+
+#     # Like Super Model, but Supa
+#     @field_serializer("id")
+#     def serialize_courses_in_order(exchange_id: uuid.UUID | None):
+#         if exchange_id is None:
+#             return None
+#         return str(exchange_id)
+
+#     @classmethod
+#     def table_name(cls) -> str:
+#         return tableize(cls.__name__)
+
+#     @cached_classproperty
+#     def table(cls) -> SyncQueryRequestBuilder:
+#         return supabase.table(cls.table_name())
+
+#     @cached_classproperty
+#     def class_type(cls):
+#         """
+#         Returns the class type of an instance created from the model. It must be an instance so tha we don't get the parent class type.
+#         It would get ModelMetaClass instead of the current model normally instead.
+#         """
+#         instance = cls.model_construct({})
+#         return type(instance)
+
+#     @cached_classproperty
+#     def dataset(cls):
+#         """
+#         Returns the dataset associated with the class.
+#         """
+#         return Dataset[cls.class_type]
+
+#     @classmethod
+#     def sync_by_id(cls, id: str) -> SupaModelT:
+#         return cls.find_one(query_params={"id": id})
+
+#     @classmethod
+#     def rpc(cls, method: str, data: dict[str, Any]) -> ReqBuilderT:
+#         query: ReqBuilderT = supabase.rpc(method, params=data)
+#         # self.execute_dataset(query)
+#         return query
+#         # return self.execute_dataset(query)
+
+#     @classmethod
+#     def select(cls, columns: list[str] = ["*"]) -> ReqBuilderT:
+#         return cls.table.select(*columns)
+
+#     @classmethod
+#     def select_eq(
+#         cls, columns: list[str] = ["*"], inputs: dict[str, Any] = {}
+#     ) -> ReqBuilderT:
+#         # Looks for exact matches in the table
+#         builder = cls.select(columns)
+#         if not inputs:
+#             return builder
+#         for key, value in inputs.items():
+#             builder = builder.eq(key, value)
+#         return builder
+
+#     @classmethod
+#     def extract(
+#         cls, query: ReqBuilderT, type_var: Optional[Type[SupaModelT]] = None
+#     ) -> Dataset[SupaModelT]:
+#         # Since most supabase queries return an object with a data attribute, and count attribute, this method will parse that information and the containing model's data attribute (subclasses of SupaModel).
+#         response = query.execute()
+#         response = ResponseModel.model_validate(response)
+#         if response.is_error():
+#             raise Exception(response.error)
+#         resp_data = response.data
+#         if type_var is not None:
+#             return Dataset[type_var](data=resp_data)
+#         return cls.dataset(data=resp_data)
+
+#     def sync(self) -> SupaModelT:
+#         dump = self.model_dump(exclude_none=True, round_trip=True)
+#         found = self.find_one(query_params=dump)
+
+#         if found is None:
+#             return None
+#         # for key, value in found:
+#         #     print((key, value))
+#         for key, value in found:
+#             with contextlib.suppress(AttributeError):
+#                 setattr(self, key, value)
+#         return found
+#         # logger.success(found)
+
+#     def save_current(self, record: dict = {}) -> Dataset[SupaModelT]:
+#         try:
+#             dump = (
+#                 record if record else self.model_dump(exclude_none=True, by_alias=True)
+#             )
+#             saved = self.save_one(dump)
+#             if saved.data:
+#                 self.id = saved[0].id
+#             else:
+#                 return saved
+#         except Exception:
+#             raise
+
+#     @classmethod
+#     def save_one(cls, record: dict = {}) -> Dataset[SupaModelT]:
+#         if not record:
+#             raise ValueError(
+#                 "No data to save. Please provide a record with something in the dictionary."
+#             )
+#         dump_id = record.pop("id", None)
+#         if dump_id:
+#             query_fn = cls.table.upsert
+#             record = {**record, "id": str(dump_id)}
+#         else:
+#             query_fn = cls.table.insert
+
+#         serialize_dict(record)
+#         query = query_fn(record)
+#         # logger.debug(query)
+#         # logger.warning(cls.table_name())
+#         return cls.extract(query)
+
+#     @classmethod
+#     def save_many(cls, records: list[dict] = []) -> Dataset[SupaModelT]:
+#         if not records:
+#             raise ValueError(
+#                 "No data to save. Please provide a record with something in the dictionary."
+#             )
+#         if not isinstance(records, list) or not all(
+#             isinstance(record, dict) for record in records
+#         ):
+#             raise ValueError("Please provide a list of records to save.")
+#         all_ids = in_all_dicts(records, "id")
+#         query_fn = cls.table.insert if not all_ids else cls.table().upsert
+
+#         query = query_fn(records)
+#         return cls.extract(query)
+
+#     def delete(self, id: str | None = None) -> Dataset[SupaModelT]:
+#         try:
+#             delete_id = id if id is not None else self.id
+#             return self.delete_one(delete_id)
+#         except Exception as e:
+#             raise e
+
+#     @classmethod
+#     def delete_one(cls, id: str | None = None) -> SupaModelT:
+
+#         query = cls.table.delete().eq("id", id)
+#         return cls.extract(query)
+
+#     # Delete many records by id
+#     @classmethod
+#     def delete_many(cls, ids: list[str] = []) -> Dataset[SupaModelT]:
+#         if not ids or not isinstance(ids, list):
+#             raise ValueError("No ids to delete. Please provide a list of ids.")
+#         query = cls.table.delete().in_("id", ids)
+#         return cls.extract(query)
+
+#     @classmethod
+#     def list_all(cls) -> Dataset[SupaModelT]:
+
+#         with contextlib.suppress(Exception):
+#             builder = cls.table.select("*")
+#             return cls.extract(builder)
+#         return cls.dataset(data=[])
+
+#     @classmethod
+#     def list_paginated(cls, page: int = 0, per_page: int = 50) -> Dataset[SupaModelT]:
+#         with contextlib.suppress(Exception):
+#             response = cls.table.select("*").range(page, per_page).execute()
+#             return cls.dataset(data=response.data)
+#         return cls.dataset(data=[])
+#         # except Exception as e:
+#         #     raise e
+
+#     @model_validator(mode="before")
+#     @classmethod
+#     def validate_model(cls, values: Any) -> Any:
+#         return values
+
+#     @classmethod
+#     def find_one(cls, query_params: dict = {}, ordering=True) -> SupaModelT | None:
+
+#         query = cls.select_eq(inputs=query_params)
+#         query = query.limit(1)
+#         dataset = cls.extract(query)
+#         if not dataset.empty():
+#             return dataset[0]
+#         return None
 
 
-def main():
-    print("Hello, World!")
+# def main():
+#     print("Hello, World!")
 
 
-if __name__ == "__main__":
-    main()
+# if __name__ == "__main__":
+#     main()
```

### Comparing `supamodel-0.3.0/supamodel/trading/clock.py` & `supamodel-0.3.1/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/trading/exchange.py` & `supamodel-0.3.1/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/trading/market_data.py` & `supamodel-0.3.1/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/trading/order_management.py` & `supamodel-0.3.1/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/trading/portfolio.py` & `supamodel-0.3.1/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/supamodel/utils.py` & `supamodel-0.3.1/supamodel/utils.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.3.0/PKG-INFO` & `supamodel-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: inflector (>=3.1.1,<4.0.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: loguru (>=0.5.0,<1.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pendulum (>=2.0.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: supabase-py (>=0.0.2,<0.0.3)
+Requires-Dist: supabase (>=2.4.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # SupaModel - Pydantic BaseModels and ORM for Supabase
 
 `SupaModel` is a Python package that provides `pydantic` BaseModels and ORM for `Supabase`. It is built on top of [supabase-py](https://supabase.com/docs/reference/python/start) and [pydantic](https://pydantic-docs.helpmanual.io/).
```

