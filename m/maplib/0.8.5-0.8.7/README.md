# Comparing `tmp/maplib-0.8.5.tar.gz` & `tmp/maplib-0.8.7.tar.gz`

## Comparing `maplib-0.8.5.tar` & `maplib-0.8.7.tar`

### file list

```diff
@@ -1,106 +1,112 @@
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 maplib-0.8.5/local_dependencies/triplestore/Cargo.toml
--rw-r--r--   0     1001      127      391 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/constants.rs
--rw-r--r--   0     1001      127     3529 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/conversion.rs
--rw-r--r--   0     1001      127     2691 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/errors.rs
--rw-r--r--   0     1001      127     9305 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/export_triples.rs
--rw-r--r--   0     1001      127      958 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/io_funcs.rs
--rw-r--r--   0     1001      127    20719 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/lib.rs
--rw-r--r--   0     1001      127     2353 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/native_parquet_write.rs
--rw-r--r--   0     1001      127    12020 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/ntriples_write.rs
--rw-r--r--   0     1001      127      496 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/rdfs_inferencing.rs
--rw-r--r--   0     1001      127      865 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/errors.rs
--rw-r--r--   0     1001      127     5904 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_aggregate.rs
--rw-r--r--   0     1001      127    17103 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_expressions.rs
--rw-r--r--   0     1001      127      939 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/distinct.rs
--rw-r--r--   0     1001      127     1407 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/extend.rs
--rw-r--r--   0     1001      127     1299 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/filter.rs
--rw-r--r--   0     1001      127     2400 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/group.rs
--rw-r--r--   0     1001      127     1172 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/join.rs
--rw-r--r--   0     1001      127     2113 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/left_join.rs
--rw-r--r--   0     1001      127     2270 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs
--rw-r--r--   0     1001      127     1204 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/minus.rs
--rw-r--r--   0     1001      127     2091 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/order_by.rs
--rw-r--r--   0     1001      127    28988 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/path.rs
--rw-r--r--   0     1001      127     1055 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/project.rs
--rw-r--r--   0     1001      127     1742 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs
--rw-r--r--   0     1001      127    17168 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/triple.rs
--rw-r--r--   0     1001      127     1245 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/union.rs
--rw-r--r--   0     1001      127     3951 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/values.rs
--rw-r--r--   0     1001      127     5571 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns.rs
--rw-r--r--   0     1001      127     1316 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_order.rs
--rw-r--r--   0     1001      127    10610 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/sparql.rs
--rw-r--r--   0     1001      127     9808 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/triplestore/src/triples_read.rs
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 maplib-0.8.5/local_dependencies/maplib/Cargo.toml
--rw-r--r--   0     1001      127    11726 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/ast.rs
--rw-r--r--   0     1001      127      925 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/constants.rs
--rw-r--r--   0     1001      127      635 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/document.rs
--rw-r--r--   0     1001      127      293 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/errors.rs
--rw-r--r--   0     1001      127      244 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/lib.rs
--rw-r--r--   0     1001      127     6494 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/mapping/constant_terms.rs
--rw-r--r--   0     1001      127     6144 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/mapping/default.rs
--rw-r--r--   0     1001      127     5785 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/mapping/errors.rs
--rw-r--r--   0     1001      127     5101 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/mapping/validation_inference.rs
--rw-r--r--   0     1001      127    25534 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/mapping.rs
--rw-r--r--   0     1001      127      800 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/parsing/errors.rs
--rw-r--r--   0     1001      127   191162 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/parsing/nom_parsing.rs
--rw-r--r--   0     1001      127    60674 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/parsing/parser_test.rs
--rw-r--r--   0     1001      127     2812 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/parsing/parsing_ast.rs
--rw-r--r--   0     1001      127      808 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/parsing.rs
--rw-r--r--   0     1001      127    13035 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/resolver.rs
--rw-r--r--   0     1001      127     1963 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/templates/errors.rs
--rw-r--r--   0     1001      127    11029 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/src/templates.rs
--rw-r--r--   0     1001      127        8 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/tests/stottr_testdata/.gitignore
--rw-r--r--   0     1001      127      462 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/tests/stottr_testdata/expected_easy_case.ttl
--rw-r--r--   0     1001      127    38008 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/tests/test_stottr.rs
--rw-r--r--   0     1001      127     1361 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/maplib/tests/utils.rs
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 maplib-0.8.5/local_dependencies/shacl/Cargo.toml
--rw-r--r--   0     1001      127       70 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/shacl/src/errors.rs
--rw-r--r--   0     1001      127      460 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/shacl/src/lib.rs
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 maplib-0.8.5/local_dependencies/parquet_io/Cargo.toml
--rw-r--r--   0     1001      127     2922 2024-03-19 08:11:26.000000 maplib-0.8.5/local_dependencies/parquet_io/src/lib.rs
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 maplib-0.8.5/Cargo.toml
--rw-r--r--   0     1001      127      391 2024-03-19 08:11:26.000000 maplib-0.8.5/.gitignore
--rw-r--r--   0     1001      127    11459 2024-03-19 08:11:26.000000 maplib-0.8.5/LICENSE
--rw-r--r--   0     1001      127     6021 2024-03-19 08:11:26.000000 maplib-0.8.5/README.md
--rw-r--r--   0     1001      127       11 2024-03-19 08:11:26.000000 maplib-0.8.5/doc/.gitignore
--rw-r--r--   0     1001      127     1731 2024-03-19 08:11:26.000000 maplib-0.8.5/doc/API.md
--rw-r--r--   0     1001      127    13686 2024-03-19 08:11:26.000000 maplib-0.8.5/doc/rds_mapping.ipynb
--rw-r--r--   0     1001      127     1283 2024-03-19 08:11:26.000000 maplib-0.8.5/pyproject.toml
--rw-r--r--   0     1001      127       22 2024-03-19 08:11:26.000000 maplib-0.8.5/python/maplib/.gitignore
--rw-r--r--   0     1001      127      127 2024-03-19 08:11:26.000000 maplib-0.8.5/python/maplib/__init__.py
--rw-r--r--   0     1001      127     8963 2024-03-19 08:11:26.000000 maplib-0.8.5/python/maplib/_maplib.pyi
--rw-r--r--   0     1001      127        0 2024-03-19 08:11:26.000000 maplib-0.8.5/python/maplib/py.typed
--rw-r--r--   0     1001      127     3500 2024-03-19 08:11:26.000000 maplib-0.8.5/src/error.rs
--rw-r--r--   0     1001      127    15100 2024-03-19 08:11:26.000000 maplib-0.8.5/src/lib.rs
--rw-r--r--   0     1001      127      138 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/.gitignore
--rw-r--r--   0     1001      127       72 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/out.ttl
--rw-r--r--   0     1001      127       20 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/requirements.txt
--rw-r--r--   0     1001      127     4994 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_basics.py
--rw-r--r--   0     1001      127     5901 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_blank_nodes_multi.py
--rw-r--r--   0     1001      127    18343 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_gtfs_benchmark.py
--rw-r--r--   0     1001      127    16847 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_integration.py
--rw-r--r--   0     1001      127     3367 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_pizza_example.py
--rw-r--r--   0     1001      127     1550 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/test_read.py
--rw-r--r--   0     1001      127       24 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/iterated_property_path_constant_object_query.csv
--rw-r--r--   0     1001      127     2935 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/iterated_property_path_constant_subject_query.csv
--rw-r--r--   0     1001      127    13780 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/iterated_property_path_query.csv
--rw-r--r--   0     1001      127     4813 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/iterated_property_path_query_with_bug.csv
--rw-r--r--   0     1001      127      122 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/larger_query.csv
--rw-r--r--   0     1001      127       88 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_join_query.csv
--rw-r--r--   0     1001      127       48 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_join_query_two_vars.csv
--rw-r--r--   0     1001      127       48 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_leftjoin_query.csv
--rw-r--r--   0     1001      127      644 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_query.csv
--rw-r--r--   0     1001      127      644 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_query_sorting.csv
--rw-r--r--   0     1001      127      166 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/multi_datatype_union_query.csv
--rw-r--r--   0     1001      127     3247 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/property_path_query.csv
--rw-r--r--   0     1001      127      660 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/read_ntriples.csv
--rw-r--r--   0     1001      127      638 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/read_ntriples.nt
--rw-r--r--   0     1001      127      498 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/read_ntriples2.csv
--rw-r--r--   0     1001      127      757 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_construct_query_nothing.csv
--rw-r--r--   0     1001      127    28024 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_construct_query_something.csv
--rw-r--r--   0     1001      127      259 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_insert_query_nothing.csv
--rw-r--r--   0     1001      127    11934 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_insert_query_something.csv
--rw-r--r--   0     1001      127     3327 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_property_path_query.csv
--rw-r--r--   0     1001      127    20308 2024-03-19 08:11:26.000000 maplib-0.8.5/tests/testdata/simple_query.csv
--rw-r--r--   0     1001      127    64340 2024-03-19 08:12:00.000000 maplib-0.8.5/Cargo.lock
--rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 maplib-0.8.5/PKG-INFO
+-rw-r--r--   0     1001      127     1033 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/Cargo.toml
+-rw-r--r--   0     1001      127    11726 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/ast.rs
+-rw-r--r--   0     1001      127      925 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/constants.rs
+-rw-r--r--   0     1001      127      635 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/document.rs
+-rw-r--r--   0     1001      127      293 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/errors.rs
+-rw-r--r--   0     1001      127      244 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/lib.rs
+-rw-r--r--   0     1001      127     6449 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/mapping/constant_terms.rs
+-rw-r--r--   0     1001      127     6094 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/mapping/default.rs
+-rw-r--r--   0     1001      127     5734 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/mapping/errors.rs
+-rw-r--r--   0     1001      127     5074 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/mapping/validation_inference.rs
+-rw-r--r--   0     1001      127    25483 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/mapping.rs
+-rw-r--r--   0     1001      127      800 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/parsing/errors.rs
+-rw-r--r--   0     1001      127   191162 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/parsing/nom_parsing.rs
+-rw-r--r--   0     1001      127    60674 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/parsing/parser_test.rs
+-rw-r--r--   0     1001      127     2812 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/parsing/parsing_ast.rs
+-rw-r--r--   0     1001      127      808 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/parsing.rs
+-rw-r--r--   0     1001      127    13035 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/resolver.rs
+-rw-r--r--   0     1001      127     1963 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/templates/errors.rs
+-rw-r--r--   0     1001      127    11029 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/src/templates.rs
+-rw-r--r--   0     1001      127        8 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/tests/stottr_testdata/.gitignore
+-rw-r--r--   0     1001      127      462 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/tests/stottr_testdata/expected_easy_case.ttl
+-rw-r--r--   0     1001      127    37941 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/tests/test_stottr.rs
+-rw-r--r--   0     1001      127     1361 2024-04-10 10:34:15.000000 maplib-0.8.7/maplib/tests/utils.rs
+-rw-r--r--   0     1001      127      876 2024-04-10 10:34:15.000000 maplib-0.8.7/Cargo.toml
+-rw-r--r--   0     1001      127     1128 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/Cargo.toml
+-rw-r--r--   0     1001      127      391 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/constants.rs
+-rw-r--r--   0     1001      127     3823 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/conversion.rs
+-rw-r--r--   0     1001      127     2691 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/errors.rs
+-rw-r--r--   0     1001      127     9279 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/export_triples.rs
+-rw-r--r--   0     1001      127      958 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/io_funcs.rs
+-rw-r--r--   0     1001      127    20676 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/lib.rs
+-rw-r--r--   0     1001      127     2353 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/native_parquet_write.rs
+-rw-r--r--   0     1001      127    11265 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/ntriples_write.rs
+-rw-r--r--   0     1001      127      496 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/rdfs_inferencing.rs
+-rw-r--r--   0     1001      127      865 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/errors.rs
+-rw-r--r--   0     1001      127     5904 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_aggregate.rs
+-rw-r--r--   0     1001      127    17103 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_expressions.rs
+-rw-r--r--   0     1001      127      939 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/distinct.rs
+-rw-r--r--   0     1001      127     1407 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/extend.rs
+-rw-r--r--   0     1001      127     1299 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/filter.rs
+-rw-r--r--   0     1001      127     2400 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/group.rs
+-rw-r--r--   0     1001      127     1172 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/join.rs
+-rw-r--r--   0     1001      127     2113 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/left_join.rs
+-rw-r--r--   0     1001      127     2270 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs
+-rw-r--r--   0     1001      127     1204 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/minus.rs
+-rw-r--r--   0     1001      127     2091 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/order_by.rs
+-rw-r--r--   0     1001      127    28820 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/path.rs
+-rw-r--r--   0     1001      127     1055 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/project.rs
+-rw-r--r--   0     1001      127     1742 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs
+-rw-r--r--   0     1001      127    17085 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/triple.rs
+-rw-r--r--   0     1001      127     1245 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/union.rs
+-rw-r--r--   0     1001      127     3927 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/values.rs
+-rw-r--r--   0     1001      127     5571 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns.rs
+-rw-r--r--   0     1001      127     1316 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql/lazy_order.rs
+-rw-r--r--   0     1001      127    10582 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/sparql.rs
+-rw-r--r--   0     1001      127     9779 2024-04-10 10:34:15.000000 maplib-0.8.7/triplestore/src/triples_read.rs
+-rw-r--r--   0     1001      127      183 2024-04-10 10:34:15.000000 maplib-0.8.7/parquet_io/Cargo.toml
+-rw-r--r--   0     1001      127     2881 2024-04-10 10:34:15.000000 maplib-0.8.7/parquet_io/src/lib.rs
+-rw-r--r--   0     1001      127      212 2024-04-10 10:34:15.000000 maplib-0.8.7/shacl/Cargo.toml
+-rw-r--r--   0     1001      127       70 2024-04-10 10:34:15.000000 maplib-0.8.7/shacl/src/errors.rs
+-rw-r--r--   0     1001      127      455 2024-04-10 10:34:15.000000 maplib-0.8.7/shacl/src/lib.rs
+-rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 maplib-0.8.7/py_maplib/Cargo.toml
+-rw-r--r--   0     1001      127      391 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/.gitignore
+-rw-r--r--   0     1001      127    11459 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/LICENSE
+-rw-r--r--   0     1001      127     6021 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/README.md
+-rw-r--r--   0     1001      127       11 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/doc/.gitignore
+-rw-r--r--   0     1001      127     1731 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/doc/API.md
+-rw-r--r--   0     1001      127    13686 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/doc/rds_mapping.ipynb
+-rw-r--r--   0     1001      127       22 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/python/maplib/.gitignore
+-rw-r--r--   0     1001      127      127 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/python/maplib/__init__.py
+-rw-r--r--   0     1001      127     8963 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/python/maplib/_maplib.pyi
+-rw-r--r--   0     1001      127        0 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/python/maplib/py.typed
+-rw-r--r--   0     1001      127     3499 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/src/error.rs
+-rw-r--r--   0     1001      127    15049 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/src/lib.rs
+-rw-r--r--   0     1001      127      138 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/.gitignore
+-rw-r--r--   0     1001      127       72 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/out.ttl
+-rw-r--r--   0     1001      127       20 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/requirements.txt
+-rw-r--r--   0     1001      127     4994 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_basics.py
+-rw-r--r--   0     1001      127     5901 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_blank_nodes_multi.py
+-rw-r--r--   0     1001      127    18343 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_gtfs_benchmark.py
+-rw-r--r--   0     1001      127    16847 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_integration.py
+-rw-r--r--   0     1001      127     3367 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_pizza_example.py
+-rw-r--r--   0     1001      127     1550 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/test_read.py
+-rw-r--r--   0     1001      127       24 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_constant_object_query.csv
+-rw-r--r--   0     1001      127     2935 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv
+-rw-r--r--   0     1001      127    13780 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_query.csv
+-rw-r--r--   0     1001      127     4813 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv
+-rw-r--r--   0     1001      127      122 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/larger_query.csv
+-rw-r--r--   0     1001      127       88 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_join_query.csv
+-rw-r--r--   0     1001      127       48 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_join_query_two_vars.csv
+-rw-r--r--   0     1001      127       48 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_leftjoin_query.csv
+-rw-r--r--   0     1001      127      644 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_query.csv
+-rw-r--r--   0     1001      127      644 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_query_sorting.csv
+-rw-r--r--   0     1001      127      166 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_union_query.csv
+-rw-r--r--   0     1001      127     3247 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/property_path_query.csv
+-rw-r--r--   0     1001      127      660 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/read_ntriples.csv
+-rw-r--r--   0     1001      127      638 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/read_ntriples.nt
+-rw-r--r--   0     1001      127      498 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/read_ntriples2.csv
+-rw-r--r--   0     1001      127      757 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_construct_query_nothing.csv
+-rw-r--r--   0     1001      127    28024 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_construct_query_something.csv
+-rw-r--r--   0     1001      127      259 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_insert_query_nothing.csv
+-rw-r--r--   0     1001      127    11934 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_insert_query_something.csv
+-rw-r--r--   0     1001      127     3327 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_property_path_query.csv
+-rw-r--r--   0     1001      127    20308 2024-04-10 10:34:15.000000 maplib-0.8.7/py_maplib/tests/testdata/simple_query.csv
+-rw-r--r--   0     1001      127    66960 2024-04-10 10:34:47.000000 maplib-0.8.7/py_maplib/Cargo.lock
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 maplib-0.8.7/pyproject.toml
+-rw-r--r--   0     1001      127      127 2024-04-10 10:34:15.000000 maplib-0.8.7/python/maplib/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-10 10:34:15.000000 maplib-0.8.7/python/maplib/py.typed
+-rw-r--r--   0     1001      127     8963 2024-04-10 10:34:15.000000 maplib-0.8.7/python/maplib/_maplib.pyi
+-rw-r--r--   0     1001      127     6021 2024-04-10 10:34:15.000000 maplib-0.8.7/README.md
+-rw-r--r--   0     1001      127    11459 2024-04-10 10:34:15.000000 maplib-0.8.7/LICENSE
+-rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 maplib-0.8.7/PKG-INFO
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/Cargo.toml` & `maplib-0.8.7/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-[package]
-name = "triplestore"
-version = "0.5.0"
-edition = "2021"
+[workspace]
 resolver = "2"
+members=[
+    "maplib",
+    "triplestore",
+    "parquet_io",
+    "shacl"
+]
 
-[dependencies]
-#query_processing = {path = "../../query_processing"}
-query_processing = { git = "https://github.com/DataTreehouse/query_processing"}
-#representation = { path = "../../representation"}
-representation = { git = "https://github.com/DataTreehouse/representation"}
-parquet_io = {path= "../parquet_io" }
-
-rayon = "1.6.0"
-sprs = {version="0.11.1", features=["multi_thread"]}
-spargebra = { git = "https://github.com/DataTreehouse/spargebra"}
-oxrdf = {version="0.1.7"}
-polars = {version="0.37.0", features=["zip_with","performant", "cse", "semi_anti_join","abs", "round_series", "lazy", "concat_str", "is_in", "dtype-full", "strings", "rows", "timezones", "polars-time", "temporal", "list_eval", "partition_by", "parquet", "diagonal_concat", "cross_join", "cum_agg"] }
-log="0.4.19"
+[workspace.dependencies]
+#representation = {path="../../representation"}
+representation = { git = "https://github.com/DataTreehouse/representation", tag="v0.5.0"}
+spargebra = { git = "https://github.com/DataTreehouse/spargebra", tag = "v0.2.8"}
+query_processing = { git = "https://github.com/DataTreehouse/query_processing", tag="v0.2.0"}
+polars = {version="0.38.3" }
+polars-utils = "0.38.3"
+polars-core = "0.38.3"
+rayon = "1.10.0"
+oxrdf = "0.1.7"
 rio_turtle = "0.8.4"
-rio_xml = "0.8.4"
 rio_api = "0.8.4"
-polars-utils = "0.37.0"
-polars-core = "0.37.0"
-chrono = "0.4"
-chrono-tz = "0.8"
-uuid = {version = "1.1.2", features = [
+rio_xml = "0.8.4"
+env_logger = "0.11.3"
+log="0.4.21"
+chrono = "0.4.37"
+chrono-tz = "0.9.0"
+uuid = {version="1.8.0", features = [
     "v4",                # Lets you generate random UUIDs
     "fast-rng",          # Use a faster (but still sufficiently random) RNG
-    ]}
+]}
 thiserror="1.0.31"
-env_logger = "0.10.0"
-oxiri = "0.2.2"
+
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/conversion.rs` & `maplib-0.8.7/triplestore/src/conversion.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 use crate::constants::{
     XSD_DATETIME_WITHOUT_TZ_FORMAT, XSD_DATETIME_WITH_TZ_FORMAT, XSD_DATE_WITHOUT_TZ_FORMAT,
 };
 use chrono::TimeZone as ChronoTimeZone;
 use chrono::{Datelike, Timelike};
 use polars::prelude::{col, lit, IntoLazy};
-use polars_core::datatypes::{DataType, TimeZone};
-use polars_core::frame::DataFrame;
-use polars_core::series::{IntoSeries, Series};
+use polars::prelude::{DataFrame, DataType, IntoSeries, Series, TimeZone};
 use representation::{LANG_STRING_LANG_FIELD, LANG_STRING_VALUE_FIELD};
 
 pub fn convert_to_string(series: &Series) -> Option<Series> {
     let series_data_type = series.dtype();
 
     match series_data_type {
         DataType::String => return None,
@@ -87,16 +85,26 @@
                 .unwrap()
                 .as_datetime_iter()
                 .map(|x| x.unwrap())
                 .map(|x| {
                     format!(
                         "{}",
                         timezone
-                            .ymd(x.year(), x.month(), x.day())
-                            .and_hms_nano(x.hour(), x.minute(), x.second(), x.nanosecond())
+                            .with_ymd_and_hms(
+                                x.year(),
+                                x.month(),
+                                x.day(),
+                                x.hour(),
+                                x.minute(),
+                                x.second()
+                            )
+                            .latest()
+                            .unwrap()
+                            .with_nanosecond(x.nanosecond())
+                            .unwrap()
                             .format(XSD_DATETIME_WITH_TZ_FORMAT)
                     )
                 }),
         );
 
         datetime_strings
     } else {
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/errors.rs` & `maplib-0.8.7/triplestore/src/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/export_triples.rs` & `maplib-0.8.7/triplestore/src/export_triples.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use super::Triplestore;
 
 use crate::constants::{OBJECT_COL_NAME, SUBJECT_COL_NAME};
 use crate::conversion::convert_to_string;
 use crate::errors::TriplestoreError;
 use oxrdf::{Literal, NamedNode, Subject, Term, Triple};
-use polars::prelude::{col, IntoLazy};
-use polars_core::prelude::AnyValue;
+use polars::prelude::{col, AnyValue, IntoLazy};
 use representation::{
     literal_iri_to_namednode, RDFNodeType, TripleType, LANG_STRING_LANG_FIELD,
     LANG_STRING_VALUE_FIELD,
 };
 
 impl Triplestore {
     pub fn object_property_triples<F, T>(
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/io_funcs.rs` & `maplib-0.8.7/triplestore/src/io_funcs.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/lib.rs` & `maplib-0.8.7/triplestore/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 use crate::io_funcs::{create_folder_if_not_exists, delete_tmp_parquets_in_caching_folder};
 use crate::sparql::lazy_graph_patterns::load_tt::multiple_tt_to_lf;
 use log::debug;
 use oxrdf::NamedNode;
 use parquet_io::{
     property_to_filename, scan_parquet, split_write_tmp_df, write_parquet, ParquetIOError,
 };
-use polars::prelude::{col, concat, IntoLazy, JoinArgs, JoinType, LazyFrame, UnionArgs};
-use polars_core::datatypes::AnyValue;
-use polars_core::frame::{DataFrame, UniqueKeepStrategy};
+use polars::prelude::{
+    col, concat, AnyValue, DataFrame, IntoLazy, JoinArgs, JoinType, LazyFrame, UnionArgs,
+    UniqueKeepStrategy,
+};
 use polars_core::utils::concat_df;
 use rayon::iter::ParallelIterator;
 use rayon::iter::{IntoParallelRefIterator, ParallelDrainRange};
 use representation::solution_mapping::SolutionMappings;
 use representation::{literal_iri_to_namednode, RDFNodeType};
 use std::collections::HashMap;
 use std::fs::remove_file;
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/native_parquet_write.rs` & `maplib-0.8.7/triplestore/src/native_parquet_write.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/ntriples_write.rs` & `maplib-0.8.7/triplestore/src/ntriples_write.rs`

 * *Files 5% similar despite different names*

```diff
@@ -24,30 +24,20 @@
 use crate::conversion::convert_to_string;
 use crate::errors::TriplestoreError;
 use oxrdf::NamedNode;
 use parquet_io::scan_parquet;
 use polars::export::rayon::iter::{IntoParallelIterator, ParallelIterator};
 use polars::export::rayon::prelude::ParallelExtend;
 use polars::prelude::{AnyValue, DataFrame, Series};
-use polars::series::SeriesIter;
+use polars_core::series::SeriesIter;
 use polars_core::POOL;
 use polars_utils::contention_pool::LowContentionPool;
 use representation::{RDFNodeType, TripleType};
 use std::io::Write;
 
-/// Utility to write to `&mut Vec<u8>` buffer
-struct StringWrap<'a>(pub &'a mut Vec<u8>);
-
-impl<'a> std::fmt::Write for StringWrap<'a> {
-    fn write_str(&mut self, s: &str) -> std::fmt::Result {
-        self.0.extend_from_slice(s.as_bytes());
-        Ok(())
-    }
-}
-
 impl Triplestore {
     pub fn write_n_triples_all_dfs<W: Write + ?Sized>(
         &mut self,
         writer: &mut W,
         chunk_size: usize,
     ) -> Result<(), TriplestoreError> {
         self.deduplicate()?;
@@ -231,32 +221,14 @@
     write!(f, " ").unwrap();
     write_iri(f, v);
     write!(f, " ").unwrap();
     write_string(f, lex);
     writeln!(f, " .").unwrap();
 }
 
-fn write_lang_string_property_triple(f: &mut Vec<u8>, mut any_values: Vec<AnyValue>, v: &str) {
-    any_values.pop().unwrap();
-    let lex = if let AnyValue::String(lex) = any_values.pop().unwrap() {
-        lex
-    } else {
-        panic!()
-    };
-    let s = if let AnyValue::String(s) = any_values.pop().unwrap() {
-        s
-    } else {
-        panic!()
-    };
-    write_iri_or_blanknode(f, s);
-    write!(f, " ").unwrap();
-    write_iri(f, v);
-    writeln!(f, " {} .", lex).unwrap();
-}
-
 //Assumes that the data has been bulk-converted
 fn write_non_string_property_triple(
     f: &mut Vec<u8>,
     dt: &str,
     mut any_values: Vec<AnyValue>,
     v: &str,
 ) {
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/errors.rs` & `maplib-0.8.7/triplestore/src/sparql/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_aggregate.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_aggregate.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_expressions.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_expressions.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/distinct.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/distinct.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/extend.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/extend.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/filter.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/filter.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/group.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/group.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/join.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/join.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/left_join.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/left_join.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/load_tt.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/minus.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/minus.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/order_by.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/order_by.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/path.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/path.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 use super::Triplestore;
 use crate::constants::{OBJECT_COL_NAME, SUBJECT_COL_NAME};
 use crate::sparql::errors::SparqlError;
-use crate::sparql::lazy_graph_patterns::triple::create_empty_lf_datatypes;
 use oxrdf::vocab::xsd;
 use oxrdf::{NamedNode, Variable};
-use polars::prelude::{col, lit, DataFrameJoinOps, IntoLazy};
-use polars::prelude::{JoinArgs, JoinType};
-use polars_core::datatypes::AnyValue;
-use polars_core::frame::{DataFrame, UniqueKeepStrategy};
-use polars_core::series::{IntoSeries, Series};
+use polars::prelude::{
+    col, lit, AnyValue, DataFrame, DataFrameJoinOps, IntoLazy, IntoSeries, JoinArgs, JoinType,
+    Series, UniqueKeepStrategy,
+};
 use query_processing::errors::QueryProcessingError;
 use query_processing::graph_patterns::{join, union};
 use representation::multitype::{
     compress_actual_multitypes, force_convert_multicol_to_single_col, group_by_workaround,
     implode_multicolumns,
 };
 use representation::query_context::{Context, PathEntry};
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/project.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/project.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/pvalues.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/triple.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/triple.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 };
 
 use crate::constants::{OBJECT_COL_NAME, SUBJECT_COL_NAME};
 use crate::sparql::lazy_graph_patterns::load_tt::multiple_tt_to_lf;
 use log::debug;
 use oxrdf::NamedNode;
 use polars::prelude::IntoLazy;
-use polars::prelude::{col, lit, Expr, JoinType};
-use polars_core::datatypes::{AnyValue, DataType};
-use polars_core::frame::DataFrame;
-use polars_core::series::Series;
+use polars::prelude::{col, lit, AnyValue, DataFrame, DataType, Expr, JoinType, Series};
 use query_processing::graph_patterns::{join, union};
 use representation::multitype::convert_lf_col_to_multitype;
 use representation::{literal_iri_to_namednode, BaseRDFNodeType, RDFNodeType};
 use spargebra::term::{NamedNodePattern, TermPattern, TriplePattern};
 use std::collections::{HashMap, HashSet};
 
 impl Triplestore {
@@ -323,15 +320,15 @@
             }
 
             if !height_0 {
                 solution_mappings.push(SolutionMappings::new(lf, datatypes_map));
             }
         }
         Ok(if !solution_mappings.is_empty() {
-            let mut sm = union(solution_mappings)?;
+            let sm = union(solution_mappings)?;
             (sm, false)
         } else {
             create_empty_lf_datatypes(
                 subject_keep_rename,
                 verb_keep_rename,
                 object_keep_rename,
                 object_datatype_req,
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/union.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/union.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns/values.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns/values.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use super::Triplestore;
 use crate::sparql::errors::SparqlError;
 use oxrdf::Variable;
-use polars::prelude::{IntoLazy, JoinType};
-use polars_core::frame::DataFrame;
+use polars::prelude::{DataFrame, IntoLazy, JoinType};
 use query_processing::graph_patterns::join;
 use representation::query_context::Context;
 use representation::solution_mapping::SolutionMappings;
 use representation::sparql_to_polars::{
     polars_literal_values_to_series, sparql_literal_to_polars_literal_value,
     sparql_named_node_to_polars_literal_value,
 };
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_graph_patterns.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_graph_patterns.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql/lazy_order.rs` & `maplib-0.8.7/triplestore/src/sparql/lazy_order.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/sparql.rs` & `maplib-0.8.7/triplestore/src/sparql.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 use std::collections::HashMap;
 
 use super::Triplestore;
 use crate::constants::{OBJECT_COL_NAME, OTTR_IRI, SUBJECT_COL_NAME, VERB_COL_NAME};
 use crate::sparql::errors::SparqlError;
 use crate::TriplesToAdd;
 use polars::frame::DataFrame;
-use polars::prelude::{col, IntoLazy};
+use polars::prelude::{col, DataType, IntoLazy, Series, UniqueKeepStrategy};
 use polars_core::enable_string_cache;
-use polars_core::prelude::{DataType, Series, UniqueKeepStrategy};
 use representation::literals::sparql_literal_to_any_value;
 use representation::multitype::split_df_multicols;
 use representation::solution_mapping::{EagerSolutionMappings, SolutionMappings};
 use representation::RDFNodeType;
 use spargebra::term::{NamedNodePattern, TermPattern, TriplePattern};
 use spargebra::Query;
 use uuid::Uuid;
```

### Comparing `maplib-0.8.5/local_dependencies/triplestore/src/triples_read.rs` & `maplib-0.8.7/triplestore/src/triples_read.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 use crate::errors::TriplestoreError;
 use crate::TriplesToAdd;
 use oxiri::Iri;
 
 use crate::constants::{OBJECT_COL_NAME, SUBJECT_COL_NAME};
 use oxrdf::vocab::{rdf, xsd};
 use oxrdf::NamedNode;
-use polars_core::frame::DataFrame;
-use polars_core::prelude::{AnyValue, Series};
+use polars::prelude::{AnyValue, DataFrame, Series};
 use representation::literals::sparql_literal_to_any_value;
 use representation::RDFNodeType;
 use rio_api::parser::TriplesParser;
 use rio_turtle::{NTriplesParser, TurtleError, TurtleParser};
 use rio_xml::{RdfXmlError, RdfXmlParser};
 use std::collections::HashMap;
 use std::fs::File;
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/ast.rs` & `maplib-0.8.7/maplib/src/ast.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/constants.rs` & `maplib-0.8.7/maplib/src/constants.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/document.rs` & `maplib-0.8.7/maplib/src/document.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/mapping/constant_terms.rs` & `maplib-0.8.7/maplib/src/mapping/constant_terms.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 use crate::ast::{ConstantLiteral, ConstantTerm, PType};
 use crate::constants::{BLANK_NODE_IRI, NONE_IRI, OTTR_IRI};
 use crate::mapping::errors::MappingError;
 use crate::mapping::RDFNodeType;
 
 use oxrdf::NamedNode;
-use polars::prelude::{concat_list, lit, Expr, LiteralValue, SpecialEq};
-use polars_core::datatypes::DataType;
-use polars_core::prelude::{AnyValue, IntoSeries, ListChunked, Series};
+use polars::prelude::{
+    concat_list, lit, AnyValue, DataType, Expr, IntoSeries, ListChunked, LiteralValue, Series,
+    SpecialEq,
+};
 use rayon::iter::ParallelIterator;
 use rayon::prelude::IntoParallelIterator;
 use representation::literals::sparql_literal_to_any_value;
 use std::ops::Deref;
 
 const BLANK_NODE_SERIES_NAME: &str = "blank_node_series";
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/mapping/default.rs` & `maplib-0.8.7/maplib/src/mapping/default.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     DEFAULT_PREDICATE_URI_PREFIX, DEFAULT_TEMPLATE_PREFIX, OTTR_IRI, OTTR_TRIPLE,
 };
 use crate::mapping::errors::MappingError;
 use crate::mapping::ExpandOptions;
 use log::warn;
 
 use oxrdf::NamedNode;
-use polars::prelude::{col, IntoLazy};
-use polars_core::frame::DataFrame;
-use polars_core::prelude::DataType;
+use polars::prelude::{col, DataFrame, DataType, IntoLazy};
 use uuid::Uuid;
 
 impl Mapping {
     pub fn expand_default(
         &mut self,
         mut df: DataFrame,
         pk_col: String,
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/mapping/errors.rs` & `maplib-0.8.7/maplib/src/mapping/errors.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 use crate::ast::{ConstantTerm, PType};
 use oxrdf::IriParseError;
-use polars_core::error::PolarsError;
-use polars_core::frame::DataFrame;
-use polars_core::prelude::DataType;
+use polars::prelude::{DataFrame, DataType, PolarsError};
 use std::fmt::{Display, Formatter};
 use std::io;
 use thiserror::Error;
 use triplestore::errors::TriplestoreError;
 
 #[derive(Error, Debug)]
 pub enum MappingError {
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/mapping/validation_inference.rs` & `maplib-0.8.7/maplib/src/mapping/validation_inference.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use super::Mapping;
 use crate::ast::{has_iritype, PType, Parameter, Signature};
 
 use crate::mapping::errors::MappingError;
 use crate::mapping::{PrimitiveColumn, RDFNodeType};
 use oxrdf::NamedNode;
-use polars_core::frame::DataFrame;
-use polars_core::prelude::DataType;
+use polars::prelude::{DataFrame, DataType};
 use representation::polars_to_sparql::primitive_polars_type_to_literal_type;
 use std::collections::{HashMap, HashSet};
 
 impl Mapping {
     pub fn validate_infer_dataframe_columns(
         &self,
         signature: &Signature,
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/mapping.rs` & `maplib-0.8.7/maplib/src/mapping.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 use crate::errors::MaplibError;
 use crate::mapping::constant_terms::{constant_blank_node_to_series, constant_to_expr};
 use crate::mapping::errors::MappingError;
 use crate::templates::TemplateDataset;
 use log::debug;
 use oxrdf::{NamedNode, Triple};
 use polars::lazy::prelude::{col, Expr};
-use polars::prelude::{lit, DataFrame, IntoLazy};
-use polars_core::prelude::NamedFrom;
-use polars_core::series::Series;
+use polars::prelude::{lit, DataFrame, IntoLazy, NamedFrom, Series};
 use rayon::iter::IndexedParallelIterator;
 use rayon::iter::ParallelDrainRange;
 use rayon::iter::ParallelIterator;
 use representation::RDFNodeType;
 use shacl::errors::ShaclError;
 use shacl::{validate, ValidationReport};
 use std::cmp::{max, min};
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/parsing/errors.rs` & `maplib-0.8.7/maplib/src/parsing/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/parsing/nom_parsing.rs` & `maplib-0.8.7/maplib/src/parsing/nom_parsing.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/parsing/parser_test.rs` & `maplib-0.8.7/maplib/src/parsing/parser_test.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/parsing/parsing_ast.rs` & `maplib-0.8.7/maplib/src/parsing/parsing_ast.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/parsing.rs` & `maplib-0.8.7/maplib/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/resolver.rs` & `maplib-0.8.7/maplib/src/resolver.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/templates/errors.rs` & `maplib-0.8.7/maplib/src/templates/errors.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/src/templates.rs` & `maplib-0.8.7/maplib/src/templates.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/maplib/tests/test_stottr.rs` & `maplib-0.8.7/maplib/tests/test_stottr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 #[cfg(test)]
 mod utils;
 
 use crate::utils::triples_from_file;
 use maplib::mapping::{ExpandOptions, Mapping};
 use oxrdf::{Literal, NamedNode, Subject, Term, Triple};
-use polars::frame::DataFrame;
-use polars::prelude::{col, IntoLazy};
-use polars::series::Series;
-use polars_core::prelude::{AnyValue, TimeUnit};
+use polars::prelude::{col, AnyValue, DataFrame, IntoLazy, Series, TimeUnit};
 use rstest::*;
 use serial_test::serial;
 use std::collections::HashSet;
 use std::fs::File;
 use std::path::PathBuf;
 
 #[fixture]
```

### Comparing `maplib-0.8.5/local_dependencies/maplib/tests/utils.rs` & `maplib-0.8.7/maplib/tests/utils.rs`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/local_dependencies/parquet_io/src/lib.rs` & `maplib-0.8.7/parquet_io/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-use polars::prelude::{LazyFrame, ParallelStrategy, ParquetWriter, ScanArgsParquet};
-use polars_core::frame::DataFrame;
+use polars::prelude::{
+    DataFrame, LazyFrame, ParallelStrategy, ParquetWriter, PolarsError, ScanArgsParquet,
+};
 use std::cmp::min;
 use std::fs::File;
 use std::path::{Path, PathBuf};
 use uuid::Uuid;
 
-use polars_core::error::PolarsError;
 use std::fmt::{Display, Formatter};
 use std::io;
 use thiserror::Error;
 
 const PARQUET_DF_SIZE: usize = 50_000_000;
 
 #[derive(Error, Debug)]
```

### Comparing `maplib-0.8.5/Cargo.toml` & `maplib-0.8.7/py_maplib/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [package]
 name = "py_maplib"
-version = "0.8.5"
+version = "0.8.7"
 edition = "2021"
 
 [workspace]
 
 [dependencies]
-pyo3 = {version = "0.19.2", features = ["extension-module"] }
-maplib = {path= "local_dependencies/maplib" }
-triplestore = {path= "local_dependencies/triplestore" }
-#representation = {path="../../representation"}
-representation = { git = "https://github.com/DataTreehouse/representation"}
-shacl = {path= "local_dependencies/shacl" }
+pyo3 = {version = "0.21.1", features = ["extension-module"] }
+maplib = {path="../maplib"}
+triplestore = {path="../triplestore"}
+representation = { git = "https://github.com/DataTreehouse/representation", tag="v0.5.0"}
+shacl = {path="../shacl"}
 oxrdf = {version="0.1.7"}
 #pydf_io = {path = "../../pydf_io"}
-pydf_io = { git = "https://github.com/DataTreehouse/pydf_io"}
+pydf_io = { git = "https://github.com/DataTreehouse/pydf_io", tag="v0.7.0"}
 thiserror="1.0.31"
-polars-lazy = "0.37.0"
-polars-core = {version="0.37.0", features=["dtype-array", "dtype-categorical", "dtype-date", "dtype-datetime",
+polars = {version="0.38.3", features=["dtype-array", "dtype-categorical", "dtype-date", "dtype-datetime",
     "dtype-decimal", "dtype-duration", "dtype-i8", "dtype-i16", "dtype-struct", "dtype-time", "dtype-u8", "dtype-u16"]}
-log ="0.4.19"
+log ="0.4.21"
 
 [lib]
 name = "maplib"
 crate-type = ["cdylib"]
 
 [package.metadata.maturin]
 python-source = "python"
```

### Comparing `maplib-0.8.5/LICENSE` & `maplib-0.8.7/py_maplib/LICENSE`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/README.md` & `maplib-0.8.7/py_maplib/README.md`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/doc/API.md` & `maplib-0.8.7/py_maplib/doc/API.md`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/doc/rds_mapping.ipynb` & `maplib-0.8.7/py_maplib/doc/rds_mapping.ipynb`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/pyproject.toml` & `maplib-0.8.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "maplib"
-description = "Dataframe-based interactive knowledge graph construction using stOTTR templates"
-dependencies = ["polars==0.20.13", "pyarrow>=7.0.0"]
+description = "Dataframe-based interactive knowledge graph construction"
+dependencies = ["polars>=0.20.13", "pyarrow>=7.0.0"]
 readme = "README.md"
 authors = [{name = "Magnus Bakken", email = "magnus@data-treehouse.com" }]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 keywords = ["rdf", "graph", "dataframe", "sparql", "ottr"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,13 +23,14 @@
 [project.urls]
 Homepage = "https://github.com/DataTreehouse/maplib"
 Documentation = "https://github.com/DataTreehouse/maplib/blob/main/doc/python_mapper_api.md"
 Repository = "https://github.com/DataTreehouse/maplib"
 Changelog = "https://github.com/DataTreehouse/maplib/releases"
 
 [build-system]
-requires = ["maturin==1.2.3"]
+requires = ["maturin==1.5.1"]
 build-backend = "maturin"
 
 [tool.maturin]
 module-name = "maplib._maplib"
-python-source = "python"
+python-source = "python"
+manifest-path = "py_maplib/Cargo.toml"
```

### Comparing `maplib-0.8.5/python/maplib/_maplib.pyi` & `maplib-0.8.7/py_maplib/python/maplib/_maplib.pyi`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/src/error.rs` & `maplib-0.8.7/py_maplib/src/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 // LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 // OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 // SOFTWARE.
 
 use maplib::errors::MaplibError;
 use maplib::mapping::errors::MappingError;
 use maplib::templates::errors::TemplateError;
-use polars_core::error::PolarsError;
+use polars::prelude::{PolarsError};
 use pyo3::{create_exception, exceptions::PyException, prelude::*};
 use shacl::errors::ShaclError;
 use std::fmt::Debug;
 use thiserror::Error;
 use triplestore::errors::TriplestoreError;
 use triplestore::sparql::errors::SparqlError;
```

### Comparing `maplib-0.8.5/src/lib.rs` & `maplib-0.8.7/py_maplib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 // AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 // LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 // OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 // SOFTWARE.
 #[cfg(target_os = "linux")]
 use jemallocator::Jemalloc;
 use oxrdf::vocab::xsd;
-use polars_core::frame::DataFrame;
-use polars_lazy::frame::IntoLazy;
-use polars_lazy::prelude::col;
+use polars::prelude::{col, IntoLazy, DataFrame};
 use pyo3::types::PyList;
 use representation::multitype::{compress_actual_multitypes, lf_column_from_categorical, multi_columns_to_string_cols};
 use representation::polars_to_sparql::primitive_polars_type_to_literal_type;
 use representation::solution_mapping::EagerSolutionMappings;
 use representation::RDFNodeType;
 use triplestore::TripleFormat;
```

### Comparing `maplib-0.8.5/tests/test_basics.py` & `maplib-0.8.7/py_maplib/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/test_blank_nodes_multi.py` & `maplib-0.8.7/py_maplib/tests/test_blank_nodes_multi.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/test_gtfs_benchmark.py` & `maplib-0.8.7/py_maplib/tests/test_gtfs_benchmark.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/test_integration.py` & `maplib-0.8.7/py_maplib/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/test_pizza_example.py` & `maplib-0.8.7/py_maplib/tests/test_pizza_example.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/test_read.py` & `maplib-0.8.7/py_maplib/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/iterated_property_path_constant_subject_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_constant_subject_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/iterated_property_path_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/iterated_property_path_query_with_bug.csv` & `maplib-0.8.7/py_maplib/tests/testdata/iterated_property_path_query_with_bug.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/multi_datatype_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/multi_datatype_query_sorting.csv` & `maplib-0.8.7/py_maplib/tests/testdata/multi_datatype_query_sorting.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/property_path_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/read_ntriples.csv` & `maplib-0.8.7/py_maplib/tests/testdata/read_ntriples.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/read_ntriples.nt` & `maplib-0.8.7/py_maplib/tests/testdata/read_ntriples.nt`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/simple_construct_query_nothing.csv` & `maplib-0.8.7/py_maplib/tests/testdata/simple_construct_query_nothing.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/simple_construct_query_something.csv` & `maplib-0.8.7/py_maplib/tests/testdata/simple_construct_query_something.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/simple_insert_query_something.csv` & `maplib-0.8.7/py_maplib/tests/testdata/simple_insert_query_something.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/simple_property_path_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/simple_property_path_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/tests/testdata/simple_query.csv` & `maplib-0.8.7/py_maplib/tests/testdata/simple_query.csv`

 * *Files identical despite different names*

### Comparing `maplib-0.8.5/Cargo.lock` & `maplib-0.8.7/py_maplib/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alga"
 version = "0.9.3"
@@ -83,14 +83,62 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.6.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
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
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
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
 name = "approx"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0e60b75072ecd4168020818c0107f2857bb6c4e64252d8d3983f6263b40a5c3"
 dependencies = [
  "num-traits",
 ]
@@ -125,26 +173,26 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.78"
+version = "0.1.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "461abc97219de0eaaf81fe3ef974a540158f3d079c2ab200f891f1a2ef201e85"
+checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -156,23 +204,23 @@
 name = "atoi_simd"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -229,17 +277,17 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
@@ -250,44 +298,44 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets 0.52.4",
@@ -296,15 +344,26 @@
 [[package]]
 name = "chrono-tz"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
 dependencies = [
  "chrono",
- "chrono-tz-build",
+ "chrono-tz-build 0.2.1",
+ "phf",
+]
+
+[[package]]
+name = "chrono-tz"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93698b29de5e97ad0ae26447b344c482a7284c737d9ddc5f9e52b74a336671bb"
+dependencies = [
+ "chrono",
+ "chrono-tz-build 0.3.0",
  "phf",
 ]
 
 [[package]]
 name = "chrono-tz-build"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -312,22 +371,39 @@
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
+name = "chrono-tz-build"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c088aee841df9c3041febbb73934cfc39708749bf96dc827e3359cd39ef11b1"
+dependencies = [
+ "parse-zoneinfo",
+ "phf",
+ "phf_codegen",
+]
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "comfy-table"
-version = "7.1.0"
+version = "7.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
+checksum = "b34115915337defe99b2aff5c2ce6771e5fbc4079f4b506301f5cf394c8452f7"
 dependencies = [
  "crossterm",
  "strum",
- "strum_macros",
+ "strum_macros 0.26.2",
  "unicode-width",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -426,35 +502,45 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "enum_dispatch"
-version = "0.3.12"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
+checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "env_filter"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
+dependencies = [
+ "log",
+ "regex",
 ]
 
 [[package]]
 name = "env_logger"
-version = "0.10.2"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
+checksum = "38b35839ba51819680ba087cd351788c9a3c476841207e0b8cee0b04722343b9"
 dependencies = [
+ "anstream",
+ "anstyle",
+ "env_filter",
  "humantime",
- "is-terminal",
  "log",
- "regex",
- "termcolor",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -563,15 +649,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -598,17 +684,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -690,44 +776,33 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "is-terminal"
-version = "0.4.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
-dependencies = [
- "hermit-abi",
- "libc",
- "windows-sys 0.52.0",
-]
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "itoap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9028f49264629065d057f340a86acb84867925865f73bbf8d47b4d149a7e88b8"
 
@@ -828,29 +903,29 @@
 ]
 
 [[package]]
 name = "maplib"
 version = "0.5.2"
 dependencies = [
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.9.0",
  "env_logger",
+ "iana-time-zone",
  "log",
+ "mio",
  "nom",
  "oxrdf",
  "parquet_io",
  "polars",
- "polars-core",
- "polars-utils",
  "rayon",
  "representation",
  "rio_api",
  "rio_turtle",
  "shacl",
- "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra)",
+ "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra?tag=v0.2.8)",
  "thiserror",
  "triplestore",
  "unic-char-range",
  "uuid",
 ]
 
 [[package]]
@@ -861,32 +936,32 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
 version = "0.1.39"
@@ -914,14 +989,15 @@
 [[package]]
 name = "mio"
 version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
+ "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.4"
@@ -1066,17 +1142,17 @@
 checksum = "23f3f87617a86af77fa3691e6350483e7154c2ead9f1261b75130e21ca0f8acb"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "oxiri"
-version = "0.2.2"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb175ec8981211357b7b379869c2f8d555881c55ea62311428ec0de46d89bd5c"
+checksum = "d05417ee46e2eb40dd9d590b4d67fc2408208b3a48a6b7f71d2bc1d7ce12a3e0"
 
 [[package]]
 name = "oxrdf"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "309287c8a757e25e06a6156acbd73770bac3e319123f5b4bc0a42e232caf97a5"
 dependencies = [
@@ -1129,15 +1205,14 @@
 ]
 
 [[package]]
 name = "parquet_io"
 version = "0.5.0"
 dependencies = [
  "polars",
- "polars-core",
  "thiserror",
  "uuid",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
@@ -1216,17 +1291,17 @@
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1243,40 +1318,44 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e43795c49010cb851d45227caa17769e83760e21d260ba6285c563b754e1652f"
+checksum = "f01006048a264047d6cba081fed8e11adbd69c15956f9e53185a9ac4a541853c"
 dependencies = [
  "getrandom",
+ "polars-arrow",
  "polars-core",
+ "polars-error",
  "polars-io",
  "polars-lazy",
  "polars-ops",
+ "polars-parquet",
  "polars-sql",
  "polars-time",
+ "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faacd21a2548fa6d50c72d6b8d4649a8e029a0f3c6c5545b7f436f0610e49b0f"
+checksum = "25197f40d71f82b2f79bb394f03e555d3cc1ce4db1dd052c28318721c71e96ad"
 dependencies = [
  "ahash",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "dyn-clone",
  "either",
  "ethnum",
  "fast-float",
  "foreign_vec",
  "futures",
  "getrandom",
@@ -1305,37 +1384,39 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d9dc87f8003ae0edeef5ad9ac92b2a345480bbe17adad64496113ae84706dd"
+checksum = "c354515f73cdbbad03c2bf723fcd68e6825943b3ec503055abc8a8cb08ce46bb"
 dependencies = [
  "bytemuck",
+ "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
+ "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "befd4d280a82219a01035c4f901319ceba65998c594d0c64f9a439cdee1d7777"
+checksum = "6f20d3c227186f74aa3c228c64ef72f5a15617322fed30b4323eaf53b25f8e7b"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "bytemuck",
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "comfy-table",
  "either",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-arrow",
@@ -1351,36 +1432,36 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50f2435b02d1ba36d8c1f6a722cad04e4c0b2705a3112c5706e6960d405d7798"
+checksum = "d66dd0ce51f8bd620eb8bd376502fe68a2b1a446d5433ecd2e75270b0755ce76"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b51fba2cf014cb39c2b38353d601540fb9db643be65abb9ca8ff44b9c4c4a88e"
+checksum = "b40bef2edcdc58394792c4d779465144283a09ff1836324e7b72df7978a6e992"
 dependencies = [
  "ahash",
  "async-trait",
  "atoi_simd",
  "bytes",
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "fast-float",
  "futures",
  "home",
  "itoa",
  "memchr",
  "memmap2",
  "num-traits",
@@ -1399,17 +1480,17 @@
  "smartstring",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d83343e413346f048f3a5ad07c0ea4b5d0bada701a482878213142970b0ddff8"
+checksum = "c27df26a19d3092298d31d47614ad84dc330c106e38aa8cd53727cd91c07cf56"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
@@ -1422,24 +1503,24 @@
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6395f5fd5e1adf016fd6403c0a493181c1a349a7a145b2687cdf50a0d630310a"
+checksum = "7f8a51c3bdc9e7c34196ff6f5c3cb17da134e5aafb1756aaf24b76c7118e63dc"
 dependencies = [
  "ahash",
  "argminmax",
  "base64",
  "bytemuck",
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "either",
  "hashbrown",
  "hex",
  "indexmap",
  "memchr",
  "num-traits",
  "polars-arrow",
@@ -1452,17 +1533,17 @@
  "smartstring",
  "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b664cac41636cc9f146fba584a8e7c2790d7335a278964529fa3e9b4eae96daf"
+checksum = "b8824ee00fbbe83d69553f2711014c50361238d210ed81a7a297695b7db97d42"
 dependencies = [
  "ahash",
  "async-stream",
  "base64",
  "brotli",
  "ethnum",
  "flate2",
@@ -1478,17 +1559,17 @@
  "snap",
  "streaming-decompression",
  "zstd",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "390a831b864bc57a4cb260b0595030dfb6a4260a3723cf8ca17968ee2078b8ff"
+checksum = "0c5e2c1f14e81d60cfa9afe4e611a9bad9631a2cb7cd19b7c0094d0dc32f0231"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown",
  "num-traits",
  "polars-arrow",
@@ -1497,58 +1578,60 @@
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
+ "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb7d7527be2aa33baace9000f6772eb9df7cd57ec010a4b273435d2dc1349e8"
+checksum = "ff48362bd1b078bbbec7e7ba9ec01fea58fee2887db22a8e3deaf78f322fa3c4"
 dependencies = [
  "ahash",
  "bytemuck",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-parquet",
  "polars-time",
  "polars-utils",
  "rayon",
  "regex",
  "smartstring",
- "strum_macros",
+ "strum_macros 0.25.3",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4984d97aad3d0db92afe76ebcab10b5e37a1216618b5703ae0d2917ccd6168c"
+checksum = "63029da56ff6a720b190490bbc7b6263f9b72d1134311b1f381fc8d306d37770"
 dependencies = [
+ "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77f62a8b8f93146ec1eb2ef340d77eeb174e8010035e449bfdd424d2b1fd944a"
+checksum = "3652c362959f608d1297196b973d1e3acb508a9562b886ac39bf7606b841052b"
 dependencies = [
  "hex",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
@@ -1556,52 +1639,59 @@
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d75348a51d0c97f3b83df860ecb35a6ac6c5dafc6278cac4e1ac101d96dc753"
+checksum = "86eb74ea6ddfe675aa5c3f33c00dadbe2b85f0e8e3887b85db1fd5a3397267fd"
 dependencies = [
  "atoi",
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.8.6",
  "now",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-ops",
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.37.0"
+version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f9c955bb1e9b55d835aeb7fe4e4e8826e01abe5f0ada979ceb7d2b9af7b569"
+checksum = "694656a7d2b0cd8f07660dbc8d0fb7a81066ff57a452264907531d805c1e58c4"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
+ "raw-cpuid",
  "rayon",
  "smartstring",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
@@ -1610,116 +1700,118 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_maplib"
-version = "0.8.5"
+version = "0.8.7"
 dependencies = [
  "jemallocator",
  "log",
  "maplib",
  "mimalloc",
  "oxrdf",
- "polars-core",
- "polars-lazy",
+ "polars",
  "pydf_io",
  "pyo3",
  "representation",
  "shacl",
  "thiserror",
  "triplestore",
 ]
 
 [[package]]
 name = "pydf_io"
-version = "0.6.0"
-source = "git+https://github.com/DataTreehouse/pydf_io#c2eb96393c997ba310ec5589702e3e760509d611"
+version = "0.7.0"
+source = "git+https://github.com/DataTreehouse/pydf_io?tag=v0.7.0#ab6bff3f20e3db415731fda51c0619146bdeda4e"
 dependencies = [
  "polars-core",
  "pyo3",
  "simple-error",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "query_processing"
-version = "0.1.0"
-source = "git+https://github.com/DataTreehouse/query_processing#0be98ea503334ae561f5c9d8f5d5742108675309"
+version = "0.2.0"
+source = "git+https://github.com/DataTreehouse/query_processing?tag=v0.2.0#7860f2005d2f68d9289622e5bd0561d174222284"
 dependencies = [
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.9.0",
  "env_logger",
  "log",
  "oxrdf",
  "polars",
  "rayon",
  "representation",
- "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra)",
+ "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra?tag=v0.2.8)",
  "thiserror",
  "uuid",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.28.2"
@@ -1727,17 +1819,17 @@
 checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1775,24 +1867,33 @@
 checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
+name = "raw-cpuid"
+version = "11.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1811,17 +1912,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -1834,30 +1935,28 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "representation"
-version = "0.4.19"
-source = "git+https://github.com/DataTreehouse/representation#9ca31d1050df8a01c977884b6867145ac0e3b0ed"
+version = "0.5.0"
+source = "git+https://github.com/DataTreehouse/representation?tag=v0.5.0#cd11a8ae1bebf399b6d40cdd3bcfb69dd2a54f0a"
 dependencies = [
  "bigdecimal",
  "chrono",
  "log",
  "oxrdf",
  "polars",
- "polars-arrow",
- "polars-core",
  "spargebra 0.2.8 (registry+https://github.com/rust-lang/crates.io-index)",
  "thiserror",
  "uuid",
 ]
 
 [[package]]
 name = "rio_api"
@@ -1892,17 +1991,17 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -1931,33 +2030,33 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "shacl"
 version = "0.1.0"
 dependencies = [
- "polars-core",
+ "polars",
  "representation",
  "thiserror",
  "triplestore",
 ]
 
 [[package]]
 name = "simdutf8"
@@ -1984,17 +2083,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -2031,15 +2130,15 @@
  "peg",
  "rand",
 ]
 
 [[package]]
 name = "spargebra"
 version = "0.2.8"
-source = "git+https://github.com/DataTreehouse/spargebra#3526be510a6a4c292f81bfeaf2fe8d2686ed0c7d"
+source = "git+https://github.com/DataTreehouse/spargebra?tag=v0.2.8#9efcd975284417bb3224c550d7c82db2885cbdc2"
 dependencies = [
  "chrono",
  "datetimeparse",
  "fundu",
  "oxilangtag",
  "oxiri",
  "oxrdf",
@@ -2096,29 +2195,42 @@
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "strum"
-version = "0.25.0"
+version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
+checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 
 [[package]]
 name = "strum_macros"
 version = "0.25.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.53",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "strum_macros"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -2126,28 +2238,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.7"
+version = "0.30.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c385888ef380a852a16209afc8cfad22795dd8873d69c9a14d2e2088f118d18"
+checksum = "e9a84fe4cfc513b41cb2596b624e561ec9e7e1c4b46328e496ed56a53514ef2a"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows",
@@ -2162,23 +2274,14 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
-name = "termcolor"
-version = "1.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "thiserror"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
@@ -2187,22 +2290,22 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
@@ -2224,30 +2327,30 @@
 ]
 
 [[package]]
 name = "triplestore"
 version = "0.5.0"
 dependencies = [
  "chrono",
- "chrono-tz",
+ "chrono-tz 0.9.0",
  "env_logger",
  "log",
  "oxiri",
  "oxrdf",
  "parquet_io",
  "polars",
  "polars-core",
  "polars-utils",
  "query_processing",
  "rayon",
  "representation",
  "rio_api",
  "rio_turtle",
  "rio_xml",
- "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra)",
+ "spargebra 0.2.8 (git+https://github.com/DataTreehouse/spargebra?tag=v0.2.8)",
  "sprs",
  "thiserror",
  "uuid",
 ]
 
 [[package]]
 name = "unic-char-range"
@@ -2280,17 +2383,23 @@
 name = "unicode-width"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
+name = "utf8parse"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
@@ -2327,15 +2436,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2349,15 +2458,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2377,23 +2486,14 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-util"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
@@ -2565,37 +2665,37 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `maplib-0.8.5/PKG-INFO` & `maplib-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: maplib
-Version: 0.8.5
+Version: 0.8.7
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: polars ==0.20.13
+Requires-Dist: polars >=0.20.13
 Requires-Dist: pyarrow >=7.0.0
 License-File: LICENSE
-Summary: Dataframe-based interactive knowledge graph construction using stOTTR templates
+Summary: Dataframe-based interactive knowledge graph construction
 Keywords: rdf,graph,dataframe,sparql,ottr
 Author-email: Magnus Bakken <magnus@data-treehouse.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/DataTreehouse/maplib
 Project-URL: Documentation, https://github.com/DataTreehouse/maplib/blob/main/doc/python_mapper_api.md
 Project-URL: Repository, https://github.com/DataTreehouse/maplib
```

