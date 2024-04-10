# Comparing `tmp/owlapy-0.1.2.tar.gz` & `tmp/owlapy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlapy-0.1.2.tar", last modified: Thu Mar 28 12:11:24 2024, max compression
+gzip compressed data, was "owlapy-0.1.3.tar", last modified: Wed Apr 10 10:55:17 2024, max compression
```

## Comparing `owlapy-0.1.2.tar` & `owlapy-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,55 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.332508 owlapy-0.1.2/
--rw-rw-r--   0 demir     (1000) demir     (1000)     1056 2024-03-25 12:18:36.000000 owlapy-0.1.2/LICENSE
--rw-r--r--   0 demir     (1000) demir     (1000)     3687 2024-03-28 12:11:24.332508 owlapy-0.1.2/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     3007 2024-03-27 12:12:27.000000 owlapy-0.1.2/README.md
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.328508 owlapy-0.1.2/owlapy/
--rw-rw-r--   0 demir     (1000) demir     (1000)       22 2024-03-25 12:36:01.000000 owlapy-0.1.2/owlapy/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)      419 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/_utils.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1186 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/io.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.332508 owlapy-0.1.2/owlapy/model/
--rw-rw-r--   0 demir     (1000) demir     (1000)   132126 2024-03-28 12:00:48.000000 owlapy-0.1.2/owlapy/model/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1889 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/model/_base.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     5618 2024-03-28 12:00:48.000000 owlapy-0.1.2/owlapy/model/_iri.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2743 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/model/providers.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     1288 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/namespaces.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.332508 owlapy-0.1.2/owlapy/owl2sparql/
--rw-rw-r--   0 demir     (1000) demir     (1000)       31 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/owl2sparql/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    26234 2024-03-27 12:12:27.000000 owlapy-0.1.2/owlapy/owl2sparql/converter.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    36135 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/parser.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    15513 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/render.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    21545 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/util.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     4377 2024-03-25 12:18:36.000000 owlapy-0.1.2/owlapy/vocab.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.332508 owlapy-0.1.2/owlapy.egg-info/
--rw-r--r--   0 demir     (1000) demir     (1000)     3687 2024-03-28 12:11:24.000000 owlapy-0.1.2/owlapy.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      611 2024-03-28 12:11:24.000000 owlapy-0.1.2/owlapy.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2024-03-28 12:11:24.000000 owlapy-0.1.2/owlapy.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       62 2024-03-28 12:11:24.000000 owlapy-0.1.2/owlapy.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        7 2024-03-28 12:11:24.000000 owlapy-0.1.2/owlapy.egg-info/top_level.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       80 2024-03-28 12:08:04.000000 owlapy-0.1.2/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)       38 2024-03-28 12:11:24.332508 owlapy-0.1.2/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)      920 2024-03-28 12:00:48.000000 owlapy-0.1.2/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-03-28 12:11:24.332508 owlapy-0.1.2/tests/
--rw-rw-r--   0 demir     (1000) demir     (1000)     1613 2024-03-25 12:18:36.000000 owlapy-0.1.2/tests/test_owlapy.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    11164 2024-03-25 12:18:36.000000 owlapy-0.1.2/tests/test_owlapy_cnf_dnf.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    18138 2024-03-25 12:18:36.000000 owlapy-0.1.2/tests/test_owlapy_nnf.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    29978 2024-03-25 12:18:36.000000 owlapy-0.1.2/tests/test_owlapy_parser.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     8586 2024-03-25 12:18:36.000000 owlapy-0.1.2/tests/test_owlapy_render.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1056 2024-03-25 12:18:36.000000 owlapy-0.1.3/LICENSE
+-rw-r--r--   0 demir     (1000) demir     (1000)     3602 2024-04-10 10:55:17.138621 owlapy-0.1.3/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2922 2024-04-10 10:54:54.000000 owlapy-0.1.3/README.md
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       22 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      419 2024-03-25 12:18:36.000000 owlapy-0.1.3/owlapy/_utils.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy/class_expression/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2206 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3206 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/class_expression.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1473 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/nary_boolean_expression.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1483 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/owl_class.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    25473 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/class_expression/restriction.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/data_ranges/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2683 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/data_ranges/__init__.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/entities/
+-rw-rw-r--   0 demir     (1000) demir     (1000)      485 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/entities/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      290 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/has.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     5347 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/iri.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1771 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/meta_classes.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/model/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35363 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/model/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2784 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/model/providers.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1288 2024-03-25 12:18:36.000000 owlapy-0.1.3/owlapy/namespaces.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/owlapy/owl2sparql/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       31 2024-04-08 17:49:23.000000 owlapy-0.1.3/owlapy/owl2sparql/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    24053 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl2sparql/converter.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1443 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_annotation.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    43211 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_axiom.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1115 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_individual.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    15935 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_literal.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     6005 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owl_property.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2466 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/owlobject.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    36488 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/parser.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    15925 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/render.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)      795 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/types.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    21630 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/util.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4389 2024-04-10 10:54:54.000000 owlapy-0.1.3/owlapy/vocab.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.134621 owlapy-0.1.3/owlapy.egg-info/
+-rw-r--r--   0 demir     (1000) demir     (1000)     3602 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1087 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       62 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        7 2024-04-10 10:55:17.000000 owlapy-0.1.3/owlapy.egg-info/top_level.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       80 2024-03-28 12:08:04.000000 owlapy-0.1.3/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)       38 2024-04-10 10:55:17.138621 owlapy-0.1.3/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)      920 2024-04-10 10:54:54.000000 owlapy-0.1.3/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2024-04-10 10:55:17.138621 owlapy-0.1.3/tests/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1191 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_class_expression_semantics.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1330 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_examples.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1613 2024-04-08 17:49:23.000000 owlapy-0.1.3/tests/test_owlapy.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    11198 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_cnf_dnf.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    18196 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_nnf.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    30062 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_parser.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     8674 2024-04-10 10:54:54.000000 owlapy-0.1.3/tests/test_owlapy_render.py
```

### Comparing `owlapy-0.1.2/LICENSE` & `owlapy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `owlapy-0.1.2/PKG-INFO` & `owlapy-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlapy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Owlapy is loosely based on owlapi - the java counterpart, successfully representing the main owl objects in python.
 Home-page: https://github.com/dice-group/owlapy
 Author: Caglar Demir
 Author-email: caglardemir8@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering
@@ -35,37 +35,34 @@
 ## Usage
 <details><summary> Click me! </summary>
 
 In this example we start with a simple atomic class expression and move to some more complex 
 ones and finally render and print the last of them in description logics syntax.
 
 ```python
-from owlapy.render import DLSyntaxObjectRenderer
-from owlapy.model import IRI, OWLClass, OWLObjectProperty, OWLObjectSomeValuesFrom, \
-                         OWLObjectIntersectionOf
+from owlapy.iri import IRI
+from owlapy.class_expression import OWLClass, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom
+from owlapy.owl_property import OWLObjectProperty
 from owlapy.owl2sparql.converter import owl_expression_to_sparql
-
-# Create an IRI object using the iri as a string for 'male' class.
-male_iri = IRI.create('http://example.com/society#male')
-
+from owlapy.render import owl_expression_to_dl
 # Create the male class
-male = OWLClass(male_iri)
+male = OWLClass("http://example.com/society#male")
 
 # Create an object property using the iri as a string for 'hasChild' property.
-hasChild = OWLObjectProperty(IRI.create('http://example.com/society#hasChild'))
+hasChild = OWLObjectProperty("http://example.com/society#hasChild")
 
 # Create an existential restrictions
 males_with_children = OWLObjectSomeValuesFrom(hasChild, male)
 
 # Let's make it more complex by intersecting with another class
-teacher = OWLClass(IRI.create('http://example.com/society#teacher'))
+teacher = OWLClass("http://example.com/society#teacher")
 male_teachers_with_children = OWLObjectIntersectionOf([males_with_children, teacher])
 
-# You can render and print owl class expressions in description logics syntax
-print(DLSyntaxObjectRenderer().render(male_teachers_with_children)) 
+# You can render and print owl class expressions in description logics syntax (and vice-versa)
+print(owl_expression_to_dl(male_teachers_with_children))
 # (∃ hasChild.male) ⊓ teacher
 print(owl_expression_to_sparql("?x", male_teachers_with_children))
 #  SELECT DISTINCT ?x WHERE {  ?x <http://example.com/society#hasChild> ?s_1 . ?s_1 a <http://example.com/society#male> . ?x a <http://example.com/society#teacher> .  } }
 ```
 For more, you can check the [API documentation](https://ontolearn-docs-dice-group.netlify.app/autoapi/owlapy/#module-owlapy).
```

### Comparing `owlapy-0.1.2/README.md` & `owlapy-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,37 +17,34 @@
 ## Usage
 <details><summary> Click me! </summary>
 
 In this example we start with a simple atomic class expression and move to some more complex 
 ones and finally render and print the last of them in description logics syntax.
 
 ```python
-from owlapy.render import DLSyntaxObjectRenderer
-from owlapy.model import IRI, OWLClass, OWLObjectProperty, OWLObjectSomeValuesFrom, \
-                         OWLObjectIntersectionOf
+from owlapy.iri import IRI
+from owlapy.class_expression import OWLClass, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom
+from owlapy.owl_property import OWLObjectProperty
 from owlapy.owl2sparql.converter import owl_expression_to_sparql
-
-# Create an IRI object using the iri as a string for 'male' class.
-male_iri = IRI.create('http://example.com/society#male')
-
+from owlapy.render import owl_expression_to_dl
 # Create the male class
-male = OWLClass(male_iri)
+male = OWLClass("http://example.com/society#male")
 
 # Create an object property using the iri as a string for 'hasChild' property.
-hasChild = OWLObjectProperty(IRI.create('http://example.com/society#hasChild'))
+hasChild = OWLObjectProperty("http://example.com/society#hasChild")
 
 # Create an existential restrictions
 males_with_children = OWLObjectSomeValuesFrom(hasChild, male)
 
 # Let's make it more complex by intersecting with another class
-teacher = OWLClass(IRI.create('http://example.com/society#teacher'))
+teacher = OWLClass("http://example.com/society#teacher")
 male_teachers_with_children = OWLObjectIntersectionOf([males_with_children, teacher])
 
-# You can render and print owl class expressions in description logics syntax
-print(DLSyntaxObjectRenderer().render(male_teachers_with_children)) 
+# You can render and print owl class expressions in description logics syntax (and vice-versa)
+print(owl_expression_to_dl(male_teachers_with_children))
 # (∃ hasChild.male) ⊓ teacher
 print(owl_expression_to_sparql("?x", male_teachers_with_children))
 #  SELECT DISTINCT ?x WHERE {  ?x <http://example.com/society#hasChild> ?s_1 . ?s_1 a <http://example.com/society#male> . ?x a <http://example.com/society#teacher> .  } }
 ```
 For more, you can check the [API documentation](https://ontolearn-docs-dice-group.netlify.app/autoapi/owlapy/#module-owlapy).
```

### Comparing `owlapy-0.1.2/owlapy/model/_base.py` & `owlapy-0.1.3/owlapy/owl_annotation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-from abc import ABCMeta, abstractmethod
-from typing import Optional, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from owlapy.model._iri import IRI
-    from owlapy.model import OWLLiteral
-
-
-class OWLObject(metaclass=ABCMeta):
-    """Base interface for OWL objects"""
-    __slots__ = ()
-
-    @abstractmethod
-    def __eq__(self, other):
-        pass
-
-    @abstractmethod
-    def __hash__(self):
-        pass
-
-    @abstractmethod
-    def __repr__(self):
-        pass
-
-    # default
-    def is_anonymous(self) -> bool:
-        return True
+from abc import ABCMeta
+from .owlobject import OWLObject
+from typing import Optional
 
 
 class OWLAnnotationObject(OWLObject, metaclass=ABCMeta):
     """A marker interface for the values (objects) of annotations."""
     __slots__ = ()
 
     # noinspection PyMethodMayBeStatic
@@ -43,21 +19,19 @@
     def as_anonymous_individual(self):
         """
         Returns:
             if the value is an anonymous, return it. Return None otherwise.
         """
         return None
 
-
 class OWLAnnotationSubject(OWLAnnotationObject, metaclass=ABCMeta):
     """A marker interface for annotation subjects, which can either be IRIs or anonymous individuals"""
     __slots__ = ()
     pass
 
-
 class OWLAnnotationValue(OWLAnnotationObject, metaclass=ABCMeta):
     """A marker interface for annotation values, which can either be an IRI (URI), Literal or Anonymous Individual."""
     __slots__ = ()
 
     def is_literal(self) -> bool:
         """
         Returns:
@@ -67,8 +41,8 @@
 
     # noinspection PyMethodMayBeStatic
     def as_literal(self) -> Optional['OWLLiteral']:
         """
         Returns:
             if the value is a literal, returns it. Return None otherwise
         """
-        return None
+        return None
```

### Comparing `owlapy-0.1.2/owlapy/model/_iri.py` & `owlapy-0.1.3/owlapy/iri.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 import weakref
 from abc import ABCMeta, abstractmethod
 from typing import Final, Union, overload
 from weakref import WeakKeyDictionary
 
 from owlapy import namespaces
-from owlapy.model._base import OWLAnnotationSubject, OWLAnnotationValue
+from .owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
 from owlapy.namespaces import Namespaces
 
 
-class HasIRI(metaclass=ABCMeta):
-    """Simple class to access the IRI."""
-    __slots__ = ()
-
-    @abstractmethod
-    def get_iri(self) -> 'IRI':
-        """Gets the IRI of this object.
-
-        Returns:
-            The IRI of this object.
-        """
-        pass
-
-
 class _WeakCached(type):
     __slots__ = ()
 
     def __init__(cls, what, bases, dct):
         super().__init__(what, bases, dct)
         cls._cache = WeakKeyDictionary()
```

### Comparing `owlapy-0.1.2/owlapy/model/providers.py` & `owlapy-0.1.3/owlapy/model/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """OWL Datatype restriction constructors."""
 from typing import Union
 from datetime import datetime, date
-from owlapy.model import OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction, OWLLiteral
+from owlapy.owl_literal import OWLLiteral
+from owlapy.class_expression import OWLDatatypeRestriction, OWLFacet, OWLFacetRestriction
 from pandas import Timedelta
 
 Restriction_Literals = Union[OWLLiteral, int, float, Timedelta, datetime, date]
 
 
 def OWLDatatypeMaxExclusiveRestriction(max_: Restriction_Literals) -> OWLDatatypeRestriction:
     """Create a max exclusive restriction."""
```

### Comparing `owlapy-0.1.2/owlapy/namespaces.py` & `owlapy-0.1.3/owlapy/namespaces.py`

 * *Files identical despite different names*

### Comparing `owlapy-0.1.2/owlapy/owl2sparql/converter.py` & `owlapy-0.1.3/owlapy/owl2sparql/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from functools import singledispatchmethod
 from types import MappingProxyType
 from typing import Set, List, Dict, Optional, Iterable
 
 from rdflib.plugins.sparql.parser import parseQuery
 
 from owlapy.model import OWLClassExpression, OWLClass, OWLEntity, OWLObjectProperty, \
-    OWLObjectUnionOf, OWLObjectComplementOf, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, OWLObjectHasValue, \
+    OWLObjectUnionOf, OWLObjectComplementOf, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
     OWLNamedIndividual, OWLObjectCardinalityRestriction, OWLObjectMinCardinality, OWLObjectExactCardinality, \
-    OWLObjectMaxCardinality, OWLDataCardinalityRestriction, OWLDataProperty, OWLObjectHasSelf, OWLObjectOneOf, \
-    OWLDataSomeValuesFrom, OWLDataAllValuesFrom, OWLDataHasValue, OWLDatatype, TopOWLDatatype, OWLDataOneOf, \
-    OWLLiteral, OWLDatatypeRestriction, OWLObjectIntersectionOf
+    OWLObjectMaxCardinality, OWLDataCardinalityRestriction, OWLDataProperty, OWLObjectHasSelf, \
+    OWLDataSomeValuesFrom, OWLDataAllValuesFrom, OWLDataHasValue, OWLDatatype, TopOWLDatatype, OWLDataOneOf, OWLObjectIntersectionOf
+from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf, OWLDatatypeRestriction
+from owlapy.owl_literal import OWLLiteral
 from owlapy.vocab import OWLFacet, OWLRDFVocabulary
 
 _Variable_facet_comp = MappingProxyType({
     OWLFacet.MIN_INCLUSIVE: ">=",
     OWLFacet.MIN_EXCLUSIVE: ">",
     OWLFacet.MAX_INCLUSIVE: "<=",
     OWLFacet.MAX_EXCLUSIVE: "<"
@@ -77,14 +78,15 @@
         return self.dict[item]
 
 
 class Owl2SparqlConverter:
     """Convert owl (owlapy model class expressions) to SPARQL."""
     __slots__ = 'ce', 'sparql', 'variables', 'parent', 'parent_var', 'properties', 'variable_entities', 'cnt', \
                 'mapping', 'grouping_vars', 'having_conditions', '_intersection'
+    # @TODO:CD: We need to document this class. The computation behind the mapping is not clear.
 
     ce: OWLClassExpression
     sparql: List[str]
     variables: List[str]
     parent: List[OWLClassExpression]
     parent_var: List[str]
     variable_entities: Set[OWLEntity]
@@ -126,18 +128,14 @@
                 self.process(ce)
         return self.sparql
 
     @property
     def modal_depth(self):
         return len(self.variables)
 
-    # @property
-    # def in_intersection(self):
-    #     return self._intersection[self.modal_depth]
-
     @singledispatchmethod
     def render(self, e):
         raise NotImplementedError(e)
 
     @render.register
     def _(self, lit: OWLLiteral):
         return f'"{lit.get_literal()}"^^<{lit.get_datatype().to_string_id()}>'
@@ -170,21 +168,14 @@
 
     def _maybe_render(self, o):
         if isinstance(o, str):
             return o
         else:
             return self.render(o)
 
-    # @contextmanager
-    # def intersection(self):
-    #     self._intersection[self.modal_depth] = True
-    #     try:
-    #         yield
-    #     finally:
-    #         del self._intersection[self.modal_depth]
 
     @contextmanager
     def stack_variable(self, var):
         self.variables.append(var)
         try:
             yield
         finally:
@@ -232,29 +223,14 @@
     # general case: C1 ⊓ ... ⊓ Cn
     @process.register
     def _(self, ce: OWLObjectIntersectionOf):
         # we iterate over the concepts that appear in the intersection
         for op in ce.operands():
             self.process(op)
 
-        # the following part was commented out because it was related to the possible optimization in the complement
-        # operator that has also been commented out
-        # with self.intersection():
-        #     for op in ce.operands():
-        #         self.process(op)
-        #     props = self.properties[self.modal_depth]
-        #     vars_ = set()
-        #     if props:
-        #         for p in props:
-        #             if p in self.mapping:
-        #                 vars_.add(self.mapping[p])
-        #         if len(vars_) == 2:
-        #             v0, v1 = sorted(vars_)
-        #             self.append(f"FILTER ( {v0} != {v1} )")
-
     # an overload of process function
     # this overload is responsible for handling unions of concepts (e.g., Brother ⊔ Sister)
     # general case: C1 ⊔ ... ⊔ Cn
     @process.register
     def _(self, ce: OWLObjectUnionOf):
         first = True
         # we iterate over the concepts that appear in the union
@@ -271,22 +247,14 @@
 
     # an overload of process function
     # this overload is responsible for handling complements of concepts (e.g., ¬Brother)
     # general case: ¬C
     @process.register
     def _(self, ce: OWLObjectComplementOf):
         subject = self.current_variable
-        # the conversion was trying here to optimize the query
-        # but the proposed optimization alters the semantics of some queries
-        # example: ( A ⊓ ( B ⊔ ( ¬C ) ) )
-        # with the proposed optimization, the group graph pattern for (¬C) will be { FILTER NOT EXISTS { ?x a C } }
-        # however, the expected pattern is { ?x ?p ?o . FILTER NOT EXISTS { ?x a C } }
-        # the exclusion of "?x ?p ?o" results in the group graph pattern to just return true or false (not bindings)
-        # as a result, we need to comment out the if-clause of the following line
-        # if not self.in_intersection and self.modal_depth == 1:
         self.append_triple(subject, self.mapping.new_individual_variable(), self.mapping.new_individual_variable())
 
         self.append("FILTER NOT EXISTS { ")
         # process the concept after the ¬
         self.process(ce.get_operand())
         self.append(" }")
 
@@ -317,27 +285,17 @@
         object_variable = self.mapping.new_individual_variable()
         # property expression holds the role of the class expression (hasChild in our example)
         property_expression = ce.get_property()
         predicate = property_expression.get_named_property()
         # filler holds the concept of the expression (Male in our example) and is processed recursively
         filler = ce.get_filler()
 
-        # if the current class expression is the first one we are processing (root of recursion), the following
-        # if-clause tries to restrict the entities (individuals) to consider using owl:NamedIndividual.
-        # However, it is not guaranteed that entities in every KG are instances of owl:NamedIndividual, hence, adding
-        # this triple will affect the results in such cases.
-        # if self.modal_depth == 1:
-        #     self.append_triple(self.current_variable, "a", f"<{OWLRDFVocabulary.OWL_NAMED_INDIVIDUAL.as_str()}>")
 
-        # here, the first group graph pattern starts
-        # the first group graph pattern ensures deals with the entities that appear in a triple with the property
         self.append("{")
-        # if filler.is_owl_thing():
-        #     self.append_triple(self.current_variable, self.mapping.new_property_variable(), object_variable)
-        # else:
+
         if property_expression.is_anonymous():
             # property expression is inverse of a property
             self.append_triple(object_variable, predicate, self.current_variable)
         else:
             self.append_triple(self.current_variable, predicate, object_variable)
 
         # restrict filler
@@ -588,21 +546,25 @@
         return f"{self._maybe_quote(subject)} {self._maybe_quote_p(predicate)} {self._maybe_render(object_)} . "
 
     def as_query(self,
                  root_variable: str,
                  ce: OWLClassExpression,
                  count: bool = False,
                  values: Optional[Iterable[OWLNamedIndividual]] = None,
-                 named_individuals: bool = False):
-        # root variable: the variable that will be projected
-        # ce: the class expression to be transformed to a SPARQL query
-        # count: True, counts the results ; False, projects the individuals
-        # values: positive or negative examples from a class expression problem
-        # named_individuals: if set to True, the generated SPARQL query will return only entities that are instances
-        #                    of owl:NamedIndividual
+                 named_individuals: bool = False)->str:
+        """
+        root variable: the variable that will be projected
+        ce: the class expression to be transformed to a SPARQL query
+        count: True, counts the results ; False, projects the individuals
+        values: positive or negative examples from a class expression problem
+        named_individuals: if set to True, the generated SPARQL query will return only entities that are instances
+        of owl:NamedIndividual
+
+        """
+
         qs = ["SELECT"]
         tp = self.convert(root_variable, ce, named_individuals)
         if count:
             qs.append(f" ( COUNT ( DISTINCT {root_variable} ) AS ?cnt ) WHERE {{ ")
         else:
             qs.append(f" DISTINCT {root_variable} WHERE {{ ")
         if values is not None and root_variable.startswith("?"):
@@ -610,30 +572,30 @@
             for x in values:
                 q.append(f"<{x.to_string_id()}>")
             q.append(f"}} . ")
             qs.extend(q)
         qs.extend(tp)
         qs.append(f" }}")
 
-        # group_by_vars = self.grouping_vars[ce]
-        # if group_by_vars:
-        #     qs.append("GROUP BY " + " ".join(sorted(group_by_vars)))
-        # conditions = self.having_conditions[ce]
-        # if conditions:
-        #     qs.append(" HAVING ( ")
-        #     qs.append(" && ".join(sorted(conditions)))
-        #     qs.append(" )")
 
         query = "\n".join(qs)
         parseQuery(query)
         return query
 
 
 converter = Owl2SparqlConverter()
 
 
-def owl_expression_to_sparql(root_variable: str,
-                             ce: OWLClassExpression,
-                             count: bool = False,
+def owl_expression_to_sparql(root_variable: str = "?x",
+                             expression: OWLClassExpression = None,
                              values: Optional[Iterable[OWLNamedIndividual]] = None,
-                             named_individuals: bool = False):
-    return converter.as_query(root_variable, ce, count, values, named_individuals)
+                             named_individuals: bool = False)->str:
+    """Convert an OWL Class Expression (https://www.w3.org/TR/owl2-syntax/#Class_Expressions) into a SPARQL query
+     root variable: the variable that will be projected
+     expression: the class expression to be transformed to a SPARQL query
+
+     values: positive or negative examples from a class expression problem. Unclear
+     named_individuals: if set to True, the generated SPARQL query will return only entities
+     that are instances of owl:NamedIndividual
+    """
+    assert expression is not None, "expression cannot be None"
+    return converter.as_query(root_variable, expression, False, values, named_individuals)
```

### Comparing `owlapy-0.1.2/owlapy/parser.py` & `owlapy-0.1.3/owlapy/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """String to OWL parsers."""
 from types import MappingProxyType
 from typing import Final, List, Optional, Union
 from parsimonious.grammar import Grammar
 from parsimonious.nodes import NodeVisitor
 from parsimonious.nodes import Node
-from owlapy.io import OWLObjectParser
-from owlapy.model import OWLObjectHasSelf, OWLObjectIntersectionOf, OWLObjectMinCardinality, OWLObjectOneOf, \
-    OWLObjectProperty, OWLObjectPropertyExpression, OWLObjectSomeValuesFrom, OWLObjectUnionOf, OWLClass, IRI, \
+from .owlobject import OWLObjectParser
+from .namespaces import Namespaces
+from .render import _DL_SYNTAX, _MAN_SYNTAX
+from .vocab import OWLFacet, OWLRDFVocabulary
+
+
+from owlapy.model import OWLObjectHasSelf, OWLObjectIntersectionOf, OWLObjectMinCardinality, OWLObjectProperty, OWLObjectPropertyExpression, OWLObjectSomeValuesFrom, OWLObjectUnionOf, OWLClass, IRI, \
     OWLClassExpression, OWLDataProperty, OWLNamedIndividual, OWLObjectComplementOf, OWLObjectExactCardinality, \
-    OWLObjectHasValue, OWLQuantifiedDataRestriction, OWLQuantifiedObjectRestriction, StringOWLDatatype,  \
+    OWLQuantifiedDataRestriction, OWLQuantifiedObjectRestriction, StringOWLDatatype,  \
     DateOWLDatatype, DateTimeOWLDatatype, DoubleOWLDatatype, DurationOWLDatatype, IntegerOWLDatatype, \
-    OWLDataSomeValuesFrom, OWLDatatypeRestriction, OWLFacetRestriction, OWLDataExactCardinality, \
-    OWLDataMaxCardinality, OWLObjectMaxCardinality, OWLDataIntersectionOf, OWLDataMinCardinality, OWLDataHasValue, \
-    OWLLiteral, OWLDataRange, OWLDataUnionOf, OWLDataOneOf, OWLDatatype, OWLObjectCardinalityRestriction, \
-    OWLDataCardinalityRestriction, OWLObjectAllValuesFrom, OWLDataAllValuesFrom, OWLDataComplementOf, BooleanOWLDatatype
-from owlapy.namespaces import Namespaces
+    OWLDataSomeValuesFrom, OWLDataExactCardinality, \
+    OWLDataMaxCardinality, OWLObjectMaxCardinality, OWLDataMinCardinality, OWLDataHasValue, \
+    OWLLiteral, OWLDataRange, OWLDataOneOf, OWLDatatype, OWLObjectCardinalityRestriction, \
+    OWLDataCardinalityRestriction, OWLObjectAllValuesFrom, OWLDataAllValuesFrom, BooleanOWLDatatype
 
-from owlapy.render import _DL_SYNTAX, _MAN_SYNTAX
-from owlapy.vocab import OWLFacet, OWLRDFVocabulary
+from owlapy.data_ranges import OWLDataIntersectionOf, OWLDataUnionOf, OWLDataComplementOf
+from owlapy.class_expression import OWLObjectHasValue, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectOneOf
 
 
 MANCHESTER_GRAMMAR = Grammar(r"""
     union = intersection (must_ws "or" must_ws intersection)*
     intersection = primary (must_ws "and" must_ws primary)*
 
     # Main entry point + object properties
@@ -760,7 +763,19 @@
 
     def visit_parentheses(self, node, children) -> OWLClassExpression:
         *_, expr, _, _ = children
         return expr
 
     def generic_visit(self, node, children):
         return children or node
+
+
+DLparser = DLSyntaxParser()
+ManchesterParser = ManchesterOWLSyntaxParser()
+
+
+def dl_to_owl_expression(dl_expression: str):
+    return DLparser.parse_expression(dl_expression)
+
+
+def manchester_to_owl_expression(manchester_expression: str):
+    return ManchesterParser.parse_expression(manchester_expression)
```

### Comparing `owlapy-0.1.2/owlapy/render.py` & `owlapy-0.1.3/owlapy/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 # -*- coding: utf-8 -*-
 
 import types
 from functools import singledispatchmethod
 from typing import List, Callable
 
 from owlapy import namespaces
-from owlapy.io import OWLObjectRenderer
-from owlapy.model import OWLLiteral, OWLNaryDataRange, OWLObject, OWLClass, OWLObjectSomeValuesFrom, \
-    OWLObjectAllValuesFrom, OWLObjectUnionOf, OWLBooleanClassExpression, OWLNaryBooleanClassExpression, \
-    OWLObjectIntersectionOf, OWLObjectComplementOf, OWLObjectInverseOf, OWLClassExpression, OWLRestriction, \
-    OWLObjectMinCardinality, OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLObjectHasSelf, OWLObjectHasValue, \
-    OWLObjectOneOf, OWLNamedIndividual, OWLEntity, IRI, OWLPropertyExpression, OWLDataSomeValuesFrom, \
-    OWLFacetRestriction, OWLDatatypeRestriction, OWLDatatype, OWLDataAllValuesFrom, OWLDataComplementOf, \
-    OWLDataUnionOf, OWLDataIntersectionOf, OWLDataHasValue, OWLDataOneOf, OWLDataMaxCardinality, \
-    OWLDataMinCardinality, OWLDataExactCardinality
+from .owlobject import OWLObjectRenderer
+from .owl_property import OWLObjectInverseOf
+from .class_expression import OWLClassExpression, OWLBooleanClassExpression
+
+from owlapy.model import (OWLLiteral, OWLObject, OWLClass, OWLObjectSomeValuesFrom, \
+    OWLObjectAllValuesFrom, OWLObjectUnionOf, OWLNaryBooleanClassExpression, \
+    OWLObjectIntersectionOf, OWLObjectComplementOf, OWLRestriction, \
+    OWLObjectMinCardinality, OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLObjectHasSelf,
+                          OWLNamedIndividual, OWLEntity, IRI, OWLPropertyExpression, OWLDataSomeValuesFrom, \
+    OWLDatatype, OWLDataAllValuesFrom, \
+    OWLDataHasValue, OWLDataOneOf, OWLDataMaxCardinality, \
+    OWLDataMinCardinality, OWLDataExactCardinality)
 from owlapy.vocab import OWLFacet
 
+from .data_ranges import OWLNaryDataRange, OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf
+from .class_expression import OWLObjectHasValue, OWLFacetRestriction, OWLDatatypeRestriction, OWLObjectOneOf
 
 _DL_SYNTAX = types.SimpleNamespace(
     SUBCLASS="⊑",
     EQUIVALENT_TO="≡",
     NOT="¬",
     DISJOINT_WITH="⊑" + " " + "¬",
     EXISTS="∃",
@@ -138,15 +143,15 @@
     @render.register
     def _(self, r: OWLObjectHasValue):
         return "%s %s.{%s}" % (_DL_SYNTAX.EXISTS, self.render(r.get_property()),
                                self.render(r.get_filler()))
 
     @render.register
     def _(self, r: OWLObjectOneOf):
-        return "{%s}" % (" %s " % _DL_SYNTAX.OR).join(
+        return "{%s}" % (" %s " % _DL_SYNTAX.COMMA).join(
             "%s" % (self.render(_)) for _ in r.individuals())
 
     @render.register
     def _(self, e: OWLDataSomeValuesFrom) -> str:
         return "%s %s.%s" % (_DL_SYNTAX.EXISTS, self.render(e.get_property()), self._render_nested(e.get_filler()))
 
     @render.register
@@ -416,7 +421,19 @@
 
     def _render_nested(self, c: OWLClassExpression) -> str:
         if isinstance(c, OWLBooleanClassExpression) or isinstance(c, OWLRestriction) \
                                                     or isinstance(c, OWLNaryDataRange):
             return "(%s)" % self.render(c)
         else:
             return self.render(c)
+
+
+DLrenderer = DLSyntaxObjectRenderer()
+ManchesterRenderer = ManchesterOWLSyntaxOWLObjectRenderer()
+
+
+def owl_expression_to_dl(o: OWLObject) -> str:
+    return DLrenderer.render(o)
+
+
+def owl_expression_to_manchester(o: OWLObject) -> str:
+    return ManchesterRenderer.render(o)
```

### Comparing `owlapy-0.1.2/owlapy/util.py` & `owlapy-0.1.3/owlapy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Owlapy utils."""
 from functools import singledispatchmethod, total_ordering
 from typing import Iterable, List, Type, TypeVar, Generic, Tuple, cast, Optional, Union, overload
-
-from owlapy.model import HasIndex, HasIRI, OWLClassExpression, OWLClass, OWLObjectCardinalityRestriction, \
+from .has import HasIndex
+from .owl_property import OWLObjectInverseOf
+from owlapy.model import HasIRI, OWLClassExpression, OWLClass, OWLObjectCardinalityRestriction, \
     OWLObjectComplementOf, OWLNothing, OWLPropertyRange, OWLRestriction, OWLThing, OWLObjectSomeValuesFrom, \
-    OWLObjectHasValue, OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, OWLObjectHasSelf, \
-    OWLObjectOneOf, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataExactCardinality, OWLDataHasValue, \
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, OWLObjectHasSelf, \
+    OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataExactCardinality, OWLDataHasValue, \
     OWLDataAllValuesFrom, OWLDataSomeValuesFrom, OWLObjectAllValuesFrom, HasFiller, HasCardinality, HasOperands, \
-    OWLObjectInverseOf, OWLDatatypeRestriction, OWLDataComplementOf, OWLDatatype, OWLDataUnionOf, \
-    OWLDataIntersectionOf, OWLDataOneOf, OWLFacetRestriction, OWLLiteral, OWLObjectIntersectionOf, \
-    OWLDataCardinalityRestriction, OWLNaryBooleanClassExpression, OWLNaryDataRange, OWLObjectUnionOf, \
+    OWLDatatype,OWLDataOneOf, OWLLiteral, OWLObjectIntersectionOf, \
+    OWLDataCardinalityRestriction, OWLNaryBooleanClassExpression, OWLObjectUnionOf, \
     OWLDataRange, OWLObject
-
+from .data_ranges import OWLDataComplementOf, OWLDataUnionOf, OWLDataIntersectionOf, OWLNaryDataRange
+from .class_expression import OWLObjectHasValue, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectOneOf
 
 _HasIRI = TypeVar('_HasIRI', bound=HasIRI)  #:
 _HasIndex = TypeVar('_HasIndex', bound=HasIndex)  #:
 _O = TypeVar('_O')  #:
 _Enc = TypeVar('_Enc')
 _Con = TypeVar('_Con')
 _K = TypeVar('_K')
```

### Comparing `owlapy-0.1.2/owlapy/vocab.py` & `owlapy-0.1.3/owlapy/vocab.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from abc import ABCMeta
 from enum import Enum, EnumMeta
 from typing import Final, Callable, TypeVar
 from operator import lt, le, gt, ge
 from re import match
 
 from owlapy import namespaces
-from owlapy.model._iri import HasIRI, IRI
+from .meta_classes import HasIRI
+from .iri import IRI
 from owlapy.namespaces import Namespaces
 
 
 class _Vocabulary(HasIRI):
     __slots__ = '_namespace', '_remainder', '_iri'
 
     _namespace: Namespaces
```

### Comparing `owlapy-0.1.2/owlapy.egg-info/PKG-INFO` & `owlapy-0.1.3/owlapy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlapy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Owlapy is loosely based on owlapi - the java counterpart, successfully representing the main owl objects in python.
 Home-page: https://github.com/dice-group/owlapy
 Author: Caglar Demir
 Author-email: caglardemir8@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering
@@ -35,37 +35,34 @@
 ## Usage
 <details><summary> Click me! </summary>
 
 In this example we start with a simple atomic class expression and move to some more complex 
 ones and finally render and print the last of them in description logics syntax.
 
 ```python
-from owlapy.render import DLSyntaxObjectRenderer
-from owlapy.model import IRI, OWLClass, OWLObjectProperty, OWLObjectSomeValuesFrom, \
-                         OWLObjectIntersectionOf
+from owlapy.iri import IRI
+from owlapy.class_expression import OWLClass, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom
+from owlapy.owl_property import OWLObjectProperty
 from owlapy.owl2sparql.converter import owl_expression_to_sparql
-
-# Create an IRI object using the iri as a string for 'male' class.
-male_iri = IRI.create('http://example.com/society#male')
-
+from owlapy.render import owl_expression_to_dl
 # Create the male class
-male = OWLClass(male_iri)
+male = OWLClass("http://example.com/society#male")
 
 # Create an object property using the iri as a string for 'hasChild' property.
-hasChild = OWLObjectProperty(IRI.create('http://example.com/society#hasChild'))
+hasChild = OWLObjectProperty("http://example.com/society#hasChild")
 
 # Create an existential restrictions
 males_with_children = OWLObjectSomeValuesFrom(hasChild, male)
 
 # Let's make it more complex by intersecting with another class
-teacher = OWLClass(IRI.create('http://example.com/society#teacher'))
+teacher = OWLClass("http://example.com/society#teacher")
 male_teachers_with_children = OWLObjectIntersectionOf([males_with_children, teacher])
 
-# You can render and print owl class expressions in description logics syntax
-print(DLSyntaxObjectRenderer().render(male_teachers_with_children)) 
+# You can render and print owl class expressions in description logics syntax (and vice-versa)
+print(owl_expression_to_dl(male_teachers_with_children))
 # (∃ hasChild.male) ⊓ teacher
 print(owl_expression_to_sparql("?x", male_teachers_with_children))
 #  SELECT DISTINCT ?x WHERE {  ?x <http://example.com/society#hasChild> ?s_1 . ?s_1 a <http://example.com/society#male> . ?x a <http://example.com/society#teacher> .  } }
 ```
 For more, you can check the [API documentation](https://ontolearn-docs-dice-group.netlify.app/autoapi/owlapy/#module-owlapy).
```

### Comparing `owlapy-0.1.2/setup.py` & `owlapy-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 setup(
     name="owlapy",
     description="Owlapy is loosely based on owlapi - the java counterpart, "
                 "successfully representing the main owl objects in python.",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "pandas>=1.5.0",
         "rdflib>=6.0.2",
         "parsimonious>=0.8.1",
         "pytest>=8.1.1"],
     author='Caglar Demir',
```

### Comparing `owlapy-0.1.2/tests/test_owlapy.py` & `owlapy-0.1.3/tests/test_owlapy.py`

 * *Files identical despite different names*

### Comparing `owlapy-0.1.2/tests/test_owlapy_cnf_dnf.py` & `owlapy-0.1.3/tests/test_owlapy_cnf_dnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from owlapy.model import OWLObjectProperty, OWLObjectSomeValuesFrom, OWLObjectUnionOf, \
     OWLClass, IRI, OWLDataProperty, OWLDataSomeValuesFrom, OWLNamedIndividual, OWLObjectComplementOf, \
-    OWLObjectIntersectionOf, OWLObjectMinCardinality, OWLObjectOneOf
+    OWLObjectIntersectionOf, OWLObjectMinCardinality
 from owlapy.model.providers import OWLDatatypeMinExclusiveRestriction
 from owlapy.util import TopLevelCNF, TopLevelDNF
-
+from owlapy.class_expression import OWLObjectOneOf
 
 class TopLevelNFTest(unittest.TestCase):
 
     def setUp(self):
         namespace = 'http://test.org/test#'
 
         # Classes
```

### Comparing `owlapy-0.1.2/tests/test_owlapy_nnf.py` & `owlapy-0.1.3/tests/test_owlapy_nnf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 #  * @author Matthew Horridge, The University of Manchester, Information Management Group
 #  * @since 3.0.0
 #
 import unittest
 
 from owlapy.model import OWLObjectProperty, OWLNamedIndividual, OWLObjectComplementOf, \
     OWLObjectAllValuesFrom, OWLObjectSomeValuesFrom, OWLObjectIntersectionOf, OWLObjectUnionOf, \
-    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectHasValue, OWLObjectOneOf, OWLClassExpression, IRI, \
-    BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype, OWLClass, OWLDataAllValuesFrom, OWLDataComplementOf, \
-    OWLDataIntersectionOf, OWLDataProperty, OWLDataSomeValuesFrom, OWLDataUnionOf, \
-    OWLDataHasValue, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataOneOf, OWLLiteral
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLClassExpression, IRI, \
+    BooleanOWLDatatype, DoubleOWLDatatype, IntegerOWLDatatype, OWLClass, OWLDataAllValuesFrom, \
+    OWLDataProperty, OWLDataSomeValuesFrom,OWLDataHasValue, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataOneOf, OWLLiteral
 from owlapy.model.providers import OWLDatatypeMinMaxExclusiveRestriction
 from owlapy.util import NNF
 
+from owlapy.data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf
 
 def iri(suffix):
     NS = "http://example.org/"
     return IRI.create(NS, suffix)
 
 
 class Owlapy_NNF_Test(unittest.TestCase):
```

### Comparing `owlapy-0.1.2/tests/test_owlapy_parser.py` & `owlapy-0.1.3/tests/test_owlapy_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import unittest
 from datetime import date, datetime, timedelta, timezone
 
 from pandas import Timedelta
-from owlapy.model import OWLObjectInverseOf, OWLObjectMinCardinality, OWLObjectSomeValuesFrom, \
-    OWLObjectUnionOf, DoubleOWLDatatype, IntegerOWLDatatype, OWLClass, IRI, OWLDataAllValuesFrom, \
-    OWLDataIntersectionOf, OWLDataOneOf, OWLDataProperty, OWLDataSomeValuesFrom, OWLDatatypeRestriction,  \
+from owlapy.owl_property import OWLObjectInverseOf
+
+from owlapy.model import OWLObjectUnionOf, DoubleOWLDatatype, IntegerOWLDatatype, OWLClass, IRI, OWLDataAllValuesFrom, \
+    OWLDataOneOf, OWLDataProperty, \
     OWLLiteral, OWLNamedIndividual, OWLObjectAllValuesFrom, OWLObjectComplementOf, OWLObjectExactCardinality, \
-    OWLObjectHasSelf, OWLObjectHasValue, OWLObjectIntersectionOf, OWLObjectMaxCardinality, OWLObjectOneOf, \
-    OWLObjectProperty, OWLDataComplementOf, OWLDataExactCardinality, OWLDataMaxCardinality, OWLDataUnionOf, \
-    OWLDataMinCardinality, OWLDataHasValue, OWLThing, OWLNothing, OWLFacetRestriction
+    OWLObjectHasSelf, OWLObjectIntersectionOf, OWLObjectMaxCardinality, OWLObjectProperty, OWLDataExactCardinality, OWLDataMaxCardinality, \
+    OWLDataMinCardinality, OWLDataHasValue, OWLThing, OWLNothing
 
+from owlapy.data_ranges import OWLDataIntersectionOf, OWLDataComplementOf, OWLDataUnionOf
 from owlapy.model.providers import OWLDatatypeMinExclusiveRestriction,\
     OWLDatatypeMinMaxExclusiveRestriction, OWLDatatypeMaxExclusiveRestriction
+from owlapy.class_expression import OWLDataSomeValuesFrom, OWLDatatypeRestriction, OWLFacetRestriction, OWLObjectSomeValuesFrom, OWLObjectMinCardinality, OWLObjectHasValue,OWLObjectOneOf
+
 from owlapy.parser import DLSyntaxParser, ManchesterOWLSyntaxParser
 from owlapy.vocab import OWLFacet
 
 
 class ManchesterOWLSyntaxParserTest(unittest.TestCase):
 
     def setUp(self):
```

### Comparing `owlapy-0.1.2/tests/test_owlapy_render.py` & `owlapy-0.1.3/tests/test_owlapy_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import unittest
-
+from owlapy.owl_property import OWLObjectProperty
 from owlapy.model import OWLDataMinCardinality, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom, \
-    OWLThing, OWLObjectComplementOf, OWLObjectUnionOf, OWLNamedIndividual, OWLObjectOneOf, OWLObjectHasValue, \
-    OWLObjectMinCardinality, IRI, OWLDataProperty, DoubleOWLDatatype, OWLClass, OWLDataComplementOf, \
-    OWLDataIntersectionOf, IntegerOWLDatatype, OWLDataExactCardinality, OWLDataHasValue, OWLDataAllValuesFrom, \
-    OWLDataOneOf, OWLDataSomeValuesFrom, OWLDataUnionOf, OWLLiteral, OWLObjectProperty, BooleanOWLDatatype, \
+    OWLThing, OWLObjectComplementOf, OWLObjectUnionOf, OWLNamedIndividual, OWLObjectMinCardinality, IRI, OWLDataProperty, DoubleOWLDatatype, OWLClass, \
+    IntegerOWLDatatype, OWLDataExactCardinality, OWLDataHasValue, OWLDataAllValuesFrom, \
+    OWLDataOneOf, OWLDataSomeValuesFrom, OWLLiteral, BooleanOWLDatatype, \
     OWLDataMaxCardinality
+
+from owlapy.data_ranges import OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
 from owlapy.model.providers import OWLDatatypeMinMaxInclusiveRestriction
 from owlapy.render import DLSyntaxObjectRenderer, ManchesterOWLSyntaxOWLObjectRenderer
-
+from owlapy.class_expression import OWLObjectHasValue, OWLObjectOneOf
 
 class Owlapy_DLRenderer_Test(unittest.TestCase):
     def test_ce_render(self):
         renderer = DLSyntaxObjectRenderer()
         NS = "http://example.com/father#"
 
         male = OWLClass(IRI.create(NS, 'male'))
@@ -39,15 +40,16 @@
         self.assertEqual(r, "∃ hasChild.(∃ hasChild.(∃ hasChild.⊤))")
 
         i1 = OWLNamedIndividual(IRI.create(NS, 'heinz'))
         i2 = OWLNamedIndividual(IRI.create(NS, 'marie'))
         oneof = OWLObjectOneOf((i1, i2))
         r = renderer.render(oneof)
         print(r)
-        self.assertEqual(r, "{heinz ⊔ marie}")
+
+        self.assertEqual(r, "{heinz , marie}")
 
         hasvalue = OWLObjectHasValue(property=has_child, individual=i1)
         r = renderer.render(hasvalue)
         print(r)
         self.assertEqual(r, "∃ hasChild.{heinz}")
 
         mincard = OWLObjectMinCardinality(cardinality=2, property=has_child, filler=OWLThing)
```

