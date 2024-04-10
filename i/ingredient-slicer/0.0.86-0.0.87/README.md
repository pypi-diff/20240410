# Comparing `tmp/ingredient_slicer-0.0.86.tar.gz` & `tmp/ingredient_slicer-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-0.0.86.tar", last modified: Mon Apr  8 13:04:33 2024, max compression
+gzip compressed data, was "ingredient_slicer-0.0.87.tar", last modified: Wed Apr 10 14:54:57 2024, max compression
```

## Comparing `ingredient_slicer-0.0.86.tar` & `ingredient_slicer-0.0.87.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.082558 ingredient_slicer-0.0.86/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.070824 ingredient_slicer-0.0.86/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.072533 ingredient_slicer-0.0.86/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.86/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.86/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.86/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.86/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3263 2024-04-08 13:04:33.082302 ingredient_slicer-0.0.86/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2289 2024-04-06 15:25:45.000000 ingredient_slicer-0.0.86/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.073747 ingredient_slicer-0.0.86/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-08 13:04:23.000000 ingredient_slicer-0.0.86/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   155365 2024-04-06 15:22:08.000000 ingredient_slicer-0.0.86/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   104930 2024-04-08 13:03:20.000000 ingredient_slicer-0.0.86/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-06 13:59:47.000000 ingredient_slicer-0.0.86/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    92634 2024-04-07 20:58:21.000000 ingredient_slicer-0.0.86/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.081671 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3263 2024-04-08 13:04:33.000000 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     1922 2024-04-08 13:04:33.000000 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-08 13:04:33.000000 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-08 13:04:33.000000 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-08 13:04:33.000000 ingredient_slicer-0.0.86/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-08 13:04:25.000000 ingredient_slicer-0.0.86/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-08 13:04:33.082612 ingredient_slicer-0.0.86/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-08 13:04:33.081452 ingredient_slicer-0.0.86/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.86/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.86/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5832 2024-03-29 21:20:16.000000 ingredient_slicer-0.0.86/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.86/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.86/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.86/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.86/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.86/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.86/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.86/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.86/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.86/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.86/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.86/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-0.0.86/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-06 15:22:20.000000 ingredient_slicer-0.0.86/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.86/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-03-29 21:19:46.000000 ingredient_slicer-0.0.86/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.86/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.86/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.86/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.86/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.86/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.86/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11034 2024-03-29 21:19:23.000000 ingredient_slicer-0.0.86/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.86/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.86/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.86/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.86/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.86/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.86/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.86/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.86/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.86/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.86/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.86/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.86/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.86/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.86/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.86/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.86/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.647555 ingredient_slicer-0.0.87/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.634620 ingredient_slicer-0.0.87/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.636262 ingredient_slicer-0.0.87/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-03-30 17:04:31.000000 ingredient_slicer-0.0.87/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-0.0.87/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-0.0.87/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-0.0.87/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-10 14:54:57.647269 ingredient_slicer-0.0.87/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-0.0.87/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.637438 ingredient_slicer-0.0.87/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1491 2024-04-10 14:53:27.000000 ingredient_slicer-0.0.87/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   155518 2024-04-10 14:53:06.000000 ingredient_slicer-0.0.87/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   105302 2024-04-10 14:53:09.000000 ingredient_slicer-0.0.87/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   108094 2024-04-10 14:53:09.000000 ingredient_slicer-0.0.87/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    98187 2024-04-10 14:53:05.000000 ingredient_slicer-0.0.87/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.646577 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3363 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2021 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-04-10 14:54:57.000000 ingredient_slicer-0.0.87/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1125 2024-04-10 14:54:41.000000 ingredient_slicer-0.0.87/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-04-10 14:54:57.647611 ingredient_slicer-0.0.87/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-04-10 14:54:57.646342 ingredient_slicer-0.0.87/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-0.0.87/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-0.0.87/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-0.0.87/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-0.0.87/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-0.0.87/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-0.0.87/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-0.0.87/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-0.0.87/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-0.0.87/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-0.0.87/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-0.0.87/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-0.0.87/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24889 2024-04-06 13:04:35.000000 ingredient_slicer-0.0.87/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20385 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-0.0.87/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.87/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-0.0.87/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-0.0.87/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-0.0.87/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-0.0.87/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-0.0.87/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-0.0.87/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-0.0.87/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-0.0.87/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-0.0.87/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-0.0.87/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-0.0.87/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-0.0.87/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-0.0.87/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-0.0.87/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-0.0.87/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-0.0.87/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-0.0.87/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-0.0.87/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-0.0.87/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-0.0.87/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-0.0.87/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-0.0.87/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-0.0.87/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-0.0.86/.github/workflows/publish-to-pypi.yml` & `ingredient_slicer-0.0.87/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-0.0.87/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/.gitignore` & `ingredient_slicer-0.0.87/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/LICENSE` & `ingredient_slicer-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/PKG-INFO` & `ingredient_slicer-0.0.87/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.86
+Version: 0.0.87
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -58,24 +58,25 @@
 
 import ingredient_slicer
 
 slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
 
 slicer.to_json()
 
-{
+{   
+    'ingredient': '2 (15-ounces) cans chickpeas, rinsed and drained', 
     'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
     'food': 'chickpeas', 
 
-    # primary units
+    # primary quantity and units
     'quantity': '30', 
     'unit': 'ounces', 
     'standardized_unit': 'ounce', 
 
-    # any other secondary units found in the string
+    # any other secondary quantity and units found in the string
     'secondary_quantity': '2', 
     'secondary_unit': 'cans', 
     'standardized_secondary_unit': 'can', 
 
     'gram_weight': '850.49', 
     'prep': ['drained', 'rinsed'], 
     'size_modifiers': [],
```

### Comparing `ingredient_slicer-0.0.86/README.md` & `ingredient_slicer-0.0.87/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,25 @@
 
 import ingredient_slicer
 
 slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
 
 slicer.to_json()
 
-{
+{   
+    'ingredient': '2 (15-ounces) cans chickpeas, rinsed and drained', 
     'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
     'food': 'chickpeas', 
 
-    # primary units
+    # primary quantity and units
     'quantity': '30', 
     'unit': 'ounces', 
     'standardized_unit': 'ounce', 
 
-    # any other secondary units found in the string
+    # any other secondary quantity and units found in the string
     'secondary_quantity': '2', 
     'secondary_unit': 'cans', 
     'standardized_secondary_unit': 'can', 
 
     'gram_weight': '850.49', 
     'prep': ['drained', 'rinsed'], 
     'size_modifiers': [],
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer/__init__.py` & `ingredient_slicer-0.0.87/ingredient_slicer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "0.0.86"
+__version__ = "0.0.87"
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP
 
 from ._ingredient_slicer import IngredientSlicer
 # from ._regex_patterns import IngredientTools
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer/_constants.py` & `ingredient_slicer-0.0.87/ingredient_slicer/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,39 +472,45 @@
     "huge",
     "giant",
     "gigantic"
     ))
 
 PREP_WORDS = {
     'baked',
+    'batonnet',
+    'batonnetted',
     'beaten',
     'beating',
     'beat',
     'blended',
     'blending',
     'blend',
     'blanch',
     'blanched',
     'blistered',
     'boil',
     'boiled',
     'broil',
     'broiled',
+    "chilled",
     'chopped',
     'chopping',
     'cored',
     'cracked',
     'cracking',
     'cooked',
     'crumbled',
     'crushed',
     'cubed',
     'cut',
     'cutting',
     'crisped',
+    'deboned',
+    'deveined',
+    'decored',
     'diced',
     'divided',
     'drained',
     'drenched',
     'dressed',
     'emulsified',
     "even",
@@ -528,14 +534,17 @@
     'juiced',
     "level",
     "leveled",
     "light",
     "lightly",
     "lightly packed",
     'mashed',
+    "matchstick",
+    "matchsticks",
+    "matchsticked",
     'melted',
     'minced',
     'packed',
     'peeled',
     'pitted',
     'poached',
     # 'pounded',
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-0.0.87/ingredient_slicer/_ingredient_slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,14 +1002,22 @@
 
         # if no numbers only parenthesis, then just return the original ingredient
         if not numbers_only:
             # print(f"\n > Return early from QUANTITY parenthesis") if self.debug else None
             description = f"not a quantity only parenthesis"
             self._parenthesis_notes.append(description)
             return
+        
+        is_approximate_quantity = _utils._is_approximate_quantity_only_parenthesis(parenthesis)
+
+        # if the quantity is approximate, then add a note to the parenthesis notes and return early
+        if is_approximate_quantity:
+            description = f"approximate quantity only"
+            self._parenthesis_notes.append(description)
+            return
 
         # pull out the self._quantity from the parenthesis
         parenthesis_quantity = numbers_only[0]
 
         # if there is not a unit or a quantity, then we can use the parenthesis number as the quantity and
         #  return the ingredient with the new quantity
         # TODO: OR the unit MIGHT be the food OR might be a "SOMETIMES_UNIT", maybe do that check here, not sure yet...
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-0.0.87/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer/_utils.py` & `ingredient_slicer-0.0.87/ingredient_slicer/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -854,17 +854,143 @@
 
         for pair in quantity_unit_pairs:
             new_triplet = (trailing_approx_string, pair[0], pair[1])
             approximate_triplets.append(new_triplet)
             # pair.append(trailing_approx_string)
         # [i.append(trailing_approx_string) for i in quantity_unit_pairs]
         # print()
-
+    
+    # return [tuple(i) for i in approximate_triplets]
     return approximate_triplets
+
+def _is_approximate_quantity_only_parenthesis(input_string: str) -> bool:
+    """Check if a string is an approximate quantity only parenthesis (e.g. "(about 12)")"""
+
+    # input_string = "(about 4)"
+    # input_string = '(about 12 tender and juicy ounces or about 14 grams)'
+    # input_string = '(juicy about or 14)'
+    # input_string = '(12 tender and juicy ounces or 14 grams about)'
+
+    if not isinstance(input_string, str):
+        return False
+
+    approximate_string_matches = _regex_patterns.APPROXIMATE_STRINGS_PATTERN.findall(input_string)
+    quantity_matches           = _regex_patterns.ALL_NUMBERS.findall(input_string)
+    unit_matches               = _regex_patterns.UNITS_PATTERN.findall(input_string)
+
+    has_approximate_string = True if approximate_string_matches else False
+    has_quantity           = True if quantity_matches else False
+    has_unit               = True if unit_matches else False
+
+    if has_unit:
+        return False
+    
+    approximate_and_quantity_only = has_approximate_string and has_quantity
+
+    return approximate_and_quantity_only
+
+def _extract_equivalent_quantity_only(input_string: str) -> list[tuple]:
+
+    """From a string get all sets of quantity/units preceeded by "approximate" strings, (e.g. "about", "approximately", "around", etc.)
+    
+    Useful for getting instances where there is a quantity and unit in parenthesis that is 
+    an approximation of the quantity and unit in the main ingredient string (e.g. "1 cup of chopped chicken breast (about 12 ounces)")
+
+    Args:
+        input_string (str): The string to parse
+    Returns:
+        list: A list of tuples containing the (approximate string, quantity, and unit)
+    """
+
+    # input_string = parenthesis
+    # input_string = "(about 4)"
+    # input_string = '(about 12 tender and juicy ounces or about 14 grams)'
+    # input_string = '(juicy about or 14)'
+    # input_string = '(12 tender and juicy ounces or 14 grams about)'
+
+    if not isinstance(input_string, str):
+        raise ValueError("Invalid input. Input must be a string.")
+
+    # regex_patterns = _regex_patterns.IngredientTools()
+
+    approximate_string_matches = _regex_patterns.APPROXIMATE_STRINGS_PATTERN.finditer(input_string)
+    
+    unit_matches = _regex_patterns.UNITS_PATTERN.findall(input_string)
+    has_units = True if unit_matches else False
+
+    if has_units:
+        return []
+
+    approximate_triplets = []
+
+    for match in approximate_string_matches:
+        match_string = match.group()
+        start, end = match.start(), match.end()
+
+        # print(f"Match String: '{match_string}'")
+        # print(f"Start: {start} | End: {end}")
+        # print(f"Input String: '{input_string}'")
+        current_result = []
+        
+        current_result.append(match_string) # add the approximate string to the result
+
+        str_after_approx_match = input_string[end:] # string after the approximate match
+
+        # _regex_patterns.ALL_NUMBERS.findall(after_approx_match)
+        nearest_number_search = _regex_patterns.ALL_NUMBERS.search(str_after_approx_match) # search for the nearest number after the approximate string
+
+        if not nearest_number_search:
+            # print(f"No number found after approximate match")
+            continue
+
+        closest_number = nearest_number_search.group() # the actual matching number string
+        # print(f"Closest Number: '{closest_number}'")
+        current_result.append(closest_number) # add the number to the result
+        
+        # string after the number 
+        str_after_number_match = str_after_approx_match[nearest_number_search.end():] # string after the number match
+
+        nearest_unit_search = _regex_patterns.UNITS_PATTERN.search(str_after_number_match) # search for the nearest unit after the number
+
+        if not nearest_unit_search: # if we don't find a unit after the number, we skip this triplet
+            # print(f"No unit found after approximate match")
+            continue
+
+        closest_unit = nearest_unit_search.group() # the actual matching unit string
+        # print(f"Closest Unit: '{closest_unit}'")
+
+        current_result.append(closest_unit) # add the unit to the result
+        # approximate_triplets.append(current_result) # add the triplet to the list of approximate triplets
+        approximate_triplets.append(tuple(current_result)) # add the triplet to the list of approximate triplets
+    
+
+    # look for trailing approximate strings
+    trailing_approx_strings = _regex_patterns.APPROXIMATE_STRINGS_PATTERN.findall(input_string)
+
+    # if we didn't get any [approximate, quantity, unit] triplets, but we did get a trailing approximate strings
+    # check the string again for quantity unit pairs and 
+    # add the trailing approximate string to the beginning of each pair
+    # This will help handle the following case:
+    #       "(12 ounces approximately)"
+    if not approximate_triplets and trailing_approx_strings:
+        # print(f"Trailing Approximate Strings: {trailing_approx_strings}")
+        trailing_approx_string = trailing_approx_strings[0]
+        
+        quantity_unit_pairs = _extract_quantity_unit_pairs(input_string)
+
+        for pair in quantity_unit_pairs:
+            new_triplet = (trailing_approx_string, pair[0], pair[1])
+            approximate_triplets.append(new_triplet)
+            # pair.append(trailing_approx_string)
+        # [i.append(trailing_approx_string) for i in quantity_unit_pairs]
+        # print()
+    
     # return [tuple(i) for i in approximate_triplets]
+    return approximate_triplets
+
 
 # pattern = regex_patterns.QUANTITY_DASH_QUANTITY
 # replacement_function=None
 
 # TODO: Deprecated --> DELETE
 def _fractions_to_decimals(input_string) -> str:
     """
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-0.0.87/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 0.0.86
+Version: 0.0.87
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -58,24 +58,25 @@
 
 import ingredient_slicer
 
 slicer = ingredient_slicer.IngredientSlicer("2 (15-ounces) cans chickpeas, rinsed and drained")
 
 slicer.to_json()
 
-{
+{   
+    'ingredient': '2 (15-ounces) cans chickpeas, rinsed and drained', 
     'standardized_ingredient': '2 cans chickpeas, rinsed and drained', 
     'food': 'chickpeas', 
 
-    # primary units
+    # primary quantity and units
     'quantity': '30', 
     'unit': 'ounces', 
     'standardized_unit': 'ounce', 
 
-    # any other secondary units found in the string
+    # any other secondary quantity and units found in the string
     'secondary_quantity': '2', 
     'secondary_unit': 'cans', 
     'standardized_secondary_unit': 'can', 
 
     'gram_weight': '850.49', 
     'prep': ['drained', 'rinsed'], 
     'size_modifiers': [],
```

### Comparing `ingredient_slicer-0.0.86/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-0.0.87/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 tests/test_find_and_remove.py
 tests/test_find_and_remove_hyphen_substrings.py
 tests/test_fraction_str_to_decimal.py
 tests/test_get_gram_weight.py
 tests/test_ingredient_slicer.py
 tests/test_ingredient_slicer_dimensions.py
 tests/test_ingredient_slicer_fraction_conversions.py
+tests/test_ingredient_slicer_parenthesis.py
 tests/test_ingredient_slicer_x_separators.py
+tests/test_is_approximate_quantity_only_parenthesis.py
 tests/test_make_int_or_float_str.py
 tests/test_merge_misleading_ranges.py
 tests/test_merge_numbers.py
 tests/test_number_ranges.py
 tests/test_number_ranges_separated_by_words.py
 tests/test_numbers_with_inch_symbols.py
 tests/test_parenthesis.py
```

### Comparing `ingredient_slicer-0.0.86/pyproject.toml` & `ingredient_slicer-0.0.87/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "0.0.86"
+version = "0.0.87"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-0.0.86/tests/test_avg_ranges.py` & `ingredient_slicer-0.0.87/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_casual_ingredients.py` & `ingredient_slicer-0.0.87/tests/test_casual_ingredients.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,23 +81,20 @@
     parsed = slicer.to_json()
     assert parsed['quantity'] == "2"
     assert parsed['unit'] == None
     assert parsed['standardized_unit'] == None
     assert parsed['food'] == 'watermelon watermelons' # TODO: this is a bug, should be just watermelon
     assert parsed['is_required'] == True
 
-# TODO: this seems like it should just be 3, options are to remove "few" from the CASUAL_QUANTITIES dictionary
-# TODO:  or to deal with parenthesis that have an approximate quantity in them WITHOUT a unit (e.g. "(about 3)"
-# TODO: For not this test will stay put...
 def test_casual_quantities_in_parenthesis_1():
 
     slicer = IngredientSlicer("a few (about 3) pinches of salt")
     # slicer.parse()
     parsed = slicer.to_json()
-    assert parsed['quantity'] == "9"
+    assert parsed['quantity'] == "3"
     assert parsed['unit'] == 'pinches'
     assert parsed['standardized_unit'] == 'pinch'
     assert parsed['food'] == 'salt'
     assert parsed['is_required'] == True
 
 def test_casual_quantities_in_parenthesis_2():
```

### Comparing `ingredient_slicer-0.0.86/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-0.0.87/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-0.0.87/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-0.0.87/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_extract_dimensions.py` & `ingredient_slicer-0.0.87/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_extract_quantities_utils.py` & `ingredient_slicer-0.0.87/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_find_and_remove.py` & `ingredient_slicer-0.0.87/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-0.0.87/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-0.0.87/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_get_gram_weight.py` & `ingredient_slicer-0.0.87/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_ingredient_slicer.py` & `ingredient_slicer-0.0.87/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-0.0.87/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_make_int_or_float_str.py` & `ingredient_slicer-0.0.87/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-0.0.87/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_merge_numbers.py` & `ingredient_slicer-0.0.87/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_number_ranges.py` & `ingredient_slicer-0.0.87/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-0.0.87/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-0.0.87/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_parenthesis.py` & `ingredient_slicer-0.0.87/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_parenthesis_utils.py` & `ingredient_slicer-0.0.87/tests/test_parenthesis_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,9 +229,10 @@
     assert _utils._is_valid_parenthesis("I love test (cases) even if they take (lots of (time) to write") == False
 
 def test_is_valid_parenthesis_12():
     assert _utils._is_valid_parenthesis("I love test (cases) even if they take lots of (time (2 (do)) to write) properly") == True
 
 def test_is_valid_parenthesis_13():
     assert _utils._is_valid_parenthesis("I love test (cases) even if they take lots of (time (2 (do)) to write) properly)") == False
+
```

### Comparing `ingredient_slicer-0.0.86/tests/test_percentages.py` & `ingredient_slicer-0.0.87/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-0.0.87/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_prep_words.py` & `ingredient_slicer-0.0.87/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_quantity_range_regex.py` & `ingredient_slicer-0.0.87/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_quantity_units_regex.py` & `ingredient_slicer-0.0.87/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-0.0.87/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_remove_x_separators.py` & `ingredient_slicer-0.0.87/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-0.0.87/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_separate_dimensions.py` & `ingredient_slicer-0.0.87/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_size_modifiers.py` & `ingredient_slicer-0.0.87/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_spaced_numbers.py` & `ingredient_slicer-0.0.87/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_unit_regex.py` & `ingredient_slicer-0.0.87/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_wild_ingredients.py` & `ingredient_slicer-0.0.87/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_word_fractions.py` & `ingredient_slicer-0.0.87/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_word_numbers.py` & `ingredient_slicer-0.0.87/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-0.0.86/tests/test_x_after_number_regex.py` & `ingredient_slicer-0.0.87/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

