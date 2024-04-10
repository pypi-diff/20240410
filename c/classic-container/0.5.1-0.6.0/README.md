# Comparing `tmp/classic-container-0.5.1.tar.gz` & `tmp/classic-container-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classic-container-0.5.1.tar", last modified: Thu Feb 15 03:16:34 2024, max compression
+gzip compressed data, was "classic-container-0.6.0.tar", last modified: Wed Apr 10 14:00:55 2024, max compression
```

## Comparing `classic-container-0.5.1.tar` & `classic-container-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:33.495728 classic-container-0.5.1/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     1071 2024-01-15 08:57:59.000000 classic-container-0.5.1/LICENSE
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    20543 2024-02-15 03:16:33.480560 classic-container-0.5.1/PKG-INFO
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    19672 2024-02-14 17:06:44.000000 classic-container-0.5.1/README.md
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      110 2024-01-15 08:57:59.000000 classic-container-0.5.1/pyproject.toml
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      851 2024-02-15 03:16:33.517899 classic-container-0.5.1/setup.cfg
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)       38 2024-01-15 08:57:59.000000 classic-container-0.5.1/setup.py
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:31.939957 classic-container-0.5.1/sources/
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:31.933055 classic-container-0.5.1/sources/classic/
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:32.732638 classic-container-0.5.1/sources/classic/container/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      473 2024-02-14 17:06:44.000000 classic-container-0.5.1/sources/classic/container/__init__.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     6554 2024-02-14 17:35:25.000000 classic-container-0.5.1/sources/classic/container/builder.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      260 2024-01-15 08:57:59.000000 classic-container-0.5.1/sources/classic/container/constants.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     6766 2024-02-14 17:35:25.000000 classic-container-0.5.1/sources/classic/container/container.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     7287 2024-02-14 17:06:44.000000 classic-container-0.5.1/sources/classic/container/registry.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    10816 2024-02-14 17:06:44.000000 classic-container-0.5.1/sources/classic/container/settings.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      288 2024-02-14 17:06:44.000000 classic-container-0.5.1/sources/classic/container/types.py
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:33.436033 classic-container-0.5.1/sources/classic_container.egg-info/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)    20543 2024-02-15 03:16:30.000000 classic-container-0.5.1/sources/classic_container.egg-info/PKG-INFO
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)      635 2024-02-15 03:16:31.000000 classic-container-0.5.1/sources/classic_container.egg-info/SOURCES.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)        1 2024-02-15 03:16:31.000000 classic-container-0.5.1/sources/classic_container.egg-info/dependency_links.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)       99 2024-02-15 03:16:31.000000 classic-container-0.5.1/sources/classic_container.egg-info/requires.txt
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)        8 2024-02-15 03:16:31.000000 classic-container-0.5.1/sources/classic_container.egg-info/top_level.txt
-drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-02-15 03:16:33.321045 classic-container-0.5.1/tests/
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     5708 2024-02-14 17:06:44.000000 classic-container-0.5.1/tests/test_container.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     2295 2024-02-15 02:55:45.000000 classic-container-0.5.1/tests/test_nested_resolve.py
--rwxrwxrwx   0 variasov  (1000) variasov  (1000)     2011 2024-02-14 17:06:44.000000 classic-container-0.5.1/tests/test_settings.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.460791 classic-container-0.6.0/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     1071 2024-01-15 08:57:59.000000 classic-container-0.6.0/LICENSE
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    20543 2024-04-10 14:00:55.460791 classic-container-0.6.0/PKG-INFO
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    19672 2024-02-14 17:06:44.000000 classic-container-0.6.0/README.md
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      110 2024-01-15 08:57:59.000000 classic-container-0.6.0/pyproject.toml
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      851 2024-04-10 14:00:55.476414 classic-container-0.6.0/setup.cfg
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)       38 2024-01-15 08:57:59.000000 classic-container-0.6.0/setup.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.134982 classic-container-0.6.0/sources/
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.134982 classic-container-0.6.0/sources/classic/
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.313647 classic-container-0.6.0/sources/classic/container/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      473 2024-02-14 17:06:44.000000 classic-container-0.6.0/sources/classic/container/__init__.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     6634 2024-04-10 12:29:51.000000 classic-container-0.6.0/sources/classic/container/builder.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      260 2024-01-15 08:57:59.000000 classic-container-0.6.0/sources/classic/container/constants.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     6766 2024-02-15 03:17:07.000000 classic-container-0.6.0/sources/classic/container/container.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     7328 2024-04-10 12:29:51.000000 classic-container-0.6.0/sources/classic/container/registry.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    10816 2024-02-14 17:06:44.000000 classic-container-0.6.0/sources/classic/container/settings.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      288 2024-02-14 17:06:44.000000 classic-container-0.6.0/sources/classic/container/types.py
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.460791 classic-container-0.6.0/sources/classic_container.egg-info/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)    20543 2024-04-10 14:00:54.000000 classic-container-0.6.0/sources/classic_container.egg-info/PKG-INFO
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)      635 2024-04-10 14:00:55.000000 classic-container-0.6.0/sources/classic_container.egg-info/SOURCES.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)        1 2024-04-10 14:00:54.000000 classic-container-0.6.0/sources/classic_container.egg-info/dependency_links.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)       99 2024-04-10 14:00:54.000000 classic-container-0.6.0/sources/classic_container.egg-info/requires.txt
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)        8 2024-04-10 14:00:54.000000 classic-container-0.6.0/sources/classic_container.egg-info/top_level.txt
+drwxrwxrwx   0 variasov  (1000) variasov  (1000)        0 2024-04-10 14:00:55.429547 classic-container-0.6.0/tests/
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     5708 2024-02-15 03:17:51.000000 classic-container-0.6.0/tests/test_container.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     2295 2024-02-15 03:17:07.000000 classic-container-0.6.0/tests/test_nested_resolve.py
+-rwxrwxrwx   0 variasov  (1000) variasov  (1000)     2011 2024-02-14 17:06:44.000000 classic-container-0.6.0/tests/test_settings.py
```

### Comparing `classic-container-0.5.1/LICENSE` & `classic-container-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/PKG-INFO` & `classic-container-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classic-container
-Version: 0.5.1
+Version: 0.6.0
 Summary: Provides container with dependencies resolving
 Home-page: https://github.com/variasov/classic-container
 Author: Sergei Variasov
 Author-email: variasov@gmail.com
 Project-URL: Bug Tracker, https://github.com/variasov/classic-container/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classic-container-0.5.1/README.md` & `classic-container-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/setup.cfg` & `classic-container-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = classic-container
-version = 0.5.1
+version = 0.6.0
 description = Provides container with dependencies resolving
 author = Sergei Variasov
 author_email = variasov@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/variasov/classic-container
 project_urls =
```

### Comparing `classic-container-0.5.1/sources/classic/container/builder.py` & `classic-container-0.6.0/sources/classic/container/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,34 +106,34 @@
         factory = target_settings.factory_ or self._registry.get(target)
         factory_settings = self.get_settings(factory)[0]
 
         # Фабрика выбрана, далее нужно собрать аргументы.
         # Нужно получаем сигнатуру для фабрики,
         # чтобы по ней построить аргументы для вызова фабрики
         factory_kwargs = {}
-        for name, annotation in self._registry.signature(factory).items():
+        for name, parameter in self._registry.signature(factory).items():
 
             # Если для параметра в init было указанно значение,
             # то берем значение "как есть".
             if name in factory_settings.init_:
                 factory_kwargs[name] = factory_settings.init_[name]
                 continue
 
             # Для аргументов простых типов контейнер не ищет фабрики
-            if annotation in SIMPLE_TYPES:
+            if parameter.annotation in SIMPLE_TYPES:
                 continue
 
             # Инстанцирование аргумента
-            if inspect.isclass(annotation):
-                instance = self.build(annotation)
+            if inspect.isclass(parameter.annotation):
+                instance = self.build(parameter.annotation)
                 if instance is not None:
                     factory_kwargs[name] = instance
 
-                # Странный случай, когда фабрика вернула None
-                if instance is None:
+                # Случай, когда нечего указать в обязательный аргумент
+                elif parameter.default is inspect.Parameter.empty:
                     raise ValueError(
                         f"Can't resole attribute {name} "
                         f"for {factory}, attribute don't have default value "
                         f"and {factory} has returned None. "
                         f"Maybe you have forgot to add 'return' "
                         f"to the end of your factory?"
                     )
```

### Comparing `classic-container-0.5.1/sources/classic/container/container.py` & `classic-container-0.6.0/sources/classic/container/container.py`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/sources/classic/container/registry.py` & `classic-container-0.6.0/sources/classic/container/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     _storage = dict[Target, list[Factory[Target]]]
 
     def __init__(self):
         self._storage = defaultdict(list)
         self._signatures_cache = {}
 
     @lru_cache(1000)
-    def signature(self, cls: Target) -> dict[str, object]:
+    def signature(self, cls: Target) -> dict[str, inspect.Parameter]:
         """
         Возвращает описание сигнатуры указанной фабрики.
         Отличается от обычного inspect.signature тем,
         что пытается разрешить ForwardReference.
 
         Например:
         >>> class Test:
@@ -42,15 +42,15 @@
         result = {}
         for name, parameter in signature.parameters.items():
             if isinstance(parameter.annotation, str):
                 hint = hints[name]
             else:
                 hint = parameter.annotation
 
-            result[name] = hint
+            result[name] = parameter.replace(annotation=hint)
 
         return result
 
     def get(self, target: Target) -> Factory[Target]:
         """
         Вернет фабрику для указанного класса.
```

### Comparing `classic-container-0.5.1/sources/classic/container/settings.py` & `classic-container-0.6.0/sources/classic/container/settings.py`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/sources/classic_container.egg-info/PKG-INFO` & `classic-container-0.6.0/sources/classic_container.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classic-container
-Version: 0.5.1
+Version: 0.6.0
 Summary: Provides container with dependencies resolving
 Home-page: https://github.com/variasov/classic-container
 Author: Sergei Variasov
 Author-email: variasov@gmail.com
 Project-URL: Bug Tracker, https://github.com/variasov/classic-container/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `classic-container-0.5.1/sources/classic_container.egg-info/SOURCES.txt` & `classic-container-0.6.0/sources/classic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/tests/test_container.py` & `classic-container-0.6.0/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/tests/test_nested_resolve.py` & `classic-container-0.6.0/tests/test_nested_resolve.py`

 * *Files identical despite different names*

### Comparing `classic-container-0.5.1/tests/test_settings.py` & `classic-container-0.6.0/tests/test_settings.py`

 * *Files identical despite different names*

