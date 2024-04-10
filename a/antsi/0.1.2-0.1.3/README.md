# Comparing `tmp/antsi-0.1.2.tar.gz` & `tmp/antsi-0.1.3.tar.gz`

## Comparing `antsi-0.1.2.tar` & `antsi-0.1.3.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 antsi-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127       22 2024-04-10 07:29:40.000000 antsi-0.1.2/.github/FUNDING.yml
--rw-r--r--   0     1001      127     4673 2024-04-10 07:29:40.000000 antsi-0.1.2/.github/workflows/distribution.yml
--rw-r--r--   0     1001      127      917 2024-04-10 07:29:40.000000 antsi-0.1.2/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      685 2024-04-10 07:29:40.000000 antsi-0.1.2/.github/workflows/test.yml
--rw-r--r--   0     1001      127     5774 2024-04-10 07:29:40.000000 antsi-0.1.2/.gitignore
--rw-r--r--   0     1001      127      228 2024-04-10 07:29:40.000000 antsi-0.1.2/.yamllint.yml
--rw-r--r--   0     1001      127     1121 2024-04-10 07:29:40.000000 antsi-0.1.2/LICENSE.md
--rw-r--r--   0     1001      127     7645 2024-04-10 07:29:40.000000 antsi-0.1.2/README.md
--rw-r--r--   0     1001      127      402 2024-04-10 07:29:40.000000 antsi-0.1.2/antsi/__init__.py
--rw-r--r--   0     1001      127      133 2024-04-10 07:29:40.000000 antsi-0.1.2/antsi/_antsi.pyi
--rw-r--r--   0     1001      127        0 2024-04-10 07:29:40.000000 antsi-0.1.2/antsi/py.typed
--rw-r--r--   0     1001      127     7061 2024-04-10 07:29:40.000000 antsi-0.1.2/pdm.lock
--rw-r--r--   0     1001      127     2180 2024-04-10 07:29:40.000000 antsi-0.1.2/src/ast/color.rs
--rw-r--r--   0     1001      127     2071 2024-04-10 07:29:40.000000 antsi-0.1.2/src/ast/decoration.rs
--rw-r--r--   0     1001      127      271 2024-04-10 07:29:40.000000 antsi-0.1.2/src/ast/mod.rs
--rw-r--r--   0     1001      127    19008 2024-04-10 07:29:40.000000 antsi-0.1.2/src/ast/style.rs
--rw-r--r--   0     1001      127    14726 2024-04-10 07:29:40.000000 antsi-0.1.2/src/ast/token.rs
--rw-r--r--   0     1001      127    19103 2024-04-10 07:29:40.000000 antsi-0.1.2/src/color.rs
--rw-r--r--   0     1001      127     4554 2024-04-10 07:29:40.000000 antsi-0.1.2/src/error.rs
--rw-r--r--   0     1001      127     5386 2024-04-10 07:29:40.000000 antsi-0.1.2/src/escape.rs
--rw-r--r--   0     1001      127    11434 2024-04-10 07:29:40.000000 antsi-0.1.2/src/lexer.rs
--rw-r--r--   0     1001      127     3834 2024-04-10 07:29:40.000000 antsi-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     2401 2024-04-10 07:29:40.000000 antsi-0.1.2/src/macros.rs
--rw-r--r--   0     1001      127     8025 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/content.rs
--rw-r--r--   0     1001      127     4439 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/markup.rs
--rw-r--r--   0     1001      127      279 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
--rw-r--r--   0     1001      127      319 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
--rw-r--r--   0     1001      127      278 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
--rw-r--r--   0     1001      127      671 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
--rw-r--r--   0     1001      127      800 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      735 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
--rw-r--r--   0     1001      127      736 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
--rw-r--r--   0     1001      127      349 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      394 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
--rw-r--r--   0     1001      127     2007 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      907 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
--rw-r--r--   0     1001      127      497 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
--rw-r--r--   0     1001      127      496 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      627 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      562 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      589 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      694 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      553 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      563 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    23178 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/style.rs
--rw-r--r--   0     1001      127    16007 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser/text.rs
--rw-r--r--   0     1001      127    12184 2024-04-10 07:29:40.000000 antsi-0.1.2/src/parser.rs
--rw-r--r--   0     1001      127      314 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
--rw-r--r--   0     1001      127      310 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
--rw-r--r--   0     1001      127     2823 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__lexer__tests__many_tokens.snap
--rw-r--r--   0     1001      127      490 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
--rw-r--r--   0     1001      127      317 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
--rw-r--r--   0     1001      127      261 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__empty_token.snap
--rw-r--r--   0     1001      127     1567 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      670 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__nested_token.snap
--rw-r--r--   0     1001      127      230 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
--rw-r--r--   0     1001      127      111 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
--rw-r--r--   0     1001      127      242 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
--rw-r--r--   0     1001      127      355 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
--rw-r--r--   0     1001      127      157 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_text.snap
--rw-r--r--   0     1001      127      231 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      245 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      385 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      235 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      109 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
--rw-r--r--   0     1001      127      620 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
--rw-r--r--   0     1001      127      230 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      614 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      502 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext.snap
--rw-r--r--   0     1001      127      685 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap
--rw-r--r--   0     1001      127      338 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_background.snap
--rw-r--r--   0     1001      127      336 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      438 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      388 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      414 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      502 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      379 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      390 2024-04-10 07:29:40.000000 antsi-0.1.2/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    15182 2024-04-10 07:29:40.000000 antsi-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127     1056 2024-04-10 07:29:40.000000 antsi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 antsi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 antsi-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127       22 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     4791 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/distribution.yml
+-rw-r--r--   0     1001      127      917 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      685 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     5774 2024-04-10 08:05:28.000000 antsi-0.1.3/.gitignore
+-rw-r--r--   0     1001      127      228 2024-04-10 08:05:28.000000 antsi-0.1.3/.yamllint.yml
+-rw-r--r--   0     1001      127     1121 2024-04-10 08:05:28.000000 antsi-0.1.3/LICENSE.md
+-rw-r--r--   0     1001      127     7645 2024-04-10 08:05:28.000000 antsi-0.1.3/README.md
+-rw-r--r--   0     1001      127      402 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/__init__.py
+-rw-r--r--   0     1001      127      133 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/_antsi.pyi
+-rw-r--r--   0     1001      127        0 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/py.typed
+-rw-r--r--   0     1001      127     7061 2024-04-10 08:05:28.000000 antsi-0.1.3/pdm.lock
+-rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/renovate.json
+-rw-r--r--   0     1001      127     2180 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/color.rs
+-rw-r--r--   0     1001      127     2071 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/decoration.rs
+-rw-r--r--   0     1001      127      271 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/mod.rs
+-rw-r--r--   0     1001      127    19008 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/style.rs
+-rw-r--r--   0     1001      127    14726 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/token.rs
+-rw-r--r--   0     1001      127    19103 2024-04-10 08:05:28.000000 antsi-0.1.3/src/color.rs
+-rw-r--r--   0     1001      127     4554 2024-04-10 08:05:28.000000 antsi-0.1.3/src/error.rs
+-rw-r--r--   0     1001      127     5386 2024-04-10 08:05:28.000000 antsi-0.1.3/src/escape.rs
+-rw-r--r--   0     1001      127    11434 2024-04-10 08:05:28.000000 antsi-0.1.3/src/lexer.rs
+-rw-r--r--   0     1001      127     3834 2024-04-10 08:05:28.000000 antsi-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     2401 2024-04-10 08:05:28.000000 antsi-0.1.3/src/macros.rs
+-rw-r--r--   0     1001      127     8025 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/content.rs
+-rw-r--r--   0     1001      127     4439 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/markup.rs
+-rw-r--r--   0     1001      127      279 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
+-rw-r--r--   0     1001      127      319 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
+-rw-r--r--   0     1001      127      278 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
+-rw-r--r--   0     1001      127      671 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
+-rw-r--r--   0     1001      127      800 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      735 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
+-rw-r--r--   0     1001      127      736 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
+-rw-r--r--   0     1001      127      349 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      394 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
+-rw-r--r--   0     1001      127     2007 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      907 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
+-rw-r--r--   0     1001      127      497 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      496 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      627 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      562 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      589 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      694 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      553 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      563 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    23178 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/style.rs
+-rw-r--r--   0     1001      127    16007 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/text.rs
+-rw-r--r--   0     1001      127    12184 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser.rs
+-rw-r--r--   0     1001      127      314 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
+-rw-r--r--   0     1001      127      310 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
+-rw-r--r--   0     1001      127     2823 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__many_tokens.snap
+-rw-r--r--   0     1001      127      490 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
+-rw-r--r--   0     1001      127      317 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
+-rw-r--r--   0     1001      127      261 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__empty_token.snap
+-rw-r--r--   0     1001      127     1567 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      670 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__nested_token.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
+-rw-r--r--   0     1001      127      111 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
+-rw-r--r--   0     1001      127      242 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
+-rw-r--r--   0     1001      127      355 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
+-rw-r--r--   0     1001      127      157 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_text.snap
+-rw-r--r--   0     1001      127      231 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      245 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      385 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      235 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      109 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      620 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      614 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext.snap
+-rw-r--r--   0     1001      127      685 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap
+-rw-r--r--   0     1001      127      338 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      336 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      438 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      388 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      414 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      379 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      390 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    15182 2024-04-10 08:05:28.000000 antsi-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127     1056 2024-04-10 08:05:28.000000 antsi-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 antsi-0.1.3/PKG-INFO
```

### Comparing `antsi-0.1.2/Cargo.toml` & `antsi-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "antsi"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 description = "A quick and user-friendly way to style your text using ANSI codes"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "antsi"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.21", features = ["extension-module", "abi3-py310"] }
+codespan-reporting = "0.11"
 indexmap = "2.2"
 logos = "0.14"
-text-size = "1.1"
-codespan-reporting = "0.11"
+pyo3 = { version = "0.21", features = ["extension-module", "abi3-py310"] }
 termcolor = "1"
+text-size = "1.1"
 
 [dev-dependencies]
 insta = "1.36.1"
 
 [profile.dev.package]
 insta.opt-level = 3
 similar.opt-level = 3
```

### Comparing `antsi-0.1.2/.github/workflows/distribution.yml` & `antsi-0.1.3/.github/workflows/distribution.yml`

 * *Files 14% similar despite different names*

```diff
@@ -112,25 +112,26 @@
 
       - name: Compare current version to released tags
         id: determine
         env:
           GH_TOKEN: ${{ github.token }}
         run: |
           current_version=$(tomlq -r .package.version Cargo.toml)
-          new_version=$( \
+          will_publish=$( \
             gh api repos/:owner/:repo/git/refs/tags \
             | jq --arg current_version $current_version \
               '[ .[].ref | ltrimstr("refs/tags/v") ] | contains([$current_version]) | not' \
           )
-          echo "result=$new_version" >> "$GITHUB_OUTPUT"
+          echo "result=$will_publish" >> "$GITHUB_OUTPUT"
+          echo "Will publish? $will_publish"
 
   publish:
     name: Publish
     runs-on: ubuntu-latest
-    if: ${{ github.event_name != 'pull_request' && needs.should-publish.outputs.result }}
+    if: ${{ github.event_name != 'pull_request' && fromJSON(needs.should-publish.outputs.result) }}
     needs: [ should-publish, linux, windows, macos, sdist ]
     environment:
       name: pypi
       url: https://pypi.org/p/antsi
     permissions:
       id-token: write
     steps:
@@ -140,42 +141,46 @@
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    if: ${{ github.event_name != 'pull_request' && needs.should-publish.outputs.result }}
     needs: [ publish ]
     permissions:
       contents: write
       id-token: write
     steps:
       - uses: actions/download-artifact@v4
         with:
           path: artifacts/
 
       - name: Relocate distribution files
-        run: >-
+        run: |
           mkdir ./dist
-          mv ./artifacts/*/*
+          mv ./artifacts/*/* ./dist
 
       - uses: sigstore/gh-action-sigstore-python@v2.1.1
         with:
           inputs: >-
             ./dist/*.tar.gz
             ./dist/*.whl
 
+      - name: Get version
+        id: version
+        run: |
+          pipx install yq
+          version=$(tomlq -r .package.version Cargo.toml)
+          echo "version=$version" >> "$GITHUB_OUTPUT"
+
       - name: Create release
         run: >-
           gh release create
-          '${{ github.ref_name }}'
-          --repo '${{ github.repository }}'
-          --generate-notes
+          ${{ steps.version.outputs.version }}
+          --generate-notes --latest
         env:
           GITHUB_TOKEN: ${{ github.token }}
 
       - name: Upload assets
         run: >-
           gh release upload
-          '${{ github.ref_name }}' dist/**
-          --repo '${{ github.repository }}'
+          ${{ steps.version.outputs.version }} dist/**
```

### Comparing `antsi-0.1.2/.github/workflows/lint.yml` & `antsi-0.1.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/.github/workflows/test.yml` & `antsi-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/.gitignore` & `antsi-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/LICENSE.md` & `antsi-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/README.md` & `antsi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/pdm.lock` & `antsi-0.1.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/ast/color.rs` & `antsi-0.1.3/src/ast/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/ast/decoration.rs` & `antsi-0.1.3/src/ast/decoration.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/ast/style.rs` & `antsi-0.1.3/src/ast/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/ast/token.rs` & `antsi-0.1.3/src/ast/token.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/color.rs` & `antsi-0.1.3/src/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/error.rs` & `antsi-0.1.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/escape.rs` & `antsi-0.1.3/src/escape.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/lexer.rs` & `antsi-0.1.3/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/lib.rs` & `antsi-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/macros.rs` & `antsi-0.1.3/src/macros.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/content.rs` & `antsi-0.1.3/src/parser/content.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/markup.rs` & `antsi-0.1.3/src/parser/markup.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap` & `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/style.rs` & `antsi-0.1.3/src/parser/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser/text.rs` & `antsi-0.1.3/src/parser/text.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/parser.rs` & `antsi-0.1.3/src/parser.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__lexer__tests__many_tokens.snap` & `antsi-0.1.3/src/snapshots/antsi__lexer__tests__many_tokens.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__parser__tests__kitchen_sink.snap` & `antsi-0.1.3/src/snapshots/antsi__parser__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__parser__tests__nested_token.snap` & `antsi-0.1.3/src/snapshots/antsi__parser__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap` & `antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap` & `antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap` & `antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/Cargo.lock` & `antsi-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "antsi"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "codespan-reporting",
  "indexmap",
  "insta",
  "logos",
  "pyo3",
  "termcolor",
@@ -294,17 +294,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
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
 name = "redox_syscall"
 version = "0.4.1"
```

### Comparing `antsi-0.1.2/pyproject.toml` & `antsi-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.2/PKG-INFO` & `antsi-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: antsi
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: A quick and user-friendly way to style your text using ANSI codes
 Author-email: Alex Krantz <alex@krantz.dev>
 License: MIT
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_mn7w46zn_/tmp_bmw9y7f_TarContainer/0/91", line 194, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: antsi Version: 0.1.2 Classifier: Programming
+Metadata-Version: 2.3 Name: antsi Version: 0.1.3 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md Summary: A quick and user-friendly way to style your
 text using ANSI codes Author-email: Alex Krantz
 krantz.dev> License: MIT Requires-Python: >=3.10 Description-Content-Type:
 text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
 github.com/akrantz01/antsi Project-URL: issues, https://github.com/akrantz01/
```

