# Comparing `tmp/pyqrlew-0.9.6.tar.gz` & `tmp/pyqrlew-0.9.7.tar.gz`

## Comparing `pyqrlew-0.9.6.tar` & `pyqrlew-0.9.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 pyqrlew-0.9.6/Cargo.toml
--rw-r--r--   0     1001      127     4629 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     3548 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/.gitignore
--rw-r--r--   0     1001      127      375 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/.readthedocs.yaml
--rw-r--r--   0     1001      127     3508 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/CHANGELOG.md
--rw-r--r--   0     1001      127    11357 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/LICENSE
--rw-r--r--   0     1001      127      807 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/README.md
--rw-r--r--   0     1001      127      634 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/Makefile
--rw-r--r--   0     1001      127      330 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/api.md
--rw-r--r--   0     1001      127     3093 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/compilation_rules.md
--rw-r--r--   0     1001      127     2426 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/conf.py
--rw-r--r--   0     1001      127      224 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/contributing.md
--rw-r--r--   0     1001      127      276 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/index.md
--rw-r--r--   0     1001      127      191 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/io.md
--rw-r--r--   0     1001      127      800 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/make.bat
--rw-r--r--   0     1001      127     3801 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/postgres_supported_expressions.md
--rw-r--r--   0     1001      127      111 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/docs/requirements.txt
--rw-r--r--   0     1001      127     4860 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/benchmark.py
--rw-r--r--   0     1001      127    36436 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/dataset_from_queries.ipynb
--rw-r--r--   0     1001      127      202 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/expose_protobufs.py
--rw-r--r--   0     1001      127    58478 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/mssql_translator.ipynb
--rw-r--r--   0     1001      127  2174976 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/my_sqlite.db
--rw-r--r--   0     1001      127   152022 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/postgres_simple_table.ipynb
--rw-r--r--   0     1001      127    66583 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/range_propagation.ipynb
--rw-r--r--   0     1001      127   146448 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/examples/rewrite_with_dp.ipynb
--rw-r--r--   0     1001      127      212 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      127      165 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/io/__init__.py
--rw-r--r--   0     1001      127    18598 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/io/dataset.py
--rw-r--r--   0     1001      127     4178 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/io/postgresql.py
--rw-r--r--   0     1001      127     5189 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/io/sqlite.py
--rw-r--r--   0     1001      127     6306 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/io/utils.py
--rw-r--r--   0     1001      127       91 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/tester/__init__.py
--rw-r--r--   0     1001      127     3604 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/tester/stochatic_dataset.py
--rw-r--r--   0     1001      127     1467 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/tester/tester.py
--rw-r--r--   0     1001      127     4493 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/tester/utils.py
--rw-r--r--   0     1001      127     1115 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/python/pyqrlew/utils.py
--rw-r--r--   0     1001      127     4796 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/dataset.rs
--rw-r--r--   0     1001      127       98 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/dialect.rs
--rw-r--r--   0     1001      127     7672 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/dp_event.rs
--rw-r--r--   0     1001      127     1725 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/error.rs
--rw-r--r--   0     1001      127      413 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/lib.rs
--rw-r--r--   0     1001      127    16627 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/src/relation.rs
--rw-r--r--   0     1001      127      457 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/tests/conftest.py
--rw-r--r--   0     1001      127    10306 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/tests/queries/base_queries.sql
--rw-r--r--   0     1001      127      204 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/tests/requirements.txt
--rw-r--r--   0     1001      127     3833 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/tests/test_base_queries.py
--rw-r--r--   0     1001      127     1823 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/tests/test_dataset.py
--rw-r--r--   0     1001      127    51547 2024-01-22 17:48:24.000000 pyqrlew-0.9.6/Cargo.lock
--rw-r--r--   0     1001      127     1493 2024-01-22 17:48:15.000000 pyqrlew-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 pyqrlew-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 pyqrlew-0.9.7/Cargo.toml
+-rw-r--r--   0     1001      127     4629 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     3546 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/.gitignore
+-rw-r--r--   0     1001      127      375 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/.readthedocs.yaml
+-rw-r--r--   0     1001      127     3843 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/CHANGELOG.md
+-rw-r--r--   0     1001      127    11357 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/LICENSE
+-rw-r--r--   0     1001      127      807 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/README.md
+-rw-r--r--   0     1001      127      634 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/Makefile
+-rw-r--r--   0     1001      127      330 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/api.md
+-rw-r--r--   0     1001      127     3093 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/compilation_rules.md
+-rw-r--r--   0     1001      127     2426 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/conf.py
+-rw-r--r--   0     1001      127      224 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/contributing.md
+-rw-r--r--   0     1001      127      276 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/index.md
+-rw-r--r--   0     1001      127      191 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/io.md
+-rw-r--r--   0     1001      127      800 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/make.bat
+-rw-r--r--   0     1001      127     3801 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/postgres_supported_expressions.md
+-rw-r--r--   0     1001      127      111 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/docs/requirements.txt
+-rw-r--r--   0     1001      127     4860 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/benchmark.py
+-rw-r--r--   0     1001      127    36436 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/dataset_from_queries.ipynb
+-rw-r--r--   0     1001      127      202 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/expose_protobufs.py
+-rw-r--r--   0     1001      127    58478 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/mssql_translator.ipynb
+-rw-r--r--   0     1001      127  2174976 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/my_sqlite.db
+-rw-r--r--   0     1001      127   152022 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/postgres_simple_table.ipynb
+-rw-r--r--   0     1001      127    66583 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/range_propagation.ipynb
+-rw-r--r--   0     1001      127   146448 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/examples/rewrite_with_dp.ipynb
+-rw-r--r--   0     1001      127      212 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      127      165 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      127    18598 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/io/dataset.py
+-rw-r--r--   0     1001      127     4178 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      127     5189 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/io/sqlite.py
+-rw-r--r--   0     1001      127     6306 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/io/utils.py
+-rw-r--r--   0     1001      127       91 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/tester/__init__.py
+-rw-r--r--   0     1001      127     3604 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/tester/stochatic_dataset.py
+-rw-r--r--   0     1001      127     1467 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/tester/tester.py
+-rw-r--r--   0     1001      127     4493 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/tester/utils.py
+-rw-r--r--   0     1001      127     1115 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/python/pyqrlew/utils.py
+-rw-r--r--   0     1001      127     5635 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/dataset.rs
+-rw-r--r--   0     1001      127      111 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/dialect.rs
+-rw-r--r--   0     1001      127     7672 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/dp_event.rs
+-rw-r--r--   0     1001      127     1725 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/error.rs
+-rw-r--r--   0     1001      127      413 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/lib.rs
+-rw-r--r--   0     1001      127    17380 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/src/relation.rs
+-rw-r--r--   0     1001      127      457 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/tests/conftest.py
+-rw-r--r--   0     1001      127    10304 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/tests/queries/base_queries.sql
+-rw-r--r--   0     1001      127      204 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/tests/requirements.txt
+-rw-r--r--   0     1001      127     4388 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/tests/test_base_queries.py
+-rw-r--r--   0     1001      127     1823 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/tests/test_dataset.py
+-rw-r--r--   0     1001      127    53677 2024-01-30 10:22:34.000000 pyqrlew-0.9.7/Cargo.lock
+-rw-r--r--   0     1001      127     1493 2024-01-30 10:22:30.000000 pyqrlew-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 pyqrlew-0.9.7/PKG-INFO
```

### Comparing `pyqrlew-0.9.6/.github/workflows/ci.yml` & `pyqrlew-0.9.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/.gitignore` & `pyqrlew-0.9.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
 #   intended to run in multiple environments; otherwise, check them in:
-# .python-version
+.python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
 #Pipfile.lock
```

### Comparing `pyqrlew-0.9.6/CHANGELOG.md` & `pyqrlew-0.9.7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
+
+## [0.9.7] - 2024-01-29
+### Added
+- support for bigquery dialect [MR42](https://github.com/Qrlew/pyqrlew/pull/42)
+### Fixed
+- quoting of query identifiers [MR42](https://github.com/Qrlew/pyqrlew/pull/42)
+### Changed
+- law for clipping bounds when DP rewriting [MR42](https://github.com/Qrlew/pyqrlew/pull/42)
+
+## [0.9.6] - 2024-01-29
 ### Fixed
 Fixing the example notebooks [MR40](https://github.com/Qrlew/pyqrlew/pull/40)
 ### Added
 Adding an example notebook with MsSqlTranslator [MR40](https://github.com/Qrlew/pyqrlew/pull/40)
 
 ## [0.9.5] - 2024-01-17
 ### Added
```

### Comparing `pyqrlew-0.9.6/LICENSE` & `pyqrlew-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/README.md` & `pyqrlew-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/docs/Makefile` & `pyqrlew-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/docs/compilation_rules.md` & `pyqrlew-0.9.7/docs/compilation_rules.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/docs/conf.py` & `pyqrlew-0.9.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/docs/make.bat` & `pyqrlew-0.9.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/docs/postgres_supported_expressions.md` & `pyqrlew-0.9.7/docs/postgres_supported_expressions.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/benchmark.py` & `pyqrlew-0.9.7/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/dataset_from_queries.ipynb` & `pyqrlew-0.9.7/examples/dataset_from_queries.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/mssql_translator.ipynb` & `pyqrlew-0.9.7/examples/mssql_translator.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/my_sqlite.db` & `pyqrlew-0.9.7/examples/my_sqlite.db`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/postgres_simple_table.ipynb` & `pyqrlew-0.9.7/examples/postgres_simple_table.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/range_propagation.ipynb` & `pyqrlew-0.9.7/examples/range_propagation.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/examples/rewrite_with_dp.ipynb` & `pyqrlew-0.9.7/examples/rewrite_with_dp.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/io/dataset.py` & `pyqrlew-0.9.7/python/pyqrlew/io/dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/io/postgresql.py` & `pyqrlew-0.9.7/python/pyqrlew/io/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/io/sqlite.py` & `pyqrlew-0.9.7/python/pyqrlew/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/io/utils.py` & `pyqrlew-0.9.7/python/pyqrlew/io/utils.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/tester/stochatic_dataset.py` & `pyqrlew-0.9.7/python/pyqrlew/tester/stochatic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/tester/tester.py` & `pyqrlew-0.9.7/python/pyqrlew/tester/tester.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/tester/utils.py` & `pyqrlew-0.9.7/python/pyqrlew/tester/utils.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/python/pyqrlew/utils.py` & `pyqrlew-0.9.7/python/pyqrlew/utils.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/src/dataset.rs` & `pyqrlew-0.9.7/src/dataset.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 use pyo3::prelude::*;
 use qrlew::{
     builder::With,
     hierarchy::Hierarchy,
     sql,
     relation,
     dialect_translation::{
-        postgresql::PostgreSqlTranslator,
-        mssql::MsSqlTranslator,
-        QueryToRelationTranslator,
+        bigquery::BigQueryTranslator, mssql::MsSqlTranslator, postgresql::PostgreSqlTranslator, QueryToRelationTranslator
     },
 };
 use qrlew_sarus::{
     data_spec,
     protobuf::print_to_string,
 };
 use std::ops::Deref;
@@ -94,14 +92,20 @@
             },
             Dialect::MsSql => {
                 let translator = MsSqlTranslator;
                 let query = sql::relation::parse_with_dialect(query, translator.dialect())?;
                 let query_with_relations = query.with(&relations);
                 Ok(Relation::new(Arc::new(relation::Relation::try_from((query_with_relations, translator))?)))
             },
+            Dialect::BigQuery => {
+                let translator = BigQueryTranslator;
+                let query = sql::relation::parse_with_dialect(query, translator.dialect())?;
+                let query_with_relations = query.with(&relations);
+                Ok(Relation::new(Arc::new(relation::Relation::try_from((query_with_relations, translator))?)))
+            },
         }  
     }
 
     pub fn from_queries(&self, queries: Vec<(Vec<String>, String)>, dialect: Option<Dialect>) -> Result<Self> {
         let relations = self.deref().relations();
         let dialect = dialect.unwrap_or(Dialect::PostgreSql);
 
@@ -118,14 +122,21 @@
                     },
                     Dialect::MsSql => {
                         let translator = MsSqlTranslator;
                         let parsed = sql::relation::parse_with_dialect(query, translator.dialect())?;
                         let query_with_rel = parsed.with(&relations);
                         let rel = relation::Relation::try_from((query_with_rel, translator))?;
                         Ok((path.clone(), Arc::new(rel)))
+                    },
+                    Dialect::BigQuery => {
+                        let translator = BigQueryTranslator;
+                        let parsed = sql::relation::parse_with_dialect(query, translator.dialect())?;
+                        let query_with_rel = parsed.with(&relations);
+                        let rel = relation::Relation::try_from((query_with_rel, translator))?;
+                        Ok((path.clone(), Arc::new(rel)))
                     }
                 }
             })
             .collect();
         let ds: data_spec::Dataset = (&result_relations?).try_into()?;
         Ok(Dataset(ds))
     }
```

### Comparing `pyqrlew-0.9.6/src/dp_event.rs` & `pyqrlew-0.9.7/src/dp_event.rs`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/src/error.rs` & `pyqrlew-0.9.7/src/error.rs`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/src/relation.rs` & `pyqrlew-0.9.7/src/relation.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 use std::{collections::HashMap, ops::Deref, str, sync::Arc};
 use pyo3::prelude::*;
 use qrlew::{
     ast,
-    differential_privacy::budget::Budget,
+    differential_privacy::DpParameters,
     expr::Identifier,
     privacy_unit_tracking::PrivacyUnit,
     relation::{self, Variant},
     synthetic_data::SyntheticData,
     dialect_translation::{
-        RelationWithTranslator,
-        postgresql::PostgreSqlTranslator,
-        mssql::MsSqlTranslator,
+        bigquery::BigQueryTranslator, mssql::MsSqlTranslator, postgresql::PostgreSqlTranslator, RelationWithTranslator
     }
 };
 use crate::{
     dataset::Dataset,
     error::{MissingKeyError, Result},
     dp_event::RelationWithDpEvent,
     dialect::Dialect,
@@ -82,15 +80,15 @@
         let privacy_unit = PrivacyUnit::from(privacy_unit);
         let epsilon = epsilon_delta
             .get("epsilon")
             .ok_or(MissingKeyError("epsilon".to_string()))?;
         let delta = epsilon_delta
             .get("delta")
             .ok_or(MissingKeyError("delta".to_string()))?;
-        let budget = Budget::new(*epsilon, *delta);
+        let budget = DpParameters::from_epsilon_delta(*epsilon, *delta);
         let relation_with_dp_event = relation.rewrite_as_privacy_unit_preserving(
             &relations,
             synthetic_data,
             privacy_unit,
             budget,
         )?;
         Ok(RelationWithDpEvent::new(Arc::new(
@@ -117,15 +115,15 @@
         let privacy_unit = PrivacyUnit::from(privacy_unit);
         let epsilon = epsilon_delta
             .get("epsilon")
             .ok_or(MissingKeyError("epsion".to_string()))?;
         let delta = epsilon_delta
             .get("delta")
             .ok_or(MissingKeyError("delta".to_string()))?;
-        let budget = Budget::new(*epsilon, *delta);
+        let budget = DpParameters::from_epsilon_delta(*epsilon, *delta);
         let relation_with_dp_event = relation.rewrite_with_differential_privacy(
             &relations,
             synthetic_data,
             privacy_unit,
             budget,
         )?;
         Ok(RelationWithDpEvent::new(Arc::new(
@@ -134,22 +132,25 @@
     }
 
     pub fn to_query(&self, dialect: Option<Dialect>) -> String {
         let relation = &*(self.0);
         let dialect = dialect.unwrap_or(Dialect::PostgreSql);
         match dialect {
             Dialect::PostgreSql => ast::Query::from(RelationWithTranslator(&relation, PostgreSqlTranslator)).to_string(),
-            Dialect::MsSql => ast::Query::from(RelationWithTranslator(&relation, MsSqlTranslator)).to_string()
+            Dialect::MsSql => ast::Query::from(RelationWithTranslator(&relation, MsSqlTranslator)).to_string(),
+            Dialect::BigQuery => ast::Query::from(RelationWithTranslator(&relation, BigQueryTranslator)).to_string(),
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
 
+    use qrlew::{ast, dialect_translation::{postgresql::PostgreSqlTranslator, RelationWithTranslator}};
+
     use crate::{
         dataset::Dataset,
         relation::Relation
     };
     use std::collections::HashMap;
 
     const DATASET: &str = r#"{"@type": "sarus_data_spec/sarus_data_spec.Dataset", "uuid": "e9cb9391ca184e89897f49bd75387a46", "name": "Transformed", "spec": {"transformed": {"transform": "98f18c2b0beb406088193dab26e24552", "arguments": [], "named_arguments": {}}}, "properties": {}, "doc": "This ia a demo dataset for testing purpose"}"#;
@@ -190,8 +191,21 @@
             let dp_relation = relation.rewrite_with_differential_privacy(
                 &dataset, privacy_unit.clone(), budget.clone(), None
             ).unwrap();
             let dp_query = dp_relation.relation().to_query(None);
             println!("\n\n{dp_query}");
         }
     }
+
+    #[test]
+    fn test_quoting() {
+        let dataset = Dataset::new(DATASET, SCHEMA, SIZE).unwrap();
+        println!("{:?}", dataset.relations()[1].0) ;
+
+        let tr = PostgreSqlTranslator;
+        let query = r#"SELECT "age" AS s1 FROM census;"#;
+        let relation = Relation::from_query(query, &dataset, None).unwrap();
+
+        let trans = ast::Query::from(RelationWithTranslator(&relation, PostgreSqlTranslator)).to_string();
+        println!("{}",trans);
+    }
 }
```

### Comparing `pyqrlew-0.9.6/tests/queries/base_queries.sql` & `pyqrlew-0.9.7/tests/queries/base_queries.sql`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 SELECT VARIANCE(education_num) AS my_var, marital_status FROM census GROUP BY marital_status;
 SELECT (VARIANCE(education_num)) AS my_var, marital_status FROM census GROUP BY marital_status;
 SELECT sex, SUM(capital_loss / 10000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY sex HAVING NOT ( sex = 'Female' ) ORDER BY my_sum DESC LIMIT 10;
 SELECT marital_status, SUM(capital_loss / 100000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY marital_status HAVING marital_status = 'Divorced';
 SELECT POWER(AVG(age), 2) AS my_res FROM census;
 SELECT 1 + AVG(age) AS my_res FROM census;
 SELECT SUM(age)  AS my_res FROM census as p;
--- SELECT COUNT(*) AS count_all FROM census WHERE workclass LIKE 'Married%'
+-- SELECT COUNT(*) AS count_all FROM census WHERE workclass LIKE 'Married%';
 SELECT SUM(education_num) AS my_sum FROM census GROUP BY LOG(CASE WHEN age < 50 THEN 50 ELSE 1 END);
 SELECT COUNT(education_num) As my_sum FROM census GROUP BY CASE WHEN age < 50 THEN 50 ELSE 1 END;
 SELECT CASE WHEN age < 50 THEN 50 ELSE 1 END AS case_age, COUNT(education_num) AS my_sum FROM census GROUP BY CASE WHEN age < 50 THEN 50 ELSE 1 END;
 SELECT age, SUM(education_num) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY age HAVING SUM(education_num) > 1 ORDER BY age;
 SELECT age AS age1, SUM(education_num) AS my_sum FROM census GROUP BY age1 ORDER BY age1;
 SELECT SUM(age) AS my_sum FROM census GROUP BY marital_status, CASE WHEN age > 90 THEN 1 ELSE 0 END;
 SELECT SUM(age) AS my_sum FROM census GROUP BY marital_status, CASE WHEN age > 90 THEN 1 ELSE 0 END ORDER BY my_sum;
@@ -28,15 +28,15 @@
 SELECT SUM(CASE WHEN age > 80 THEN 1 ELSE 0 END) AS s1, SUM(age) AS s2 FROM census;
 SELECT ( 2 * (SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END))) AS s1 FROM census;
 SELECT capital_loss, COUNT(*) AS my_count FROM census GROUP BY capital_loss;
 SELECT capital_loss, COUNT(1) AS my_count FROM census GROUP BY capital_loss;
 SELECT capital_loss, COUNT(age) AS count_all FROM census GROUP BY capital_loss;
 -- SELECT EXTRACT( YEAR FROM "検知日時" ) AS _year, COUNT(*) AS my_count FROM beacon GROUP BY EXTRACT(YEAR FROM "検知日時");
 -- SELECT age AS "my age", 3 * COS(COUNT(*)) AS my_ln_count, AVG(education_num) AS "my avg" FROM census GROUP BY age ORDER BY age, "my avg";
--- SELECT age AS "my age", 3 * COS(COUNT(*)) AS my_ln_count, AVG(education_num) AS "my avg" FROM census GROUP BY "my age" ORDER BY "my age", "my avg";
+SELECT age AS "my age", 3 * COS(COUNT(*)) AS my_ln_count, AVG(education_num) AS "my avg" FROM census GROUP BY "my age" ORDER BY "my age", "my avg";
 SELECT age, COUNT(*) AS my_count FROM census WHERE age BETWEEN 18 AND 30 GROUP BY age;
 SELECT age, COUNT(*) AS my_count FROM census WHERE age NOT BETWEEN 18 AND 30 GROUP BY age;
 SELECT COUNT(*) AS my_count FROM census WHERE native_country IN ('Holand-Netherlands', 'Cuba', 'Italy', 'England');
 SELECT native_country, COUNT(*) AS my_count FROM census WHERE native_country NOT IN ('Holand-Netherlands', 'Cuba', 'Italy', 'England') GROUP BY native_country;
 SELECT CAST(age AS VARCHAR) AS my_age, COUNT(*) AS my_count FROM census GROUP BY age;
 SELECT UPPER(marital_status) AS m, COUNT(*) AS my_count FROM census GROUP BY marital_status;
 SELECT LOWER(marital_status)AS m, COUNT(*) AS my_count FROM census GROUP BY marital_status;
```

### Comparing `pyqrlew-0.9.6/tests/test_base_queries.py` & `pyqrlew-0.9.7/tests/test_base_queries.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     return True
 
 def test_queries_consistency(queries):
     """Test the consistency of results for queries stored in a file."""
     database = PostgreSQL()
     dataset = database.extract() # load the db
-    
+
     for query in queries:
         print(f"\n{colored(query, 'blue')}")
         replaced_query = query.replace("census", "extract.census").replace("beacon", "extract.beacon")
         result = pd.read_sql(replaced_query, database.engine())            
         relation = dataset.relation(query)
         new_query = relation.to_query()
         print('===================')
@@ -95,7 +95,25 @@
 def test_simple_mssql_translation():
     database = PostgreSQL()
     dataset = database.extract()
     query = "SELECT * FROM census LIMIT 10;"
     relation = dataset.relation(query, Dialect.PostgreSql)
     translated = relation.to_query(Dialect.MsSql)
     assert "SELECT TOP (10) * FROM" in translated
+
+
+def test_quoting():
+    database = PostgreSQL()
+    dataset = database.extract()
+    query = """
+    SELECT 
+        age AS "my age"
+    FROM census;"""
+    relation = dataset.relation(query, Dialect.PostgreSql)
+    translated = relation.to_query(Dialect.PostgreSql)
+    assert translated.replace(' ', '')=='''
+        WITH "map_p5al" ("my age") AS (
+            SELECT "age" AS "my age" FROM "extract"."census"
+        ) SELECT * FROM "map_p5al"
+    '''.replace('\n', '').replace(' ', '')
+    results = pd.read_sql(relation.to_query(), database.engine())
+
```

### Comparing `pyqrlew-0.9.6/tests/test_dataset.py` & `pyqrlew-0.9.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/Cargo.lock` & `pyqrlew-0.9.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,62 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.6.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e2e1ebcb11de5c03c67de28a7df593d32191b44939c482e97702baaaa6ab6a5"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2faccea4cc4ab4a667ce676a30e8ec13922a692c99bb8f5b11f1502c72e04220"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+dependencies = [
+ "windows-sys 0.52.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "3.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "anyhow"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
 
 [[package]]
 name = "approx"
@@ -194,17 +242,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "bytemuck"
-version = "1.14.0"
+version = "1.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+checksum = "ed2490600f404f2b94c167e31d3ed1d5f3c225a0f3b80230053b3e0b7b962bd9"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -233,28 +281,34 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "9f13690e35a5e4ace198e7beea2895d29f3a9cc55015fcebe6336bd2010af9eb"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.0",
 ]
 
 [[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "colored"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
 dependencies = [
  "lazy_static",
  "windows-sys 0.48.0",
@@ -305,27 +359,50 @@
 [[package]]
 name = "either"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
+name = "env_filter"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
+dependencies = [
+ "log",
+ "regex",
+]
+
+[[package]]
 name = "env_logger"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "env_logger"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05e7cf40684ae96ade6232ed84582f40ce0a66efcd43a5117aef610534f8e0b8"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "env_filter",
+ "humantime",
+ "log",
+]
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
@@ -530,17 +607,17 @@
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "433de089bd45971eecf4668ee0ee8f4cec17db4f8bd8f7bc3197a6ce37aa7d9b"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
@@ -557,17 +634,17 @@
  "hermit-abi",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.12.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25db6b064527c5d482d0423354fcd07a89a2dfe07b67892e62411946db7f07b0"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.10"
@@ -1059,33 +1136,33 @@
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.9.6"
+version = "0.9.7"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
  "serde_json",
 ]
 
 [[package]]
 name = "qrlew"
-version = "0.9.6"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b546ecf20deef5625a3fa97957751ca9e5ef1ca1f9c173ac785b0341b8aedc70"
+checksum = "48327b20f043e0fe9e85502a46353aa7edec3938ad7d2d707d0994d2007a79e2"
 dependencies = [
  "base64",
  "chrono",
  "colored",
  "dot",
- "env_logger",
+ "env_logger 0.11.1",
  "itertools",
  "log",
  "paste",
  "postgres",
  "r2d2",
  "r2d2_postgres",
  "rand",
@@ -1101,15 +1178,15 @@
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe13d492daacd14afcce0bb4e578fa668401f09ba6e43826702163ec75855df7"
 dependencies = [
  "anyhow",
  "chrono",
  "colored",
- "env_logger",
+ "env_logger 0.10.2",
  "glob",
  "itertools",
  "log",
  "paste",
  "protobuf",
  "protobuf-codegen",
  "protobuf-json-mapping",
@@ -1219,17 +1296,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b7fa1134405e2ec9353fd416b17f8dacd46c473d7d3fd1cf202706a14eb792a"
+checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -1347,37 +1424,37 @@
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.196"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.196"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.113"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1439,17 +1516,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "sqlparser"
-version = "0.41.0"
+version = "0.43.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cc2c25a6c66789625ef164b4c7d2e548d627902280c13710d33da8222169964"
+checksum = "f95c4bae5aba7cd30bd506f7140026ade63cff5afd778af8854026f9606bf5d4"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "statrs"
 version = "0.16.0"
@@ -1646,15 +1723,15 @@
 
 [[package]]
 name = "toml_edit"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d34d383cd00a163b4a5b85053df514d45bc330f6de7737edfe0a93311d1eaa03"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap 2.2.1",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
@@ -1704,14 +1781,20 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "uuid"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 
 [[package]]
 name = "version_check"
@@ -1809,17 +1892,17 @@
 dependencies = [
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.14"
+version = "0.7.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b31891d644eba1789fb6715f27fbc322e4bdf2ecdc412ede1993246159271613"
+checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1991,17 +2074,17 @@
 name = "windows_x86_64_msvc"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
 
 [[package]]
 name = "winnow"
-version = "0.5.34"
+version = "0.5.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7cf47b659b318dccbd69cc4797a39ae128f533dce7902a1096044d1967b9c16"
+checksum = "1931d78a9c73861da0134f453bb1f790ce49b2e30eba8410b4b79bac72b46a2d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
```

### Comparing `pyqrlew-0.9.6/pyproject.toml` & `pyqrlew-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.9.6/PKG-INFO` & `pyqrlew-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrlew
-Version: 0.9.6
+Version: 0.9.7
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

