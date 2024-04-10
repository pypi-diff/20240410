# Comparing `tmp/earthmover-0.2.1-py3-none-any.whl.zip` & `tmp/earthmover-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,51 +1,51 @@
-Zip file size: 68583 bytes, number of entries: 49
--rwxrwxrwx  2.0 unx        5 b- defN 24-Apr-08 23:07 earthmover/VERSION.txt
+Zip file size: 68904 bytes, number of entries: 49
+-rwxrwxrwx  2.0 unx        5 b- defN 24-Apr-09 19:30 earthmover/VERSION.txt
 -rw-r--r--  2.0 unx        2 b- defN 22-Sep-15 19:37 earthmover/__init__.py
 -rw-r--r--  2.0 unx     6377 b- defN 24-Mar-06 16:19 earthmover/__main__.py
 -rw-r--r--  2.0 unx    15311 b- defN 24-Mar-06 16:19 earthmover/earthmover.py
 -rw-r--r--  2.0 unx     3100 b- defN 23-Oct-16 12:59 earthmover/error_handler.py
 -rw-r--r--  2.0 unx     9310 b- defN 23-Oct-16 12:59 earthmover/graph.py
 -rw-r--r--  2.0 unx     6035 b- defN 23-Oct-16 12:59 earthmover/node.py
 -rw-r--r--  2.0 unx     8374 b- defN 23-Oct-16 12:59 earthmover/runs_file.py
--rw-r--r--  2.0 unx     3885 b- defN 24-Apr-08 23:04 earthmover/util.py
+-rw-r--r--  2.0 unx     3958 b- defN 24-Apr-09 19:26 earthmover/util.py
 -rw-r--r--  2.0 unx     5550 b- defN 24-Mar-06 16:19 earthmover/yaml_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-15 19:41 earthmover/nodes/__init__.py
 -rw-r--r--  2.0 unx     4851 b- defN 24-Mar-06 16:19 earthmover/nodes/destination.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Oct-16 12:59 earthmover/nodes/operation.py
+-rw-r--r--  2.0 unx     3963 b- defN 24-Apr-09 19:26 earthmover/nodes/operation.py
 -rw-r--r--  2.0 unx    14481 b- defN 23-Oct-16 12:59 earthmover/nodes/source.py
 -rw-r--r--  2.0 unx     1746 b- defN 23-Oct-16 12:59 earthmover/nodes/transformation.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-15 19:41 earthmover/operations/__init__.py
 -rw-r--r--  2.0 unx    16116 b- defN 23-Oct-16 12:59 earthmover/operations/column.py
 -rw-r--r--  2.0 unx     7208 b- defN 23-Oct-16 12:59 earthmover/operations/dataframe.py
 -rw-r--r--  2.0 unx     9125 b- defN 23-Oct-16 12:59 earthmover/operations/groupby.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Oct-16 12:59 earthmover/operations/row.py
+-rw-r--r--  2.0 unx     4269 b- defN 24-Apr-09 19:26 earthmover/operations/row.py
 -rwxrwxrwx  2.0 unx     6876 b- defN 23-Oct-16 12:59 earthmover/tests/earthmover.yaml
 -rwxrwxrwx  2.0 unx     7571 b- defN 22-Sep-16 13:53 earthmover/tests/expected/animals.jsonl
 -rwxrwxrwx  2.0 unx      434 b- defN 22-Sep-16 13:32 earthmover/tests/expected/big_cats.jsonl
--rwxrwxrwx  2.0 unx      406 b- defN 24-Mar-06 16:35 earthmover/tests/expected/species_count_by_zoo.jsonl
+-rwxrwxrwx  2.0 unx      405 b- defN 24-Apr-09 19:26 earthmover/tests/expected/species_count_by_zoo.jsonl
 -rwxrwxrwx  2.0 unx      821 b- defN 22-Sep-16 13:35 earthmover/tests/expected/total_of_each_species.jsonl
 -rwxrwxrwx  2.0 unx      797 b- defN 22-Sep-16 13:32 earthmover/tests/expected/zoo_count_by_species.jsonl
 -rwxrwxrwx  2.0 unx      280 b- defN 22-Sep-16 13:32 earthmover/tests/expected/zoo_count_by_year_founded.jsonl
 -rwxrwxrwx  2.0 unx     7571 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/animals.jsonl
 -rwxrwxrwx  2.0 unx      434 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/big_cats.jsonl
 -rwxrwxrwx  2.0 unx      406 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/species_count_by_zoo.jsonl
 -rwxrwxrwx  2.0 unx      821 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/total_of_each_species.jsonl
 -rwxrwxrwx  2.0 unx      797 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/zoo_count_by_species.jsonl
 -rwxrwxrwx  2.0 unx      280 b- defN 23-Nov-10 20:34 earthmover/tests/outputs/zoo_count_by_year_founded.jsonl
 -rwxrwxrwx  2.0 unx      712 b- defN 22-Sep-16 15:38 earthmover/tests/sources/birds.csv
 -rwxrwxrwx  2.0 unx      422 b- defN 22-May-24 21:36 earthmover/tests/sources/fishes.csv
 -rwxrwxrwx  2.0 unx      156 b- defN 22-May-24 21:14 earthmover/tests/sources/inventories.csv
 -rwxrwxrwx  2.0 unx      926 b- defN 23-Oct-16 12:59 earthmover/tests/sources/mammals.csv
 -rwxrwxrwx  2.0 unx      478 b- defN 22-May-24 21:06 earthmover/tests/sources/reptiles.csv
--rwxrwxrwx  2.0 unx      284 b- defN 24-Mar-06 16:35 earthmover/tests/sources/zoos.csv
+-rwxrwxrwx  2.0 unx      282 b- defN 24-Apr-09 19:26 earthmover/tests/sources/zoos.csv
 -rwxrwxrwx  2.0 unx      215 b- defN 22-Jul-14 20:55 earthmover/tests/templates/animal.jsont
 -rwxrwxrwx  2.0 unx      184 b- defN 22-May-24 21:33 earthmover/tests/templates/cats.jsont
 -rwxrwxrwx  2.0 unx       93 b- defN 22-Jun-20 13:40 earthmover/tests/templates/count.jsont
--rwxrwxrwx  2.0 unx    11349 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    47059 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      135 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       56 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4436 b- defN 24-Apr-08 23:44 earthmover-0.2.1.dist-info/RECORD
-49 files, 212526 bytes uncompressed, 61375 bytes compressed:  71.1%
+-rwxrwxrwx  2.0 unx    11349 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    47358 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      135 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx       56 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       11 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4436 b- defN 24-Apr-09 19:31 earthmover-0.2.2.dist-info/RECORD
+49 files, 214179 bytes uncompressed, 61696 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -120,29 +120,29 @@
 
 Filename: earthmover/tests/templates/cats.jsont
 Comment: 
 
 Filename: earthmover/tests/templates/count.jsont
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/LICENSE
+Filename: earthmover-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/METADATA
+Filename: earthmover-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/WHEEL
+Filename: earthmover-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/dependency_links.txt
+Filename: earthmover-0.2.2.dist-info/dependency_links.txt
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/entry_points.txt
+Filename: earthmover-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/top_level.txt
+Filename: earthmover-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: earthmover-0.2.1.dist-info/RECORD
+Filename: earthmover-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## earthmover/VERSION.txt

```diff
@@ -1 +1 @@
-0.2.1
+0.2.2
```

## earthmover/util.py

```diff
@@ -1,9 +1,10 @@
 import jinja2
 import hashlib
+import json
 import os
 
 from sys import exc_info
 
 from typing import Optional
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
@@ -125,9 +126,10 @@
 
     """
     template = jinja2.Environment(
         loader=jinja2.FileSystemLoader(os.path.dirname('./'))
     ).from_string(macros.strip() + template_string)
 
     template.globals['md5'] = lambda x: hashlib.md5(x.encode('utf-8')).hexdigest()
+    template.globals['fromjson'] = lambda x: json.loads(x)
 
     return template
```

## earthmover/nodes/operation.py

```diff
@@ -40,14 +40,15 @@
             'combine_columns': column_operations.CombineColumnsOperation,
             'map_values': column_operations.MapValuesOperation,
             'date_format': column_operations.DateFormatOperation,
             'snake_case_columns': column_operations.SnakeCaseColumnsOperation,
 
             'distinct_rows': row_operations.DistinctRowsOperation,
             'filter_rows': row_operations.FilterRowsOperation,
+            'sort_rows': row_operations.SortRowsOperation,
 
             'group_by_with_count': groupby_operations.GroupByWithCountOperation,
             'group_by_with_ag': groupby_operations.GroupByWithAggOperation,
             'group_by': groupby_operations.GroupByOperation,
         }
 
         operation = config.get('operation')
```

## earthmover/operations/row.py

```diff
@@ -109,7 +109,46 @@
         except Exception as _:
             self.error_handler.throw(
                 "error during `filter_rows` operation... check query format?"
             )
             raise
 
         return data
+
+class SortRowsOperation(Operation):
+        """
+
+        """
+        allowed_configs: Tuple[str] = (
+            'operation', 'repartition',
+            'columns', 'descending',
+        )
+
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.columns_list: List[str] = None
+            self.descending: bool = None
+
+        def compile(self):
+            """
+
+            :return:
+            """
+            super().compile()
+
+            self.columns_list = self.error_handler.assert_get_key(self.config, 'columns', dtype=list)
+            self.descending = self.error_handler.assert_get_key(self.config, 'descending', required=False, default=False)
+
+        def execute(self, data: 'DataFrame', **kwargs):
+            """
+
+            :return:
+            """
+            super().execute(data, **kwargs)
+
+            if not set(self.columns_list).issubset(data.columns):
+                self.error_handler.throw(
+                    "one or more columns for sorting are undefined in the dataset"
+                )
+                raise
+
+            return data.sort_values(by=self.columns_list, ascending=(not self.descending))
```

## earthmover/tests/expected/species_count_by_zoo.jsonl

```diff
@@ -1,6 +1,6 @@
-{ "entity": "zoo", "name": "Cincinnatti Zoo and Botanical Garden", "species_count": 8 }
+{ "entity": "zoo", "name": "Cincinnati Zoo and Botanical Garden", "species_count": 8 }
 { "entity": "zoo", "name": "Denver Zoo", "species_count": 8 }
 { "entity": "zoo", "name": "Dallas Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "Oregon Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "Saint Louis Zoo", "species_count": 0 }
 { "entity": "zoo", "name": "San Diego Zoo", "species_count": 0 }
```

## earthmover/tests/sources/zoos.csv

```diff
@@ -1,7 +1,7 @@
 id,name,city,state,date_founded
-1,Cincinnatti Zoo and Botanical Garden,Cincinnatti,OH,Jan 1 1875
+1,Cincinnati Zoo and Botanical Garden,Cincinnati,OH,Jan 1 1875
 2,Denver Zoo,Denver,CO,Jan 1 1896
 3,Dallas Zoo,Dallas,TX,Jan 1 1888
 4,Oregon Zoo,Portland,OR,Jan 1 1888
 5,Saint Louis Zoo,Saint Louis,MO,Jan 1 1910
 6,San Diego Zoo,San Diego,CA,Jan 1 1916
```

## Comparing `earthmover-0.2.1.dist-info/LICENSE` & `earthmover-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `earthmover-0.2.1.dist-info/METADATA` & `earthmover-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthmover
-Version: 0.2.1
+Version: 0.2.2
 Summary: Transforms tabular data sources into text-based data via YAML configuration
 Home-page: https://github.com/edanalytics/earthmover
 Download-URL: https://github.com/edanalytics/earthmover/archive/refs/tags/v0.0.4.tar.gz
 Author: Tom Reitz, Jay Kaiser
 Author-email: treitz@edanalytics.org, jkaiser@edanalytics.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
@@ -279,15 +279,15 @@
     - `.dta`: a [Stata data file](https://www.stata.com/manuals/gsw5.pdf)
 
   
   File type is inferred from the file extension, however you may manually specify `type:` (`csv`, `tsv`, `fixedwidth`, `parquet`, `feather`, `orc`, `json`, `jsonl`, `xml`, `html`, `excel`, `pickle`, `sas`, `spss`, or `stata`) to force `earthmover` to treat a file with an arbitrary extension as a certain type. Remote file paths (`https://somesite.com/path/to/file.csv`) generally work.
 * Database sources are supported via [SQLAlchemy](https://www.sqlalchemy.org/). They must specify a database `connection` string and SQL `query` to run.
 * FTP file sources are supported via [ftplib](https://docs.python.org/3/library/ftplib.html). They must specify an FTP `connection` string.
 
-For any source, optionally specify conditions you `expect` data to meet which, if not true for any row, will cause the run to fail with an error. (This can be useful for detecing and rejecting NULL or missing values before processing the data.) The format must be a Jinja expression that returns a boolean value. This is enables casting values (which are all treated as strings) to numeric formats like int and float for numeric comparisons.
+For any source, optionally specify conditions you `expect` data to meet which, if not true for any row, will cause the run to fail with an error. (This can be useful for detecting and rejecting NULL or missing values before processing the data.) The format must be a Jinja expression that returns a boolean value. This is enables casting values (which are all treated as strings) to numeric formats like int and float for numeric comparisons.
 
 The examples above show `user:pass` in the `connection` string, but if you are version-controlling your YAML you must avoid publishing such credentials. Typically this is done via [environment variables](#environment-variable-references) or [command line parameters](#command-line-parameters), which are both supported by this tool. Such environment variable references may be used throughout your YAML (not just in the `sources` section), and are parsed at load time.
 
 
 ### **`transformations`**
 The `transformations` section of the [YAML configuration](#yaml-configuration) specifies how source data is manipulated by the tool.
 
@@ -551,14 +551,28 @@
         query: school_year < 2020
         behavior: exclude | include
 ```
 The query format is anything supported by [Pandas.DataFrame.query](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.query.html). Specifying `behavior` as `exclude` wraps the Pandas `query()` with `not()`.
 </details>
 
 
+<details>
+<summary><code>sort_rows</code></summary>
+
+Sort rows by one or more columns.
+```yaml
+      - operation: sort_rows
+        columns:
+          - sort_column_1
+        descending: False
+```
+By default, rows are sorted ascendingly. Set `descending: True` to reverse this order.
+</details>
+
+
 #### Group operations
 
 <details>
 <summary><code>group_by</code></summary>
 
 Reduce the number of rows by grouping, and add columns with values calculated over each group.
 ```yaml
@@ -570,16 +584,16 @@
           min_score: min(item_score)
           max_score: max(item_score)
           avg_score: mean(item_score)
           item_scores: agg(item_score,;)
 ```
 Valid aggregation functions are
 * `count()` or `size()` - the number of rows in each group
-* `min(column)` - the minumum (numeric) value in `column` for each group
-* `str_min(column)` - the minumum (string) value in `column` for each group
+* `min(column)` - the minimum (numeric) value in `column` for each group
+* `str_min(column)` - the minimum (string) value in `column` for each group
 * `max(column)` - the maximum (numeric) value in `column` for each group
 * `str_max(column)` - the maximum (string) value in `column` for each group
 * `sum(column)` - the sum of (numeric) values in `column` for each group
 * `mean(column)` or `avg(column)` - the mean of (numeric) values in `column` for each group
 * `std(column)` - the standard deviation of (numeric) values in `column` for each group
 * `var(column)` - the variance of (numeric) values in `column` for each group
 * `agg(column,separator)` - the values of `column` in each group are concatenated, delimited by `separator` (default `separator` is none)
@@ -886,15 +900,15 @@
 ```
 Generally you should separate the mappings, transformations, and structure of your data &ndash; which are probably *not* sensitive &ndash; from the actual input and output &ndash; which may be large and/or sensitive, and therefore should not be committed to a version control system. This can be accomplished in two ways:
 1. include a `.gitignore` or similar file in your project which excludes the `sources/` and `output/` directories from being committed the repository
 1. remove the `sources/` and `output/` directories from your project and update `earthmover.yaml`'s `sources` and `destinations` to reference another location outside the `project/` directory
 
 When dealing with sensitive source data, you may have to comply with security protocols, such as referencing sensitive data from a network storage location rather than copying it to your own computer. In this situation, option 2 above is a good choice.
 
-To facilitate [operationalization]($operationalization-practices), we recommended using [environment vairables](#environment-variable-references) or [command-line parameters](#command-line-parameters) to pass input and output directories and filenames to `earthmover`, rather than hard-coding them into `earthmover.yaml`. For example, rather than
+To facilitate [operationalization]($operationalization-practices), we recommended using [environment variables](#environment-variable-references) or [command-line parameters](#command-line-parameters) to pass input and output directories and filenames to `earthmover`, rather than hard-coding them into `earthmover.yaml`. For example, rather than
 ```yaml
 config:
   output_dir: path/to/outputs/
 ...
 sources:
   source_1:
     file: path/to/inputs/source_file_1.csv
@@ -965,15 +979,15 @@
 * avoid name-sharing for a `source`, a `transformation`, and/or a `destination` - this is allowed but can make debugging confusing
 * [install pygraphviz](https://pygraphviz.github.io/documentation/stable/install.html) and turn on `config` &raquo; `show_graph: True`, then visually inspect your transformations in `graph.png` for structural errors
 * use a linter/validator to validate the formatting of your generated data
 
 You can remove these settings once your `earthmover` project is ready for operationalization.
 
 ## Operationalization practices
-Typically `earthmover` is used when the same (or simlar) data transformations must be done repeatedly. (A one-time data transformation task may be more easily done with [SQLite](https://www.sqlite.org/index.html) or a similar tool.) When deploying/operationalizing `earthmover`, whether with a simple scheduler like [cron](https://en.wikipedia.org/wiki/Cron) or an orchestration tool like [Airflow](https://airflow.apache.org/) or [Dagster](https://dagster.io/), consider
+Typically `earthmover` is used when the same (or similar) data transformations must be done repeatedly. (A one-time data transformation task may be more easily done with [SQLite](https://www.sqlite.org/index.html) or a similar tool.) When deploying/operationalizing `earthmover`, whether with a simple scheduler like [cron](https://en.wikipedia.org/wiki/Cron) or an orchestration tool like [Airflow](https://airflow.apache.org/) or [Dagster](https://dagster.io/), consider
 * specifying conditions you `expect` your [sources](#sources) to meet, so `earthmover` will fail on source data errors
 * specifying `config` &raquo; `log_level: INFO` and monitoring logs for phrases like
   > `distinct_rows` operation removed NN duplicate rows
 
   > `filter_rows` operation removed NN rows
```

## Comparing `earthmover-0.2.1.dist-info/RECORD` & `earthmover-0.2.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-earthmover/VERSION.txt,sha256=GWZm1qfrRYP7nLHhWZcQELLim1t1Kqc_RW4OIGG2Ql8,5
+earthmover/VERSION.txt,sha256=yQ34TPijI3G2D_9VaJi-yv9jQDbp5YZSBMGHlXhDWEc,5
 earthmover/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 earthmover/__main__.py,sha256=h149nOOjizsBUgljvkym9V6UtPB-PFLKz9xJMZ-LssY,6377
 earthmover/earthmover.py,sha256=IW1swcDa41VxhR_fP8ozgH9mcvfM-KMLx6Nndjtgc3I,15311
 earthmover/error_handler.py,sha256=st1uD2I1DVghtKtJZisN66CEIgw7qZSrqZPxzQJsnF4,3100
 earthmover/graph.py,sha256=PBcw2imbxrml7VJfvJSh8iNAtGArNS0gR3hnIcVIwSE,9310
 earthmover/node.py,sha256=238R35PJ93hRSRsyeLJOhkpOPH6DnMzqEUmKNX2GIHc,6035
 earthmover/runs_file.py,sha256=qb2bPCuXLOkVqW-og8VjaoHSuan8ES7j4qJjRdvnEGY,8374
-earthmover/util.py,sha256=jD2HnbsjxpDMTE1mnURQTOky9ER9AHcKNWnWesZoqrc,3885
+earthmover/util.py,sha256=X0vxaTGY3h3-EZuqXYF8FUoFZ6OurHaFC4SBCI1IS90,3958
 earthmover/yaml_parser.py,sha256=rQbDdiImxiQcNhkz3xH8qxFXSRxqHUAmYjTaF0L66_0,5550
 earthmover/nodes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 earthmover/nodes/destination.py,sha256=OzV7kttVIFHa-cSN3DXBYY9pTb_rtrFeXOxWb3YiE2o,4851
-earthmover/nodes/operation.py,sha256=2JsVM_lHOr-0yUpwvD6_GcbZNAjk3CwJEETsr5dMMSg,3904
+earthmover/nodes/operation.py,sha256=IBMRncWnlA-SwqYoXgEASnKoNwJoQMw648TsPiR2wXU,3963
 earthmover/nodes/source.py,sha256=x3Km3D5BIpVaK238IAOFVcbDMQY_kgp5eGGpv7dbwBc,14481
 earthmover/nodes/transformation.py,sha256=diWeO-nwLQHd5p3IhBiCGNk-Q_jtL24z27_hKFiq-pI,1746
 earthmover/operations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 earthmover/operations/column.py,sha256=thNSuC8_zsaWo8Y6_65-cwv7GY9nt9v-CHVaPtOl4FU,16116
 earthmover/operations/dataframe.py,sha256=JUsXFeUMk5hhEiWrIzxJ_EErnofYyfeqcU_wQW01sNQ,7208
 earthmover/operations/groupby.py,sha256=2rpZ1qoMmRdQMCVsvaW041tIbVRro7fiinPjpKha3z8,9125
-earthmover/operations/row.py,sha256=Qv-_e8JiPl5DzDrrs5co6U_oeoZk8tZ9I9nRegRaqSo,3044
+earthmover/operations/row.py,sha256=zzu7YuLrPihmIT36zGhuUAEW4FlyMAJDKxL2JXnYbxY,4269
 earthmover/tests/earthmover.yaml,sha256=bOKpY_PDj9teFo0tABHsouX5BxWv04gnpk0zG_iuC98,6876
 earthmover/tests/expected/animals.jsonl,sha256=-fcwp9JAXBPJ0XzAaF8QV9mF2iagW7O5NizVUkzF6tQ,7571
 earthmover/tests/expected/big_cats.jsonl,sha256=DzBuJyRJ57FJHnC0DqkV7nh3xwOAtQtCcs-OfR70_FA,434
-earthmover/tests/expected/species_count_by_zoo.jsonl,sha256=qrH1-B-_93abquxL5eSo6b1yJnBBJjdUwrSiWmxEVU8,406
+earthmover/tests/expected/species_count_by_zoo.jsonl,sha256=VSzkVW0xWATkDWajTXgnHGyJKSzefqhnw-fhJoVy_8Y,405
 earthmover/tests/expected/total_of_each_species.jsonl,sha256=hhzJTQSmWRQZtOXT7sOy9vY_Eyk-GjxPg8WSEpbFvDQ,821
 earthmover/tests/expected/zoo_count_by_species.jsonl,sha256=5UCl--EX52_UpOs5LxSyOAwKWmf5b6BF9Xtau1jzyzE,797
 earthmover/tests/expected/zoo_count_by_year_founded.jsonl,sha256=Yq336WQSRJJWTqpAqLO70wk7_zAasjwSgPzmy8-1gAQ,280
 earthmover/tests/outputs/animals.jsonl,sha256=-fcwp9JAXBPJ0XzAaF8QV9mF2iagW7O5NizVUkzF6tQ,7571
 earthmover/tests/outputs/big_cats.jsonl,sha256=DzBuJyRJ57FJHnC0DqkV7nh3xwOAtQtCcs-OfR70_FA,434
 earthmover/tests/outputs/species_count_by_zoo.jsonl,sha256=qrH1-B-_93abquxL5eSo6b1yJnBBJjdUwrSiWmxEVU8,406
 earthmover/tests/outputs/total_of_each_species.jsonl,sha256=hhzJTQSmWRQZtOXT7sOy9vY_Eyk-GjxPg8WSEpbFvDQ,821
 earthmover/tests/outputs/zoo_count_by_species.jsonl,sha256=5UCl--EX52_UpOs5LxSyOAwKWmf5b6BF9Xtau1jzyzE,797
 earthmover/tests/outputs/zoo_count_by_year_founded.jsonl,sha256=Yq336WQSRJJWTqpAqLO70wk7_zAasjwSgPzmy8-1gAQ,280
 earthmover/tests/sources/birds.csv,sha256=U7QTv-b-83BlbYJO7Sb0hLFaXOcRAdqtNhHsfKF21BI,712
 earthmover/tests/sources/fishes.csv,sha256=j35oTgJMihVopB5qmDgskgGJtaA8GDl0SDWums996B4,422
 earthmover/tests/sources/inventories.csv,sha256=5fERQS45u7YSg0fW35QvnHUbYThwYdWW5KDVQoHHRss,156
 earthmover/tests/sources/mammals.csv,sha256=XQmF6jXpphai3ZymStuStf0k8SDlRnKG4CEh6XjmSdY,926
 earthmover/tests/sources/reptiles.csv,sha256=HE5LXBv2zwfS_Ccbx5UFzG-FGwCUAaHGDUoQ949tAtY,478
-earthmover/tests/sources/zoos.csv,sha256=qHchJkWezmCKL7Wu82Mlhhpc9YyB0LqzyGtquS5fYjM,284
+earthmover/tests/sources/zoos.csv,sha256=QLB_NCtmn7Z8TZvl-jhBjQItwSp3uZaXt9kCY70F0_w,282
 earthmover/tests/templates/animal.jsont,sha256=WVANYqoyPAysz2eFjIgftCk9XbN_7bM-Dr1awGSIxwM,215
 earthmover/tests/templates/cats.jsont,sha256=drWhdwDPwv_mDqvYbHJgVRODGkt7iq5yGYQguSmFfTc,184
 earthmover/tests/templates/count.jsont,sha256=CRmgEGZ0PYfyTfT0_bnSZvap9lst8SKUrDBtn51r-fo,93
-earthmover-0.2.1.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
-earthmover-0.2.1.dist-info/METADATA,sha256=nKx-xgEfP4VvkBJyvq7v3NwxBRV0lOW9pFt5C3ZCDGo,47059
-earthmover-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-earthmover-0.2.1.dist-info/dependency_links.txt,sha256=zUjtOVgogWsGh-RNRqXTvs-OUh-L6P7e4OmQNBt6iWU,135
-earthmover-0.2.1.dist-info/entry_points.txt,sha256=3Tx8TE2CCFvNikmltqOCkCLlLmlf3x7P51PxpNrPOOQ,56
-earthmover-0.2.1.dist-info/top_level.txt,sha256=M55nBRq8JtBFEJcnqz1GpG8EtnXFHeWJ38QIFp0N26Q,11
-earthmover-0.2.1.dist-info/RECORD,,
+earthmover-0.2.2.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
+earthmover-0.2.2.dist-info/METADATA,sha256=9bifSy1FDAR1YOHNi9EltOXw8qmg9PH-Qn8NRfySAV8,47358
+earthmover-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+earthmover-0.2.2.dist-info/dependency_links.txt,sha256=zUjtOVgogWsGh-RNRqXTvs-OUh-L6P7e4OmQNBt6iWU,135
+earthmover-0.2.2.dist-info/entry_points.txt,sha256=3Tx8TE2CCFvNikmltqOCkCLlLmlf3x7P51PxpNrPOOQ,56
+earthmover-0.2.2.dist-info/top_level.txt,sha256=M55nBRq8JtBFEJcnqz1GpG8EtnXFHeWJ38QIFp0N26Q,11
+earthmover-0.2.2.dist-info/RECORD,,
```

