# Comparing `tmp/abses-0.5.6.tar.gz` & `tmp/abses-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.5.6.tar", max compression
+gzip compressed data, was "abses-0.5.7.tar", max compression
```

## Comparing `abses-0.5.6.tar` & `abses-0.5.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.6/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.6/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-06 08:14:34.863287 abses-0.5.6/README.md
--rw-r--r--   0        0        0      978 2024-04-06 15:04:19.556382 abses-0.5.6/abses/__init__.py
--rw-r--r--   0        0        0     9396 2024-04-06 01:06:25.258369 abses-0.5.6/abses/actor.py
--rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.6/abses/bases.py
--rw-r--r--   0        0        0     5608 2024-04-06 01:06:25.259525 abses-0.5.6/abses/cells.py
--rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.6/abses/components.py
--rw-r--r--   0        0        0    16509 2024-04-06 01:06:25.260683 abses-0.5.6/abses/container.py
--rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.6/abses/decision.py
--rw-r--r--   0        0        0     2814 2024-04-04 10:58:12.165326 abses-0.5.6/abses/dynamic.py
--rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.6/abses/errors.py
--rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.6/abses/human.py
--rw-r--r--   0        0        0    18110 2024-04-06 01:06:25.262363 abses-0.5.6/abses/links.py
--rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.6/abses/logging.py
--rw-r--r--   0        0        0    11515 2024-04-06 01:06:25.262785 abses-0.5.6/abses/main.py
--rw-r--r--   0        0        0     4389 2024-04-06 01:06:25.263178 abses-0.5.6/abses/modules.py
--rw-r--r--   0        0        0     8216 2024-04-06 01:06:25.263593 abses-0.5.6/abses/move.py
--rw-r--r--   0        0        0    21209 2024-04-06 01:06:25.263971 abses-0.5.6/abses/nature.py
--rw-r--r--   0        0        0     2942 2024-04-06 01:06:25.264485 abses-0.5.6/abses/objects.py
--rw-r--r--   0        0        0     5962 2024-04-06 01:06:25.265050 abses-0.5.6/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.6/abses/selection.py
--rw-r--r--   0        0        0    11402 2024-04-06 01:06:25.265385 abses-0.5.6/abses/sequences.py
--rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.6/abses/states.py
--rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.6/abses/time.py
--rw-r--r--   0        0        0     3216 2024-04-06 01:06:25.266508 abses-0.5.6/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-04 10:58:12.169839 abses-0.5.6/abses/tools/regex.py
--rw-r--r--   0        0        0     2469 2024-04-06 15:04:19.555747 abses-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 abses-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.7/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.7/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-06 08:14:34.863287 abses-0.5.7/README.md
+-rw-r--r--   0        0        0      978 2024-04-10 01:55:14.951298 abses-0.5.7/abses/__init__.py
+-rw-r--r--   0        0        0     9396 2024-04-06 01:06:25.258369 abses-0.5.7/abses/actor.py
+-rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.7/abses/bases.py
+-rw-r--r--   0        0        0     5608 2024-04-06 01:06:25.259525 abses-0.5.7/abses/cells.py
+-rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.7/abses/components.py
+-rw-r--r--   0        0        0    16509 2024-04-08 13:53:41.188553 abses-0.5.7/abses/container.py
+-rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.7/abses/decision.py
+-rw-r--r--   0        0        0     2814 2024-04-04 10:58:12.165326 abses-0.5.7/abses/dynamic.py
+-rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.7/abses/errors.py
+-rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.7/abses/human.py
+-rw-r--r--   0        0        0    18407 2024-04-09 03:29:02.639690 abses-0.5.7/abses/links.py
+-rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.7/abses/logging.py
+-rw-r--r--   0        0        0    11515 2024-04-08 13:53:41.189260 abses-0.5.7/abses/main.py
+-rw-r--r--   0        0        0     4389 2024-04-06 01:06:25.263178 abses-0.5.7/abses/modules.py
+-rw-r--r--   0        0        0     8216 2024-04-06 01:06:25.263593 abses-0.5.7/abses/move.py
+-rw-r--r--   0        0        0    21209 2024-04-08 13:53:41.189388 abses-0.5.7/abses/nature.py
+-rw-r--r--   0        0        0     2942 2024-04-06 01:06:25.264485 abses-0.5.7/abses/objects.py
+-rw-r--r--   0        0        0     5962 2024-04-06 01:06:25.265050 abses-0.5.7/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.7/abses/selection.py
+-rw-r--r--   0        0        0    11565 2024-04-09 03:29:02.589027 abses-0.5.7/abses/sequences.py
+-rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.7/abses/states.py
+-rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.7/abses/time.py
+-rw-r--r--   0        0        0     3216 2024-04-06 01:06:25.266508 abses-0.5.7/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-04 10:58:12.169839 abses-0.5.7/abses/tools/regex.py
+-rw-r--r--   0        0        0     2469 2024-04-10 01:55:14.948942 abses-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 abses-0.5.7/PKG-INFO
```

### Comparing `abses-0.5.6/LICENSE` & `abses-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/README.md` & `abses-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/__init__.py` & `abses-0.5.7/abses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Decision",
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
 ]
-__version__ = "v0.5.6"
+__version__ = "v0.5.7"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .decision import Decision
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
```

### Comparing `abses-0.5.6/abses/actor.py` & `abses-0.5.7/abses/actor.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/bases.py` & `abses-0.5.7/abses/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/cells.py` & `abses-0.5.7/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/components.py` & `abses-0.5.7/abses/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/container.py` & `abses-0.5.7/abses/container.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/decision.py` & `abses-0.5.7/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/dynamic.py` & `abses-0.5.7/abses/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/human.py` & `abses-0.5.7/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/links.py` & `abses-0.5.7/abses/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     from abses import MainModel
     from abses.actor import Actor
     from abses.cells import PatchCell
 
 LinkingNode: TypeAlias = "Actor | PatchCell"
 Direction: TypeAlias = Optional[Literal["in", "out"]]
 DEFAULT_TARGETS: Tuple[str, str] = ("cell", "actor")
-TargetName: TypeAlias = Union[Literal["cell", "actor"], str]
+TargetName: TypeAlias = Union[Literal["cell", "actor", "self"], str]
 AttrGetter: TypeAlias = Union["Actor", "PatchCell", ActorsList["Actor"]]
 
 
 class _LinkContainer:
     """Container for links."""
 
     def __init__(self) -> None:
@@ -502,21 +502,23 @@
                 If the target is an agent, get the attribute from the agent.
                 If the target is a cell, get the attribute from the cell.
 
         Returns:
             The value of the attribute.
         """
         if target in DEFAULT_TARGETS:
-            return self._default_redirection(target).get(attr)
+            return self._default_redirection(target).get(attr, "self")
+        if target == "self":
+            return getattr(self, attr)
         if hasattr(self, attr):
             assert (
                 target is None
-            ), "The target '{target}' is ignored because '{self}' already has attr '{attr}'."
+            ), f"The target '{target}' is set when '{self}' already has attr '{attr}'."
             return getattr(self, attr)
-        return self._redirect_getting(target=target).get(attr)
+        return self._redirect_getting(target=target).get(attr, "self")
 
     def set(
         self, attr: str, value: Any, target: Optional[TargetName] = None
     ) -> None:
         """Sets the value of an attribute.
 
         Parameters:
@@ -538,18 +540,23 @@
         # If the attribute is not a string, raise an error.
         if not isinstance(attr, str):
             raise TypeError("The attribute must be a string.")
         # If the attribute is protected, raise an error
         if attr.startswith("_"):
             raise ABSESpyError(f"Attribute '{attr}' is protected.")
         if target in DEFAULT_TARGETS:
-            self._default_redirection(target).set(attr, value)
+            self._default_redirection(target).set(attr, value, "self")
+            return
+        if target == "self":
+            if not hasattr(self, attr):
+                raise AttributeError(f"{self} has no attribute '{attr}'.")
+            setattr(self, attr, value)
             return
         # Set the attribute on the target.
         if hasattr(self, attr):
             assert (
                 target is None
-            ), "The target '{target}' is ignored, because '{self}' already has attr '{attr}'."
+            ), f"The target '{target}' is set when '{self}' already has attr '{attr}'."
             setattr(self, attr, value)
         else:
             new_target = self._redirect_getting(target=target)
-            new_target.set(attr, value)
+            new_target.set(attr, value, "self")
```

### Comparing `abses-0.5.6/abses/main.py` & `abses-0.5.7/abses/main.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/modules.py` & `abses-0.5.7/abses/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/move.py` & `abses-0.5.7/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/nature.py` & `abses-0.5.7/abses/nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/objects.py` & `abses-0.5.7/abses/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/random.py` & `abses-0.5.7/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/selection.py` & `abses-0.5.7/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/sequences.py` & `abses-0.5.7/abses/sequences.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from abses.selection import selecting
 
 from .tools.func import make_list
 
 if TYPE_CHECKING:
     from abses.main import MainModel
 
-    from .actor import Actor
+    from .actor import Actor, TargetName
 
 Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, bool]]
 HOW: TypeAlias = Literal["only", "random", "item"]
 ActorType = TypeVar("ActorType", bound="Actor")
 
 
 def get_only_agent(agents: ActorsList) -> Actor:
@@ -276,44 +276,50 @@
         Returns:
             An array of the results of applying the function to each actor.
         """
         func = partial(ufunc, *args, **kwargs)
         return np.array(list(map(func, self)))
 
     def get(
-        self, attr: str, how: HOW = "only", default: Optional[Any] = None
+        self,
+        attr: str,
+        target: Optional[TargetName] = None,
+        how: HOW = "only",
+        default: Optional[Any] = None,
     ) -> Any:
         """Retrieve the attribute of an either specified or randomly chosen agent.
 
         Parameters:
             attr:
                 The name of the attribute to retrieve.
             how:
                 The method to use to retrieve the attribute. Can be either "only" or "random".
 
         Returns:
             The attribute of the specified agent.
         """
         if agent := self.item(how=how, index=0):
-            return agent.get(attr)
+            return agent.get(attr, target=target)
         if default is not None:
             return default
         raise ValueError("No agent found or default value.")
 
-    def set(self, attr: str, value: Any) -> None:
+    def set(
+        self, attr: str, value: Any, target: Optional[TargetName] = None
+    ) -> None:
         """Set the attribute of all agents in the sequence to the specified value.
 
         Parameters:
             attr:
                 The name of the attribute to set.
             value:
                 The value to set the attribute to.
         """
         for agent in iter(self):
-            agent.set(attr, value)
+            agent.set(attr, value, target=target)
 
     def item(self, how: HOW = "item", index: int = 0) -> Optional[Actor]:
         """Retrieve one agent if possible.
 
         Parameters:
             how:
                 The method to use to retrieve the agent.
```

### Comparing `abses-0.5.6/abses/states.py` & `abses-0.5.7/abses/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/time.py` & `abses-0.5.7/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/tools/func.py` & `abses-0.5.7/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/abses/tools/regex.py` & `abses-0.5.7/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.6/pyproject.toml` & `abses-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.5.6"
+version = "0.5.7"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `abses-0.5.6/PKG-INFO` & `abses-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.5.6
+Version: 0.5.7
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abses Version: 0.5.6 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.5.7 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
```

