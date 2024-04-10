# Comparing `tmp/django_markov-0.2.2.tar.gz` & `tmp/django_markov-0.2.3.tar.gz`

## Comparing `django_markov-0.2.2.tar` & `django_markov-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/admin.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/apps.py
--rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/py.typed
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0003_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.2/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/settings.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.2/tests/urls.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.2/.gitignore
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.2/LICENSE
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.2/README.md
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/apps.py
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/py.typed
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/settings.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.3/README.md
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.3/PKG-INFO
```

### Comparing `django_markov-0.2.2/src/django_markov/models.py` & `django_markov-0.2.3/src/django_markov/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 
 class MarkovCombineError(Exception):
     """Exception raised when attempt to combine incompatible model chains."""
 
     pass
 
 
+class MarkovEmptyError(Exception):
+    """Raised when attempting to do model comparison and inspection on
+    empty models."""
+
+    pass
+
+
 sentence_generated = dispatch.Signal()
 
 
 def _get_corpus_char_limit() -> int:
     """Get the corpus character limit from settings or return a default."""
     if not hasattr(settings, "MARKOV_CORPUS_MAX_CHAR_LIMIT") or not isinstance(
         settings.MARKOV_CORPUS_MAX_CHAR_LIMIT, int
@@ -45,15 +52,15 @@
 
     Attributes:
         created (datetime.datetime): Date and time when the model was created.
         modified (datetime.datetime): Date and time when the model was last modified.
         data (JSON): The text model as JSON.
     """
 
-    cached_properties: ClassVar[list[str]] = ["_compiled_model"]
+    cached_properties: ClassVar[list[str]] = ["_compiled_model", "is_compiled_model"]
 
     created = models.DateTimeField(
         auto_now_add=True, help_text=_("When the model was created.")
     )
     modified = models.DateTimeField(
         auto_now=True, help_text=_("Last modification of the record.")
     )
@@ -92,14 +99,25 @@
         """
         if not self.is_ready:
             return None
         text_model = POSifiedText.from_json(self.data)
         return text_model
 
     @cached_property
+    def is_compiled_model(self) -> bool:
+        """
+        Checks if the stored data for the text mile is compiled.
+        """
+        text_model = self._as_text_model()
+        if text_model is None:
+            msg = "There is not data in this model and it cannot be inspected."
+            raise MarkovEmptyError(msg)
+        return text_model.chain.compiled
+
+    @cached_property
     def _compiled_model(self) -> POSifiedText | None:
         """
         The text model loaded into a POSifiedText object and compiled. You shouldn't
         ever access this property directly. It's used to optimize performance when you
         generate multiple sentences over the course of the model.
 
         Returns:
```

### Comparing `django_markov-0.2.2/src/django_markov/text_models.py` & `django_markov-0.2.3/src/django_markov/text_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/src/django_markov/migrations/0001_initial.py` & `django_markov-0.2.3/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.2.3/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/src/django_markov/migrations/0003_markovtextmodel_compiled.py` & `django_markov-0.2.3/src/django_markov/migrations/0003_markovtextmodel_compiled.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/tests/settings.py` & `django_markov-0.2.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/tests/test_models.py` & `django_markov-0.2.3/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any
 
 import pytest
 from faker import Faker
 
 from django_markov.models import (
     MarkovCombineError,
+    MarkovEmptyError,
     MarkovTextModel,
     _get_corpus_char_limit,
 )
 from django_markov.text_models import POSifiedText
 
 pytestmark = pytest.mark.django_db(transaction=True)
 
@@ -44,14 +45,15 @@
 def test_text_models_return_none_on_empty_directive():
     model = MarkovTextModel.objects.create()
     assert not model._as_text_model()
     assert not model._compiled_model
 
 
 def test_do_not_recompile_compiled_model(compiled_model):
+    assert compiled_model.is_compiled_model
     assert (
         compiled_model._as_text_model().to_json()
         == compiled_model._compiled_model.to_json()
     )
 
 
 def test_compile_non_compiled_model(sample_corpus):
@@ -59,14 +61,21 @@
     model.update_model_from_corpus(
         [sample_corpus, "My name is Inigo Montoya."], store_compiled=False
     )
     assert model.data
     model.refresh_from_db()
     assert not model._as_text_model().chain.compiled
     assert model._compiled_model.chain.compiled
+    assert not model.is_compiled_model
+
+
+def test_inspect_empty_model():
+    model = MarkovTextModel.objects.create()
+    with pytest.raises(MarkovEmptyError):
+        compiled = model.is_compiled_model  # noqa: F841
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "settings_limit,char_limit,expect_error",
     [
         (500, None, True),
```

### Comparing `django_markov-0.2.2/tests/urls.py` & `django_markov-0.2.3/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/LICENSE` & `django_markov-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/README.md` & `django_markov-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.2/pyproject.toml` & `django_markov-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-markov"
-version = "0.2.2"
+version = "0.2.3"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
     "django>=4.2",
     "markovify>=0.9.4",
@@ -224,15 +224,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.2.2"
+current_version = "0.2.3"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_markov-0.2.2/PKG-INFO` & `django_markov-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.2.2
+Version: 0.2.3
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

