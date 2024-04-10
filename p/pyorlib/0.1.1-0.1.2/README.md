# Comparing `tmp/pyorlib-0.1.1.tar.gz` & `tmp/pyorlib-0.1.2.tar.gz`

## Comparing `pyorlib-0.1.1.tar` & `pyorlib-0.1.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pyorlib-0.1.1/CITATION.cff
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/__init__.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/element.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/expressions/__init__.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/expressions/expression.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/__init__.py
--rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/term.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/constants/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/constants/constant.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/variables/__init__.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/algebra/terms/variables/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/constants/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/constants/stdout_colors.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/exceptions/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/exceptions/pyorlib_exception.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/loggers/__init__.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/loggers/logger.py
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/loggers/stdout_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/validators/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/validators/fields/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/core/validators/fields/field_validator.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/engine.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/cplex/__init__.py
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/cplex/cplex_engine.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/gurobi/__init__.py
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/gurobi/gurobi_engine.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/ortools/__init__.py
--rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/ortools/ortools_engine.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/pulp/__init__.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/engines/pulp/pulp_engine.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/optimization_type.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/parameter_type.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/solution_status.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/term_type.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/enums/value_type.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/cplex_exception.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/gurobi_exception.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/model_exception.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/ortools_exception.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/pulp_exception.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/exceptions/term_exception.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/model/__init__.py
--rw-r--r--   0        0        0    20460 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/model/model.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/definitions/__init__.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/definitions/dimension_definition.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/definitions/parameter_definition.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/definitions/term_definition.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/parameters/__init__.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/parameters/multi_value_parameter.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/parameters/parameter.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/structures/parameters/single_value_parameter.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/validators/__init__.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/validators/value_type_validator.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/validators/fields/__init__.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/validators/fields/dimension_field.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 pyorlib-0.1.1/src/pyorlib/validators/fields/parameter_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/__init__.py
--rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/test_element.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/expressions/__init__.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/expressions/test_expression.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/__init__.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/test_term.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/constants/__init__.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/constants/test_constant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/variables/__init__.py
--rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/algebra/terms/variables/test_variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/core/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/core/test_logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/__init__.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/test_cplex.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/test_engine.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/test_gurobi.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/test_or_tools.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/engines/test_pulp.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/fixtures/engine_fixture.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/model/__init__.py
--rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/model/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/structures/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/structures/parameters/__init__.py
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/structures/parameters/test_multi_value_parameter.py
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/structures/parameters/test_single_value_parameter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/validators/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/validators/test_value_type_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/validators/fields/__init__.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/validators/fields/test_dimension_field.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 pyorlib-0.1.1/tests/validators/fields/test_parameter_field.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyorlib-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyorlib-0.1.1/LICENSE
--rw-r--r--   0        0        0    27518 2020-02-02 00:00:00.000000 pyorlib-0.1.1/README.md
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 pyorlib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 pyorlib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pyorlib-0.1.2/CITATION.cff
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/__init__.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/element.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/expressions/__init__.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/expressions/expression.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/__init__.py
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/term.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/constants/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/constants/constant.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/variables/__init__.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/algebra/terms/variables/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/constants/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/constants/stdout_colors.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/exceptions/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/exceptions/pyorlib_exception.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/loggers/__init__.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/loggers/logger.py
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/loggers/stdout_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/validators/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/validators/fields/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/core/validators/fields/field_validator.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/engine.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/cplex/__init__.py
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/cplex/cplex_engine.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/gurobi/__init__.py
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/gurobi/gurobi_engine.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/ortools/__init__.py
+-rw-r--r--   0        0        0     8326 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/ortools/ortools_engine.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/pulp/__init__.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/engines/pulp/pulp_engine.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/optimization_type.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/parameter_type.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/solution_status.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/term_type.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/enums/value_type.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/cplex_exception.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/gurobi_exception.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/model_exception.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/ortools_exception.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/pulp_exception.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/exceptions/term_exception.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/model/__init__.py
+-rw-r--r--   0        0        0    20460 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/model/model.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/definitions/__init__.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/definitions/dimension_definition.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/definitions/parameter_definition.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/definitions/term_definition.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/parameters/__init__.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/parameters/multi_value_parameter.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/parameters/parameter.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/structures/parameters/single_value_parameter.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/validators/__init__.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/validators/value_type_validator.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/validators/fields/__init__.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/validators/fields/dimension_field.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 pyorlib-0.1.2/src/pyorlib/validators/fields/parameter_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/__init__.py
+-rw-r--r--   0        0        0    12192 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/test_element.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/expressions/__init__.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/expressions/test_expression.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/__init__.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/test_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/constants/__init__.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/constants/test_constant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/variables/__init__.py
+-rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/algebra/terms/variables/test_variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/core/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/core/test_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/__init__.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/test_cplex.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/test_engine.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/test_gurobi.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/test_or_tools.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/engines/test_pulp.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/fixtures/engine_fixture.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/model/__init__.py
+-rw-r--r--   0        0        0    18553 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/model/test_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/structures/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/structures/parameters/__init__.py
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/structures/parameters/test_multi_value_parameter.py
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/structures/parameters/test_single_value_parameter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/validators/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/validators/test_value_type_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/validators/fields/__init__.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/validators/fields/test_dimension_field.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 pyorlib-0.1.2/tests/validators/fields/test_parameter_field.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pyorlib-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pyorlib-0.1.2/LICENSE
+-rw-r--r--   0        0        0    27518 2020-02-02 00:00:00.000000 pyorlib-0.1.2/README.md
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 pyorlib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    30276 2020-02-02 00:00:00.000000 pyorlib-0.1.2/PKG-INFO
```

### Comparing `pyorlib-0.1.1/CITATION.cff` & `pyorlib-0.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/algebra/element.py` & `pyorlib-0.1.2/src/pyorlib/algebra/element.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/algebra/expressions/expression.py` & `pyorlib-0.1.2/src/pyorlib/algebra/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/algebra/terms/term.py` & `pyorlib-0.1.2/src/pyorlib/algebra/terms/term.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/algebra/terms/constants/constant.py` & `pyorlib-0.1.2/src/pyorlib/algebra/terms/constants/constant.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/algebra/terms/variables/variable.py` & `pyorlib-0.1.2/src/pyorlib/algebra/terms/variables/variable.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/core/constants/stdout_colors.py` & `pyorlib-0.1.2/src/pyorlib/core/constants/stdout_colors.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/core/exceptions/pyorlib_exception.py` & `pyorlib-0.1.2/src/pyorlib/core/exceptions/pyorlib_exception.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/core/loggers/logger.py` & `pyorlib-0.1.2/src/pyorlib/core/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/core/loggers/stdout_logger.py` & `pyorlib-0.1.2/src/pyorlib/core/loggers/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/core/validators/fields/field_validator.py` & `pyorlib-0.1.2/src/pyorlib/core/validators/fields/field_validator.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/engines/engine.py` & `pyorlib-0.1.2/src/pyorlib/engines/engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/engines/cplex/cplex_engine.py` & `pyorlib-0.1.2/src/pyorlib/engines/cplex/cplex_engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/engines/gurobi/gurobi_engine.py` & `pyorlib-0.1.2/src/pyorlib/engines/gurobi/gurobi_engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/engines/ortools/ortools_engine.py` & `pyorlib-0.1.2/src/pyorlib/engines/ortools/ortools_engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/engines/pulp/pulp_engine.py` & `pyorlib-0.1.2/src/pyorlib/engines/pulp/pulp_engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/enums/parameter_type.py` & `pyorlib-0.1.2/src/pyorlib/enums/parameter_type.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/enums/solution_status.py` & `pyorlib-0.1.2/src/pyorlib/enums/solution_status.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/enums/value_type.py` & `pyorlib-0.1.2/src/pyorlib/enums/value_type.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/model/model.py` & `pyorlib-0.1.2/src/pyorlib/model/model.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/definitions/__init__.py` & `pyorlib-0.1.2/src/pyorlib/structures/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/definitions/dimension_definition.py` & `pyorlib-0.1.2/src/pyorlib/structures/definitions/dimension_definition.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/definitions/parameter_definition.py` & `pyorlib-0.1.2/src/pyorlib/structures/definitions/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/definitions/term_definition.py` & `pyorlib-0.1.2/src/pyorlib/structures/definitions/term_definition.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/parameters/multi_value_parameter.py` & `pyorlib-0.1.2/src/pyorlib/structures/parameters/multi_value_parameter.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/parameters/parameter.py` & `pyorlib-0.1.2/src/pyorlib/structures/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/structures/parameters/single_value_parameter.py` & `pyorlib-0.1.2/src/pyorlib/structures/parameters/single_value_parameter.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/validators/value_type_validator.py` & `pyorlib-0.1.2/src/pyorlib/validators/value_type_validator.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/validators/fields/dimension_field.py` & `pyorlib-0.1.2/src/pyorlib/validators/fields/dimension_field.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/src/pyorlib/validators/fields/parameter_field.py` & `pyorlib-0.1.2/src/pyorlib/validators/fields/parameter_field.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/algebra/test_element.py` & `pyorlib-0.1.2/tests/algebra/test_element.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/algebra/expressions/test_expression.py` & `pyorlib-0.1.2/tests/algebra/expressions/test_expression.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/algebra/terms/test_term.py` & `pyorlib-0.1.2/tests/algebra/terms/test_term.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/algebra/terms/constants/test_constant.py` & `pyorlib-0.1.2/tests/algebra/terms/constants/test_constant.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/algebra/terms/variables/test_variable.py` & `pyorlib-0.1.2/tests/algebra/terms/variables/test_variable.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/engines/test_cplex.py` & `pyorlib-0.1.2/tests/engines/test_cplex.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/engines/test_engine.py` & `pyorlib-0.1.2/tests/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/engines/test_gurobi.py` & `pyorlib-0.1.2/tests/engines/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/engines/test_or_tools.py` & `pyorlib-0.1.2/tests/engines/test_or_tools.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/engines/test_pulp.py` & `pyorlib-0.1.2/tests/engines/test_pulp.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/fixtures/engine_fixture.py` & `pyorlib-0.1.2/tests/fixtures/engine_fixture.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/model/test_model.py` & `pyorlib-0.1.2/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/structures/parameters/test_multi_value_parameter.py` & `pyorlib-0.1.2/tests/structures/parameters/test_multi_value_parameter.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/structures/parameters/test_single_value_parameter.py` & `pyorlib-0.1.2/tests/structures/parameters/test_single_value_parameter.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/validators/test_value_type_validator.py` & `pyorlib-0.1.2/tests/validators/test_value_type_validator.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/validators/fields/test_dimension_field.py` & `pyorlib-0.1.2/tests/validators/fields/test_dimension_field.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/tests/validators/fields/test_parameter_field.py` & `pyorlib-0.1.2/tests/validators/fields/test_parameter_field.py`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/.gitignore` & `pyorlib-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/LICENSE` & `pyorlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/README.md` & `pyorlib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyorlib-0.1.1/pyproject.toml` & `pyorlib-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,19 @@
 ]
 
 # --------------------
 # | Docs dependencies
 # ----------
 
 docs = [
-    "mkdocs-material>=9.4.0",
+    "mkdocs-material>=9.5.17",
     "mkdocstrings[python]>=0.24.0",
     "mkdocs-git-revision-date-localized-plugin>=1.2.1",
     "mkdocs-git-committers-plugin-2>=2.3.0",
+    "mkdocs-material[imaging]",
 ]
 
 # --------------------
 # | Tests dependencies
 # ----------
 
 tests = [
```

### Comparing `pyorlib-0.1.1/PKG-INFO` & `pyorlib-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyorlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: A powerful Python library for operations research. Define, solve, and interact with mathematical models in a standardized manner across different optimization packages.
 Project-URL: Homepage, https://github.com/dapensoft/pyorlib
 Project-URL: Documentation, https://dapensoft.github.io/pyorlib/
 Project-URL: Repository, https://github.com/dapensoft/pyorlib
 Project-URL: Changelog, https://dapensoft.github.io/pyorlib/release-notes
 Author-email: Isaac Da Pena <dapensoft@gmail.com>, Manuel Da Pena <dapensoft@gmail.com>
 License-Expression: MIT
@@ -36,15 +36,16 @@
 Provides-Extra: dev
 Requires-Dist: hatch>=1.8.1; extra == 'dev'
 Requires-Dist: pyorlib[docs]; extra == 'dev'
 Requires-Dist: pyorlib[tests]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-git-committers-plugin-2>=2.3.0; extra == 'docs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == 'docs'
-Requires-Dist: mkdocs-material>=9.4.0; extra == 'docs'
+Requires-Dist: mkdocs-material>=9.5.17; extra == 'docs'
+Requires-Dist: mkdocs-material[imaging]; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.24.0; extra == 'docs'
 Provides-Extra: gurobi
 Requires-Dist: gurobipy>=10.0.0; extra == 'gurobi'
 Provides-Extra: ortools
 Requires-Dist: ortools>=9.6.2534; extra == 'ortools'
 Provides-Extra: pulp
 Requires-Dist: pulp>=2.7.0; extra == 'pulp'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyorlib Version: 0.1.1 Summary: A powerful Python
+Metadata-Version: 2.3 Name: pyorlib Version: 0.1.2 Summary: A powerful Python
 library for operations research. Define, solve, and interact with mathematical
 models in a standardized manner across different optimization packages.
 Project-URL: Homepage, https://github.com/dapensoft/pyorlib Project-URL:
 Documentation, https://dapensoft.github.io/pyorlib/ Project-URL: Repository,
 https://github.com/dapensoft/pyorlib Project-URL: Changelog, https://
 dapensoft.github.io/pyorlib/release-notes Author-email: Isaac Da Pena
 gmail.com>, Manuel Da Pena
@@ -22,23 +22,23 @@
 'all' Requires-Dist: pyorlib[pulp]; extra == 'all' Provides-Extra: cplex
 Requires-Dist: cplex>=20.1.0.4; extra == 'cplex' Requires-Dist:
 docplex>=2.24.231; extra == 'cplex' Provides-Extra: dev Requires-Dist:
 hatch>=1.8.1; extra == 'dev' Requires-Dist: pyorlib[docs]; extra == 'dev'
 Requires-Dist: pyorlib[tests]; extra == 'dev' Provides-Extra: docs Requires-
 Dist: mkdocs-git-committers-plugin-2>=2.3.0; extra == 'docs' Requires-Dist:
 mkdocs-git-revision-date-localized-plugin>=1.2.1; extra == 'docs' Requires-
-Dist: mkdocs-material>=9.4.0; extra == 'docs' Requires-Dist: mkdocstrings
-[python]>=0.24.0; extra == 'docs' Provides-Extra: gurobi Requires-Dist:
-gurobipy>=10.0.0; extra == 'gurobi' Provides-Extra: ortools Requires-Dist:
-ortools>=9.6.2534; extra == 'ortools' Provides-Extra: pulp Requires-Dist:
-pulp>=2.7.0; extra == 'pulp' Provides-Extra: tests Requires-Dist:
-black>=23.12.0; extra == 'tests' Requires-Dist: coverage[toml]>=7.3.3; extra ==
-'tests' Requires-Dist: mypy>=1.7.1; extra == 'tests' Requires-Dist: pyorlib
-[all]; extra == 'tests' Requires-Dist: pytest>=7.4.0; extra == 'tests'
-Description-Content-Type: text/markdown
+Dist: mkdocs-material>=9.5.17; extra == 'docs' Requires-Dist: mkdocs-material
+[imaging]; extra == 'docs' Requires-Dist: mkdocstrings[python]>=0.24.0; extra
+== 'docs' Provides-Extra: gurobi Requires-Dist: gurobipy>=10.0.0; extra ==
+'gurobi' Provides-Extra: ortools Requires-Dist: ortools>=9.6.2534; extra ==
+'ortools' Provides-Extra: pulp Requires-Dist: pulp>=2.7.0; extra == 'pulp'
+Provides-Extra: tests Requires-Dist: black>=23.12.0; extra == 'tests' Requires-
+Dist: coverage[toml]>=7.3.3; extra == 'tests' Requires-Dist: mypy>=1.7.1; extra
+== 'tests' Requires-Dist: pyorlib[all]; extra == 'tests' Requires-Dist:
+pytest>=7.4.0; extra == 'tests' Description-Content-Type: text/markdown
                                    [PyORlib]
 
 _[_T_e_s_t_s_]_[_D_o_c_s_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_C_o_d_e
                                  _s_t_y_l_e_:_ _b_l_a_c_k_]
 
 --- **Documentation**: _h_t_t_p_s_:_/_/_d_a_p_e_n_s_o_f_t_._g_i_t_h_u_b_._i_o_/_p_y_o_r_l_i_b **Source Code**:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_a_p_e_n_s_o_f_t_/_p_y_o_r_l_i_b ---
```

