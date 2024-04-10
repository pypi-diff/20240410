# Comparing `tmp/fgen-0.3.1.tar.gz` & `tmp/fgen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgen-0.3.1.tar", max compression
+gzip compressed data, was "fgen-0.4.1.tar", max compression
```

## Comparing `fgen-0.3.1.tar` & `fgen-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,112 @@
--rw-r--r--   0        0        0     1461 2024-01-25 02:39:25.621738 fgen-0.3.1/LICENSE
--rw-r--r--   0        0        0     3440 2024-01-25 02:39:25.621738 fgen-0.3.1/README.md
--rw-r--r--   0        0        0     6375 2024-01-25 02:39:25.624738 fgen-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/__init__.py
--rw-r--r--   0        0        0      122 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/commands/__init__.py
--rw-r--r--   0        0        0     1098 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/commands/base.py
--rw-r--r--   0        0        0     2397 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/commands/generate.py
--rw-r--r--   0        0        0     2797 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/f2py.py
--rw-r--r--   0        0        0    23879 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/fortran_parsing.py
--rw-r--r--   0        0        0      165 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/main.py
--rw-r--r--   0        0        0    12588 2024-01-25 02:39:25.624738 fgen-0.3.1/src/fgen/models.py
--rw-r--r--   0        0        0        0 2024-01-25 02:39:25.661738 fgen-0.3.1/src/fgen/py.typed
--rw-r--r--   0        0        0     2239 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/calculator_manager.f90.jinja
--rw-r--r--   0        0        0     5839 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/python_module.py.jinja
--rw-r--r--   0        0        0      771 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/fortran/attribute_deferred_array.jinja
--rw-r--r--   0        0        0      357 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/fortran/attribute_derived.jinja
--rw-r--r--   0        0        0      346 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/fortran/attribute_intrinsic.jinja
--rw-r--r--   0        0        0     1059 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/python/attribute_deferred_array.jinja
--rw-r--r--   0        0        0      308 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/python/attribute_derived.jinja
--rw-r--r--   0        0        0      429 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/python/attribute_intrinsic.jinja
--rw-r--r--   0        0        0      790 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/python/method.jinja
--rw-r--r--   0        0        0      172 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/snippets/python/verify_units_parameters.jinja
--rw-r--r--   0        0        0     4727 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templates/wrap_module.f90.jinja
--rw-r--r--   0        0        0     4991 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen/templator.py
--rw-r--r--   0        0        0      111 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen_runtime/__init__.py
--rw-r--r--   0        0        0     3061 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen_runtime/arrays.py
--rw-r--r--   0        0        0     4760 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen_runtime/base.py
--rw-r--r--   0        0        0     3593 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen_runtime/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-25 02:39:25.661738 fgen-0.3.1/src/fgen_runtime/py.typed
--rw-r--r--   0        0        0     9225 2024-01-25 02:39:25.625738 fgen-0.3.1/src/fgen_runtime/units.py
--rw-r--r--   0        0        0     4719 1970-01-01 00:00:00.000000 fgen-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-04-10 12:18:04.979820 fgen-0.4.1/LICENCE
+-rw-r--r--   0        0        0     3347 2024-04-10 12:18:04.979820 fgen-0.4.1/README.md
+-rw-r--r--   0        0        0     6745 2024-04-10 12:18:04.985819 fgen-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      817 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/commands/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/commands/base.py
+-rw-r--r--   0        0        0     4434 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/commands/generate.py
+-rw-r--r--   0        0        0     1454 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/data_models/__init__.py
+-rw-r--r--   0        0        0     9158 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/data_models/fortran_derived_type.py
+-rw-r--r--   0        0        0     2199 2024-04-10 12:18:04.985819 fgen-0.4.1/src/fgen/data_models/method.py
+-rw-r--r--   0        0        0     3301 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/module.py
+-rw-r--r--   0        0        0      982 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/module_enum_defining.py
+-rw-r--r--   0        0        0     1035 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/module_requirement.py
+-rw-r--r--   0        0        0     3509 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/multi_return.py
+-rw-r--r--   0        0        0     4238 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/package.py
+-rw-r--r--   0        0        0     2152 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/package_shared_elements.py
+-rw-r--r--   0        0        0     5830 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/serialisation.py
+-rw-r--r--   0        0        0     4262 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/unitless_value.py
+-rw-r--r--   0        0        0     3945 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/data_models/value.py
+-rw-r--r--   0        0        0     2826 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/f2py.py
+-rw-r--r--   0        0        0    28872 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/fortran_parsing.py
+-rw-r--r--   0        0        0     4331 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/jinja_environment.py
+-rw-r--r--   0        0        0      165 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/main.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:18:05.035819 fgen-0.4.1/src/fgen/py.typed
+-rw-r--r--   0        0        0    10864 2024-04-10 12:18:04.986820 fgen-0.4.1/src/fgen/wrapper_building/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/formatting.py
+-rw-r--r--   0        0        0     1286 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_manager_module/__init__.py
+-rw-r--r--   0        0        0     3972 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_manager_module/fortran-manager-module.f90.jinja
+-rw-r--r--   0        0        0    20627 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/__init__.py
+-rw-r--r--   0        0        0     2467 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/fortran-wrapper-module.f90.jinja
+-rw-r--r--   0        0        0      187 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/module-level-docstring.f90.jinja
+-rw-r--r--   0        0        0      489 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/module-use-requirements.f90.jinja
+-rw-r--r--   0        0        0      701 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/module-use-statements.f90.jinja
+-rw-r--r--   0        0        0     1550 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/provided-type-method-no-return.f90.jinja
+-rw-r--r--   0        0        0     1755 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/fortran_wrapper_module/provided-type-setter.f90.jinja
+-rw-r--r--   0        0        0     1312 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/python_enums_module/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/python_enums_module/python-enum-definition.py.jinja
+-rw-r--r--   0        0        0      186 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/python_enums_module/python-enums-module.py.jinja
+-rw-r--r--   0        0        0      897 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/python_init_module/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-10 12:18:04.987820 fgen-0.4.1/src/fgen/wrapper_building/python_init_module/python-init-module.py.jinja
+-rw-r--r--   0        0        0    23062 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/__init__.py
+-rw-r--r--   0        0        0     2129 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/getters-and-setters.py.jinja
+-rw-r--r--   0        0        0     1960 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/methods.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/module-imports-requirements.py.jinja
+-rw-r--r--   0        0        0     1359 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/module-imports.py.jinja
+-rw-r--r--   0        0        0      175 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/module-level-docstring.py.jinja
+-rw-r--r--   0        0        0      379 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/module-units.py.jinja
+-rw-r--r--   0        0        0     3953 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/provided-type-class-methods.py.jinja
+-rw-r--r--   0        0        0       96 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/provided-type-docstring.py.jinja
+-rw-r--r--   0        0        0      825 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/provided-type-str-repr-methods.py.jinja
+-rw-r--r--   0        0        0     4187 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/python-wrapper-module.py.jinja
+-rw-r--r--   0        0        0      169 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapper_building/python_wrapper_module/verify-units-decorator.py.jinja
+-rw-r--r--   0        0        0     2250 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/__init__.py
+-rw-r--r--   0        0        0    10819 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/__init__.py
+-rw-r--r--   0        0        0     2151 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     4666 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      142 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/fortran-statement-declarations-getter-setter.f90.jinja
+-rw-r--r--   0        0        0      150 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/fortran-statement-declarations-method-returning-to-python.f90.jinja
+-rw-r--r--   0        0        0     1573 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0       86 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/python-for-preparing-to-pass-to-fortran-dynamic-unit.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/array_deferred_size/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0     7750 2024-04-10 12:18:04.988819 fgen-0.4.1/src/fgen/wrapping_strategies/character/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     1833 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      181 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0     9057 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     3805 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      143 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/fortran-statement-declarations-getter-setter.f90.jinja
+-rw-r--r--   0        0        0      151 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/fortran-statement-declarations-method-returning-to-python.f90.jinja
+-rw-r--r--   0        0        0      494 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/character_deferred_size/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0    10260 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     1833 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      471 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0       86 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/python-for-preparing-to-pass-to-fortran-dynamic-unit.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/default/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0    11378 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/__init__.py
+-rw-r--r--   0        0        0     2178 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     3280 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0       93 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/fortran-for-receiving-from-python.f90.jinja
+-rw-r--r--   0        0        0      341 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0       74 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/python-for-preparing-to-pass-to-fortran.py.jinja
+-rw-r--r--   0        0        0      295 2024-04-10 12:18:04.989819 fgen-0.4.1/src/fgen/wrapping_strategies/derived_type/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0     8258 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     1833 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      260 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0       60 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/python-for-preparing-to-pass-to-fortran.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/enum/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0     1557 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/information_injection.py
+-rw-r--r--   0        0        0    10870 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/interface.py
+-rw-r--r--   0        0        0     7450 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/logical/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/logical/fortran-for-getter.f90.jinja
+-rw-r--r--   0        0        0     1833 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/logical/fortran-for-method-returning-wrapped-type.f90.jinja
+-rw-r--r--   0        0        0      210 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/logical/python-for-fortran-return-value-processing.py.jinja
+-rw-r--r--   0        0        0      326 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/logical/python-getter-docstring.py.jinja
+-rw-r--r--   0        0        0     1277 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/passing_to_fortran_steps.py
+-rw-r--r--   0        0        0     5026 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/receiving_from_python_steps.py
+-rw-r--r--   0        0        0      856 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen/wrapping_strategies/type_annotations.py
+-rw-r--r--   0        0        0      188 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen_runtime/__init__.py
+-rw-r--r--   0        0        0     3092 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen_runtime/arrays.py
+-rw-r--r--   0        0        0     4816 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen_runtime/base.py
+-rw-r--r--   0        0        0     4372 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen_runtime/exceptions.py
+-rw-r--r--   0        0        0     5356 2024-04-10 12:18:04.990820 fgen-0.4.1/src/fgen_runtime/formatting.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:18:05.041819 fgen-0.4.1/src/fgen_runtime/py.typed
+-rw-r--r--   0        0        0     4263 2024-04-10 12:18:04.991819 fgen-0.4.1/src/fgen_runtime/testing.py
+-rw-r--r--   0        0        0     1487 2024-04-10 12:18:04.991819 fgen-0.4.1/src/fgen_runtime/timeseries_collection.py
+-rw-r--r--   0        0        0    18597 2024-04-10 12:18:04.991819 fgen-0.4.1/src/fgen_runtime/units.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 fgen-0.4.1/PKG-INFO
```

### Comparing `fgen-0.3.1/LICENSE` & `fgen-0.4.1/LICENCE`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023, Jared Lewis
+Copyright 2023-2024, Jared Lewis, Zebedee Nicholls and their employers
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `fgen-0.3.1/README.md` & `fgen-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 We recommend reading the docs there because the internal documentation links
 don't render correctly on GitLab's viewer. TODO: Create docs
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
-Fortran-Python wrapper can be installed with conda or pip:
+fgen can be installed with pip:
 
 ```bash
 pip install fgen
-conda install -c conda-forge fgen
 ```
 
 ## Usage
 
 TODO
 
 ### libfgen
@@ -92,14 +91,13 @@
 
 Once the virtual environment has been created, `libfgen` can be built
 using `make build`. This library contains the common Fortran code used by
 all wrappers and uses [CMake](https://cmake.org/) to build and requires
 a working Fortran compiler.
 
 If there are any issues, the messages from the `Makefile` should guide you
-through. If not, please raise an issue in the [issue tracker][issue_tracker].
+through. If not, please raise an issue in the
+[issue tracker](https://gitlab.com/magicc/fgen/issues).
 
 For the rest of our developer docs, please see [](development-reference).
 
-[issue_tracker]: https://gitlab.com/magicc/fgen/issues
-
 <!--- sec-end-installation-dev -->
```

### Comparing `fgen-0.3.1/pyproject.toml` & `fgen-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "fgen"
-version = "0.3.1"
+version = "0.4.1"
 description = "Automatically generate wrapper to integrate Fortran and Python"
-authors = ["Jared Lewis <jared.lewis@climate-energy-college.org>"]
+authors = [
+    "Zebedee Nicholls <zebedee.nicholls@climate-energy-college.org>",
+    "Jared Lewis <jared.lewis@climate-energy-college.org>",
+]
 readme = "README.md"
 packages = [
     {include = "fgen", from = "src"},
     {include = "fgen_runtime", from = "src"},
 ]
 keywords = ["fortran"]
 license = "BSD-3-Clause"
@@ -20,31 +23,32 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering"
 ]
 homepage = "https://gitlab.com/magicc/fgen"
+include = ["LICENCE"]  # poetry uses US English so assumes it will be spelt LICENSE
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cattrs = "^23.0.0"
 attrs = "^23.0.0"
-openscm-units = "^0.5.0"
 click = "^8.0.0"
 pyyaml = "^6.0"
-black = "^23.3.0"
-jinja2 = "^3.1.2"
-cmakelang = "^0.6.13"
+black = {version = "^23.3.0", optional = true}
+jinja2 = {version = "^3.1.2", optional = true}
 loguru = "^0.7.2"
+typing-extensions = "^4.9.0"  # Can drop once we remove Python 3.9 support
+pint = "*"
+numpy = ">1.23"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 pytest-xdist = "^3.3.1"
-[tool.poetry.group.test.dependencies]
 pytest-regressions = "^2.4.2"
 
 [tool.poetry.group.docs.dependencies]
 myst-nb = "^0.17.0"
 sphinx-book-theme = "^1.1.0"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-autodocgen = "^1.3"
@@ -62,14 +66,18 @@
 towncrier = "^23.6.0"
 cmake = "^3.26.4"
 # Temporary fix until next towncrier release
 importlib-resources = {"version" = "<6", python = "<=3.9" }
 fprettify = "^0.3.7"
 notebook = "^7.0.7"
 liccheck = "^0.9.1"
+cmakelang = "^0.6.13"
+
+[tool.poetry.extras]
+templates = ["black", "jinja2"]
 
 [tool.poetry.scripts]
 fgen = 'fgen.main:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -85,15 +93,16 @@
 fail_under = 95
 skip_empty = true
 show_missing = true
 # Regexes for lines to exclude from consideration in addition to the defaults
 exclude_also = [
     # Don't complain about missing type checking code:
     "if TYPE_CHECKING",
-    "@overload"
+    "@overload",
+    "\\.\\.\\.",
 ]
 
 [tool.mypy]
 strict = true
 # prevent unimported libraries silently being treated as Any
 disallow_any_unimported = true
 # show error codes on failure with context
@@ -137,17 +146,18 @@
     "PD002",  # Disable autofix for inplace as this often introduces bugs
 ]
 ignore = [
     "D200",  # One-line docstring should fit on one line with quotes
     "D400",  # First line should end with a period
     "D105",  # Missing docstring in magic method
     "UP007",
+    "PD011",  # Ruff confused about APIs
 ]
 # Provide some leeway for long docstring, this is otherwise handled by black
-line-length = 110
+line-length = 88
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.ruff.per-file-ignores]
 "test*.py" = [
     "D",  # Documentation not needed in tests
```

### Comparing `fgen-0.3.1/src/fgen/commands/base.py` & `fgen-0.4.1/src/fgen/commands/base.py`

 * *Files identical despite different names*

### Comparing `fgen-0.3.1/src/fgen/f2py.py` & `fgen-0.4.1/src/fgen/f2py.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 f2py wrapper
 
-Patches the default behaviour of f2py with some custom error handling. This was inspired by the amazing
-[f90wrap](https://github.com/jameskermode/f90wrap).
+Patches the default behaviour of f2py with some custom error handling.
+This was inspired by the amazing [f90wrap](https://github.com/jameskermode/f90wrap).
 """
 import sys
 
 import numpy.f2py.rules as f2py_rules
 from numpy.f2py import main as f2py_main  # type: ignore
 
 
 def patch_f2py() -> None:
     """
     Patch f2py to raise a RuntimeError if :c:func:`on_error` is called during execution
 
-    Interrupt signals are also captured and handled. This has only been tested with numpy 1.21.0
-    and may be flakey if f2py has substantial changes
+    Interrupt signals are also captured and handled.
+    This has only been tested with numpy 1.21.0
+    and may be flakey if f2py has substantial changes.
     """
     includes_inject = "#includes0#\n"
 
     if sys.platform == "win32":
-        includes_inject = includes_inject + "#include <signal.h>\n#include <setjmpex.h>\n"
+        includes_inject = (
+            includes_inject + "#include <signal.h>\n#include <setjmpex.h>\n"
+        )
     else:
         includes_inject = includes_inject + "#include <setjmp.h>\n"
 
     includes_inject = (
         includes_inject
         + """
     #include <stdlib.h>
@@ -52,17 +55,17 @@
     {
       char message[] = "User interrupt occurred";
       on_error_(message, strlen(message));
     }
     """
     )
 
-    f2py_rules.module_rules["modulebody"] = f2py_rules.module_rules["modulebody"].replace(
-        "#includes0#\n", includes_inject
-    )
+    f2py_rules.module_rules["modulebody"] = f2py_rules.module_rules[
+        "modulebody"
+    ].replace("#includes0#\n", includes_inject)
 
     f2py_rules.routine_rules["body"] = f2py_rules.routine_rules["body"].replace(  # type: ignore
         "volatile int f2py_success = 1;\n",
         "volatile int f2py_success = 1; int setjmp_value;",
     )
 
     f2py_rules.routine_rules["body"] = f2py_rules.routine_rules["body"].replace(  # type: ignore
```

### Comparing `fgen-0.3.1/src/fgen/fortran_parsing.py` & `fgen-0.4.1/src/fgen/fortran_parsing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 """
 Support for parsing Fortran type declarations
 
-We just want to make this as helpful as possible when auto-generating our wrappers while keeping the
-implemenation here as minimal as possible because duplicating the Fortran implementation logic is
-not the point of this module. The fortran compiler will catch any odd type declarations at
-compile-time.
+We just want to make this as helpful as possible
+when auto-generating our wrappers
+while keeping the implemenation here as minimal as possible
+because duplicating the Fortran implementation logic is not the point of this module.
+The fortran compiler will catch any odd type declarations at compile-time.
 
-To understand what is going on, we start with the syntax for declaring fortran types as defined in
+To understand what is going on,
+we start with the syntax for declaring fortran types as defined in
 Section 5.1 of the `Fortran 2003 standard <https://j3-fortran.org/doc/year/04/04-007.pdf>`_.
 It looks like the below:
 
 .. syntax higlighting below is wrong, not sure what language the specs are given in
 .. code-block:: fortran
 
     R501 type-declaration-stmt  is declaration-type-spec [ [ , attr-spec ] ... :: ] entity-decl-list
     R502 declaration-type-spec  is intrinsic-type-spec
                                 or TYPE ( derived-type-spec )
                                 or CLASS ( derived-type-spec )
                                 or CLASS ( * )
 
-In short, a type declaration statement is composed of a declaration type specification, a collection
-of one or more attribute specifications and then an entity declaration list. The declaration type
-specification can be either an intrinsic type that has been defined by the language, or a derived
-type which has been declared using a ``type`` block elsewhere.
-
-We focus on the combination of the declaration type specification (which we typically shorten to
-type specification) and the attribute specifications i.e. we largely ignore the entity declarations.
-In the absence of a defined term in the Fortran standard, we call this combination the type
-attribute declaration throughout.
+In short, a type declaration statement is composed of a declaration type specification,
+a collection of one or more attribute specifications
+and then an entity declaration list.
+The declaration type specification can be either an intrinsic type
+that has been defined by the language,
+or a derived type which has been declared using a ``type`` block elsewhere.
+
+We focus on the combination of the declaration type specification
+(which we typically shorten to type specification)
+and the attribute specifications i.e. we largely ignore the entity declarations.
+In the absence of a defined term in the Fortran standard,
+we call this combination the type attribute declaration throughout.
 
 To illustrate, consider the following example
 
 .. code-block:: fortran
 
     real(8), dimension(3), pointer :: heat_uptake
 
 Here is how we would refer to the parts of this example:
 
 - type declaration statement: ``real(8), dimension(3), pointer :: heat_uptake``
 - declaration type specification (or simply type specification): ``real(8)``
 - attribute specifications: ``dimension(3), pointer``
 - type attribute declaration: ``real(8), dimension(3), pointer``
-- entity declaration (largely ignored by this module, we treat the double colon ``::`` as part of
-  the entity declaration): ``:: heat_uptake``
+- entity declaration (largely ignored by this module, we treat the double colon ``::`` as part of the entity declaration): ``:: heat_uptake``
 
 One other example using a derived type
 
 .. code-block:: fortran
 
     type(my_calculator) :: heat_uptake_calculator
 
 Here is how we would refer to the parts of this example:
 
 - type declaration statement: ``type(my_calculator) :: heat_uptake_calculator``
 - declaration type specification (or simply type specification): ``type(my_calculator)``
 - attribute specifications: none
 - type attribute declaration (same as type specification in this case): ``type(my_calculator)``
-- entity declaration (largely ignored by this module, we treat the double colon ``::`` as part of
-  the entity declaration): ``:: heat_uptake_calculator``
+- entity declaration (largely ignored by this module, we treat the double colon ``::`` as part of the entity declaration): ``:: heat_uptake_calculator``
 
 Notes
 -----
 Fortran type declaration statements (and Fortran in general) are case-insensitive
 
 This module relies heavily on regular expressions. If needed, use an online tool like
 `regex101.com <https://regex101.com/>`_ to help you understand them.
-"""
+"""  # noqa: E501
 from __future__ import annotations
 
 import re
 from collections.abc import Sequence
 from typing import Any, Optional, Union
 
 from attrs import define, field
@@ -77,22 +80,27 @@
 _AT_LEAST_ONE_ALPHANUMERIC_REGEXP: str = r"[a-z0-9]+"
 """Regex representing a search for at least one alphanumeric character"""
 
 _DIMENSION_SPECIFICATION: str = f"(\\*|:|{_AT_LEAST_ONE_ALPHANUMERIC_REGEXP})"
 """
 Regex representing a possible dimension attribute specification in a Fortran definition
 
-This also captures deferred and assumed shaped arrays which are not currently supported by fgen, but may
-be supported in future.
+This also captures deferred and assumed shaped arrays
+which are not currently supported by fgen,
+but may be supported in future.
 
 e.g. "(4, 3)", "(n, m)", "(5)", "(n, 4)"
 """
 
 _DIMENSION_REGEX: str = (
-    r"DIMENSION\(" r"(?P<dimension>" f"{_DIMENSION_SPECIFICATION}(,\\s*{_DIMENSION_SPECIFICATION})*" ")" r"\)"
+    r"DIMENSION\("
+    r"(?P<dimension>"
+    f"{_DIMENSION_SPECIFICATION}(,\\s*{_DIMENSION_SPECIFICATION})*"
+    ")"
+    r"\)"
 )
 """
 Regex string used to check for dimension information within attribute specifications
 
 e.g. "dimension(4, 3)", "dimension(n)"
 """
 
@@ -102,44 +110,51 @@
 
 e.g. "(kind=8)" in "real(kind=8)"
 """
 
 _INTRINSIC_TYPE_SPECIFICATIONS: tuple[str, ...] = (
     "INTEGER",
     "REAL",
-    "DOUBLE PRECISION",
     "COMPLEX",
     "CHARACTER",
     "LOGICAL",
 )
 """Intrinsic Fortran type specifications that we support (case insensitive)"""
 
-_DERIVED_TYPE_REGEX: str = r"type\(\s?(?P<derived_type_name>[a-z]+)\s?\)"
+_ENUM_LIKE_REGEX: str = r"integer\(\s?kind\s?\(\s?(?P<enum_name>[a-z0-9]+)\s?\)\s?\)"
+"""
+Regex string to capture Fortran enum-like specifications
+
+Matches things like "integer(kind(Enum))" and "integer(kind(EnumValue))".
+The enum type is captured in a group called "enum_name".
+"""
+
+_DERIVED_TYPE_REGEX: str = r"type\(\s?(?P<derived_type_name>[a-z0-9]+)\s?\)"
 """
 Regex string to capture derived type specifications
 
-Matches things like "type(my_derived_type)" and "type(calculator)". The derived type
-is captured in a group called "derived_type_name". We currently don't support "class(abc)"
-specifications.
+Matches things like "type(my_derived_type)" and "type(calculator)".
+The derived type is captured in a group called "derived_type_name".
+We currently don't support "class(abc)" specifications.
 """
 
 SUPPORTED_TYPE_SPECIFICATIONS: tuple[str, ...] = (
     *[
         f"^{intrinsic_type_spec}{_KIND_SPECIFICATION}"
         for intrinsic_type_spec in _INTRINSIC_TYPE_SPECIFICATIONS
     ],
     _DERIVED_TYPE_REGEX,
+    _ENUM_LIKE_REGEX,
 )
 """
 The collection of valid type specifications that are supported
 
 This covers both intrinsic type specifications and derived type specifications.
 """
 
-
 SUPPORTED_ATTRIBUTE_SPECIFICATIONS: tuple[Union[str, re.Pattern[str]], ...] = (
     "ALLOCATABLE",
     # "ASYNCHRONOUS",
     _DIMENSION_REGEX,
     # "INTENT",
     # "INTRINSIC",
     # "language-binding-spec"
@@ -150,19 +165,22 @@
     "TARGET",
     # "VALUE",
     # "VOLATILE",
 )
 """
 The collection of valid attribute specifications that are supported
 
-In the type declaration, "type(my_calculator), pointer", the attribute specification is "pointer"
-(the other part, "type(my_calculator)", is simply the type specification
+In the type declaration, "type(my_calculator), pointer",
+the attribute specification is "pointer"
+(the other part, "type(my_calculator)",
+is simply the type specification
 (or declaration type specification if you're being very precise))
 
-Note that only a subset of valid attributes can be specified. The more esoteric attributes have been excluded
+Note that only a subset of valid attributes can be specified.
+The more esoteric attributes have been excluded
 until the use case for these attributes is better understood.
 """
 
 
 def _get_type_attribute_declaration(type_declaration_statement: str) -> str:
     """
     Get type attribute declaration from a type declaration statement
@@ -170,29 +188,33 @@
     Simply removes the entity declaration
     """
     return type_declaration_statement.split("::")[0]
 
 
 def _get_parts(type_declaration_statement: str) -> tuple[str, tuple[str, ...]]:
     """
-    Split a type declaration statement into a type specification and a collection of attribute specifications
+    Split a type declaration statement into its parts
 
-    This function is used below by :meth:`FortranDataType.as_str`. That method takes care of validating
-    the different parts of a Fortran type declaration statement.
+    Specifically, into a type specification and a collection of attribute specifications
 
-    See the docstring of :mod:`fgen.fortran_parsing` for further details on how we interpret Fortran
-    type declaration statements.
+    This function is used below by :meth:`FortranDataType.as_str`.
+    That method takes care of
+    validating the different parts of a Fortran type declaration statement.
+
+    See the docstring of :mod:`fgen.fortran_parsing`
+    for further details on how we interpret Fortran type declaration statements.
 
     Parameters
     ----------
     type_declaration_statement
         Type declaration statement to parse
 
-        The entity declaration component (any parts including and after the "::") is optional
-        and will be ignored
+        The entity declaration component
+        (any parts including and after the "::")
+        is optional and will be ignored
 
     Returns
     -------
         The type specification and any additional attribute specifications
 
     Examples
     --------
@@ -204,20 +226,33 @@
     ('real', ('dimension(5, 3)',))
     >>> _get_parts("integer, dimension(:, :)")
     ('integer', ('dimension(:, :)',))
     >>> _get_parts("logical, dimension(2, :)")
     ('logical', ('dimension(2, :)',))
     >>> _get_parts("logical, dimension(2, :), pointer")
     ('logical', ('dimension(2, :)', 'pointer'))
+    >>> _get_parts("integer(kind(EnumValue))")
+    ('integer(kind(EnumValue))', ())
     """
-    type_attribute_declaration = _get_type_attribute_declaration(type_declaration_statement)
+    type_attribute_declaration = _get_type_attribute_declaration(
+        type_declaration_statement
+    )
+
+    # Check if this is enum type, such things break everything below
+    enum_regex_match = re.match(
+        _ENUM_LIKE_REGEX, type_attribute_declaration, flags=re.IGNORECASE
+    )
+    if enum_regex_match:
+        return type_attribute_declaration, tuple()
 
     part_regexp_including_brackets = r"[^,\s]+(?:\([^\(]*?\))"
     part_regexp_no_brackets = r"[^,\s]+"
-    part_regexp: str = "|".join([part_regexp_including_brackets, part_regexp_no_brackets])
+    part_regexp: str = "|".join(
+        [part_regexp_including_brackets, part_regexp_no_brackets]
+    )
     """
     Regular expression that captures the parts of the type declaration statement
 
     It effectively just splits the string into comma separated pieces without
     surrounding whitespace (with a little extra piece to make sure you don't
     get nested brackets (e.g. "dimension((4, 3))") in any part, which is invalid
     Fortran as far as we know anyway)
@@ -225,61 +260,66 @@
     e.g. this can be used to split "real, dimension(2, 3, 4)"
     into ["real", "dimension(2, 3, 4)"]
     """
     parts = re.findall(part_regexp, type_attribute_declaration)
 
     if not len(parts):
         raise ValueError(  # noqa: TRY003
-            f"An invalid type attribute declaration was provided: {type_attribute_declaration!r}"
+            "An invalid type attribute declaration was provided: "
+            f"{type_attribute_declaration!r}"
         )
 
     # The Fortran spec states that the first part must be the type specification and
     # the rest are attribute specifications so we can safely assume order here
     return parts[0], tuple(parts[1:])
 
 
 def _validate_fortran_type_attribute_declaration(
     type_specification: str, attribute_specifications: tuple[str, ...]
 ) -> None:
     """
     Validate that a fortran type attribute declaration is supported by fgen
 
-    The type attribute declaration must have been split (using e.g. :func:`_get_parts`) before using
-    this function.
+    The type attribute declaration must have been split
+    (using e.g. :func:`_get_parts`)
+    before using this function.
 
-    We don't support all valid fortran. See the examples below and the tests for examples of
-    supported options.
+    We don't support all valid fortran.
+    See the examples below and the tests for examples of supported options.
 
     This validation is pretty crude as invalid Fortran will be caught at compile time.
 
-    See the docstring of :mod:`fgen.fortran_parsing` for further details on how we interpret Fortran
-    type declaration statements.
+    See the docstring of :mod:`fgen.fortran_parsing`
+    for further details on how we interpret Fortran type declaration statements.
 
     Parameters
     ----------
     type_specification
         Type specification
 
     attribute_specifications
         Attribute specifications
 
-        See :data:`SUPPORTED_ATTRIBUTE_SPECIFICATIONS` for the attributes that are currently supported by fgen
+        See :data:`SUPPORTED_ATTRIBUTE_SPECIFICATIONS`
+        for the attributes that are currently supported by fgen
 
     Raises
     ------
     ValueError
         An unsupported fortran type specification is supplied
 
     Examples
     --------
     Below are some examples of (split) fortran type declarations that pass
 
     >>> _validate_fortran_type_attribute_declaration("integer", ())
     >>> _validate_fortran_type_attribute_declaration("real", ("dimension(5)",))
-    >>> _validate_fortran_type_attribute_declaration("type(calculator)", ("dimension(5)", "pointer"))
+    >>> _validate_fortran_type_attribute_declaration(
+    ...     "type(calculator)", ("dimension(5)", "pointer")
+    ... )
 
     See Also
     --------
     :func:`_get_parts`
     """
     # Any attributes must match the regex of a supported attribute
     if not any(
@@ -304,83 +344,101 @@
 def _convert_complex_attribute_specifications(
     attribute_specifications: Sequence[str],
 ) -> tuple[Union[str, DimensionAttributeSpecification], ...]:
     """
     Convert any complex attribute specifications to their supporting classes
 
     For example, a dimension attribute specification is converted to a
-    :class:`DimensionAttributeSpecification` which holds additional information about the attribute.
-    If the attribute specification doesn't have a matching class than it will remain as a string.
+    :class:`DimensionAttributeSpecification`
+    which holds additional information about the attribute.
+    If the attribute specification doesn't have a matching class
+    then it will remain as a string.
 
     Parameters
     ----------
     attribute_specifications
         Collection of attribute specifications
 
     Returns
     -------
         Tuple that contains a combination of strings and classes in the case of the more
         complicated attributes
     """
-    attributes: list[Union[str, DimensionAttributeSpecification]] = list(attribute_specifications)
+    attributes: list[Union[str, DimensionAttributeSpecification]] = list(
+        attribute_specifications
+    )
 
     for i in range(len(attribute_specifications)):
-        match = re.search(_DIMENSION_REGEX, attribute_specifications[i], flags=re.IGNORECASE)
+        match = re.search(
+            _DIMENSION_REGEX, attribute_specifications[i], flags=re.IGNORECASE
+        )
         if match:
-            attributes[i] = DimensionAttributeSpecification.from_dimension_info(match.group("dimension"))
+            attributes[i] = DimensionAttributeSpecification.from_dimension_info(
+                match.group("dimension")
+            )
 
     return tuple(attributes)
 
 
 @define
 class DimensionAttributeSpecification:
     """
     Dimension attribute specification
 
     Defines the shape of a data type. See Section 5.1.2.5 of the
-    `Fortran 2003 standard <https://j3-fortran.org/doc/year/04/04-007.pdf>`_ for a description of the
-    dimension attribute specification.
+    `Fortran 2003 standard <https://j3-fortran.org/doc/year/04/04-007.pdf>`_
+    for a description of the dimension attribute specification.
 
-    Currently, we only support explicit dimensions where the size of the dimension is explicitly declared
-    at compile-time with an integer or execution-time using a variable provided to a procedure (e.g. using
-    "n" which is a variable that is also provided to a procedure).
-    The later form is an automatic explicit dimension and will rely upon the Fortran compiler to validate the
-    attribute declaration since additional context is required about where the attribute is used.
+    Currently, we only support explicit dimensions
+    where the size of the dimension
+    is explicitly declared at compile-time with an integer or execution-time
+    using a variable provided to a procedure
+    (e.g. using "n" which is a variable that is also provided to a procedure).
+    The later form is an automatic explicit dimension
+    and will rely upon the Fortran compiler to validate the attribute declaration
+    since additional context is required about where the attribute is used.
 
     Assumed-sized dimensions ("*") are not currently supported.
     """
 
     dimensions: tuple[Union[str, int], ...] = field()
     """
     Collection of dimensions of the attribute specification
 
-    Can include explicit dimensions (e.g. 5) or automatic explicit dimensions (e.g. "n"). Deferred
-    dimensions (e.g. ":") are allowed.
+    Can include explicit dimensions (e.g. 5)
+    or automatic explicit dimensions (e.g. "n").
+    Deferred dimensions (e.g. ":") are allowed.
     """
 
     @dimensions.validator
-    def _check_dimensions(self, attribute: Any, value: tuple[Union[str, int], ...]) -> None:
+    def _check_dimensions(
+        self, attribute: Any, value: tuple[Union[str, int], ...]
+    ) -> None:
         for dimension in value:
             if dimension == "*":
                 raise ValueError(  # noqa: TRY003
                     "Assumed-sized dimensions are not supported"
                 )
 
     @classmethod
-    def from_dimension_info(cls, dimension_info: str) -> DimensionAttributeSpecification:
+    def from_dimension_info(
+        cls, dimension_info: str
+    ) -> DimensionAttributeSpecification:
         """
         Create a DimensionAttributeSpecification from the dimension information
 
         The dimension information describes the shape and dimensionality of a variable.
 
         Parameters
         ----------
         dimension_info
-            The dimension information is the content between the () for a dimension attribute. For example,
-            for an attribute "dimension(8, n)" the dimension_info would be `"8, n"`.
+            The dimension information
+            is the content between the () for a dimension attribute.
+            For example, for an attribute "dimension(8, n)"
+            the dimension_info would be `"8, n"`.
 
             Static dimensions are converted to integers before initialising.
 
         Returns
         -------
             New DimensionAttributeSpecification
         """
@@ -413,24 +471,27 @@
 def _get_python_type_with_dimensions(
     dimension_info: Sequence[Union[str, int]],
     base: str,
 ) -> str:
     """
     Get a Python type that supports dimension information
 
-    See [#1](https://gitlab.com/magicc/fgen/-/issues/1) for ongoing discussions about updating this
-    to return more sophisticated Python types
+    See [#1](https://gitlab.com/magicc/fgen/-/issues/1)
+    for ongoing discussions about updating this
+    to return more sophisticated Python types.
 
     Parameters
     ----------
     dimension_info
-        Dimension information (e.g. extracted elsewhere from a Fortran type declaration statement)
+        Dimension information
+        (e.g. extracted elsewhere from a Fortran type declaration statement)
 
     base
-        Base Python type to which the dimension information applies (e.g. "float", "int", "str")
+        Base Python type to which the dimension information applies
+        (e.g. "float", "int", "str")
 
     Returns
     -------
         Python type with dimension information
 
     Examples
     --------
@@ -465,148 +526,310 @@
 
 
 @define
 class FortranDataType:
     """
     A fortran data type including its attributes
 
-    See the docstring of :mod:`fgen.fortran_parsing` for further details on Fortran type declaration
+    See the docstring of :mod:`fgen.fortran_parsing`
+    for further details on Fortran type declaration
     statements and how we handle and describe them.
 
-    We are only interested in the type attribute declaration so anything including and after a "::"
-    should be stripped before initialising this class.
+    We are only interested in the type attribute declaration
+    so anything including and after a "::" should be stripped
+    before initialising this class.
     """
 
     type_specification: str
     """
     This can be either an intrinsic type, or a derived type.
 
     For example, "real(8)", "logical", "type(my_calculator)"
     """
 
-    attribute_specifications: tuple[Union[str, DimensionAttributeSpecification], ...] = field()
+    attribute_specifications: tuple[
+        Union[str, DimensionAttributeSpecification], ...
+    ] = field()
     """
     List of attribute specifications that apply to the Fortran data type
 
-    These are our internal representation of attribute specifications e.g. "pointer", "target",
-    "dimension(3, 3)"
+    These are our internal representation of attribute specifications
+    e.g. "pointer", "target", "dimension(3, 3)"
     """
 
+    def __str__(self) -> str:
+        return self.fortran_type_attribute_declaration
+
     @attribute_specifications.validator
     def _check_attribute_specifications(
         self,
         attribute: Any,
         value: tuple[Union[str, DimensionAttributeSpecification], ...],
     ) -> None:
-        dimension_count = sum(isinstance(a, DimensionAttributeSpecification) for a in value)
+        dimension_count = sum(
+            isinstance(a, DimensionAttributeSpecification) for a in value
+        )
         if dimension_count > 1:
             raise ValueError(  # noqa: TRY003
-                "More than one dimension attribute specification (can Fortran be compiled with "
-                "more than one dimension attribute specification?)"
+                "More than one dimension attribute specification "
+                "(can Fortran be compiled "
+                "with more than one dimension attribute specification?)"
             )
 
     @classmethod
     def from_str(cls, fortran_type_attribute_declaration: str) -> FortranDataType:
         """
         Create :obj:`FortranDataType` from type declaration statement
 
         Parses and validates a type declaration statement
 
         Parameters
         ----------
         fortran_type_attribute_declaration
-            Fortran type declaration statement e.g. "real(8), dimension(2) :: heat_uptake_sensitivity"
+            Fortran type declaration statement
 
-            The entity declaration component (including and after "::") is ignored hence is optional.
+            For example, "real(8), dimension(2) :: heat_uptake_sensitivity"
+
+            The entity declaration component (including and after "::")
+            is ignored hence is optional.
 
             See the docstring of :mod:`fgen.fortran_parsing` for further details.
 
         Raises
         ------
         ValueError
             The type declaration statement is invalid
         """
-        type_specification, attribute_specifications = _get_parts(fortran_type_attribute_declaration)
-        _validate_fortran_type_attribute_declaration(type_specification, attribute_specifications)
+        type_specification, attribute_specifications = _get_parts(
+            fortran_type_attribute_declaration
+        )
+        _validate_fortran_type_attribute_declaration(
+            type_specification, attribute_specifications
+        )
 
         return cls(
             type_specification=type_specification,
-            attribute_specifications=_convert_complex_attribute_specifications(attribute_specifications),
+            attribute_specifications=_convert_complex_attribute_specifications(
+                attribute_specifications
+            ),
         )
 
     @property
     def fortran_type_attribute_declaration(self) -> str:
         """
-        Fortran type attribute declaration, including attribute specifications if applicable.
+        Fortran type attribute declaration, including attribute specifications.
+
+        Attribute specifications are only included if they are applicable.
 
         See the docstring of :mod:`fgen.fortran_parsing` for further details.
         """
         if not self.attribute_specifications:
             return self.type_specification
 
-        attribute_specifications = ", ".join(str(item) for item in self.attribute_specifications)
+        attribute_specifications = ", ".join(
+            str(item) for item in self.attribute_specifications
+        )
         return f"{self.type_specification}, {attribute_specifications}"
 
-    def __str__(self) -> str:
-        return self.fortran_type_attribute_declaration
+    @property
+    def python_equivalent_type_annotation(self) -> str:
+        """
+        Type annotation for the python-equivalent of this Fortran type
+        """
+        base_type = self._base_python_type()
+        dimension_attribute_specification = self.dimension_attribute_specification
+        if not dimension_attribute_specification:
+            return base_type
+
+        # TODO: Remove this.
+        # This custom handling of shapes will be silly if we have an array of say,
+        # size 100, so it makes more sense to just use numpy return types here.
+        return _get_python_type_with_dimensions(
+            dimension_attribute_specification.dimensions, base_type
+        )
+
+    @property
+    def is_array(self) -> bool:
+        """
+        Whether this instance represents an array or not.
+
+        Returns
+        -------
+            ``True`` if self represents an array, ``False`` otherwise.
+        """
+        return self.dimension_attribute_specification is not None
+
+    @property
+    def has_deferred_size(self) -> bool:
+        """
+        Whether this instance represents a type with a deferred size or not.
+
+        Returns
+        -------
+            ``True`` if self represents a type with a deferred size,
+            ``False`` otherwise.
+        """
+        return ":" in self.fortran_type_attribute_declaration
+
+    @property
+    def is_character(self) -> bool:
+        """
+        Whether this instance represents a character type
+
+        Returns
+        -------
+            ``True`` if self represents a character type, ``False`` otherwise.
+        """
+        return self.type_specification.startswith("character")
+
+    @property
+    def is_logical(self) -> bool:
+        """
+        Whether this instance represents a logical type
+
+        Returns
+        -------
+            ``True`` if self represents a logical type, ``False`` otherwise.
+        """
+        return self.type_specification.startswith("logical")
+
+    @property
+    def is_float_double(self) -> bool:
+        """
+        Whether this instance represents a type which is a floating double-point type.
+
+        Returns
+        -------
+            ``True`` if self represents a type which is a floating double-point type,
+            ``False`` otherwise.
+        """
+        return "real" in self.type_specification and "8" in self.type_specification
+
+    @property
+    def is_derived_type(self) -> bool:
+        """
+        Whether this instance represents a type which is a derived type
+
+        Returns
+        -------
+            ``True`` if self represents a type which is a derived type
+            ``False`` otherwise.
+            True if a type is a derived type, False if it is an intrinsic type
+        """
+        return self.type_specification.startswith("type(")
+
+    @property
+    def is_pointer(self) -> bool:
+        """
+        Whether this instance represents a type which is a pointer
+
+        Returns
+        -------
+            ``True`` if self represents a type which is a pointer
+            ``False`` otherwise.
+        """
+        return "pointer" in self.attribute_specifications
+
+    @property
+    def is_deferred_array(self) -> bool:
+        """
+        Whether this instance represents a deferred size array
+
+        Returns
+        -------
+            ``True`` if self represents a type which is a deferred size array
+            ``False`` otherwise.
+        """
+        dim_attrs = self.dimension_attribute_specification
+
+        if dim_attrs is None:
+            return False
+        return ":" in dim_attrs.dimensions
+
+    @property
+    def is_enum(self) -> bool:
+        """
+        Whether this instance represents a type which is an enum.
+
+        Returns
+        -------
+            ``True`` if self represents a type which is an enum.
+            ``False`` otherwise.
+        """
+        # Hmm, not sure whether integer(kind(8)) is valid Fortran
+        # and would trip this up....
+        return (
+            "integer" in self.type_specification and "kind(" in self.type_specification
+        )
 
     @property
     def equivalent_python_type(self) -> str:
         """
         Python type-hint for the data type
 
         The "base" type of the equivalent Python type will be:
 
-        * `str` for `character`-based types
-        * `bool` for `logical`-based types
-        * `pint.Quantity` for other intrinsic types such as `real` and `integer`
-        * a custom type for (Fortran) derived types
-
-        If the Fortran type has a "dimension" attribute specification, this modifies the "base" type
-        to a `tuple` that respects the intended shape of the value. n-dimensional variables are supported.
+        If the Fortran type has a "dimension" attribute specification,
+        this modifies the "base" type to a `tuple`
+        that respects the intended shape of the value.
+        n-dimensional variables are supported.
+        TODO: remove this behaviour, doesn't scale well to long arrays
+        and doesn't help with deferred shape arrays.
         """
         base_type = self._base_python_type()
-        dimension_attribute_specification = self._get_dimension_attribute_specification()
+        dimension_attribute_specification = self.dimension_attribute_specification
 
         if base_type != "Quantity" and dimension_attribute_specification:
-            # Pint doesn't support dimension attributes so we only do this if the Python type is not
-            # a pint type
-            return _get_python_type_with_dimensions(dimension_attribute_specification.dimensions, base_type)
+            # Pint doesn't support dimension attributes
+            # so we only do this if the Python type is not a pint type
+            return _get_python_type_with_dimensions(
+                dimension_attribute_specification.dimensions, base_type
+            )
 
         return base_type
 
     def _base_python_type(self) -> str:
         """
         Determine the "base" Python type that represents the Fortran type declaration
 
-        This focuses on the base type (float, int etc.) and ignores the modification of this type
-        from attributes such as "dimension" (which mean the 'full' python type is some sort of array
-        or iterable). Such dimension handling is done in :attr:`~equivalent_python_type`.
+        This focuses on the base type (float, int etc.)
+        and ignores the modification of this type from attributes such as "dimension"
+        (which mean the 'full' python type is some sort of array or iterable).
+        Such dimension handling is done in :attr:`~equivalent_python_type`.
 
         Returns
         -------
-            The string representation of the python type that is equivalent to the base type
+            The string representation of the python type
+            that is equivalent to the base type
             (i.e. ignoring any array or other container) of ``self``
         """
-        if self.is_derived_type():
-            match = re.match(_DERIVED_TYPE_REGEX, self.type_specification, flags=re.IGNORECASE)
+        if self.is_derived_type:
+            match = re.match(
+                _DERIVED_TYPE_REGEX, self.type_specification, flags=re.IGNORECASE
+            )
             if not match:
-                raise ValueError(  # noqa: TRY003
+                raise ValueError(  # noqa: TRY003 # pragma: no cover # should be impossible to get here
                     f"Could not determine python type for {self.type_specification}"
                 )
 
             return match.group("derived_type_name").strip()
 
         else:
             tsl = self.type_specification.lower()
 
             if tsl.startswith("real"):
                 return "float"
 
             if tsl.startswith("integer"):
+                match = re.match(
+                    _ENUM_LIKE_REGEX, self.type_specification, flags=re.IGNORECASE
+                )
+                if match:
+                    return match.group("enum_name").strip()
+
                 return "int"
 
             if tsl.startswith("character"):
                 return "str"
 
             if tsl.startswith("logical"):
                 return "bool"
@@ -614,37 +837,20 @@
             if tsl.startswith("complex"):
                 msg = (
                     "We have not yet worked out how to support "
                     f"{self.type_specification}, please raise an issue"
                 )
                 raise NotImplementedError(msg)
 
-            raise ValueError(self.type_specification)
-
-    def is_derived_type(self) -> bool:
-        """
-        Check if the fortran type is a derived type
-
-        Returns
-        -------
-            True if a type is a derived type, False if it is an intrinsic type
-        """
-        return self.type_specification.startswith("type(")
-
-    def is_deferred_array(self) -> bool:
-        """
-        Check if the fortran type is an array with at least one deferred dimension
-        """
-        dim_attrs = self._get_dimension_attribute_specification()
-
-        if dim_attrs is None:
-            return False
-        return ":" in dim_attrs.dimensions
+            raise ValueError(  # pragma: no cover # not sure how you could reach here
+                self.type_specification
+            )
 
-    def _get_dimension_attribute_specification(
+    @property
+    def dimension_attribute_specification(
         self,
     ) -> Optional[DimensionAttributeSpecification]:
         """
         Get the dimension attribute of the type if it exists
 
         Returns
         -------
```

### Comparing `fgen-0.3.1/src/fgen/templator.py` & `fgen-0.4.1/src/fgen/jinja_environment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,167 @@
 """
-Output file generation from templates
+Jinja environment to use while generating wrappers
 """
-import functools
-import os
-from typing import Callable
-
-from black import Mode, format_str
-from jinja2 import Environment, PackageLoader, select_autoescape
-from loguru import logger
-
-from fgen.models import ModuleDefinition
-
-env = Environment(
-    loader=PackageLoader("fgen"),
-    autoescape=select_autoescape(),
+
+from __future__ import annotations
+
+from pathlib import Path
+
+import jinja2
+
+JINJA_ENV = jinja2.Environment(
+    loader=jinja2.FileSystemLoader(Path(__file__).parent.absolute()),
+    autoescape=jinja2.select_autoescape(),
     trim_blocks=True,
     lstrip_blocks=True,
+    undefined=jinja2.StrictUndefined,
 )
+"""Jinja2 environment to use for template rendering"""
 
 
-def _add_trailing_line(inp: str) -> str:
-    # jinja trims the trailing line-break from the template
-    return inp + "\n"
-
-
-def generate_calculator_manager(module: ModuleDefinition) -> str:
-    """
-    Generate manager module for a module
+def indent_based_on_first_line(
+    code: str,
+    indent: str,
+) -> str:
+    """
+    Indent code based on the indent of the first line.
+
+    If the first line does not have indent equal to ``indent``,
+    all the code except the first line
+    will have an indent added
+    such that the first line would have an indent of ``indent``.
+    We exclude the first line
+    so that the indent can be included in the jinja template too,
+    which makes it easier to read what is going on.
 
     Parameters
     ----------
-    module
-        Module configuration
+    code
+        Code to indent
+
+    indent
+        Indent to ensure that the first line has
 
-        Each module contains a single calculator
 
     Returns
     -------
-        Serialised fortran code
+        Indented code
     """
-    template = env.get_template("calculator_manager.f90.jinja")
+    if not code:
+        # Empty line
+        return code
 
-    result = _add_trailing_line(
-        template.render(
-            module=module,
-            calculator=module.provides,
-        )
-    )
+    code_split = code.splitlines()
+
+    if len(code_split) == 1:
+        # Nothing to indent
+        return code
 
-    return result
+    first_line = code_split[0]
+
+    first_line_indent = len(first_line) - len(first_line.lstrip())
+    indent_len = len(indent)
+    if first_line_indent >= indent_len:
+        return code
+
+    required_extra_indent = " " * (indent_len - first_line_indent)
+
+    after_first_line = code_split[1:]
+    return "\n".join(
+        [first_line, *[f"{required_extra_indent}{line}" for line in after_first_line]]
+    )
 
 
-def generate_python_module(module: ModuleDefinition, extension: str) -> str:
+def strip_empty_lines(inp: str) -> str:
     """
-    Generate python module for a calculator
+    Strip empty lines
+
+    More specifically, turn lines
+    that only have whitespace into a single newline character.
+    This is a workaround until we start formatting our Fortran
+    as part of the generation process
+    (https://gitlab.com/magicc/fgen/-/issues/26).
 
     Parameters
     ----------
-    module
-        Module configuration
-
-        Each module contains a single calculator
-    extension
-        Name of the extension module that will contain the compiled wrappers
+    inp
+        Input string
 
     Returns
     -------
-        Serialised python code
+        Input string, with all whitespace lines replaced by a single newline character.
     """
-    template = env.get_template("python_module.py.jinja")
+    out = [line if line.strip() else "\n" for line in inp.splitlines()]
+
+    return "\n".join(out)
 
-    result = _add_trailing_line(
-        template.render(module=module, calculator=module.provides, extension=extension)
-    )
-    # Format result with black
-    # This doesn't automatically read `pyproject.toml` so settings must be prescribed
-    return format_str(result, mode=Mode(line_length=88))
 
+JINJA_ENV.filters["indent_based_on_first_line"] = indent_based_on_first_line
+JINJA_ENV.filters["strip_empty_lines"] = strip_empty_lines
 
-def generate_wrap_module(module: ModuleDefinition) -> str:
+
+def get_template_in_directory(
+    template_name: str, template_directory: Path, env: jinja2.Environment
+) -> jinja2.Template:
     """
-    Generate the fortran wrapper for a module
+    Get template that is in the directory specified by ``file_dunder``
 
     Parameters
     ----------
-    module
-        Module configuration
+    template_name
+        Name of the template to get
+
+    template_directory
+        The directory from which to retrieve the template.
 
-        Each module contains a single calculator
+        If you want to retrieve a template in the same directory as the file
+        that is calling this function,
+        call ``get_template_in_directory(template_name, Path(__file__).parent), env)``.
+
+    env
+        Jinja2 environment to use when loading the template.
+        This must be using a :obj:`jinja2.loaders.FileSystemLoader` loader.
+        The loader must only have one search path.
 
     Returns
     -------
-        Serialised fortran code
+        Loaded template
     """
-    template = env.get_template("wrap_module.f90.jinja")
+    if not isinstance(env.loader, jinja2.loaders.FileSystemLoader):
+        raise NotImplementedError(f"{env.loader=}")
 
-    result = _add_trailing_line(
-        template.render(
-            module=module,
-            calculator=module.provides,
-            calculator_module=f"mod_{ module.short_name }_manager",
+    if len(env.loader.searchpath) > 1:
+        raise NotImplementedError(
+            f"More than one search path: {env.loader.searchpath=}"
         )
-    )
-
-    return result
 
+    loader_searchpath = env.loader.searchpath[0]
 
-def _write_file(data: str, filename: str, force: bool = False) -> None:
-    if os.path.exists(filename):
-        if force:
-            logger.warning(f"Forcefully overwriting existing file: {filename}")
-        else:
-            raise FileExistsError(filename)
+    template_path = (template_directory / template_name).relative_to(loader_searchpath)
 
-    with open(filename, mode="w", encoding="utf-8") as file_handle:
-        file_handle.write(data)
+    return env.get_template(str(template_path))
 
 
-def process_module(  # noqa: PLR0913
-    module: ModuleDefinition,
-    extension: str,
-    manager_directory: str,
-    wrapper_directory: str,
-    python_directory: str,
-    force: bool = True,
-) -> None:
+def post_process_jinja_rendering(inp: str) -> str:
     """
-    Autogenerate python and fortran code according to a module definition
+    Post-process the result from Jinja
 
-    This function writes 3 files:
-
-    * manager - Lifecycle handling for calculators (in Fortran)
-    * wrapper - Provides a fortran wrapper to the generated functions that can be
-      made available to Python
-    * python module - Python interface for creating and manipulating calculators.
+    This fixes things we can't work out how to fix with jinja
 
     Parameters
     ----------
-    module
-
-    extension
-        Package name for the compiled extension module
+    inp
+        Result of formatting with jinja
 
-        Typically, this is of the form `my_module._lib`
-
-    manager_directory
-        Directory to write the manager module
-
-        This is typically beside the yaml file describing the module and the calculator
-
-    wrapper_directory
-        Directory to write the wrapper module
-
-        This is typically ``libmagicc/wrappers``
-
-    python_directory
-        Directory to write the python module
-
-        This is typically in magiccly under ``_lib``
-
-    force
-        If True, overwrite any existing files
-
-    Raises
-    ------
-    FileExistError
-        If ``not force`` and a targeted file exists
-    """
-    template_config: tuple[tuple[str, Callable[[ModuleDefinition], str], str, str], ...] = (
-        (
-            "manager",
-            generate_calculator_manager,
-            "_manager.f90",
-            manager_directory,
-        ),
-        ("wrapper", generate_wrap_module, "_wrapped.f90", wrapper_directory),
-        (
-            "python",
-            functools.partial(generate_python_module, extension=extension),
-            ".py",
-            python_directory,
-        ),
-    )
+    Returns
+    -------
+        Post-processed result
+    """
+    # Strip out two blank lines in a row
+    two_blank_lines = "\n\n\n"
+    one_blank_line = "\n\n"
+    while two_blank_lines in inp:
+        inp = inp.replace(two_blank_lines, one_blank_line)
 
-    for desc, generator_function, suffix, outdir in template_config:
-        try:
-            filename = os.path.join(outdir, f"{module.short_name}{suffix}")
-            logger.info(f"Writing {desc} module to {filename}")
-            _write_file(generator_function(module), filename, force=force)
-        except Exception:
-            logger.exception("One or more files maybe partly written")
-            raise
+    # Jinja trims the trailing line-break from the end of the rendered text,
+    # add that back in too
+    return inp + "\n"
```

### Comparing `fgen-0.3.1/src/fgen_runtime/arrays.py` & `fgen-0.4.1/src/fgen_runtime/arrays.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     result_type = _ctype_ndarray(ctype_scalar, shape)
     result = result_type.from_address(ptr)
 
     d = np.ascontiguousarray(result).T
 
     exp = (ptr, False)
     if d.__array_interface__["data"] != exp:
-        raise PointerArrayConversionError(array=d, ptr=ptr, expected_array_interface_data=exp)
+        raise PointerArrayConversionError(
+            array=d, ptr=ptr, expected_array_interface_data=exp
+        )
 
     return d
 
 
 @functools.lru_cache(128)
 def ftype_to_np(type_specification: str) -> str:
     """
@@ -58,15 +60,16 @@
     Only supports logical, integer and real types.
 
     Parameters
     ----------
     type_specification
         Type specification
 
-        See :mod:`fgen.fortran_parsing` for more information about fortran type specifications
+        See :mod:`fgen.fortran_parsing`
+        for more information about fortran type specifications.
 
     Returns
     -------
         A numpy equivalent dtype (where possible)
 
     Raises
     ------
```

### Comparing `fgen-0.3.1/src/fgen_runtime/base.py` & `fgen-0.4.1/src/fgen_runtime/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Base class for wrapped calculators
+Base class for wrapped derived types
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from contextlib import AbstractContextManager
 from functools import wraps
 from types import TracebackType
@@ -12,31 +12,32 @@
 import attrs
 from attrs import define, field
 from typing_extensions import Concatenate, ParamSpec
 
 from fgen_runtime.exceptions import InitialisationError
 from fgen_runtime.units import FuncT
 
-INVALID_MODEL_INDEX: int = -1
+INVALID_INSTANCE_INDEX: int = -1
 """
-Value used to denote an invalid ``model_index``.
+Value used to denote an invalid ``instance_index``.
 
-This can occur value when a wrapper class has not yet been initialised (connected to a Fortran instance).
+This can occur value when a wrapper class
+has not yet been initialised (connected to a Fortran instance).
 """
 
 
 @define
 class FinalizableWrapperBase(ABC):
     """
     Base class for model wrappers
     """
 
-    model_index: int = field(
+    instance_index: int = field(
         validator=attrs.validators.instance_of(int),
-        default=INVALID_MODEL_INDEX,
+        default=INVALID_INSTANCE_INDEX,
     )
     """
     Model index of wrapper Fortran instance
     """
 
     @classmethod
     @abstractmethod
@@ -47,37 +48,38 @@
         This requests a new model index from the Fortran module and then
         initialises a class instance
 
         Returns
         -------
         New class instance
         """
+        ...
 
     @abstractmethod
     def finalize(self) -> None:
         """
         Finalise the Fortran instance and set self back to being uninitialised
 
-        This method resets ``self.model_index`` back to
-        ``_UNINITIALISED_MODEL_INDEX``
+        This method resets ``self.instance_index`` back to
+        ``_UNINITIALISED_instance_index``
 
         Should be decorated with :func:`check_initialised`
         """
         # call to Fortran module goes here when implementing
-        self._uninitialise_model_index()
+        self._uninitialise_instance_index()
 
-    def _uninitialise_model_index(self) -> None:
-        self.model_index = INVALID_MODEL_INDEX
+    def _uninitialise_instance_index(self) -> None:
+        self.instance_index = INVALID_INSTANCE_INDEX
 
     @property
     def initialized(self) -> bool:
         """
         Is the instance initialised, i.e. connected to a Fortran instance?
         """
-        return self.model_index != INVALID_MODEL_INDEX
+        return self.instance_index != INVALID_INSTANCE_INDEX
 
 
 @define
 class FinalizableWrapperBaseContext(AbstractContextManager):  # type: ignore
     """
     Context manager for a wrapper
     """
@@ -165,22 +167,22 @@
         Passed to ``func_to_try``
 
     **kwargs
         Passed to ``func_to_try``
 
     Returns
     -------
-    Result of calling ``func_to_try(inst.model_index, *args, **kwargs)``
+    Result of calling ``func_to_try(inst.instance_index, *args, **kwargs)``
 
     Raises
     ------
     Exception
         Any exception which occurs when calling ``func_to_try. Before the
         exception is raised, ``inst.finalize()`` is called.
     """
     try:
-        return func_to_try(inst.model_index, *args, **kwargs)
+        return func_to_try(inst.instance_index, *args, **kwargs)
     except RuntimeError:
         # finalize the instance before raising
         inst.finalize()
 
         raise
```

### Comparing `fgen-0.3.1/src/fgen_runtime/exceptions.py` & `fgen-0.4.1/src/fgen_runtime/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 
 class InitialisationError(WrapperError):
     """
     Raised when the wrapper around the Fortran module hasn't been initialised yet
     """
 
-    def __init__(self, model: Any, method: Optional[Callable[..., Any]] = None):
+    def __init__(self, instance: Any, method: Optional[Callable[..., Any]] = None):
         if method:
-            error_msg = f"{model} must be initialised before {method} is called"
+            error_msg = f"{instance} must be initialised before {method} is called"
         else:
-            error_msg = f"model ({model:r}) is not initialized yet"
+            error_msg = f"instance ({instance:r}) is not initialized yet"
 
         super().__init__(error_msg)
 
 
 class CompiledExtensionNotFoundError(ImportError):
     """
     Raised when a compiled extension can't be import i.e. found
@@ -83,14 +83,32 @@
             f"The expected value is {expected_array_interface_data}. "
             f"Full context: {ptr=} {array.__array_interface__=}"
         )
 
         super().__init__(error_msg)
 
 
+class UnallocatedMemoryError(ValueError):
+    """
+    Raised when we try to allocate memory that has not yet been allocated
+
+    We can't always catch this error, but this is what we raise when we can.
+    """
+
+    def __init__(self, variable_name: str):
+        error_msg = (
+            f"The memory required to access ``{variable_name}`` is unallocated. "
+            "You must allocate it before trying to access its value. "
+            "Unfortunately, we cannot provide more information "
+            "about why this memory is not yet allocated."
+        )
+
+        super().__init__(error_msg)
+
+
 class RelativePythonModuleNotFoundError(ImportError):
     """
     Raised when a Python import configured by fgen fails
     """
 
     def __init__(
         self,
@@ -120,7 +138,15 @@
             "Somewhere (likely in the `.yaml` file which is used to generate "
             f"{requesting_python_module!r} with fgen) you are specifying that "
             f"{requested!r} can be imported from "
             f"{requested_from_python_module!r}, but this is failing."
         )
 
         super().__init__(error_msg)
+
+
+class SolveError(ValueError):
+    """
+    Exception raised when an solver can't solve
+
+    For example, because the integration has a runaway effect in it
+    """
```

### Comparing `fgen-0.3.1/PKG-INFO` & `fgen-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: fgen
-Version: 0.3.1
+Version: 0.4.1
 Summary: Automatically generate wrapper to integrate Fortran and Python
 Home-page: https://gitlab.com/magicc/fgen
 License: BSD-3-Clause
 Keywords: fortran
-Author: Jared Lewis
-Author-email: jared.lewis@climate-energy-college.org
+Author: Zebedee Nicholls
+Author-email: zebedee.nicholls@climate-energy-college.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
+Provides-Extra: templates
 Requires-Dist: attrs (>=23.0.0,<24.0.0)
-Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0) ; extra == "templates"
 Requires-Dist: cattrs (>=23.0.0,<24.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
-Requires-Dist: cmakelang (>=0.6.13,<0.7.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "templates"
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: openscm-units (>=0.5.0,<0.6.0)
+Requires-Dist: numpy (>1.23)
+Requires-Dist: pint
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Fortran-Python wrapper
 
 <!---
 Can use start-after and end-before directives in docs, see
 https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html#inserting-other-documents-directly-into-the-current-document
@@ -56,19 +58,18 @@
 We recommend reading the docs there because the internal documentation links
 don't render correctly on GitLab's viewer. TODO: Create docs
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
-Fortran-Python wrapper can be installed with conda or pip:
+fgen can be installed with pip:
 
 ```bash
 pip install fgen
-conda install -c conda-forge fgen
 ```
 
 ## Usage
 
 TODO
 
 ### libfgen
@@ -125,15 +126,14 @@
 
 Once the virtual environment has been created, `libfgen` can be built
 using `make build`. This library contains the common Fortran code used by
 all wrappers and uses [CMake](https://cmake.org/) to build and requires
 a working Fortran compiler.
 
 If there are any issues, the messages from the `Makefile` should guide you
-through. If not, please raise an issue in the [issue tracker][issue_tracker].
+through. If not, please raise an issue in the
+[issue tracker](https://gitlab.com/magicc/fgen/issues).
 
 For the rest of our developer docs, please see [](development-reference).
 
-[issue_tracker]: https://gitlab.com/magicc/fgen/issues
-
 <!--- sec-end-installation-dev -->
```

