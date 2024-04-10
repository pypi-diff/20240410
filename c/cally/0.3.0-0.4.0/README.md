# Comparing `tmp/cally-0.3.0.tar.gz` & `tmp/cally-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cally-0.3.0.tar", last modified: Fri Apr  5 09:41:52 2024, max compression
+gzip compressed data, was "cally-0.4.0.tar", last modified: Wed Apr 10 09:19:34 2024, max compression
```

## Comparing `cally-0.3.0.tar` & `cally-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-05 09:41:45.000000 cally-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-04-05 09:41:52.818641 cally-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-05 09:41:45.000000 cally-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-05 09:41:45.000000 cally-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:41:52.818641 cally-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.810641 cally-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.810641 cally-0.3.0/src/cally/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cdk/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cdk/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/commands/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.814641 cally-0.3.0/src/cally/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/cli/tools/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:45.000000 cally-0.3.0/src/cally/testing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:41:52.818641 cally-0.3.0/src/cally.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 09:41:52.000000 cally-0.3.0/src/cally.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.620816 cally-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-10 09:19:30.000000 cally-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27479 2024-04-10 09:19:34.620816 cally-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-10 09:19:30.000000 cally-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-10 09:19:30.000000 cally-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:19:34.620816 cally-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.608816 cally-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cdk/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cdk/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.612816 cally-0.4.0/src/cally/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/commands/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/cli/tools/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:30.000000 cally-0.4.0/src/cally/testing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:34.616816 cally-0.4.0/src/cally.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27479 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 09:19:34.000000 cally-0.4.0/src/cally.egg-info/top_level.txt
```

### Comparing `cally-0.3.0/LICENSE` & `cally-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/PKG-INFO` & `cally-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.3.0
+Version: 0.4.0
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -385,23 +385,29 @@
 Requires-Dist: cdktf
 Requires-Dist: click
 Requires-Dist: dynaconf
 Requires-Dist: PyYAML
 Provides-Extra: development
 Requires-Dist: black; extra == "development"
 Requires-Dist: build; extra == "development"
-Requires-Dist: coverage; extra == "development"
 Requires-Dist: isort; extra == "development"
 Requires-Dist: mypy; extra == "development"
+Requires-Dist: coverage; extra == "development"
 Requires-Dist: pytest; extra == "development"
 Requires-Dist: pytest-black; extra == "development"
 Requires-Dist: pytest-mypy; extra == "development"
 Requires-Dist: pytest-ruff<0.3; extra == "development"
 Requires-Dist: ruff; extra == "development"
 Requires-Dist: types-PyYAML; extra == "development"
+Requires-Dist: sphinx; extra == "development"
+Requires-Dist: sphinx-autobuild; extra == "development"
+Requires-Dist: sphinx-issues; extra == "development"
+Requires-Dist: sphinxcontrib-log-cabinet; extra == "development"
+Requires-Dist: sphinx-tabs; extra == "development"
+Requires-Dist: Pallets-Sphinx-Themes; extra == "development"
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-black; extra == "test"
```

### Comparing `cally-0.3.0/README.md` & `cally-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/pyproject.toml` & `cally-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,33 @@
 Repository = "https://github.com/CallyCo-io/Cally/"
 Issues = "https://github.com/CallyCo-io/Cally/issues"
 
 [project.optional-dependencies]
 development = [
   "black",
   "build",
-  "coverage",
   "isort",
   "mypy",
+
+  # test
+  "coverage",
   "pytest",
   "pytest-black",
   "pytest-mypy",
   "pytest-ruff<0.3",  # 0.3 + 0.3.1 are currently not working
   "ruff",
   "types-PyYAML",
+
+  # docs
+  "sphinx",
+  "sphinx-autobuild",
+  "sphinx-issues",
+  "sphinxcontrib-log-cabinet",
+  "sphinx-tabs",
+  "Pallets-Sphinx-Themes",
 ]
 test = [
   "black",
   "build",
   "coverage",
   "mypy",
   "pytest",
```

### Comparing `cally-0.3.0/src/cally/cdk/__init__.py` & `cally-0.4.0/src/cally/cdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import inspect
 from copy import deepcopy
 from dataclasses import dataclass, field, make_dataclass
 from importlib import import_module
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from types import MappingProxyType
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from cdktf import (
     App,
     TerraformBackend,
+    TerraformOutput,
     TerraformProvider,
     TerraformResource,
     TerraformStack,
 )
 from constructs import Construct
 
 if TYPE_CHECKING:
@@ -50,70 +52,76 @@
         if not self._instantiated_attributes:
             self.instantiate_attributes()
         return self._instantiated_attributes
 
 
 class CallyResource:
     _cdktf_resource: Any  # This is probably a callable TerraformResource
-    _identifier: Optional[str]
+    _tf_identifier: Optional[str]
     _instantiated_resource: TerraformResource
     attributes: CallyResourceAttributes
     provider: str
     resource: str
-    defaults: dict
+    defaults: Union[dict, MappingProxyType]
 
-    def __init__(self, identifier: Optional[str] = None, **kwargs) -> None:
+    def __init__(self, tf_identifier: Optional[str] = None, **kwargs) -> None:
         module = import_module(f'cally.providers.{self.provider}.{self.resource}')
         self._cdktf_resource = getattr(module, self.__class__.__name__)
-        self.attributes = self._build_attributes(identifier, **kwargs)
+        self.attributes = self._build_attributes(tf_identifier, **kwargs)
 
     def __str__(self) -> str:
-        if self.identifier:
-            return f'${{{self.resource}.{self.identifier}.id}}'
+        if self.tf_identifier:
+            return f'${{{self.tf_resource}.{self.tf_identifier}.id}}'
         return self.__class__.__name__
 
     def __getattr__(self, item: str) -> Optional[str]:
         # TODO: This likely could use some improvement
         if item.startswith('__jsii'):
             return getattr(self._instantiated_resource, item)
         if item in {'attributes', 'defaults', '_instantiated_resource'}:
             return None
-        if self.identifier:
-            return f'${{{self.resource}.{self.identifier}.{item}}}'
+        if self.tf_identifier:
+            return f'${{{self.tf_resource}.{self.tf_identifier}.{item}}}'
         return None
 
     def _get_attribute_default(self, name: str) -> Any:
         if self.defaults is None:
             return None
         return deepcopy(self.defaults.get(name, None))
 
     def _build_attributes(
-        self, identifier: Optional[str] = None, **kwargs
+        self, tf_identifier: Optional[str] = None, **kwargs
     ) -> CallyResourceAttributes:
         func = self._cdktf_resource.__init__  # type: ignore
         parameters = inspect.signature(func).parameters
         fields = [
             (name, param.annotation, self._get_attribute_default(name))
             for name, param in parameters.items()
             if param.annotation is not inspect._empty and name not in {'scope'}
         ]
         name = f'{self.__class__.__name__}CallyAttributes'
         cls = make_dataclass(name, fields, bases=(CallyResourceAttributes,))
-        if identifier:
+        if tf_identifier:
             # Some newer provider releases appear to use 'id_'
             id_field = 'id'
             if 'id_' in parameters:
                 id_field = 'id_'
-            kwargs.update({id_field: identifier})
-        self._identifier = identifier
+            kwargs.update({id_field: tf_identifier})
+        self._tf_identifier = tf_identifier
         return cls(**kwargs)
 
     @property
-    def identifier(self) -> Optional[str]:
-        return self._identifier
+    def tf_identifier(self) -> Optional[str]:
+        return self._tf_identifier
+
+    @property
+    def tf_resource(self) -> Optional[str]:
+        if self.resource.startswith('data_'):
+            return f'data.{self.resource[5:]}'
+        return self.resource
 
     def construct_resource(
         self,
         scope: Optional[Construct] = None,
         provider: Optional[TerraformProvider] = None,
     ) -> TerraformResource:
         if getattr(self, '_instantiated_resource', None) is None:
@@ -126,21 +134,25 @@
                     }
                 )
             self._instantiated_resource = self._cdktf_resource(**attrubtes)
         return self._instantiated_resource
 
 
 class CallyStack:
+    _outputs: List[Tuple[str, str]]
     _providers: Dict[str, TerraformProvider]
     _resources: List[CallyResource]
     service: 'CallyStackService'
 
     def __init__(self, service: 'CallyStackService') -> None:
         self.service = service
 
+    def add_output(self, tf_identifier: str, output: str) -> None:
+        self.outputs.append((tf_identifier, output))
+
     def add_resource(self, resource: CallyResource) -> None:
         self.resources.append(resource)
 
     def add_resources(self, resources: List[CallyResource]) -> None:
         self.resources.extend(resources)
 
     def get_backend(self) -> TerraformBackend:
@@ -176,14 +188,20 @@
     @property
     def resources(self) -> List[CallyResource]:
         if getattr(self, '_resources', None) is None:
             self._resources = []
         return self._resources
 
     @property
+    def outputs(self) -> List[Tuple[str, str]]:
+        if getattr(self, '_outputs', None) is None:
+            self._outputs = []
+        return self._outputs
+
+    @property
     def providers(self) -> Dict[str, TerraformProvider]:
         if getattr(self, '_providers', None) is None:
             self._providers = {}
         return self._providers
 
     def synth_stack(self, outdir='cdktf.out'):
         stack = self
@@ -193,13 +211,15 @@
             def __init__(self, scope: Construct) -> None:
                 super().__init__(scope, stack.name)
                 for resource in stack.resources:
                     resource.construct_resource(
                         self,
                         provider=stack.get_provider(self, resource.provider),
                     )
+                for tf_identifier, value in stack.outputs:
+                    TerraformOutput(self, tf_identifier, value=value)
                 stack.get_backend()(self, **stack.service.backend_config)
 
         app = App(outdir=outdir)
         MyStack(app)
 
         app.synth()
```

### Comparing `cally-0.3.0/src/cally/cdk/stacks/__init__.py` & `cally-0.4.0/src/cally/cdk/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/__init__.py` & `cally-0.4.0/src/cally/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/commands/tf.py` & `cally-0.4.0/src/cally/cli/commands/tf.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/config/__init__.py` & `cally-0.4.0/src/cally/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/config/loader.py` & `cally-0.4.0/src/cally/cli/config/loader.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/config/types.py` & `cally-0.4.0/src/cally/cli/config/types.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/config/validators.py` & `cally-0.4.0/src/cally/cli/config/validators.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/constants.py` & `cally-0.4.0/src/cally/cli/constants.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/tools/provider.py` & `cally-0.4.0/src/cally/cli/tools/provider.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/cli/tools/terraform.py` & `cally-0.4.0/src/cally/cli/tools/terraform.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally/testing/__init__.py` & `cally-0.4.0/src/cally/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.3.0/src/cally.egg-info/PKG-INFO` & `cally-0.4.0/src/cally.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.3.0
+Version: 0.4.0
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -385,23 +385,29 @@
 Requires-Dist: cdktf
 Requires-Dist: click
 Requires-Dist: dynaconf
 Requires-Dist: PyYAML
 Provides-Extra: development
 Requires-Dist: black; extra == "development"
 Requires-Dist: build; extra == "development"
-Requires-Dist: coverage; extra == "development"
 Requires-Dist: isort; extra == "development"
 Requires-Dist: mypy; extra == "development"
+Requires-Dist: coverage; extra == "development"
 Requires-Dist: pytest; extra == "development"
 Requires-Dist: pytest-black; extra == "development"
 Requires-Dist: pytest-mypy; extra == "development"
 Requires-Dist: pytest-ruff<0.3; extra == "development"
 Requires-Dist: ruff; extra == "development"
 Requires-Dist: types-PyYAML; extra == "development"
+Requires-Dist: sphinx; extra == "development"
+Requires-Dist: sphinx-autobuild; extra == "development"
+Requires-Dist: sphinx-issues; extra == "development"
+Requires-Dist: sphinxcontrib-log-cabinet; extra == "development"
+Requires-Dist: sphinx-tabs; extra == "development"
+Requires-Dist: Pallets-Sphinx-Themes; extra == "development"
 Provides-Extra: test
 Requires-Dist: black; extra == "test"
 Requires-Dist: build; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-black; extra == "test"
```

### Comparing `cally-0.3.0/src/cally.egg-info/SOURCES.txt` & `cally-0.4.0/src/cally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

