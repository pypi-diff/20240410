# Comparing `tmp/pytest-node-dependency-1.2.0.tar.gz` & `tmp/pytest-node-dependency-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-node-dependency-1.2.0.tar", last modified: Mon Apr  8 13:11:15 2024, max compression
+gzip compressed data, was "pytest-node-dependency-1.3.0.tar", last modified: Tue Apr  9 15:08:58 2024, max compression
```

## Comparing `pytest-node-dependency-1.2.0.tar` & `pytest-node-dependency-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/pytest_node_dependency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/pytest_node_dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/pytest_node_dependency/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 13:11:15.000000 pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:11:15.760700 pytest-node-dependency-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 13:11:11.000000 pytest-node-dependency-1.2.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/pytest_node_dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/pytest_node_dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/pytest_node_dependency/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 15:08:58.000000 pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:08:58.748742 pytest-node-dependency-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 15:08:54.000000 pytest-node-dependency-1.3.0/tests/test_plugin.py
```

### Comparing `pytest-node-dependency-1.2.0/LICENSE` & `pytest-node-dependency-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-node-dependency-1.2.0/PKG-INFO` & `pytest-node-dependency-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-node-dependency
-Version: 1.2.0
+Version: 1.3.0
 Summary: pytest plugin for controlling execution flow
 Home-page: https://github.com/Formartha/pytest-node-dependency
 Author: Mor Dabastany
 License: MIT
 Keywords: pyest-node-dependency
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -18,26 +18,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 
 ------
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit)
+![PyPI](https://img.shields.io/pypi/v/PACKAGE?label=pytest-node-dependency)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-node-dependency)
 
 What?
 ------
 pytest-node-dependency is a pytest plugin that allows you to define dependencies between tests and reorder their execution based on those dependencies. This plugin ensures that tests with dependencies run after their required prerequisites have completed successfully.
 
 How to install?
 ----------
 ```
 pip install pytest-node-dependency
 ```
 
-how to use?
+How to use?
 -----------------------------------------------------
 To set up a test dependency, decorate the test function with the `depends` mark and provide a list of dependencies via the `on` keyword argument to the decorator. Dependencies can be specified by name only when in the same file as the test being decorated or by the pytest node path for tests in other files/classes.
 
 ```
 import pytest
 
 
@@ -53,11 +55,42 @@
 
 
 def test_first(request):
     print("first")
     assert request.session.items[0].name == 'test_first'
 ```
 
+Xdist adoption:
+---------------
+The way xdist plugin works is by utilizing multiple cores and spreads the tests among them.
+The problem with the plugin is that if you wish to use reordering, you probably want to set some dependency among the tests,
+However, the xdist plugin will break it.
+
+For that, you should set the group for the tests. The group means that a gateway worker will collect the tests, and will 
+place all the grouped tests in a single gateway worker. 
+This will lead creation of serial testing among parallel exectuion.
+
+```
+import pytest
+
+@pytest.mark.depends(xdist_group='a')
+def test_second(request):
+    print("second")
+    assert request.session.items[1].name == 'test_second'
+
+
+@pytest.mark.depends(on=["test_plugin.py::test_second"], xdist_group='a')
+def test_last(request):
+    print("last")
+    assert request.session.items[2].name == 'test_last'
+
+
+def test_first(request):
+    print("first")
+    assert request.session.items[0].name == 'test_first'
+```
+
+
 Limitations and known issues:
 -----------------------------------------------------
-* The plugin logic makes tests run one after the other in a serial way, as a result, x-dist isn't supported (currently).
-* All the tests without depednecy (both dependent on and depends on) will run first, afterwards all tests with connections will run (e.g. the list of items will be as described)
+* All the tests without dependency (both dependent-on) will run first, then, all tests with connections will run
+(e.g. the list of items will be as described)
```

### Comparing `pytest-node-dependency-1.2.0/README.md` & `pytest-node-dependency-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ------
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit)
+![PyPI](https://img.shields.io/pypi/v/PACKAGE?label=pytest-node-dependency)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-node-dependency)
 
 What?
 ------
 pytest-node-dependency is a pytest plugin that allows you to define dependencies between tests and reorder their execution based on those dependencies. This plugin ensures that tests with dependencies run after their required prerequisites have completed successfully.
 
 How to install?
 ----------
 ```
 pip install pytest-node-dependency
 ```
 
-how to use?
+How to use?
 -----------------------------------------------------
 To set up a test dependency, decorate the test function with the `depends` mark and provide a list of dependencies via the `on` keyword argument to the decorator. Dependencies can be specified by name only when in the same file as the test being decorated or by the pytest node path for tests in other files/classes.
 
 ```
 import pytest
 
 
@@ -32,11 +34,42 @@
 
 
 def test_first(request):
     print("first")
     assert request.session.items[0].name == 'test_first'
 ```
 
+Xdist adoption:
+---------------
+The way xdist plugin works is by utilizing multiple cores and spreads the tests among them.
+The problem with the plugin is that if you wish to use reordering, you probably want to set some dependency among the tests,
+However, the xdist plugin will break it.
+
+For that, you should set the group for the tests. The group means that a gateway worker will collect the tests, and will 
+place all the grouped tests in a single gateway worker. 
+This will lead creation of serial testing among parallel exectuion.
+
+```
+import pytest
+
+@pytest.mark.depends(xdist_group='a')
+def test_second(request):
+    print("second")
+    assert request.session.items[1].name == 'test_second'
+
+
+@pytest.mark.depends(on=["test_plugin.py::test_second"], xdist_group='a')
+def test_last(request):
+    print("last")
+    assert request.session.items[2].name == 'test_last'
+
+
+def test_first(request):
+    print("first")
+    assert request.session.items[0].name == 'test_first'
+```
+
+
 Limitations and known issues:
 -----------------------------------------------------
-* The plugin logic makes tests run one after the other in a serial way, as a result, x-dist isn't supported (currently).
-* All the tests without depednecy (both dependent on and depends on) will run first, afterwards all tests with connections will run (e.g. the list of items will be as described)
+* All the tests without dependency (both dependent-on) will run first, then, all tests with connections will run
+(e.g. the list of items will be as described)
```

### Comparing `pytest-node-dependency-1.2.0/pytest_node_dependency/plugin.py` & `pytest-node-dependency-1.3.0/pytest_node_dependency/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 import os
 import platform
-
 import networkx as nx
 import pytest
 
+NODE_DEPENDENCY_ITEMS_CACHE = 'node-dependency-items'
+
+try:
+    from xdist.scheduler.loadscope import LoadScopeScheduling
+
+    def pytest_xdist_make_scheduler(config, log):
+        return Scheduler(config, log)
+
+    class Scheduler(LoadScopeScheduling):
+        def _split_scope(self, nodeid):
+            return TestDependencyHandler.xdist_get_group(self.config, nodeid)
+
+except ImportError:
+    pass
+
 
 class TestDependencyHandler:
 
     with_deps = []
     without_deps = []
 
     @staticmethod
@@ -61,19 +75,38 @@
                 current_nodeid = nodeid
 
         depends_on = [nodeid_to_item_map[dependency_nodeid], item]
         if nodeid_to_item_map[dependency_nodeid] in TestDependencyHandler.without_deps:
             TestDependencyHandler.without_deps.remove(nodeid_to_item_map[dependency_nodeid])
 
         TestDependencyHandler.with_deps.extend(dep for dep in depends_on if str(dep) not in str(TestDependencyHandler.with_deps))
+        TestDependencyHandler.xdist_register_group(item)
 
     @staticmethod
     def without_deps_parser(item):
         if item not in TestDependencyHandler.with_deps:
             TestDependencyHandler.without_deps.append(item)
+            TestDependencyHandler.xdist_register_group(item)
+
+    @staticmethod
+    def xdist_register_group(item):
+        l = item.config.cache.get(NODE_DEPENDENCY_ITEMS_CACHE, dict())
+        try:
+            l[item.name] = item.get_closest_marker("depends").kwargs.get("xdist_group")
+            item.config.cache.set(NODE_DEPENDENCY_ITEMS_CACHE, l)
+        except:
+            pass
+
+    @staticmethod
+    def xdist_get_group(config, nodeid):
+        group = config.cache.get(NODE_DEPENDENCY_ITEMS_CACHE, {}).get(nodeid.split("::")[1])
+        if group:
+            return config.cache.get(NODE_DEPENDENCY_ITEMS_CACHE, {}).get(nodeid.split("::")[1])
+        else:
+            return nodeid
 
     @staticmethod
     def reorder_tests(items):
         """
         Reorder the execution of tests based on the dependency marks.
 
         To set up a test dependency, decorate the test function with the "depends"
@@ -88,19 +121,19 @@
         nodeid_to_item_map = {TestDependencyHandler.clean_nodeid(item.nodeid): item for item in items}
 
         for item in items:
             dag.add_node(TestDependencyHandler.clean_nodeid(item.nodeid))
 
             marker = item.get_closest_marker('depends')
             if marker is not None:
-                for dependency in marker.kwargs['on']:
-                    dependency_nodeid = TestDependencyHandler.get_dependency_nodeid(item, dependency)
-                    dag.add_edge(dependency_nodeid, TestDependencyHandler.clean_nodeid(item.nodeid))
+                if marker.kwargs.get('on'):
+                    for dependency in marker.kwargs['on']:
+                        dependency_nodeid = TestDependencyHandler.get_dependency_nodeid(item, dependency)
+                        dag.add_edge(dependency_nodeid, TestDependencyHandler.clean_nodeid(item.nodeid))
 
-        for item in items:
             if not dag.pred[TestDependencyHandler.clean_nodeid(item.nodeid)]:
                 TestDependencyHandler.without_deps_parser(item)
             else:
                 TestDependencyHandler.with_deps_parser(item, dag, nodeid_to_item_map)
 
         return TestDependencyHandler.without_deps + TestDependencyHandler.with_deps
 
@@ -152,14 +185,15 @@
         if tests_failed_after - tests_failed_before > 0:
             test_list = item.config.cache.get('failed_test_list', dict())
             test_list[item.name] = 'Failed'
             item.config.cache.set('failed_test_list', test_list)
 
 
 def pytest_configure(config):
+    config.cache.set(NODE_DEPENDENCY_ITEMS_CACHE, dict())
     config.addinivalue_line(
         "markers", "depends: This marker aims to reshuffle test execution. @pytest.mark.dedpends(on=['a_module.py::a_test'])"
     )
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_collection_modifyitems(items):
```

### Comparing `pytest-node-dependency-1.2.0/pytest_node_dependency.egg-info/PKG-INFO` & `pytest-node-dependency-1.3.0/pytest_node_dependency.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-node-dependency
-Version: 1.2.0
+Version: 1.3.0
 Summary: pytest plugin for controlling execution flow
 Home-page: https://github.com/Formartha/pytest-node-dependency
 Author: Mor Dabastany
 License: MIT
 Keywords: pyest-node-dependency
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
@@ -18,26 +18,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 
 ------
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit)
+![PyPI](https://img.shields.io/pypi/v/PACKAGE?label=pytest-node-dependency)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-node-dependency)
 
 What?
 ------
 pytest-node-dependency is a pytest plugin that allows you to define dependencies between tests and reorder their execution based on those dependencies. This plugin ensures that tests with dependencies run after their required prerequisites have completed successfully.
 
 How to install?
 ----------
 ```
 pip install pytest-node-dependency
 ```
 
-how to use?
+How to use?
 -----------------------------------------------------
 To set up a test dependency, decorate the test function with the `depends` mark and provide a list of dependencies via the `on` keyword argument to the decorator. Dependencies can be specified by name only when in the same file as the test being decorated or by the pytest node path for tests in other files/classes.
 
 ```
 import pytest
 
 
@@ -53,11 +55,42 @@
 
 
 def test_first(request):
     print("first")
     assert request.session.items[0].name == 'test_first'
 ```
 
+Xdist adoption:
+---------------
+The way xdist plugin works is by utilizing multiple cores and spreads the tests among them.
+The problem with the plugin is that if you wish to use reordering, you probably want to set some dependency among the tests,
+However, the xdist plugin will break it.
+
+For that, you should set the group for the tests. The group means that a gateway worker will collect the tests, and will 
+place all the grouped tests in a single gateway worker. 
+This will lead creation of serial testing among parallel exectuion.
+
+```
+import pytest
+
+@pytest.mark.depends(xdist_group='a')
+def test_second(request):
+    print("second")
+    assert request.session.items[1].name == 'test_second'
+
+
+@pytest.mark.depends(on=["test_plugin.py::test_second"], xdist_group='a')
+def test_last(request):
+    print("last")
+    assert request.session.items[2].name == 'test_last'
+
+
+def test_first(request):
+    print("first")
+    assert request.session.items[0].name == 'test_first'
+```
+
+
 Limitations and known issues:
 -----------------------------------------------------
-* The plugin logic makes tests run one after the other in a serial way, as a result, x-dist isn't supported (currently).
-* All the tests without depednecy (both dependent on and depends on) will run first, afterwards all tests with connections will run (e.g. the list of items will be as described)
+* All the tests without dependency (both dependent-on) will run first, then, all tests with connections will run
+(e.g. the list of items will be as described)
```

### Comparing `pytest-node-dependency-1.2.0/setup.py` & `pytest-node-dependency-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION_NUMBER = "1.2.0"
+VERSION_NUMBER = "1.3.0"
 
 # Load the README file as the long description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name="pytest-node-dependency",
       version=VERSION_NUMBER,
```

