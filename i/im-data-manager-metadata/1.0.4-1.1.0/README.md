# Comparing `tmp/im_data_manager_metadata-1.0.4-py3-none-any.whl.zip` & `tmp/im_data_manager_metadata-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 18673 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 16:14 data_manager_metadata/__init__.py
--rw-r--r--  2.0 unx     1942 b- defN 23-Jul-20 16:14 data_manager_metadata/annotation_utils.py
--rw-r--r--  2.0 unx    24263 b- defN 23-Jul-20 16:14 data_manager_metadata/data_tier_api.py
--rw-r--r--  2.0 unx     4004 b- defN 23-Jul-20 16:14 data_manager_metadata/exceptions.py
--rw-r--r--  2.0 unx    31629 b- defN 23-Jul-20 16:14 data_manager_metadata/metadata.py
--rw-r--r--  2.0 unx     1080 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4328 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 23-Jul-20 16:14 im_data_manager_metadata-1.0.4.dist-info/RECORD
-10 files, 68295 bytes uncompressed, 17043 bytes compressed:  75.0%
+Zip file size: 18693 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 16:08 data_manager_metadata/__init__.py
+-rw-r--r--  2.0 unx     2304 b- defN 24-Apr-10 16:08 data_manager_metadata/annotation_utils.py
+-rw-r--r--  2.0 unx    24263 b- defN 24-Apr-10 16:08 data_manager_metadata/data_tier_api.py
+-rw-r--r--  2.0 unx     4005 b- defN 24-Apr-10 16:08 data_manager_metadata/exceptions.py
+-rw-r--r--  2.0 unx    31795 b- defN 24-Apr-10 16:08 data_manager_metadata/metadata.py
+-rw-r--r--  2.0 unx     1080 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4231 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      935 b- defN 24-Apr-10 16:08 im_data_manager_metadata-1.1.0.dist-info/RECORD
+10 files, 68727 bytes uncompressed, 17063 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: data_manager_metadata/exceptions.py
 Comment: 
 
 Filename: data_manager_metadata/metadata.py
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.4.dist-info/LICENSE
+Filename: im_data_manager_metadata-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.4.dist-info/METADATA
+Filename: im_data_manager_metadata-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.4.dist-info/WHEEL
+Filename: im_data_manager_metadata-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.4.dist-info/top_level.txt
+Filename: im_data_manager_metadata-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: im_data_manager_metadata-1.0.4.dist-info/RECORD
+Filename: im_data_manager_metadata-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_manager_metadata/annotation_utils.py

```diff
@@ -1,25 +1,28 @@
 """Utilities for creating annotations
 """
+
 from ast import literal_eval
 
+
 def _check_array(field_value: str) -> bool:
     """If the field is a string that contains commas there is a fair chance
     that its an array of something.
 
     returns: true if estimated to be an array
              false otherwise
     """
 
     element_list = field_value.split(",")
     if len(element_list) > 1:
         return True
 
     return False
 
+
 def est_schema_field_type(field_value: str) -> str:
     """Estimates a standard json schema type for an input field_value.
 
     Returns one of:
         string
         number
         integer
@@ -35,16 +38,29 @@
 
     try:
         field_type = literal_eval(field_value)
     except ValueError:
         # If a type cannot be identified, then check specific values.
         # If no specific value can be found return a string.
         if field_value in [
-            True, False, 'TRUE', 'FALSE', 'true', 'false', 'yes', 'no',
-            'YES', 'NO', 'Yes', 'No', "True", "False" ]:
+            True,
+            False,
+            'TRUE',
+            'FALSE',
+            'true',
+            'false',
+            'yes',
+            'no',
+            'YES',
+            'NO',
+            'Yes',
+            'No',
+            "True",
+            "False",
+        ]:
             return 'boolean'
         return 'string'
     except SyntaxError:
         return 'string'
     else:
         # Check types
         if type(field_type) in [int, float, list]:
@@ -52,13 +68,26 @@
                 return 'integer'
             if type(field_type) is float:
                 return 'number'
             if type(field_type) is list:
                 return 'array'
         else:
             if field_value in [
-                True, False, 'TRUE', 'FALSE', 'true', 'false', 'yes', 'no',
-                'YES', 'NO', 'Yes', 'No', "True", "False"]:
+                True,
+                False,
+                'TRUE',
+                'FALSE',
+                'true',
+                'false',
+                'yes',
+                'no',
+                'YES',
+                'NO',
+                'Yes',
+                'No',
+                "True",
+                "False",
+            ]:
                 return 'boolean'
             if _check_array(field_value):
                 return 'array'
             return 'string'
```

## data_manager_metadata/data_tier_api.py

 * *Ordering differences only*

```diff
@@ -12,14 +12,15 @@
     - travelling metadata is a combination of dataset and version metadata that is typically
     downloaded to a project as a meta.json file, added to after a job and then re-uploaded back
     as a dataset.
     - The job related annotations that are added to the metadata depend on the configuration
     and specification of the job.
 
 """
+
 from typing import Any, Dict, Tuple, Optional
 import copy
 import os
 import json
 import logging
 
 from data_manager_metadata.metadata import (
@@ -543,15 +544,14 @@
     project_directory: str,
     job_application_spec: Dict[str, Any],
     job_rendered_spec: Dict[str, Any],
     output_spec: Dict[str, Any],
     username: str,
     create_param_file: bool = False,
 ) -> Tuple[list, str]:
-
     """For each specified output file with a set of annotations-parameters,
     create a metadata file in the directory specified.
 
     Errors will be simply suppressed as this should not stop a job completing
 
     If create_param_file is set to True, then also create a json file containing a list of
     the parameters added to the SDF.
```

## data_manager_metadata/exceptions.py

```diff
@@ -7,14 +7,15 @@
 
     ANNOTATION_ERRORS notes:
     1. The field 'regex' is normally used for the field identified by the
     annotation class and field.
     2. The exception is for the 'type' field where a list of enumerated
     types are used.
 """
+
 SCHEMA_FIELD_TYPES = [
     'string',
     'number',
     'integer',
     'object',
     'array',
     'boolean',
```

## data_manager_metadata/metadata.py

```diff
@@ -1,14 +1,15 @@
 """Data Manager Metadata Class Definitions.
 
     Note that the Metadata class is pickled when saved in the database so that
     we can hold the annotations as an ordered list of objects.
     The other classes should be searialisable without pickling hopefully:
     Hints: https://pynative.com/make-python-class-json-serializable/
 """
+
 import json
 import datetime
 import logging
 import copy
 from typing import Any, Dict, List, Optional
 from abc import ABC, abstractmethod
 import re
@@ -598,15 +599,21 @@
     Purpose: Object to add a Fields Descriptor annotation to the metadata.
     The class contains a list of fields that a dataset will contain.
     This is expected to be of the format:
     { "name": string, "type": string, "description": string, "active": boolean}
 
     """
 
-    def __init__(self, origin: str = '', description: str = '', fields: dict = None, job_spec: dict = None):
+    def __init__(
+        self,
+        origin: str = '',
+        description: str = '',
+        fields: dict = None,
+        job_spec: dict = None,
+    ):
 
         self.validate_origin(origin)
         self.origin = origin
         self.validate_description(description)
         self.description = description
         self.spec = job_spec
         if fields:
@@ -690,29 +697,37 @@
         """Add an individual property to the fields list"""
 
         # If an expression is provided it is assumed to be a jinja2 expression
         # that's expanded using the Job's original variables (in the specification).
         # The field name is then replaced using the result of the expression.
         rendered_field_name: str = field_name
         if expression:
-            basic_logger.info('Handling expression for "%s" (%s)', field_name, expression)
+            basic_logger.info(
+                'Handling expression for "%s" (%s)', field_name, expression
+            )
             # A Job spec must be provided
             if not job_spec:
-                raise RuntimeError(f'Field "{field_name}" with expression but no job_spec')
+                raise RuntimeError(
+                    f'Field "{field_name}" with expression but no job_spec'
+                )
             # Extract variables from the Job spec using our decoder
             # and the "jinja2_3_0" templating engine (that's all that's available atm).
             variables: Dict[str, str] = job_spec.get('variables', {})
             rendered_field_name, success = decoder.decode(
-                expression, variables, 'field-expression', decoder.TextEncoding.JINJA2_3_0
+                expression,
+                variables,
+                'field-expression',
+                decoder.TextEncoding.JINJA2_3_0,
             )
             if not success:
                 # Failed to render the expression.
                 # Do not add this field.
-                basic_logger.warning('Expression failure for "%s" (%s)',
-                                     field_name, rendered_field_name)
+                basic_logger.warning(
+                    'Expression failure for "%s" (%s)', field_name, rendered_field_name
+                )
                 return
 
         # validate the field data
         self.validate_field(rendered_field_name, prop_type, description)
 
         # Add to list
         if rendered_field_name not in self.fields:
```

## Comparing `im_data_manager_metadata-1.0.4.dist-info/LICENSE` & `im_data_manager_metadata-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `im_data_manager_metadata-1.0.4.dist-info/METADATA` & `im_data_manager_metadata-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: im-data-manager-metadata
-Version: 1.0.4
+Version: 1.1.0
 Summary: A framework for Informatics Matters dataset metadata
 Home-page: https://github.com/InformaticsMatters/squonk2-data-manager-metadata
 Author: Tim Dudgeon
 Author-email: tdudgeon@informaticsmatters.com
 License: MIT
 Keywords: jenkins
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3, <4
 License-File: LICENSE
-Requires-Dist: PyYAML (<7.0,>=6.0.1)
-Requires-Dist: jsonpickle (<3.0.0,>=2.0.0)
-Requires-Dist: im-data-manager-job-decoder (<2.0.0,>=1.17.2)
+Requires-Dist: PyYAML <7.0,>=6.0.1
+Requires-Dist: im-data-manager-job-decoder <2.0.0,>=1.17.2
 
 Informatics Matters Data-Manager Metadata
 =========================================
 
 A metadata framework package for the Data Tier Data Manager service.
 The ``im-data-manager-metadata`` package is a set of utilities
 employed by the `Informatics Matters`_ Data-Manager service
@@ -36,16 +35,16 @@
 ************
 - PyYAML>=5.3
 
 
 Running the Unit Tests
 **********************
 
-    >>> python -m venv ~/.venv/data-manager-metadata
-    >>> source ~/.venv/data-manager-metadata/bin/activate
+    >>> python -m venv venv
+    >>> source venv/bin/activate
     >>> pip install --upgrade pip
     >>> pip install -r package-requirements.txt
     >>> python -m unittest test.test_metadata
     >>> python -m unittest test.test_api
 
 Running the Command Line Interface *md-manage.py*
 *************************************************
```

