# Comparing `tmp/scinumtools-2.8.0.tar.gz` & `tmp/scinumtools-2.9.0.tar.gz`

## Comparing `scinumtools-2.8.0.tar` & `scinumtools-2.9.0.tar`

### file list

```diff
@@ -1,197 +1,198 @@
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 scinumtools-2.8.0/build_doc.sh
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 scinumtools-2.8.0/build_tables.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-2.8.0/requirements.txt
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 scinumtools-2.8.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-2.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-2.8.0/.github/workflows/static.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/conf.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/index.rst
--rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_plots/logarithmic_conversions.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_plots/logarithmic_conversions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/empty.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/unit_prefixes.csv
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/css/sphinxdoc.css
--rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/figures/operation_flow.drawio
--rw-r--r--   0        0        0    54464 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/figures/operation_flow.png
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_128.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_16.png
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_20.png
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_24.png
--rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_256.png
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_32.png
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_48.png
--rw-r--r--   0        0        0    41693 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_512.png
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/logo/dip_logo_64.png
--rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt.svg
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_128.png
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_16.png
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_24.png
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_256.png
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_32.png
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_48.png
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_512.png
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/snt/snt_64.png
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/constants.csv
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/prefixes.csv
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/quantities_au.csv
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/quantities_cgs.csv
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/quantities_si.csv
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/unit_base.csv
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/unit_logarithmic.csv
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/unit_standard.csv
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/_static/tables/unit_temperature.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/__init__.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/index.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/intro.rst
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax.rst
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/intro/about.rst
--rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/intro/example.rst
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/dipdocs.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/doc_definitions.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/doc_docstest.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/doc_nodes.rst
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/schema_highliter.rst
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/sphinx/syntax_highliter.rst
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/conditions.rst
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/expressions.rst
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/functions.rst
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/nodes.rst
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/references.rst
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/units.rst
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/validation.rst
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/dip/syntax/values.rst
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/misc/cached_function.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/misc/image_thumbnails.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/misc/index.rst
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/solver/index.rst
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/units/conversions.rst
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/units/index.rst
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/units/other.rst
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/units/quantities.rst
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scinumtools-2.8.0/docs/source/units/tables.rst
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/cached_function.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/data_combination.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/data_plot_grid.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/normalize_data.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/parameter_table.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/progress_bar.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/row_collector.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/stopwatch.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/thumbnail_image.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/__init__.py
--rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/dip.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/environment.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/source.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_boolean.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_float.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_integer.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_number.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_string.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/docs/__init__.py
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/docs/sphinx_docs.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node.py
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_base.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_boolean.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_case.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_condition.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_constant.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_empty.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_float.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_format.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_group.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_import.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_integer.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_mod.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_option.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_select.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_source.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_string.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_table.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/node_unit.py
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/nodes/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/pygments/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/pygments/schema_lexer.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/pygments/style_lexer.py
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/pygments/syntax_lexer.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/settings/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/solvers/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/solvers/function_solver.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/solvers/logical_solver.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/solvers/numerical_solver.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/dip/solvers/template_solver.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/atom.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/expression.py
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/operators.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/solver.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/solver/tokens.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/__init__.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/base_units.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/constant.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/dimensions.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/fraction.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/magnitude.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/nan.py
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/quantity.py
--rw-r--r--   0        0        0    25687 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/settings.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/unit.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/unit_environment.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/unit_list.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/unit_solver.py
--rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 scinumtools-2.8.0/src/scinumtools/units/unit_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_cached_function.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_data_combination.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_data_plot_grid.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_normalize_data.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_parameter_table.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_progress_bar.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_row_collector.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_stopwatch.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/test_thumbnail_image.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_blocks.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_conditions.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_examples.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_expressions.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_finalizing.py
--rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_references.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_solver_logical.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_solver_numerical.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_solver_templates.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_types.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/test_validation.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/blocks/matrix.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/blocks/nodes.dip
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/blocks/query.dip
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/blocks/table.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/blocks/text.txt
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/definitions.dip
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/docstest.dip
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/processed.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/settings.dip
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/settings2.dip
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/dip/examples/template.txt
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/solver/test_customisation.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/solver/test_operations.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_baseunits.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_benchmark.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_decimal.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_dimensions.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_fractions.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_list.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_magnitude.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_numpy.py
--rw-r--r--   0        0        0    12625 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_quantity.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 scinumtools-2.8.0/tests/units/test_solver.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 scinumtools-2.8.0/.gitignore
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 scinumtools-2.8.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 scinumtools-2.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 scinumtools-2.9.0/build_doc.sh
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 scinumtools-2.9.0/build_tables.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-2.9.0/requirements.txt
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 scinumtools-2.9.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-2.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 scinumtools-2.9.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_plots/logarithmic_conversions.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_plots/logarithmic_conversions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/unit_prefixes.csv
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/css/sphinxdoc.css
+-rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/figures/operation_flow.drawio
+-rw-r--r--   0        0        0    54464 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/figures/operation_flow.png
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_128.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_16.png
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_20.png
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_24.png
+-rw-r--r--   0        0        0    18911 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_256.png
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_32.png
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_48.png
+-rw-r--r--   0        0        0    41693 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_512.png
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/logo/dip_logo_64.png
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt.svg
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_128.png
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_16.png
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_24.png
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_256.png
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_32.png
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_48.png
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_512.png
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/snt/snt_64.png
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/constants.csv
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/prefixes.csv
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/quantities_au.csv
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/quantities_cgs.csv
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/quantities_si.csv
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/unit_base.csv
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/unit_logarithmic.csv
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/unit_standard.csv
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/_static/tables/unit_temperature.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/__init__.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/index.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/intro.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax.rst
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/intro/about.rst
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/intro/example.rst
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/dipdocs.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/doc_definitions.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/doc_docstest.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/doc_nodes.rst
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/schema_highliter.rst
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/sphinx/syntax_highliter.rst
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/conditions.rst
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/expressions.rst
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/functions.rst
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/nodes.rst
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/references.rst
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/units.rst
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/validation.rst
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/dip/syntax/values.rst
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/misc/cached_function.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/misc/image_thumbnails.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/misc/index.rst
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/solver/index.rst
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/units/conversions.rst
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/units/index.rst
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/units/other.rst
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/units/quantities.rst
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 scinumtools-2.9.0/docs/source/units/tables.rst
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/cached_function.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/data_combination.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/data_plot_grid.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/normalize_data.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/parameter_table.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/progress_bar.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/row_collector.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/stopwatch.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/thumbnail_image.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/__init__.py
+-rw-r--r--   0        0        0    10542 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/dip.py
+-rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/environment.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/settings.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/source.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_boolean.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_float.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_integer.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_number.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_string.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/docs/__init__.py
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/docs/sphinx_docs.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node.py
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_base.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_boolean.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_case.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_condition.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_constant.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_empty.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_float.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_format.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_group.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_import.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_integer.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_mod.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_option.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_select.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_source.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_string.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_table.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_tags.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/node_unit.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/nodes/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/pygments/__init__.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/pygments/schema_lexer.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/pygments/style_lexer.py
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/pygments/syntax_lexer.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/solvers/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/solvers/function_solver.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/solvers/logical_solver.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/solvers/numerical_solver.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/dip/solvers/template_solver.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/atom.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/expression.py
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/operators.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/solver.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/solver/tokens.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/__init__.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/base_units.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/constant.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/dimensions.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/fraction.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/magnitude.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/nan.py
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/quantity.py
+-rw-r--r--   0        0        0    25687 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/settings.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/unit.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/unit_environment.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/unit_list.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/unit_solver.py
+-rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 scinumtools-2.9.0/src/scinumtools/units/unit_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_cached_function.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_data_combination.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_data_plot_grid.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_normalize_data.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_parameter_table.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_progress_bar.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_row_collector.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_stopwatch.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/test_thumbnail_image.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_blocks.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_conditions.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_examples.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_expressions.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_finalizing.py
+-rw-r--r--   0        0        0     8331 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_references.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_solver_logical.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_solver_numerical.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_solver_templates.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_types.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/test_validation.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/blocks/matrix.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/blocks/nodes.dip
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/blocks/query.dip
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/blocks/table.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/blocks/text.txt
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/definitions.dip
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/docstest.dip
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/processed.txt
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/settings.dip
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/settings2.dip
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/dip/examples/template.txt
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/solver/test_customisation.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/solver/test_operations.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_baseunits.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_benchmark.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_decimal.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_dimensions.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_fractions.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_list.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_magnitude.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_numpy.py
+-rw-r--r--   0        0        0    12625 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_quantity.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 scinumtools-2.9.0/tests/units/test_solver.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 scinumtools-2.9.0/.gitignore
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 scinumtools-2.9.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 scinumtools-2.9.0/PKG-INFO
```

### Comparing `scinumtools-2.8.0/build_tables.py` & `scinumtools-2.9.0/build_tables.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/.github/workflows/python-publish.yml` & `scinumtools-2.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/.github/workflows/static.yml` & `scinumtools-2.9.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/Makefile` & `scinumtools-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/make.bat` & `scinumtools-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/conf.py` & `scinumtools-2.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/index.rst` & `scinumtools-2.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_plots/logarithmic_conversions.png` & `scinumtools-2.9.0/docs/source/_plots/logarithmic_conversions.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_plots/logarithmic_conversions.py` & `scinumtools-2.9.0/docs/source/_plots/logarithmic_conversions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/figures/operation_flow.drawio` & `scinumtools-2.9.0/docs/source/_static/figures/operation_flow.drawio`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/figures/operation_flow.png` & `scinumtools-2.9.0/docs/source/_static/figures/operation_flow.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_128.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_128.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_16.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_16.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_20.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_20.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_24.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_24.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_256.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_256.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_32.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_32.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_48.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_48.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_512.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_512.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/logo/dip_logo_64.png` & `scinumtools-2.9.0/docs/source/_static/logo/dip_logo_64.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt.svg` & `scinumtools-2.9.0/docs/source/_static/snt/snt.svg`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_128.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_128.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_16.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_16.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_24.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_24.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_256.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_256.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_32.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_32.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_48.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_48.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_512.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_512.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/snt/snt_64.png` & `scinumtools-2.9.0/docs/source/_static/snt/snt_64.png`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/tables/constants.csv` & `scinumtools-2.9.0/docs/source/_static/tables/constants.csv`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/tables/quantities_au.csv` & `scinumtools-2.9.0/docs/source/_static/tables/quantities_au.csv`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/tables/quantities_si.csv` & `scinumtools-2.9.0/docs/source/_static/tables/quantities_si.csv`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/_static/tables/unit_standard.csv` & `scinumtools-2.9.0/docs/source/_static/tables/unit_standard.csv`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/index.rst` & `scinumtools-2.9.0/docs/source/dip/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/intro/about.rst` & `scinumtools-2.9.0/docs/source/dip/intro/about.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/intro/example.rst` & `scinumtools-2.9.0/docs/source/dip/intro/example.rst`

 * *Files 6% similar despite different names*

```diff
@@ -60,19 +60,26 @@
 Getting parsed data
 -------------------
        
 Particular nodes can be selected using :doc:`references <../syntax/references>`.
 
 .. code-block:: python
        
-   nodes = env2.query("mpi.*")            # select nodes using a query method
-   geom = env2.request("?box.geometry")   # select a node using a request method
+   nodes = env2.query("mpi.*")                       # select nodes using a query method
+   nodes = env2.query("runtime.*", tags=['step'])    # refine selection using tags
+   geom = env2.request("?box.geometry")              # select a node using a request method
+   geom = env2.request("?runtime.*", tags=['step'])  # refine selection using tags
 
 In the example above, variable ``nodes`` is a list of two nodes: ``mpi.nodes`` and ``mpi.cores``.
 The variable ``geom`` is a list with only one node ``box.geometry`` that was loaded from a file ``settings.dip``.
+Additionally one can select nodes according to their tags.
+
+.. code-block:: 
+
+   nodes = env2.query("mpi.*", tags=['step'])
 
 All environmental data can be parsed as a dictionary.
 
 .. code-block::
 
    # Values are returned as Python datatypes
    data = env2.data()
@@ -130,14 +137,21 @@
    #     'box.geometry':      IntegerType(3),
    #     'box.size.x':        FloatType(10, 'nm'),
    #     'box.size.y':        FloatType(3e7, 'nm'),
    #     'modules.heating':   BooleanType(False),
    #     'modules.radiation': BooleanType(True),
    # }
    
+Besides specifying output format, it is also possible to select specific nodes using ``query`` or ``tag`` selectors:
+
+.. code-block::
+
+   env2.data(query="mpi.*")                # selects all nodes in the mpi group
+   env2.data(tags=['step'])                # selects all nodes with corresponding tags
+   env2.data(query="mpi.*", tags=['step']) # combination of a query and tag selectors
 
 Definitions
 -----------
 
 Often code users can modify initial settings in order to choose functionality of a code to what they currently need.
 DIP gives code developers a tool to manage such input parameter lists and control what parameters are compulsory or mandatory and what is their format.
 In the following example, we first create a definition file with description of all input parameter of a fictional numerical code:
```

### Comparing `scinumtools-2.8.0/docs/source/dip/sphinx/dipdocs.rst` & `scinumtools-2.9.0/docs/source/dip/sphinx/dipdocs.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/sphinx/schema_highliter.rst` & `scinumtools-2.9.0/docs/source/dip/sphinx/schema_highliter.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/sphinx/syntax_highliter.rst` & `scinumtools-2.9.0/docs/source/dip/sphinx/syntax_highliter.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/conditions.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/conditions.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/expressions.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/expressions.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/functions.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/functions.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/nodes.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/nodes.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/references.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/references.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/units.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/units.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/validation.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/validation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -76,27 +76,27 @@
    # all options: [23, 45, 10, 234, 490, 1939, 3.4e-6, 2.34e-7] J
 
 Condition
 ---------
 
 Numerical values can usually have values ranging in some intervals.
 In order to restrict node values to some particular interval, it is possible to set logical using ``!condition`` directive and logical expression.
-A given expression has to be evaluated as `true` after each definition or modification of a node.
+A given expression has to be evaluated as ``true`` after each definition or modification of a node.
 
 .. code-block:: DIPSchema
    :caption: Schema of a node condition requirement
       
    <indent>!condition ('<expression>')    
    <indent>!condition ("<expression>")    
    <indent>!condition ("""
    <expression>
    """)                                   
 
-In the example below, node `energy` can have values in a range of 23 and 26 erg.
-The actual value of node `energy` is matched using a special self-reference sign ``{?}``.
+In the example below, node ``energy`` can have values in a range of 23 and 26 erg.
+The actual value of node ``energy`` is matched using a special self-reference sign ``{?}``.
 
 .. code-block:: DIP
 
    energy float = 25 erg
      !condition ("23 < {?} && {?} < 26")
 
 Format
@@ -124,15 +124,46 @@
 This can be achieved by a directive ``!constant``.
 
 .. code-block:: DIPSchema
    :caption: Schema of a constant node requirement
 
    <indent>!constant
 
-Node `name` in the following example cannot be further modified.
+Node ``name`` in the following example cannot be further modified.
      
 .. code-block:: DIP
 
    name str = 'John'
      !constant
 
    name = 'Mary'   # this modification will raise an error exception
+
+Tags
+----
+
+Tags have proven to be a good way how to sort and categorize large number of information.
+Boolean, integer, float and string nodes support tagging using a dedicated property ``!tags`` that accept a list of tags.
+It is advised to use only string tags.
+
+.. code-block:: DIPSchema
+   :caption: Schema for node tags property
+   
+   <indent>!tags <value>
+   
+Tagged nodes can be later on selected from environment using a tag selector.
+
+.. code-block:: 
+
+   >>> with DIP() as p:
+   >>>     p.from_string('''
+   >>>     name str = John
+   >>>         !tags ["name","male"]
+   >>>     age int = 34
+   >>>     ''')
+   >>>     env = p.parse()
+   >>> env.query("*", tags=['male'])
+   [StringNode(John)]
+   >>> env.data(tags=['male'])
+   {'name': StringType('John')}
+   
+
+
```

### Comparing `scinumtools-2.8.0/docs/source/dip/syntax/values.rst` & `scinumtools-2.9.0/docs/source/dip/syntax/values.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/misc/image_thumbnails.rst` & `scinumtools-2.9.0/docs/source/misc/image_thumbnails.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/solver/index.rst` & `scinumtools-2.9.0/docs/source/solver/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/units/conversions.rst` & `scinumtools-2.9.0/docs/source/units/conversions.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/units/index.rst` & `scinumtools-2.9.0/docs/source/units/index.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/units/other.rst` & `scinumtools-2.9.0/docs/source/units/other.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/units/quantities.rst` & `scinumtools-2.9.0/docs/source/units/quantities.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/docs/source/units/tables.rst` & `scinumtools-2.9.0/docs/source/units/tables.rst`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/__init__.py` & `scinumtools-2.9.0/src/scinumtools/__init__.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/cached_function.py` & `scinumtools-2.9.0/src/scinumtools/cached_function.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/data_combination.py` & `scinumtools-2.9.0/src/scinumtools/data_combination.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/data_plot_grid.py` & `scinumtools-2.9.0/src/scinumtools/data_plot_grid.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/normalize_data.py` & `scinumtools-2.9.0/src/scinumtools/normalize_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/parameter_table.py` & `scinumtools-2.9.0/src/scinumtools/parameter_table.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/progress_bar.py` & `scinumtools-2.9.0/src/scinumtools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/row_collector.py` & `scinumtools-2.9.0/src/scinumtools/row_collector.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/stopwatch.py` & `scinumtools-2.9.0/src/scinumtools/stopwatch.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/thumbnail_image.py` & `scinumtools-2.9.0/src/scinumtools/thumbnail_image.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/dip.py` & `scinumtools-2.9.0/src/scinumtools/dip/dip.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from inspect import getframeinfo, stack
 
 from .environment import Environment
 from .source import Source
 from .settings import Keyword, Sign
 from .nodes.parser import Parser
 from .nodes import EmptyNode, ImportNode, UnitNode, SourceNode, CaseNode
-from .nodes import OptionNode, ConstantNode, FormatNode, ConditionNode
+from .nodes import OptionNode, ConstantNode, FormatNode, ConditionNode, TagsNode
 from .nodes import ModNode, GroupNode
 from .nodes import BooleanNode, IntegerNode, FloatNode, StringNode, TableNode
 from .solvers import LogicalSolver
 from .datatypes import Type
 
 class DIP:
     """ DIP parser class
@@ -138,15 +138,15 @@
                 parsed = node.parse(self.env)
                 if parsed: 
                     # Add parsed nodes to the queue and continue
                     env.prepend_nodes(parsed)
                     continue
             # Create hierarchical name
             excluded = ['empty','unit','source',
-                        'option','constant','format','condition']
+                        'option','constant','format','condition','tags']
             self.env.update_hierarchy(node, excluded)
             # Add nodes to the list
             excluded += ['group']
             if node.keyword in excluded:
                 continue
             elif node.keyword=='case':   # Parse cases
                 self.env.solve_case(node)
@@ -212,14 +212,15 @@
             ImportNode.is_node,           # parse root import directive
             UnitNode.is_node,             # parse unit directive
             SourceNode.is_node,           # parse source directive
             CaseNode.is_node,             # parse case directive
             OptionNode.is_node,           # parse option setting
             ConstantNode.is_node,         # parse constant setting
             FormatNode.is_node,           # parse format setting
+            TagsNode.is_node,             # parse node tags
             ConditionNode.is_node,        # parse condition setting
             parser.part_name,             
             GroupNode.is_node,            # parse group node
             ImportNode.is_node,           # parse group import directive
             ModNode.is_node,              # parse modification
             parser.part_type,             
             BooleanNode.is_node,          # parse boolean node
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/environment.py` & `scinumtools-2.9.0/src/scinumtools/dip/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,36 +134,43 @@
         :param source: Source can be either a DIP object or a text
         :param str path: Source path
         """
         if name in self.sources:
             raise Exception("Reference source alread exists:", name)
         self.sources[name] = EnvSource(source=source, path=str(path), name=name)
         
-    def query(self, query:str, namespace:int=Namespace.NODES):
+    def query(self, query:str, namespace:int=Namespace.NODES, tags:list=None):
         """ Select local nodes according to a query
 
         :param str query: Node selection query
         :param str namespace: Query namespace (nodes, sources, or units)
+        :param list tags: List of tags
         """
         if namespace==Namespace.NODES:
             nodes = []
             if query==Sign.WILDCARD:
-                return [node.copy() for node in self.nodes]
+                nodes = [node.copy() for node in self.nodes]
             elif query[-2:]==Sign.SEPARATOR + Sign.WILDCARD:
                 for node in self.nodes:
                     if node.name.startswith(query[:-1]):
                         node = node.copy()
                         node.name = node.name[len(query[:-1]):]
                         nodes.append(node.copy())
             else:
                 for node in self.nodes:
                     if node.name==query:
                         node = node.copy()
                         node.name = node.name.split(Sign.SEPARATOR)[-1]
                         nodes.append(node.copy())
+            if tags:
+                tagged = []
+                for n in range(len(nodes)):
+                    if nodes[n].tags and np.in1d(tags, nodes[n].tags):
+                        tagged.append(nodes[n])
+                nodes = tagged
             return nodes
         elif namespace==Namespace.SOURCES:
             if query==Sign.WILDCARD:   # return all sources
                 return self.sources
             else:                     # return particular source
                 if query not in self.sources:
                     raise Exception("Requested source does not exists:", query)
@@ -174,52 +181,61 @@
             else:                     # return particular unit
                 if query not in self.units:
                     raise Exception("Requested unit does not exists:", query)
                 return {query: self.units[query]}
         else:
             raise Exception("Invalid query namespace selected:", namespace)
         
-    def request(self, path:str, count:int=None, namespace:str=Namespace.NODES):
+    def request(self, path:str, count:int=None, namespace:str=Namespace.NODES, tags:list=None):
         """ Request nodes from a path
 
         :param str path: Request path
         :param int count: Number of nodes that should be selected
         :param str namespace: Query namespace (nodes, sources, or units)
+        :param list tags: List of tags
         """
         if self.autoref and path == Sign.QUERY: # reference type {?}
             filename,query = '', self.autoref
         elif Sign.QUERY in path:                    # reference type {source?query}
             filename,query = path.split(Sign.QUERY)
         else:                                      # reference type {source}
             filename,query = path,Sign.WILDCARD
         if filename:  # use external source to parse the values
             source = self.sources[filename].source
             if isinstance(source, str):
                 return source
             else:
-                nodes = source.env.query(query, namespace)
+                nodes = source.env.query(query, namespace, tags=tags)
         else:         # use values parsed in the current file
             if not self.nodes:
                 raise Exception(f"Local nodes are not available for DIP import:", path)
-            nodes = self.query(query, namespace)
+            nodes = self.query(query, namespace, tags=tags)
         if count:
             if isinstance(count, list) and len(nodes) not in count:
                 raise Exception(f"Path returned invalid number of nodes:", path, count, len(nodes))
             elif np.isscalar(count) and len(nodes)!=count:
                 raise Exception(f"Path returned invalid number of nodes:", path, count, len(nodes))
         return nodes
 
-    def data(self, format=Format.VALUE, verbose=False):
+    def data(self, format:Format=Format.VALUE, verbose:bool=False, query:str=None, tags:list=None):
         """ Return parsed values as a dictionary
 
         :param bool verbose: Display node values
         :param str format: Return data as values only, DIP datatypes, or tuples
+        :param str query: Node selection query
+        :param list tags: List of tags
         """
         data = {}
-        for node in self.nodes:
+        if query is not None:
+            nodes = self.query(query, tags=tags)
+        elif tags is not None:
+            nodes = self.query("*", tags=tags)
+        else:
+            nodes = self.nodes
+        for node in nodes:
             if format==Format.VALUE:
                 data[node.name] = node.value.value
             elif format==Format.TYPE:
                 data[node.name] = node.value
             elif format==Format.TUPLE:
                 if isinstance(node.value, NumberType) and node.value.unit is not None:
                     data[node.name] = (node.value.value, node.value.unit)
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_boolean.py` & `scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_boolean.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_float.py` & `scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_float.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_integer.py` & `scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_integer.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/datatypes/type_number.py` & `scinumtools-2.9.0/src/scinumtools/dip/datatypes/type_number.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/docs/sphinx_docs.py` & `scinumtools-2.9.0/src/scinumtools/dip/docs/sphinx_docs.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/__init__.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 from .node_import import ImportNode
 from .node_mod import ModNode
 from .node_boolean import BooleanNode
 from .node_integer import IntegerNode
 from .node_float import FloatNode
 from .node_string import StringNode
 from .node_table import TableNode
+from .node_tags import TagsNode
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_base.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,26 @@
                 kwargs['keyword'] = parser.keyword
             if parser.value_fn:
                 kwargs['value_fn'] = parser.value_fn
             if parser.value_expr:
                 kwargs['value_expr'] = parser.value_expr
         super().__init__(*args, **kwargs)
     
+    def __str__(self):
+        if self.value.unit:
+            return f"{self.__class__.__name__}({self.value.value} {self.value.unit})"
+        else:
+            return f"{self.__class__.__name__}({self.value.value})"
+    
+    def __repr__(self):
+        if self.value.unit:
+            return f"{self.__class__.__name__}({self.value.value} {self.value.unit})"
+        else:
+            return f"{self.__class__.__name__}({self.value.value})"
+
     def parse(self, env):
         return False
 
     def cast_value(self, value=None):
         """ Cast (raw-)value as a datatype self, or another node
         """
         if not value:
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_boolean.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_boolean.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .node_base import BaseNode
 from ..solvers import LogicalSolver, FunctionSolver
 from ..datatypes import BooleanType
 
 class BooleanNode(BaseNode):
     keyword: str = 'bool'
     value: bool = None
+    tags: list = None
     dtype = bool
 
     @staticmethod
     def is_node(parser):
         if parser.keyword=='bool':
              parser.part_dimension()
              parser.part_equal()
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_case.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_case.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_float.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_float.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..datatypes import FloatType, IntegerType
 
 class FloatNode(BaseNode, SelectNode):
     keyword: str = 'float'
     value: float = None
     options: List = None
     value_expr: str = False
+    tags: list = None
     dtype = float
     bits = 64
 
     def __init__(self, *args, **kwargs):
         self.options = []
         super().__init__(*args, **kwargs)
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_format.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_format.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_import.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_import.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_integer.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_integer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..solvers import NumericalSolver, FunctionSolver
 
 class IntegerNode(BaseNode, SelectNode):
     keyword: str = 'int'
     value: int = None
     options: List = None
     value_expr: str = False
+    tags: list = None
     dtype = int
     bits = 32
 
     def __init__(self, *args, **kwargs):
         self.options = []
         super().__init__(*args, **kwargs)
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_option.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_option.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_select.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_select.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_source.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_source.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_string.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_string.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .node_select import SelectNode
 from ..solvers import TemplateSolver, FunctionSolver
 from ..datatypes import StringType
 
 class StringNode(BaseNode, SelectNode):
     keyword: str = 'str'
     format: str = None
+    tags: list = None
 
     @staticmethod
     def is_node(parser):
         if parser.keyword=='str':
              parser.part_dimension()
              parser.part_equal()
              if parser.is_parsed('part_equal'): # definition
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_table.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_table.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/node_unit.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/node_unit.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/nodes/parser.py` & `scinumtools-2.9.0/src/scinumtools/dip/nodes/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,23 @@
             r'^(('+re.escape(Sign.VALIDATION)+Keyword.FORMAT+r')\s*)',
             self.ccode
         )
         if m:
             self.parsed.append('kwd_format')
             self._strip(m.group(1))
             
+    def kwd_tags(self):
+        m=re.match(
+            r'^(('+re.escape(Sign.VALIDATION)+Keyword.TAGS+r')\s*)',
+            self.ccode
+        )
+        if m:
+            self.parsed.append('kwd_tags')
+            self._strip(m.group(1))
+            
     def kwd_condition(self):
         m=re.match(
             r'^(('+re.escape(Sign.VALIDATION)+Keyword.CONDITION+r')\s*)',
             self.ccode
         )
         if m:
             self.parsed.append('kwd_condition')
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/pygments/schema_lexer.py` & `scinumtools-2.9.0/src/scinumtools/dip/pygments/schema_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             (r'(\()("""\n|"|\')(<expression>)(\n"""|"|\')(\))',
               bygroups(Token.Text, Token.Expression, Token.Expression,
                        Token.Expression, Token.Text)),
             (r'(\()(<function>)(\))',
               bygroups(Token.Text, Token.Expression,  Token.Text)),
             (r'<[^ ]',        Token.Name.Tag, 'tag'),
             (r'{',            Token.Reference, 'reference'),
-            (r'!(options|format|condition|constant)',  Token.Keyword),
+            (r'!(options|format|condition|constant|tags)',  Token.Keyword),
             (r'\$(source|unit)',     Token.Keyword),
             (r'\@(case|else|end)',     Token.Keyword),
             (r'( |=|<|>|\.\*|\*)',    Token.Text),
             (r'#[^\n]*',  Token.Comment),
             (r'[ ]*\n',   Token.Text), 
         ],
         'tag': [
```

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/pygments/style_lexer.py` & `scinumtools-2.9.0/src/scinumtools/dip/pygments/style_lexer.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/pygments/syntax_lexer.py` & `scinumtools-2.9.0/src/scinumtools/dip/pygments/syntax_lexer.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/solvers/function_solver.py` & `scinumtools-2.9.0/src/scinumtools/dip/solvers/function_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/solvers/logical_solver.py` & `scinumtools-2.9.0/src/scinumtools/dip/solvers/logical_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/solvers/numerical_solver.py` & `scinumtools-2.9.0/src/scinumtools/dip/solvers/numerical_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/dip/solvers/template_solver.py` & `scinumtools-2.9.0/src/scinumtools/dip/solvers/template_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/solver/atom.py` & `scinumtools-2.9.0/src/scinumtools/solver/atom.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/solver/expression.py` & `scinumtools-2.9.0/src/scinumtools/solver/expression.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/solver/operators.py` & `scinumtools-2.9.0/src/scinumtools/solver/operators.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/solver/solver.py` & `scinumtools-2.9.0/src/scinumtools/solver/solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/solver/tokens.py` & `scinumtools-2.9.0/src/scinumtools/solver/tokens.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/base_units.py` & `scinumtools-2.9.0/src/scinumtools/units/base_units.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/constant.py` & `scinumtools-2.9.0/src/scinumtools/units/constant.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/dimensions.py` & `scinumtools-2.9.0/src/scinumtools/units/dimensions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/fraction.py` & `scinumtools-2.9.0/src/scinumtools/units/fraction.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/magnitude.py` & `scinumtools-2.9.0/src/scinumtools/units/magnitude.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/quantity.py` & `scinumtools-2.9.0/src/scinumtools/units/quantity.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/settings.py` & `scinumtools-2.9.0/src/scinumtools/units/settings.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/unit.py` & `scinumtools-2.9.0/src/scinumtools/units/unit.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/unit_environment.py` & `scinumtools-2.9.0/src/scinumtools/units/unit_environment.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/unit_list.py` & `scinumtools-2.9.0/src/scinumtools/units/unit_list.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/unit_solver.py` & `scinumtools-2.9.0/src/scinumtools/units/unit_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/src/scinumtools/units/unit_types.py` & `scinumtools-2.9.0/src/scinumtools/units/unit_types.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_cached_function.py` & `scinumtools-2.9.0/tests/test_cached_function.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_data_combination.py` & `scinumtools-2.9.0/tests/test_data_combination.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_data_plot_grid.py` & `scinumtools-2.9.0/tests/test_data_plot_grid.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_normalize_data.py` & `scinumtools-2.9.0/tests/test_normalize_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_parameter_table.py` & `scinumtools-2.9.0/tests/test_parameter_table.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_row_collector.py` & `scinumtools-2.9.0/tests/test_row_collector.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_stopwatch.py` & `scinumtools-2.9.0/tests/test_stopwatch.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/test_thumbnail_image.py` & `scinumtools-2.9.0/tests/test_thumbnail_image.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_blocks.py` & `scinumtools-2.9.0/tests/dip/test_blocks.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_conditions.py` & `scinumtools-2.9.0/tests/dip/test_conditions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_examples.py` & `scinumtools-2.9.0/tests/dip/test_examples.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,14 +82,58 @@
         'box.geometry':      IntegerType(3),
         'box.size.x':        FloatType(10, 'nm'),
         'box.size.y':        FloatType(3e7, 'nm'),
         'modules.heating':   BooleanType(False),
         'modules.radiation': BooleanType(True),
     })
     
+def test_query_request_tag(test_path):
+    
+    with DIP() as dip:
+        dip.from_string("""
+        mpi
+          nodes int = 36
+          cores int = 96
+        """)                               
+        dip.from_file(test_path+"settings2.dip") 
+        env = dip.parse()               
+    
+    nodes = env.query("mpi.*")
+    assert len(nodes) == 2
+    nodes = env.query("runtime.*", tags=['step'])  
+    assert len(nodes) == 1
+    geom = env.request("?box.geometry") 
+    assert len(nodes) == 1
+    geom = env.request("?runtime.*", tags=['step'])  
+    assert len(nodes) == 1
+
+    
+def test_data_tag(test_path):
+    
+    with DIP() as dip:
+        dip.from_string("""
+        mpi
+          nodes int = 36
+          cores int = 96
+        """)                               
+        dip.from_file(test_path+"settings2.dip") 
+        env = dip.parse()                 # parse the code
+    
+    data = env.data(query="mpi.*")
+    np.testing.assert_equal(data,{
+        'nodes': 36,
+        'cores': 96,
+    })
+    data = env.data(tags=['step'])       
+    np.testing.assert_equal(data,{
+        'runtime.timestep': 0.01,
+    })         
+    data = env.data(query="mpi.*", tags=['step']) 
+    np.testing.assert_equal(data,{})         
+
 
 def test_definition_template(test_path):
     
     with DIP() as dip:
         dip.from_file(test_path+'definitions.dip')
         env3 = dip.parse()
         data = env3.data(format=Format.TYPE)
```

### Comparing `scinumtools-2.8.0/tests/dip/test_expressions.py` & `scinumtools-2.9.0/tests/dip/test_expressions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_finalizing.py` & `scinumtools-2.9.0/tests/dip/test_finalizing.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_references.py` & `scinumtools-2.9.0/tests/dip/test_references.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_solver_logical.py` & `scinumtools-2.9.0/tests/dip/test_solver_logical.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_solver_numerical.py` & `scinumtools-2.9.0/tests/dip/test_solver_numerical.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_solver_templates.py` & `scinumtools-2.9.0/tests/dip/test_solver_templates.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_types.py` & `scinumtools-2.9.0/tests/dip/test_types.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/dip/test_validation.py` & `scinumtools-2.9.0/tests/dip/test_validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -102,7 +102,39 @@
     })
     with pytest.raises(Exception) as e_info:
         parse("""
 size float = 23 cm
   !condition ('250 mm < {?} && {?} < 30 cm')
         """)
     assert e_info.value.args[0] == "Node does not fullfil a condition:"
+
+def test_tags():
+    with DIP() as p:
+        p.from_string('''
+        name str = John
+          !tags ["name","male"]
+        age int = 34
+        ''')
+        env = p.parse()
+
+    nodes = env.query("*", tags=['male'])
+    assert len(nodes)     == 1
+    assert nodes[0].tags  == ['name','male']
+    
+    data = env.data(verbose=True,format=Format.TYPE)
+    np.testing.assert_equal(data,{
+        'name': StringType('John'),
+        'age':  IntegerType(34)
+    })
+    
+    data = env.data(verbose=True,format=Format.TYPE,query="age")
+    np.testing.assert_equal(data,{
+        'age':  IntegerType(34)
+    })
+
+    data = env.data(verbose=True,format=Format.TYPE,query="age",tags=['name'])
+    np.testing.assert_equal(data,{})
+
+    data = env.data(verbose=True,format=Format.TYPE,tags=['name'])
+    np.testing.assert_equal(data,{
+      'name': StringType('John')
+    })
```

### Comparing `scinumtools-2.8.0/tests/dip/examples/definitions.dip` & `scinumtools-2.9.0/tests/dip/examples/definitions.dip`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/solver/test_customisation.py` & `scinumtools-2.9.0/tests/solver/test_customisation.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/solver/test_operations.py` & `scinumtools-2.9.0/tests/solver/test_operations.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_baseunits.py` & `scinumtools-2.9.0/tests/units/test_baseunits.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_benchmark.py` & `scinumtools-2.9.0/tests/units/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_decimal.py` & `scinumtools-2.9.0/tests/units/test_decimal.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_dimensions.py` & `scinumtools-2.9.0/tests/units/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_fractions.py` & `scinumtools-2.9.0/tests/units/test_fractions.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_list.py` & `scinumtools-2.9.0/tests/units/test_list.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_magnitude.py` & `scinumtools-2.9.0/tests/units/test_magnitude.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_numpy.py` & `scinumtools-2.9.0/tests/units/test_numpy.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_quantity.py` & `scinumtools-2.9.0/tests/units/test_quantity.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/tests/units/test_solver.py` & `scinumtools-2.9.0/tests/units/test_solver.py`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/.gitignore` & `scinumtools-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/README.md` & `scinumtools-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `scinumtools-2.8.0/pyproject.toml` & `scinumtools-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "2.8.0"
+version = "2.9.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-2.8.0/PKG-INFO` & `scinumtools-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 2.8.0
+Version: 2.9.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

