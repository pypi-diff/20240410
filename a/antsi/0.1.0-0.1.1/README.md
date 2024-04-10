# Comparing `tmp/antsi-0.1.0.tar.gz` & `tmp/antsi-0.1.1.tar.gz`

## Comparing `antsi-0.1.0.tar` & `antsi-0.1.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 antsi-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2833 2024-04-08 06:05:49.000000 antsi-0.1.0/.github/workflows/distribution.yml
--rw-r--r--   0     1001      127      917 2024-04-08 06:05:49.000000 antsi-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      685 2024-04-08 06:05:49.000000 antsi-0.1.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127     5774 2024-04-08 06:05:49.000000 antsi-0.1.0/.gitignore
--rw-r--r--   0     1001      127      228 2024-04-08 06:05:49.000000 antsi-0.1.0/.yamllint.yml
--rw-r--r--   0     1001      127     1121 2024-04-08 06:05:49.000000 antsi-0.1.0/LICENSE.md
--rw-r--r--   0     1001      127      301 2024-04-08 06:05:49.000000 antsi-0.1.0/README.md
--rw-r--r--   0     1001      127      402 2024-04-08 06:05:49.000000 antsi-0.1.0/antsi/__init__.py
--rw-r--r--   0     1001      127      133 2024-04-08 06:05:49.000000 antsi-0.1.0/antsi/_antsi.pyi
--rw-r--r--   0     1001      127        0 2024-04-08 06:05:49.000000 antsi-0.1.0/antsi/py.typed
--rw-r--r--   0     1001      127     7061 2024-04-08 06:05:49.000000 antsi-0.1.0/pdm.lock
--rw-r--r--   0     1001      127     2180 2024-04-08 06:05:49.000000 antsi-0.1.0/src/ast/color.rs
--rw-r--r--   0     1001      127     2071 2024-04-08 06:05:49.000000 antsi-0.1.0/src/ast/decoration.rs
--rw-r--r--   0     1001      127      271 2024-04-08 06:05:49.000000 antsi-0.1.0/src/ast/mod.rs
--rw-r--r--   0     1001      127    19008 2024-04-08 06:05:49.000000 antsi-0.1.0/src/ast/style.rs
--rw-r--r--   0     1001      127    14726 2024-04-08 06:05:49.000000 antsi-0.1.0/src/ast/token.rs
--rw-r--r--   0     1001      127    19103 2024-04-08 06:05:49.000000 antsi-0.1.0/src/color.rs
--rw-r--r--   0     1001      127     4554 2024-04-08 06:05:49.000000 antsi-0.1.0/src/error.rs
--rw-r--r--   0     1001      127     5386 2024-04-08 06:05:49.000000 antsi-0.1.0/src/escape.rs
--rw-r--r--   0     1001      127    11434 2024-04-08 06:05:49.000000 antsi-0.1.0/src/lexer.rs
--rw-r--r--   0     1001      127     3834 2024-04-08 06:05:49.000000 antsi-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     2401 2024-04-08 06:05:49.000000 antsi-0.1.0/src/macros.rs
--rw-r--r--   0     1001      127     8025 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/content.rs
--rw-r--r--   0     1001      127     4439 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/markup.rs
--rw-r--r--   0     1001      127      279 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
--rw-r--r--   0     1001      127      319 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
--rw-r--r--   0     1001      127      278 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
--rw-r--r--   0     1001      127      348 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      348 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
--rw-r--r--   0     1001      127      671 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
--rw-r--r--   0     1001      127      800 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      735 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
--rw-r--r--   0     1001      127      736 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
--rw-r--r--   0     1001      127      348 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
--rw-r--r--   0     1001      127      349 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
--rw-r--r--   0     1001      127      348 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      394 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
--rw-r--r--   0     1001      127     2007 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      907 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
--rw-r--r--   0     1001      127      497 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
--rw-r--r--   0     1001      127      496 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      627 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      562 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      589 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      694 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      553 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      563 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    23178 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/style.rs
--rw-r--r--   0     1001      127    16007 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser/text.rs
--rw-r--r--   0     1001      127    12184 2024-04-08 06:05:49.000000 antsi-0.1.0/src/parser.rs
--rw-r--r--   0     1001      127      314 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
--rw-r--r--   0     1001      127      310 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
--rw-r--r--   0     1001      127     2823 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__lexer__tests__many_tokens.snap
--rw-r--r--   0     1001      127      490 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
--rw-r--r--   0     1001      127      317 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
--rw-r--r--   0     1001      127      261 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__empty_token.snap
--rw-r--r--   0     1001      127     1567 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      670 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__nested_token.snap
--rw-r--r--   0     1001      127      230 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
--rw-r--r--   0     1001      127      111 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
--rw-r--r--   0     1001      127      242 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
--rw-r--r--   0     1001      127      355 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
--rw-r--r--   0     1001      127      157 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_text.snap
--rw-r--r--   0     1001      127      231 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      245 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      385 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      235 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      109 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
--rw-r--r--   0     1001      127      620 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
--rw-r--r--   0     1001      127      230 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      614 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      502 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext.snap
--rw-r--r--   0     1001      127      685 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap
--rw-r--r--   0     1001      127      338 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_background.snap
--rw-r--r--   0     1001      127      336 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      438 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      388 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      414 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      502 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      379 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      390 2024-04-08 06:05:49.000000 antsi-0.1.0/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    15182 2024-04-08 06:05:49.000000 antsi-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      939 2024-04-08 06:05:49.000000 antsi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 antsi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 antsi-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3744 2024-04-10 02:46:02.000000 antsi-0.1.1/.github/workflows/distribution.yml
+-rw-r--r--   0     1001      127      917 2024-04-10 02:46:02.000000 antsi-0.1.1/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      685 2024-04-10 02:46:02.000000 antsi-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     5774 2024-04-10 02:46:02.000000 antsi-0.1.1/.gitignore
+-rw-r--r--   0     1001      127      228 2024-04-10 02:46:02.000000 antsi-0.1.1/.yamllint.yml
+-rw-r--r--   0     1001      127     1121 2024-04-10 02:46:02.000000 antsi-0.1.1/LICENSE.md
+-rw-r--r--   0     1001      127      301 2024-04-10 02:46:02.000000 antsi-0.1.1/README.md
+-rw-r--r--   0     1001      127      402 2024-04-10 02:46:02.000000 antsi-0.1.1/antsi/__init__.py
+-rw-r--r--   0     1001      127      133 2024-04-10 02:46:02.000000 antsi-0.1.1/antsi/_antsi.pyi
+-rw-r--r--   0     1001      127        0 2024-04-10 02:46:02.000000 antsi-0.1.1/antsi/py.typed
+-rw-r--r--   0     1001      127     7061 2024-04-10 02:46:02.000000 antsi-0.1.1/pdm.lock
+-rw-r--r--   0     1001      127     2180 2024-04-10 02:46:02.000000 antsi-0.1.1/src/ast/color.rs
+-rw-r--r--   0     1001      127     2071 2024-04-10 02:46:02.000000 antsi-0.1.1/src/ast/decoration.rs
+-rw-r--r--   0     1001      127      271 2024-04-10 02:46:02.000000 antsi-0.1.1/src/ast/mod.rs
+-rw-r--r--   0     1001      127    19008 2024-04-10 02:46:02.000000 antsi-0.1.1/src/ast/style.rs
+-rw-r--r--   0     1001      127    14726 2024-04-10 02:46:02.000000 antsi-0.1.1/src/ast/token.rs
+-rw-r--r--   0     1001      127    19103 2024-04-10 02:46:02.000000 antsi-0.1.1/src/color.rs
+-rw-r--r--   0     1001      127     4554 2024-04-10 02:46:02.000000 antsi-0.1.1/src/error.rs
+-rw-r--r--   0     1001      127     5386 2024-04-10 02:46:02.000000 antsi-0.1.1/src/escape.rs
+-rw-r--r--   0     1001      127    11434 2024-04-10 02:46:02.000000 antsi-0.1.1/src/lexer.rs
+-rw-r--r--   0     1001      127     3834 2024-04-10 02:46:02.000000 antsi-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     2401 2024-04-10 02:46:02.000000 antsi-0.1.1/src/macros.rs
+-rw-r--r--   0     1001      127     8025 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/content.rs
+-rw-r--r--   0     1001      127     4439 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/markup.rs
+-rw-r--r--   0     1001      127      279 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
+-rw-r--r--   0     1001      127      319 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
+-rw-r--r--   0     1001      127      278 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
+-rw-r--r--   0     1001      127      671 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
+-rw-r--r--   0     1001      127      800 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      735 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
+-rw-r--r--   0     1001      127      736 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
+-rw-r--r--   0     1001      127      349 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      394 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
+-rw-r--r--   0     1001      127     2007 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      907 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
+-rw-r--r--   0     1001      127      497 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      496 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      627 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      562 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      589 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      694 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      553 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      563 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    23178 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/style.rs
+-rw-r--r--   0     1001      127    16007 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser/text.rs
+-rw-r--r--   0     1001      127    12184 2024-04-10 02:46:02.000000 antsi-0.1.1/src/parser.rs
+-rw-r--r--   0     1001      127      314 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
+-rw-r--r--   0     1001      127      310 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
+-rw-r--r--   0     1001      127     2823 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__lexer__tests__many_tokens.snap
+-rw-r--r--   0     1001      127      490 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
+-rw-r--r--   0     1001      127      317 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
+-rw-r--r--   0     1001      127      261 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__empty_token.snap
+-rw-r--r--   0     1001      127     1567 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      670 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__nested_token.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
+-rw-r--r--   0     1001      127      111 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
+-rw-r--r--   0     1001      127      242 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
+-rw-r--r--   0     1001      127      355 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
+-rw-r--r--   0     1001      127      157 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_text.snap
+-rw-r--r--   0     1001      127      231 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      245 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      385 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      235 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      109 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      620 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      614 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext.snap
+-rw-r--r--   0     1001      127      685 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap
+-rw-r--r--   0     1001      127      338 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      336 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      438 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      388 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      414 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      379 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      390 2024-04-10 02:46:02.000000 antsi-0.1.1/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    15182 2024-04-10 02:46:02.000000 antsi-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1056 2024-04-10 02:46:02.000000 antsi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 antsi-0.1.1/PKG-INFO
```

### Comparing `antsi-0.1.0/Cargo.toml` & `antsi-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "antsi"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 description = "A quick and user-friendly way to style your text using ANSI codes"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "antsi"
 crate-type = ["cdylib"]
```

### Comparing `antsi-0.1.0/.github/workflows/distribution.yml` & `antsi-0.1.1/.github/workflows/distribution.yml`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     tags:
       - '*'
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
-  id-token: write
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [ x86_64, x86, aarch64, armv7, s390x, ppc64le ]
@@ -100,19 +99,58 @@
           args: --out dist
       - name: Upload sdist
         uses: actions/upload-artifact@v4
         with:
           name: wheels-sdist
           path: dist
 
-  release:
-    name: Release
+  publish:
+    name: Publish
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ linux, windows, macos, sdist ]
+    environment:
+      name: pypi
+      url: https://pypi.org/p/antsi
+    permissions:
+      id-token: write
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
+
+  release:
+    name: Release
+    runs-on: ubuntu-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [ publish ]
+    permissions:
+      contents: write
+      id-token: write
+    steps:
+      - uses: actions/download-artifact@v4
+        with:
+          path: dist/
+
+      - uses: sigstore/gh-action-sigstore-python@v2.1.1
+        with:
+          inputs: >-
+            ./dist/*.tar.gz
+            ./dist/*.whl
+
+      - name: Create release
+        run: >-
+          gh release create
+          '${{ github.ref_name }}'
+          --repo '${{ github.repository }}'
+          --generate-notes
+        env:
+          GITHUB_TOKEN: ${{ github.token }}
+
+      - name: Upload assets
+        run: >-
+          gh release upload
+          '${{ github.ref_name }}' dist/**
+          --repo '${{ github.repository }}'
```

### Comparing `antsi-0.1.0/.github/workflows/lint.yml` & `antsi-0.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/.github/workflows/test.yml` & `antsi-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/.gitignore` & `antsi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/LICENSE.md` & `antsi-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/pdm.lock` & `antsi-0.1.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/ast/color.rs` & `antsi-0.1.1/src/ast/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/ast/decoration.rs` & `antsi-0.1.1/src/ast/decoration.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/ast/style.rs` & `antsi-0.1.1/src/ast/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/ast/token.rs` & `antsi-0.1.1/src/ast/token.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/color.rs` & `antsi-0.1.1/src/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/error.rs` & `antsi-0.1.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/escape.rs` & `antsi-0.1.1/src/escape.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/lexer.rs` & `antsi-0.1.1/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/lib.rs` & `antsi-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/macros.rs` & `antsi-0.1.1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/content.rs` & `antsi-0.1.1/src/parser/content.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/markup.rs` & `antsi-0.1.1/src/parser/markup.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap` & `antsi-0.1.1/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/style.rs` & `antsi-0.1.1/src/parser/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser/text.rs` & `antsi-0.1.1/src/parser/text.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/parser.rs` & `antsi-0.1.1/src/parser.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__lexer__tests__many_tokens.snap` & `antsi-0.1.1/src/snapshots/antsi__lexer__tests__many_tokens.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap` & `antsi-0.1.1/src/snapshots/antsi__parser__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__parser__tests__nested_token.snap` & `antsi-0.1.1/src/snapshots/antsi__parser__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap` & `antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap` & `antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap` & `antsi-0.1.1/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.0/Cargo.lock` & `antsi-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "antsi"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "codespan-reporting",
  "indexmap",
  "insta",
  "logos",
  "pyo3",
  "termcolor",
```

### Comparing `antsi-0.1.0/pyproject.toml` & `antsi-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 
 dependencies = []
 
+[project.urls]
+homepage = "https://github.com/akrantz01/antsi"
+issues = "https://github.com/akrantz01/antsi/issues"
+
 [tool.maturin]
 module-name = "antsi._antsi"
 features = ["pyo3/extension-module"]
 
 [tool.pdm]
 distribution = true
```

