# Comparing `tmp/rp2-1.5.0.tar.gz` & `tmp/rp2-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2-1.5.0.tar", last modified: Mon Jun 19 10:31:02 2023, max compression
+gzip compressed data, was "rp2-1.5.1.tar", last modified: Wed Apr 10 04:04:36 2024, max compression
```

## Comparing `rp2-1.5.0.tar` & `rp2-1.5.1.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.338540 rp2-1.5.0/
--rw-r--r--   0 marcoz     (501) staff       (20)    13978 2023-06-19 10:26:47.000000 rp2-1.5.0/CHANGELOG.md
--rw-r--r--   0 marcoz     (501) staff       (20)     2761 2023-06-19 10:26:47.000000 rp2-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 marcoz     (501) staff       (20)    11357 2023-06-19 10:26:47.000000 rp2-1.5.0/LICENSE
--rw-r--r--   0 marcoz     (501) staff       (20)      263 2023-06-19 10:26:47.000000 rp2-1.5.0/MANIFEST.in
--rw-r--r--   0 marcoz     (501) staff       (20)    33890 2023-06-19 10:31:02.338637 rp2-1.5.0/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)    22251 2023-06-19 10:26:47.000000 rp2-1.5.0/README.dev.md
--rw-r--r--   0 marcoz     (501) staff       (20)    18215 2023-06-19 10:26:47.000000 rp2-1.5.0/README.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.253499 rp2-1.5.0/config/
--rw-r--r--   0 marcoz     (501) staff       (20)      636 2023-06-19 10:26:47.000000 rp2-1.5.0/config/crypto_example.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      762 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_bad_data.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      597 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      556 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data4.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      675 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data_multi_method.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      516 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_large_input.ini
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.254120 rp2-1.5.0/docs/
--rw-r--r--   0 marcoz     (501) staff       (20)     2893 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/developer_faq.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.256130 rp2-1.5.0/docs/images/
--rw-r--r--   0 marcoz     (501) staff       (20)    94354 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/input_spreadsheet.png
--rw-r--r--   0 marcoz     (501) staff       (20)    66768 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_asset.png
--rw-r--r--   0 marcoz     (501) staff       (20)    87502 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_asset_exchange.png
--rw-r--r--   0 marcoz     (501) staff       (20)    16751 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_input.png
--rw-r--r--   0 marcoz     (501) staff       (20)   126454 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_in_out.png
--rw-r--r--   0 marcoz     (501) staff       (20)    43264 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_summary.png
--rw-r--r--   0 marcoz     (501) staff       (20)   229926 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_tax.png
--rw-r--r--   0 marcoz     (501) staff       (20)   156431 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_header.png
--rw-r--r--   0 marcoz     (501) staff       (20)    61646 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/tax_report_us_output_capital_gains.png
--rw-r--r--   0 marcoz     (501) staff       (20)    24446 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/tax_report_us_output_interest.png
--rw-r--r--   0 marcoz     (501) staff       (20)    15575 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/input_files.md
--rw-r--r--   0 marcoz     (501) staff       (20)     8402 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/output_files.md
--rw-r--r--   0 marcoz     (501) staff       (20)    27064 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/user_faq.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.257687 rp2-1.5.0/input/
--rw-r--r--   0 marcoz     (501) staff       (20)    18562 2023-06-19 10:26:47.000000 rp2-1.5.0/input/crypto_example.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.277056 rp2-1.5.0/input/golden/
--rw-r--r--   0 marcoz     (501) staff       (20)    39476 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28227 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27598 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27561 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12608 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    46257 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    57435 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27560 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    49835 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38189 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29720 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37998 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29513 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13044 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    56093 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    76795 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38085 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29748 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31353 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31002 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23181 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30871 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23125 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    43773 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23558 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31831 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23324 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12780 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    50213 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    70575 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31703 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23268 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    42672 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31106 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20872 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30959 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20807 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12317 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    49159 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    59596 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30917 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    47327 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35766 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29160 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28958 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    53767 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    73415 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    13272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_kl_fifo_open_positions.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35898 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28957 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    44766 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_multi_method_mixed_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23648 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_multi_method_mixed_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31746 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18147 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32073 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18258 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32296 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18266 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36717 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29719 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36742 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29722 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36422 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29521 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    63483 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31061 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    61078 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29914 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    62257 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30873 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29407 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20139 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31894 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28051 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32967 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35588 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34926 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41201 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36006 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41330 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33576 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36146 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41378 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31327 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27939 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34044 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33598 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29968 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20351 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33128 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    26109 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30811 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20491 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29617 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20378 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    49022 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37403 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41639 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37172 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41412 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    55100 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)   140328 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37171 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41409 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    14261 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_bad_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    19489 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    16939 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data2.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    13203 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data3.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    17177 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data4.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    22355 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data_multi_method.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34398 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_hifo.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    22517 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_hifo2.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    19469 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_many_year_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)      276 2023-06-19 10:26:47.000000 rp2-1.5.0/pyproject.toml
--rw-r--r--   0 marcoz     (501) staff       (20)     2445 2023-06-19 10:31:02.340252 rp2-1.5.0/setup.cfg
--rw-r--r--   0 marcoz     (501) staff       (20)       92 2023-06-19 10:26:47.000000 rp2-1.5.0/setup.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243163 rp2-1.5.0/src/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.281322 rp2-1.5.0/src/rp2/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4220 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_accounting_method.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3562 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_country.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3497 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_entry.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7808 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_entry_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1287 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_report_generator.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5123 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9503 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/accounting_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9017 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/balance.py
--rw-r--r--   0 marcoz     (501) staff       (20)    18062 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/computed_data.py
--rw-r--r--   0 marcoz     (501) staff       (20)    22917 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/configuration.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7696 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/configuration_schema.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4748 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/entry_types.py
--rw-r--r--   0 marcoz     (501) staff       (20)    10702 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/gain_loss.py
--rw-r--r--   0 marcoz     (501) staff       (20)    15603 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/gain_loss_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)     8760 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/in_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3799 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/input_data.py
--rw-r--r--   0 marcoz     (501) staff       (20)     6384 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/intra_transaction.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.302824 rp2-1.5.0/src/rp2/locales/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243630 rp2-1.5.0/src/rp2/locales/en/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.303293 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)      439 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    13689 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243916 rp2-1.5.0/src/rp2/locales/es/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.305827 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)    22319 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    23003 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.244196 rp2-1.5.0/src/rp2/locales/ja/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.306506 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)      432 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    13318 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.245072 rp2-1.5.0/src/rp2/locales/kl/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.307057 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)    22133 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    23016 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.po
--rw-r--r--   0 marcoz     (501) staff       (20)    13276 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/messages.pot
--rw-r--r--   0 marcoz     (501) staff       (20)     1582 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/localization.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1749 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/logger.py
--rw-r--r--   0 marcoz     (501) staff       (20)    16314 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/ods_parser.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9463 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/out_transaction.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.311374 rp2-1.5.0/src/rp2/plugin/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.312372 rp2-1.5.0/src/rp2/plugin/accounting_method/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2719 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/fifo.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2817 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/hifo.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2989 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/lifo.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.326641 rp2-1.5.0/src/rp2/plugin/country/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1697 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/es.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     1964 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1820 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/us.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.327924 rp2-1.5.0/src/rp2/plugin/report/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    11252 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/abstract_ods_generator.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.328144 rp2-1.5.0/src/rp2/plugin/report/data/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.330290 rp2-1.5.0/src/rp2/plugin/report/data/es/
--rw-r--r--   0 marcoz     (501) staff       (20)    31636 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/es/template_open_positions_es.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30525 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.333893 rp2-1.5.0/src/rp2/plugin/report/data/jp/
--rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_en.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_kl.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    47091 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    47104 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334420 rp2-1.5.0/src/rp2/plugin/report/data/us/
--rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_open_positions_en.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    19993 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34429 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334626 rp2-1.5.0/src/rp2/plugin/report/es/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/es/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334893 rp2-1.5.0/src/rp2/plugin/report/jp/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/jp/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    21833 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/jp/tax_report_jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)    29443 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/open_positions.py
--rw-r--r--   0 marcoz     (501) staff       (20)    52465 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/rp2_full_report.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.335273 rp2-1.5.0/src/rp2/plugin/report/us/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/us/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9714 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/us/tax_report_us.py
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/py.typed
--rw-r--r--   0 marcoz     (501) staff       (20)     4450 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_configuration_translator.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5725 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_decimal.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1236 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_error.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14337 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_main.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9893 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/tax_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1993 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/transaction_set.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.302432 rp2-1.5.0/src/rp2.egg-info/
--rw-r--r--   0 marcoz     (501) staff       (20)    33890 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)    10838 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/SOURCES.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        1 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/dependency_links.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      216 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/entry_points.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      239 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/requires.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        4 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/top_level.txt
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.338407 rp2-1.5.0/tests/
--rw-r--r--   0 marcoz     (501) staff       (20)     4193 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/abstract_test_ods_output_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4792 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/ods_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)    38722 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/rp2_test_output.py
--rw-r--r--   0 marcoz     (501) staff       (20)    37707 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_configuration.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14527 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_gain_loss.py
--rw-r--r--   0 marcoz     (501) staff       (20)    19000 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_gain_loss_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)    34051 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_in_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)    16951 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_input_parser.py
--rw-r--r--   0 marcoz     (501) staff       (20)    27920 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_intra_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5653 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_large_input.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2399 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_localized_output.py
--rw-r--r--   0 marcoz     (501) staff       (20)    17379 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4150 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff_es.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     6035 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff_jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)    25709 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_out_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7230 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_rp2_decimal.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5464 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_tax_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14675 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_transaction_set.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.466689 rp2-1.5.1/
+-rw-r--r--   0 marcoz     (501) staff       (20)    14362 2024-04-10 03:56:16.000000 rp2-1.5.1/CHANGELOG.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     2761 2024-04-10 03:42:50.000000 rp2-1.5.1/CONTRIBUTING.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    11337 2024-04-10 03:42:50.000000 rp2-1.5.1/LICENSE
+-rw-r--r--   0 marcoz     (501) staff       (20)      263 2024-04-10 03:42:50.000000 rp2-1.5.1/MANIFEST.in
+-rw-r--r--   0 marcoz     (501) staff       (20)    35458 2024-04-10 04:04:36.466510 rp2-1.5.1/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)    22624 2024-04-10 03:58:21.000000 rp2-1.5.1/README.dev.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    18611 2024-04-10 03:58:21.000000 rp2-1.5.1/README.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.411982 rp2-1.5.1/config/
+-rw-r--r--   0 marcoz     (501) staff       (20)      636 2024-04-10 03:42:50.000000 rp2-1.5.1/config/crypto_example.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      762 2024-04-10 03:42:50.000000 rp2-1.5.1/config/test_bad_data.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      597 2024-04-10 03:42:50.000000 rp2-1.5.1/config/test_data.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      556 2024-04-10 03:42:50.000000 rp2-1.5.1/config/test_data4.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      675 2024-04-10 03:42:50.000000 rp2-1.5.1/config/test_data_multi_method.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      516 2024-04-10 03:42:50.000000 rp2-1.5.1/config/test_large_input.ini
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.412726 rp2-1.5.1/docs/
+-rw-r--r--   0 marcoz     (501) staff       (20)     2893 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/developer_faq.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.414882 rp2-1.5.1/docs/images/
+-rw-r--r--   0 marcoz     (501) staff       (20)    94354 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/input_spreadsheet.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    66768 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/open_positions_asset.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    87502 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/open_positions_asset_exchange.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    16751 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/open_positions_input.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   126454 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/rp2_full_report_output_in_out.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    43264 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/rp2_full_report_output_summary.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   229926 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/rp2_full_report_output_tax.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   156431 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/rp2_header.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    61646 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/tax_report_us_output_capital_gains.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    24446 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/images/tax_report_us_output_interest.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    15575 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/input_files.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     8402 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/output_files.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    27658 2024-04-10 03:42:50.000000 rp2-1.5.1/docs/user_faq.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.416598 rp2-1.5.1/input/
+-rw-r--r--   0 marcoz     (501) staff       (20)    18562 2024-04-10 03:42:50.000000 rp2-1.5.1/input/crypto_example.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.439662 rp2-1.5.1/input/golden/
+-rw-r--r--   0 marcoz     (501) staff       (20)    39476 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28227 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27598 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28267 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27561 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12608 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    46257 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    57435 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28267 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27560 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/crypto_example_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    49835 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38189 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29720 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37998 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29513 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13044 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    56093 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    76795 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38085 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29748 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data2_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31353 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23272 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31002 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23181 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30871 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23125 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    43773 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32272 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23558 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31831 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23324 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12780 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    50213 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    70575 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31703 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23268 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data3_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    42672 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31106 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20872 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30959 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20807 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12317 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    49159 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    59596 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30917 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20784 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data4_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    47327 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35766 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29160 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35784 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28958 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    53767 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    73415 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    13272 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_jp_kl_fifo_open_positions.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35898 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35784 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28957 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    44766 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_multi_method_mixed_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23648 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_data_multi_method_mixed_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31746 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18147 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32073 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18258 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32296 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18266 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo2_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36717 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29719 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36742 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29722 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36422 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29521 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_hifo_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    63483 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31061 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    61078 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29914 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    62257 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30873 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_large_input_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29407 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20139 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31894 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28051 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32967 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35588 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34926 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41201 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36006 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41330 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33576 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38267 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36146 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41378 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31327 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27939 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34044 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33598 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29968 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20351 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33128 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    26109 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30811 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20491 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29617 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20378 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    49022 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37403 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41639 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37172 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41412 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    55100 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)   140328 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37171 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41409 2024-04-10 03:42:50.000000 rp2-1.5.1/input/golden/test_many_year_data_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    14261 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_bad_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19489 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    16939 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_data2.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    13203 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_data3.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    17177 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_data4.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    22355 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_data_multi_method.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34398 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_hifo.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    22517 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_hifo2.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19469 2024-04-10 03:42:50.000000 rp2-1.5.1/input/test_many_year_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)      276 2024-04-10 03:42:50.000000 rp2-1.5.1/pyproject.toml
+-rw-r--r--   0 marcoz     (501) staff       (20)     2461 2024-04-10 04:04:36.469138 rp2-1.5.1/setup.cfg
+-rw-r--r--   0 marcoz     (501) staff       (20)       92 2024-04-10 03:42:50.000000 rp2-1.5.1/setup.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.404882 rp2-1.5.1/src/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.444536 rp2-1.5.1/src/rp2/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4220 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_accounting_method.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3562 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_country.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3497 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_entry.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7808 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_entry_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1287 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_report_generator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5123 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/abstract_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9503 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/accounting_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    10272 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/balance.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    18062 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/computed_data.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    23185 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/configuration.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7696 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/configuration_schema.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4748 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/entry_types.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    10702 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/gain_loss.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    15603 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/gain_loss_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     8760 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/in_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3799 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/input_data.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     6384 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/intra_transaction.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.455214 rp2-1.5.1/src/rp2/locales/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.405177 rp2-1.5.1/src/rp2/locales/en/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.455644 rp2-1.5.1/src/rp2/locales/en/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)      439 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    13689 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.405682 rp2-1.5.1/src/rp2/locales/es/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.456045 rp2-1.5.1/src/rp2/locales/es/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)    22319 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    23003 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.406056 rp2-1.5.1/src/rp2/locales/ja/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.456394 rp2-1.5.1/src/rp2/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)      432 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    13318 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.406628 rp2-1.5.1/src/rp2/locales/kl/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.456761 rp2-1.5.1/src/rp2/locales/kl/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)    22133 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/kl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    23016 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/kl/LC_MESSAGES/messages.po
+-rw-r--r--   0 marcoz     (501) staff       (20)    13276 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/locales/messages.pot
+-rw-r--r--   0 marcoz     (501) staff       (20)     1582 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/localization.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1749 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/logger.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    16314 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/ods_parser.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9463 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/out_transaction.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.456939 rp2-1.5.1/src/rp2/plugin/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.457499 rp2-1.5.1/src/rp2/plugin/accounting_method/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/accounting_method/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3070 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/accounting_method/fifo.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3169 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/accounting_method/hifo.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3323 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/accounting_method/lifo.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.458099 rp2-1.5.1/src/rp2/plugin/country/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/country/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1697 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/country/es.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     1964 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/country/jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1744 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/country/us.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.458720 rp2-1.5.1/src/rp2/plugin/report/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    11252 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/abstract_ods_generator.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.458913 rp2-1.5.1/src/rp2/plugin/report/data/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.459226 rp2-1.5.1/src/rp2/plugin/report/data/es/
+-rw-r--r--   0 marcoz     (501) staff       (20)    31636 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/es/template_open_positions_es.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30525 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.460286 rp2-1.5.1/src/rp2/plugin/report/data/jp/
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_open_positions_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_open_positions_kl.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    47091 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    47104 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.460786 rp2-1.5.1/src/rp2/plugin/report/data/us/
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/us/template_open_positions_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19993 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34429 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.460954 rp2-1.5.1/src/rp2/plugin/report/es/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/es/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.461197 rp2-1.5.1/src/rp2/plugin/report/jp/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/jp/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    21833 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/jp/tax_report_jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    29443 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/open_positions.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    52465 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/rp2_full_report.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.461499 rp2-1.5.1/src/rp2/plugin/report/us/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/us/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9714 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/plugin/report/us/tax_report_us.py
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/py.typed
+-rw-r--r--   0 marcoz     (501) staff       (20)     4450 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/rp2_configuration_translator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5725 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/rp2_decimal.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1236 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/rp2_error.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14975 2024-04-10 03:58:21.000000 rp2-1.5.1/src/rp2/rp2_main.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9893 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/tax_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1993 2024-04-10 03:42:50.000000 rp2-1.5.1/src/rp2/transaction_set.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.465231 rp2-1.5.1/src/rp2.egg-info/
+-rw-r--r--   0 marcoz     (501) staff       (20)    35458 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)    10838 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/SOURCES.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        1 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/dependency_links.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      216 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/entry_points.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      239 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/requires.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        4 2024-04-10 04:04:36.000000 rp2-1.5.1/src/rp2.egg-info/top_level.txt
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2024-04-10 04:04:36.464918 rp2-1.5.1/tests/
+-rw-r--r--   0 marcoz     (501) staff       (20)     4329 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/abstract_test_ods_output_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4792 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/ods_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    38722 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/rp2_test_output.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    37613 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_configuration.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14527 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_gain_loss.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    19000 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_gain_loss_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    34051 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_in_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    16951 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_input_parser.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    27920 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_intra_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5653 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_large_input.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2399 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_localized_output.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    18597 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_ods_output_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4408 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_ods_output_diff_es.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     6293 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_ods_output_diff_jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    25709 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_out_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7230 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_rp2_decimal.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5464 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_tax_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14675 2024-04-10 03:42:50.000000 rp2-1.5.1/tests/test_transaction_set.py
```

### Comparing `rp2-1.5.0/CHANGELOG.md` & `rp2-1.5.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.1
+* re-enabled LIFO and HIFO accounting methods (see discussion at #79)
+* added Python 3.11 to test matrix (#107)
+* on certain Linux distribution the mpdecimal library is missing, which causes runtime errors. This is now detected and reported to the users (#108)
+* added -n CLI option to allow negative balances on exchanges (#106)
+* multiple small documentation improvements
+
 ## 1.5.0
 * added support for Spain (see #97)
 
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
```

### Comparing `rp2-1.5.0/CONTRIBUTING.md` & `rp2-1.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/LICENSE` & `rp2-1.5.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2021 eprbell
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `rp2-1.5.0/PKG-INFO` & `rp2-1.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rp2
-Version: 1.5.0
-Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
+Version: 1.5.1
+Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO, LIFO and HIFO accounting methods, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 Home-page: https://github.com/eprbell/rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/rp2/blob/main/README.md
 Project-URL: Contact, https://eprbell.github.io/eprbell/about.html
@@ -18,16 +18,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Babel>=2.10.3
+Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: prezzemolo>=0.0.4
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pyexcel-ezodf>=0.3.4
+Provides-Extra: dev
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: bandit; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pep8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: rope; extra == "dev"
+Requires-Dist: types-jsonschema; extra == "dev"
+Requires-Dist: types-python-dateutil; extra == "dev"
 
 <!--- Copyright 2021 eprbell --->
 
 <!--- Licensed under the Apache License, Version 2.0 (the "License"); --->
 <!--- you may not use this file except in compliance with the License. --->
 <!--- You may obtain a copy of the License at --->
 
@@ -37,15 +57,15 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.5.0
+# RP2 v1.5.1
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
@@ -80,15 +100,18 @@
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the following accounting methods:
+* US: [FIFO](https://www.investopedia.com/terms/f/fifo.asp), [LIFO](https://www.investopedia.com/terms/l/lifo.asp) and [HIFO](https://www.investopedia.com/terms/h/hifo.asp). Note that these methods use universal application (not per-wallet application), as explained [here](https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/);
+* Spain: FIFO;
+* Japan: Total Average Method.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
 RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
@@ -99,17 +122,17 @@
 **IMPORTANT DISCLAIMERS**:
 * RP2 offers no guarantee of correctness (read the [license](https://github.com/eprbell/rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
 * The author of RP2 is not a tax professional, but has used RP2 personally for a few years.
 
 ### How RP2 Operates
 RP2 has been designed to have expressive primitives that can be used as building blocks for most tax scenarios: complex tax events can be described with patterns, built on top of these primitives (see the [FAQ list](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#tax-scenarios) for examples).
 
-RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
+For the US case, RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
 
-RP2 supports the FIFO accounting method: however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
+RP2 supports various accounting methods (e.g. FIFO, LIFO, HIFO): however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
 
 RP2 groups lot fractions into the following taxable event categories, each of which has a [specific tax treatment](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#which-crypto-tax-forms-to-file):
 * [AIRDROP](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-airdrops): gains from airdrops;
 * [DONATE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-donations): donations to charitable organizations;
 * [FEE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#hhow-to-handle-fee-only-defi-transactions): fee-only transaction, used in some DeFi scenarios (e.g. gas fee for running certain smart contracts);
 * [GIFT](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-gifts): gifts to parties who are not charitable organizations (not tax-deductible).
 * [HARDFORK](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-hard-forks): gains from hard forks;
@@ -163,15 +186,19 @@
 ```
 pip install rp2
 ```
 
 ### Installation on Other Unix-like Systems
 * install python 3.7 or greater
 * install pip3
-* `pip install rp2`
+
+Then install RP2:
+```
+pip install rp2
+```
 
 ## Running
 RP2 requires two files as input:
 * an ODS-format spreadsheet, containing crypto transactions (ODS-format files can be opened and edited with [LibreOffice](https://www.libreoffice.org/) and many other spreadsheet applications);
 * a config file, describing the format of the spreadsheet file: what value each column corresponds to (e.g. timestamp, amount, exchange, fee, etc.) and which cryptocurrencies and exchanges to expect.
 
 The two input files can either:
@@ -189,19 +216,19 @@
 To try RP2 with example files, download [crypto_example.ods](https://github.com/eprbell/rp2/tree/main/input/crypto_example.ods) and [crypto_example.ini](https://github.com/eprbell/rp2/tree/main/config/crypto_example.ini). Let's call `<download_directory>` the location of the downloaded files.
 
 The RP2 executable is country-dependent: `rp2_<country_code>`, where country code is a [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2), 2-letter identifier (e.g. `rp2_us`, `rp2_jp`, etc).
 
 To generate US tax output for the example files open a terminal window (or PowerShell if on Windows) and enter the following commands:
   ```
   cd <download_directory>
-  rp2_us -o output -p crypto_example_ crypto_example.ini crypto_example.ods
+  rp2_us -m fifo -o output -p crypto_example_ crypto_example.ini crypto_example.ods
   ```
 Results are generated in the `output` directory and logs are stored in the `log` directory.
 
-<!--- The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO). --->
+The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO).
 
 To print full command usage information for the `rp2_us` command:
   ```
   rp2_us --help
   ```
 
 ## Input and Output Files
@@ -252,14 +279,21 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.1
+* re-enabled LIFO and HIFO accounting methods (see discussion at #79)
+* added Python 3.11 to test matrix (#107)
+* on certain Linux distribution the mpdecimal library is missing, which causes runtime errors. This is now detected and reported to the users (#108)
+* added -n CLI option to allow negative balances on exchanges (#106)
+* multiple small documentation improvements
+
 ## 1.5.0
 * added support for Spain (see #97)
 
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
```

### Comparing `rp2-1.5.0/README.dev.md` & `rp2-1.5.1/README.dev.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# RP2 v1.5.0 Developer Guide
+# RP2 v1.5.1 Developer Guide
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
 
 ## Table of Contents
@@ -90,21 +90,27 @@
 Then install RP2 Python package requirements:
 ```
 cd <rp2_directory>
 virtualenv -p python .venv
 .venv\Scripts\activate.ps1
 python -m pip install -e ".[dev]"
 ```
+
+If `activate.ps1` cannot be loaded because running scripts is disabled on the system, run `activate.bat` instead or change the PowerShell execution policy `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser`.
 ### Setup on Other Unix-like Systems
 * install python 3.7 or greater
 * install pip3
 * install virtualenv
-* cd _<rp2_directory>_
-* `virtualenv -p python3 .venv`
-* `.venv/bin/pip3 install -e '.[dev]'`
+
+Then install RP2 Python package requirements:
+```
+cd <rp2_directory>
+virtualenv -p python3 .venv
+.venv/bin/pip3 install -e '.[dev]'
+```
 
 ## Source Code
 The RP2 source tree is organized as follows:
 * `.bumpversion.cfg`: bumpversion configuration;
 * `CHANGELOG.md`: change log document;
 * `config/`: config files for examples and tests;
 * `CONTRIBUTING.md`: contribution guidelines;
@@ -259,15 +265,15 @@
     * the rp2_full_report plugin uses `generation_language` because it generates a generic report that can be useful in any country (so it has to be localization-friendly)
 
 Report plugin output can be localized in many languages (see the [Localization](#localization) section for more on this): for an example of a localization-aware plugin see [rp2_full_report](src/rp2/plugin/report/rp2_full_report.py).
 
 **NOTE**: If you're interested in adding support for a new report generator, open a [PR](CONTRIBUTING.md).
 
 ### Adding a New Accounting Method
-Accounting method plugins modify the behavior of the tax engine. They pair in/out lots according to the given accounting algorithm: [FIFO](src/rp2/plugin/accounting_method/fifo.py) is an example of accounting method plugin.
+Accounting method plugins modify the behavior of the tax engine. They pair in/out lots according to the given accounting algorithm: [FIFO](src/rp2/plugin/accounting_method/fifo.py), [LIFO](src/rp2/plugin/accounting_method/lifo.py) and [HIFO](src/rp2/plugin/accounting_method/hifo.py) are examples of accounting method plugins.
 
 Accounting method plugins are discovered by RP2 at runtime and they must adhere to the conventions shown below. To add a new plugin follow this procedure:
 * add a new Python file to the `src/rp2/plugin/accounting_method/` directory and give it a meaningful name (like fifo.py)
 * import the following (plus any other RP2 or Python package you might need):
 ```
 from typing import Optional
 
@@ -315,15 +321,15 @@
 
  To add a new plugin follow this procedure:
 * add a new Python file to the `src/rp2/plugin/country/` directory and name it after the ISO 3166-1 alpha-2, 2-letter code for the country (e.g. us.py or jp.py);
 * add a class named as the ISO 3166-1 alpha-2, 2-letter code for the country (all uppercase), deriving from AbstractCountry;
 * in the constructor invoke the superclass constructor passing in country code and currency code;
 * add the `get_long_term_capital_gain_period()` method with the appropriate value. If there is no long-term capital gains, return `sys.maxsize`;
 * `get_default_accounting_method()` method returning accounting method to use if the user doesn't specify one on the command line (e.g. for the US case it's `"fifo"`);
-* `get_accounting_methods()` method returning a set of accounting methods that are accepted in the country (e.g. `{"fifo"}`);
+* `get_accounting_methods()` method returning a set of accounting methods that are accepted in the country (e.g. `{"fifo", "lifo", "hifo"}`);
 * `get_report_generators()`: method returning a set of report generators to use if the user doesn't specify them on the command line;
 * `get_default_generation_language()`: method returning the default language (in [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format) to use at report generation if the user doesn't specify it on the command line;
 * `rp2_entry()` global function calling `rp2_main()` and passing it an instance of the new country class (in fact technically subclasses of `AbstractCountry` are entry points, not plugins).
 
 As an example see the [us.py](src/rp2/plugin/country/us.py) file.
 
 Finally add a console script to [setup.cfg](setup.cfg) pointing the new country rp2_entry (see the US example in the console_scripts section of setup.cfg).
```

### Comparing `rp2-1.5.0/README.md` & `rp2-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.5.0
+# RP2 v1.5.1
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
@@ -53,15 +53,18 @@
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the following accounting methods:
+* US: [FIFO](https://www.investopedia.com/terms/f/fifo.asp), [LIFO](https://www.investopedia.com/terms/l/lifo.asp) and [HIFO](https://www.investopedia.com/terms/h/hifo.asp). Note that these methods use universal application (not per-wallet application), as explained [here](https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/);
+* Spain: FIFO;
+* Japan: Total Average Method.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
 RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
@@ -72,17 +75,17 @@
 **IMPORTANT DISCLAIMERS**:
 * RP2 offers no guarantee of correctness (read the [license](https://github.com/eprbell/rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
 * The author of RP2 is not a tax professional, but has used RP2 personally for a few years.
 
 ### How RP2 Operates
 RP2 has been designed to have expressive primitives that can be used as building blocks for most tax scenarios: complex tax events can be described with patterns, built on top of these primitives (see the [FAQ list](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#tax-scenarios) for examples).
 
-RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
+For the US case, RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
 
-RP2 supports the FIFO accounting method: however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
+RP2 supports various accounting methods (e.g. FIFO, LIFO, HIFO): however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
 
 RP2 groups lot fractions into the following taxable event categories, each of which has a [specific tax treatment](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#which-crypto-tax-forms-to-file):
 * [AIRDROP](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-airdrops): gains from airdrops;
 * [DONATE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-donations): donations to charitable organizations;
 * [FEE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#hhow-to-handle-fee-only-defi-transactions): fee-only transaction, used in some DeFi scenarios (e.g. gas fee for running certain smart contracts);
 * [GIFT](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-gifts): gifts to parties who are not charitable organizations (not tax-deductible).
 * [HARDFORK](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-hard-forks): gains from hard forks;
@@ -136,15 +139,19 @@
 ```
 pip install rp2
 ```
 
 ### Installation on Other Unix-like Systems
 * install python 3.7 or greater
 * install pip3
-* `pip install rp2`
+
+Then install RP2:
+```
+pip install rp2
+```
 
 ## Running
 RP2 requires two files as input:
 * an ODS-format spreadsheet, containing crypto transactions (ODS-format files can be opened and edited with [LibreOffice](https://www.libreoffice.org/) and many other spreadsheet applications);
 * a config file, describing the format of the spreadsheet file: what value each column corresponds to (e.g. timestamp, amount, exchange, fee, etc.) and which cryptocurrencies and exchanges to expect.
 
 The two input files can either:
@@ -162,19 +169,19 @@
 To try RP2 with example files, download [crypto_example.ods](https://github.com/eprbell/rp2/tree/main/input/crypto_example.ods) and [crypto_example.ini](https://github.com/eprbell/rp2/tree/main/config/crypto_example.ini). Let's call `<download_directory>` the location of the downloaded files.
 
 The RP2 executable is country-dependent: `rp2_<country_code>`, where country code is a [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2), 2-letter identifier (e.g. `rp2_us`, `rp2_jp`, etc).
 
 To generate US tax output for the example files open a terminal window (or PowerShell if on Windows) and enter the following commands:
   ```
   cd <download_directory>
-  rp2_us -o output -p crypto_example_ crypto_example.ini crypto_example.ods
+  rp2_us -m fifo -o output -p crypto_example_ crypto_example.ini crypto_example.ods
   ```
 Results are generated in the `output` directory and logs are stored in the `log` directory.
 
-<!--- The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO). --->
+The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO).
 
 To print full command usage information for the `rp2_us` command:
   ```
   rp2_us --help
   ```
 
 ## Input and Output Files
```

### Comparing `rp2-1.5.0/config/crypto_example.ini` & `rp2-1.5.1/config/crypto_example.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/config/test_bad_data.ini` & `rp2-1.5.1/config/test_bad_data.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/config/test_data.ini` & `rp2-1.5.1/config/test_data.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/config/test_data4.ini` & `rp2-1.5.1/config/test_data4.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/config/test_data_multi_method.ini` & `rp2-1.5.1/config/test_data_multi_method.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/config/test_large_input.ini` & `rp2-1.5.1/config/test_large_input.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/developer_faq.md` & `rp2-1.5.1/docs/developer_faq.md`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/input_spreadsheet.png` & `rp2-1.5.1/docs/images/input_spreadsheet.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/open_positions_asset.png` & `rp2-1.5.1/docs/images/open_positions_asset.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/open_positions_asset_exchange.png` & `rp2-1.5.1/docs/images/open_positions_asset_exchange.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/open_positions_input.png` & `rp2-1.5.1/docs/images/open_positions_input.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/rp2_full_report_output_in_out.png` & `rp2-1.5.1/docs/images/rp2_full_report_output_in_out.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/rp2_full_report_output_summary.png` & `rp2-1.5.1/docs/images/rp2_full_report_output_summary.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/rp2_full_report_output_tax.png` & `rp2-1.5.1/docs/images/rp2_full_report_output_tax.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/rp2_header.png` & `rp2-1.5.1/docs/images/rp2_header.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/tax_report_us_output_capital_gains.png` & `rp2-1.5.1/docs/images/tax_report_us_output_capital_gains.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/images/tax_report_us_output_interest.png` & `rp2-1.5.1/docs/images/tax_report_us_output_interest.png`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/input_files.md` & `rp2-1.5.1/docs/input_files.md`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/output_files.md` & `rp2-1.5.1/docs/output_files.md`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/docs/user_faq.md` & `rp2-1.5.1/docs/user_faq.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,21 +81,29 @@
 ### What if I Don't Have the Spot Price for Some Transactions?
 In some cases exchange reports miss spot price information. In such situations you can retrieve historical price data from [Yahoo](https://finance.yahoo.com/quote/BTC-USD/history/), [CoinMarketCap](https://coinmarketcap.com/currencies/bitcoin/historical-data/) and others.
 
 ### What Tokens Does RP2 Support?
 The user adds the tokens to the `assets` field of the [config file](input_files.md#the-config-file): RP2 accepts as valid all the tokens present in this field. See also the question on [writing a config file from scratch](#can-i-avoid-writing-a-config-file-from-scratch).
 
 ### What Accounting Methods Are Supported?
-Currently only the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method is supported for US and Spanish taxes. Only the Total Average Method is supported for Japanese taxes.
+RP2 currently supports the following accounting methods:
+* US: [FIFO](https://www.investopedia.com/terms/f/fifo.asp), [LIFO](https://www.investopedia.com/terms/l/lifo.asp) and [HIFO](https://www.investopedia.com/terms/h/hifo.asp). Note that these methods use universal application (not per-wallet application), as explained [here](https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/);
+* Spain: FIFO;
+* Japan: Total Average Method.
 
 ### Can I Change Accounting Method?
-No, currently RP2 only supports FIFO for US taxes and the Total Average Method for JP taxes.
+Yes, for countries that support more than one accounting method, you can select which one to use via the `-m` command line option.
 
 ### What Countries Are Supported?
-Currently the US, Japan and Spain are supported, but more countries are being added. As new countries are added this FAQ will be updated.
+Currently the following countries are supported:
+* US;
+* Japan;
+* Spain.
+
+However more countries are being added. As new countries are added this FAQ will be updated.
 
 ### How to Switch from Another Tax Software to RP2?
 In other words, how does RP2 handle transactions that were managed by other software in previous years? In this case the user can just leave out from the RP2 input spreadsheet the transactions/lots that were already sold in previous years.
 
 E.g. suppose the user's first year of trading BTC was 2020 and these were their transactions:
 
 <ol type="a">
@@ -166,24 +174,21 @@
 
 ### What Does RP2 Mean?
 It's a humorous reference to Warren Buffett’s claim that Bitcoin is [“rat poison squared”](https://www.cnbc.com/2018/05/05/warren-buffett-says-bitcoin-is-probably-rat-poison-squared.html). Other smart people occasionally made [famously](https://www.snopes.com/fact-check/paul-krugman-internets-effect-economy/) [wrong](https://libquotes.com/thomas-edison/quote/lbx5e7q) [remarks](https://en.wikipedia.org/wiki/Robert_Metcalfe#Incorrect_predictions) about technology: I have a feeling Buffett’s quote might end up among those.
 
 ## Tax Questions
 
 ### What Events Are Taxable?
-Selling, swapping, donating, mining, staking, earning cryptocurrency are some common taxable events. For an up-to-date list in any given year, ask your tax professional. For additional information on taxable events read the [Cryptocurrency Tax FAQ](https://www.reddit.com/r/CryptoTax/comments/re6jal/cryptocurrency_tax_faq/) on Reddit and
-<!-- markdown-link-check-disable -->
-[CoinTracker's summary on crypto taxes](https://www.cointracker.io/blog/what-tax-forms-should-crypto-holders-file).
-<!-- markdown-link-check-enable-->
+Selling, swapping, donating, mining, staking, earning cryptocurrency are some common taxable events. For an up-to-date list in any given year, ask your tax professional. For additional information on taxable events read the <!-- markdown-link-check-disable -->[Cryptocurrency Tax FAQ](https://www.reddit.com/r/CryptoTax/comments/re6jal/cryptocurrency_tax_faq/)<!-- markdown-link-check-enable--> on Reddit and <!-- markdown-link-check-disable -->[CoinTracker's summary on crypto taxes](https://www.cointracker.io/blog/what-tax-forms-should-crypto-holders-file).<!-- markdown-link-check-enable-->
 
 ### Can I Avoid Paying Crypto Taxes?
-No. The IRS has made it clear that [crypto taxes must be paid](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
+No. The IRS has made it clear that [crypto taxes must be paid](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions). Various tax agencies in other jurisdictions have made similar statements.
 
 ### Which Resources Can I Use to Learn About Crypto Taxes?
-A good starting point is the [Cryptocurrency Tax FAQ](https://www.reddit.com/r/CryptoTax/comments/re6jal/cryptocurrency_tax_faq/) on Reddit. Also read the question on [which tax forms to file](#which-crypto-tax-forms-to-file) and consult with your tax professional.
+A good starting point is the <!-- markdown-link-check-disable -->[Cryptocurrency Tax FAQ](https://www.reddit.com/r/CryptoTax/comments/re6jal/cryptocurrency_tax_faq/)<!-- markdown-link-check-enable--> on Reddit. Also read the question on [which tax forms to file](#which-crypto-tax-forms-to-file) and consult with your tax professional.
 
 ### Which Crypto Tax Forms to File?
 RP2 keeps track of in/out lot relationship, lot fractioning and it computes capital gains and losses, but it doesn't generate the final tax forms. The computed information is written to the tax_report_us output, which is intended for tax professionals: all taxable events are grouped in different tabs by type (mining, staking, selling, donating, etc.). Each tax event type has a specific tax treatment: your tax professional can transfer the information from the tax_report_us output tabs to the appropriate forms in any given year.
 
 For additional information on which forms to file read:
 <!-- markdown-link-check-disable -->
 * [CoinTracker's summary on this topic](https://www.cointracker.io/blog/what-tax-forms-should-crypto-holders-file)
```

### Comparing `rp2-1.5.0/input/crypto_example.ods` & `rp2-1.5.1/input/crypto_example.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/crypto_example_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/crypto_example_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/crypto_example_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/crypto_example_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/crypto_example_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/crypto_example_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/crypto_example_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/crypto_example_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data2_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data2_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data2_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data2_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data2_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_data2_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data2_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data2_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data2_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_data3_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data3_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data3_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data3_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data4_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data4_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data4_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data4_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data4_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_data4_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data4_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data4_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data4_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_data_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/test_data_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_jp_kl_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_data_jp_kl_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_multi_method_mixed_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_data_multi_method_mixed_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_data_multi_method_mixed_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_data_multi_method_mixed_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo2_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo2_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo2_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo2_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo2_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo2_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo2_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_hifo_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_hifo_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_hifo_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_large_input_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_large_input_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_large_input_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_large_input_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_large_input_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_large_input_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_large_input_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_fifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_hifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_hifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods` & `rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.1/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_lifo_rp2_full_report.ods` & `rp2-1.5.1/input/golden/test_many_year_data_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/golden/test_many_year_data_lifo_tax_report_us.ods` & `rp2-1.5.1/input/golden/test_many_year_data_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_bad_data.ods` & `rp2-1.5.1/input/test_bad_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_data.ods` & `rp2-1.5.1/input/test_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_data2.ods` & `rp2-1.5.1/input/test_data2.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_data3.ods` & `rp2-1.5.1/input/test_data3.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_data4.ods` & `rp2-1.5.1/input/test_data4.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_data_multi_method.ods` & `rp2-1.5.1/input/test_data_multi_method.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_hifo.ods` & `rp2-1.5.1/input/test_hifo.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_hifo2.ods` & `rp2-1.5.1/input/test_hifo2.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/input/test_many_year_data.ods` & `rp2-1.5.1/input/test_many_year_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/setup.cfg` & `rp2-1.5.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = rp2
-version = 1.5.0
-description = Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
+version = 1.5.1
+description = Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO, LIFO and HIFO accounting methods, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 long_description_content_type = text/markdown
 long_description = file: README.md, CHANGELOG.md
 keywords = accounting, altcoin, bitcoin, BTC, capital gains, cost basis, crypto, cryptocurrency, DeFi, ETH, ethereum, finance, form 8949, NFT, privacy, wallet, tax
 license = Apache License 2.0
 author = eprbell
 url = https://github.com/eprbell/rp2
 classifiers =
```

### Comparing `rp2-1.5.0/src/rp2/abstract_accounting_method.py` & `rp2-1.5.1/src/rp2/abstract_accounting_method.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/abstract_country.py` & `rp2-1.5.1/src/rp2/abstract_country.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/abstract_entry.py` & `rp2-1.5.1/src/rp2/abstract_entry.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/abstract_entry_set.py` & `rp2-1.5.1/src/rp2/abstract_entry_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/abstract_report_generator.py` & `rp2-1.5.1/src/rp2/abstract_report_generator.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/abstract_transaction.py` & `rp2-1.5.1/src/rp2/abstract_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/accounting_engine.py` & `rp2-1.5.1/src/rp2/accounting_engine.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/balance.py` & `rp2-1.5.1/src/rp2/balance.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from datetime import date
+from decimal import Decimal
 from typing import Callable, Dict, List, Optional, cast
 
 from prezzemolo.utility import to_string
 
 from rp2.configuration import Configuration
 from rp2.in_transaction import InTransaction
 from rp2.input_data import InputData
 from rp2.intra_transaction import IntraTransaction
 from rp2.logger import LOGGER
 from rp2.out_transaction import OutTransaction
 from rp2.rp2_decimal import ZERO, RP2Decimal
-from rp2.rp2_error import RP2TypeError
+from rp2.rp2_error import RP2TypeError, RP2ValueError
+
+
+CRYPTO_BALANCE_DECIMAL_MASK: Decimal = Decimal("1." + "0" * 10)
 
 
 @dataclass(frozen=True, eq=True)
 class Balance:
     configuration: Configuration
     asset: str
     exchange: str
@@ -131,23 +135,41 @@
             intra_transaction: IntraTransaction = cast(IntraTransaction, transaction)
             from_account = Account(intra_transaction.from_exchange, intra_transaction.from_holder)
             to_account = Account(intra_transaction.to_exchange, intra_transaction.to_holder)
             sent_balances[from_account] = sent_balances.get(from_account, ZERO) + intra_transaction.crypto_sent
             received_balances[to_account] = received_balances.get(to_account, ZERO) + intra_transaction.crypto_received
             final_balances[from_account] = final_balances.get(from_account, ZERO) - intra_transaction.crypto_sent
             final_balances[to_account] = final_balances.get(to_account, ZERO) + intra_transaction.crypto_received
+            if (
+                not RP2Decimal.is_equal_within_precision(final_balances[from_account], ZERO, CRYPTO_BALANCE_DECIMAL_MASK)
+                and final_balances[from_account] < ZERO
+                and not configuration.allow_negative_balances
+            ):
+                raise RP2ValueError(
+                    f'{intra_transaction.asset} balance of account "{from_account.exchange}" (holder "{from_account.holder}") went negative '
+                    f'({final_balances[from_account]}) on the following transaction: {intra_transaction}'
+                )
 
         # Balances for sold and gifted currency
         for transaction in self.__input_data.unfiltered_out_transaction_set:
             if transaction.timestamp.date() > to_date:
                 break
             out_transaction: OutTransaction = cast(OutTransaction, transaction)
             from_account = Account(out_transaction.exchange, out_transaction.holder)
             sent_balances[from_account] = sent_balances.get(from_account, ZERO) + out_transaction.crypto_out_no_fee + out_transaction.crypto_fee
             final_balances[from_account] = final_balances.get(from_account, ZERO) - out_transaction.crypto_out_no_fee - out_transaction.crypto_fee
+            if (
+                not RP2Decimal.is_equal_within_precision(final_balances[from_account], ZERO, CRYPTO_BALANCE_DECIMAL_MASK)
+                and final_balances[from_account] < ZERO
+                and not configuration.allow_negative_balances
+            ):
+                raise RP2ValueError(
+                    f'{out_transaction.asset} balance of account "{from_account.exchange}" (holder "{from_account.holder}") went negative '
+                    f'({final_balances[from_account]}) on the following transaction: {out_transaction}'
+                )
 
         for account, final_balance in final_balances.items():
             balance = Balance(
                 configuration,
                 self.__asset,
                 account.exchange,
                 account.holder,
```

### Comparing `rp2-1.5.0/src/rp2/computed_data.py` & `rp2-1.5.1/src/rp2/computed_data.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/configuration.py` & `rp2-1.5.1/src/rp2/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,26 +124,27 @@
 
     def __init__(  # pylint: disable=too-many-branches
         self,
         configuration_path: str,
         country: AbstractCountry,
         from_date: date = MIN_DATE,
         to_date: date = MAX_DATE,
+        allow_negative_balances: bool = False,
     ) -> None:
         self.__configuration_path: str = self.type_check_string("configuration_path", configuration_path)
         self.__country = AbstractCountry.type_check("country", country)
         if not isinstance(from_date, date):
             raise RP2TypeError("Parameter 'from_date' is not of type date")
         self.__from_date: date = from_date
         if not isinstance(to_date, date):
             raise RP2TypeError("Parameter 'to_date' is not of type date")
         self.__to_date: date = to_date
-
         if self.__from_date > self.__to_date:
             raise RP2ValueError("Parameter from_date cannot be greater than to_date")
+        self.__allow_negative_balances = self.type_check_bool("allow_negative_balances", allow_negative_balances)
 
         self.__in_header: Dict[str, int] = {}
         self.__out_header: Dict[str, int] = {}
         self.__intra_header: Dict[str, int] = {}
         self.__assets: Set[str] = set()
         self.__exchanges: Set[str] = set()
         self.__holders: Set[str] = set()
@@ -312,14 +313,18 @@
         return self.__from_date
 
     @property
     def to_date(self) -> date:
         return self.__to_date
 
     @property
+    def allow_negative_balances(self) -> bool:
+        return self.__allow_negative_balances
+
+    @property
     def assets(self) -> Set[str]:
         return self.__assets
 
     @property
     def generators(self) -> Set[str]:
         return self.__generators
```

### Comparing `rp2-1.5.0/src/rp2/configuration_schema.py` & `rp2-1.5.1/src/rp2/configuration_schema.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/entry_types.py` & `rp2-1.5.1/src/rp2/entry_types.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/gain_loss.py` & `rp2-1.5.1/src/rp2/gain_loss.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/gain_loss_set.py` & `rp2-1.5.1/src/rp2/gain_loss_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/in_transaction.py` & `rp2-1.5.1/src/rp2/in_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/input_data.py` & `rp2-1.5.1/src/rp2/input_data.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/intra_transaction.py` & `rp2-1.5.1/src/rp2/intra_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.po` & `rp2-1.5.1/src/rp2/locales/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.mo` & `rp2-1.5.1/src/rp2/locales/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.po` & `rp2-1.5.1/src/rp2/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.po` & `rp2-1.5.1/src/rp2/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.mo` & `rp2-1.5.1/src/rp2/locales/kl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.po` & `rp2-1.5.1/src/rp2/locales/kl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/locales/messages.pot` & `rp2-1.5.1/src/rp2/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/localization.py` & `rp2-1.5.1/src/rp2/localization.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/logger.py` & `rp2-1.5.1/src/rp2/logger.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/ods_parser.py` & `rp2-1.5.1/src/rp2/ods_parser.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/out_transaction.py` & `rp2-1.5.1/src/rp2/out_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/accounting_method/fifo.py` & `rp2-1.5.1/src/rp2/plugin/accounting_method/fifo.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     AcquiredLotCandidatesOrder,
 )
 from rp2.abstract_transaction import AbstractTransaction
 from rp2.in_transaction import InTransaction
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 
-# FIFO plugin. See https://www.investopedia.com/terms/l/fifo.asp.
+# FIFO plugin. See https://www.investopedia.com/terms/l/fifo.asp. This plugin uses universal application, not per-wallet application:
+# this means there is one queue for each coin across every wallet and exchange and the accounting method is applied to each such queue.
+# More on this at https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/
 class AccountingMethod(AbstractAccountingMethod):
     def seek_non_exhausted_acquired_lot(
         self,
         lot_candidates: AcquiredLotCandidates,
         taxable_event: Optional[AbstractTransaction],
         taxable_event_amount: RP2Decimal,
     ) -> Optional[AcquiredLotAndAmount]:
```

### Comparing `rp2-1.5.0/src/rp2/plugin/accounting_method/lifo.py` & `rp2-1.5.1/src/rp2/plugin/accounting_method/hifo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 eprbell
+# Copyright 2022 ninideol
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,17 +21,17 @@
     AcquiredLotCandidatesOrder,
 )
 from rp2.abstract_transaction import AbstractTransaction
 from rp2.in_transaction import InTransaction
 from rp2.rp2_decimal import ZERO, RP2Decimal
 
 
-# LIFO plugin. See https://www.investopedia.com/terms/l/lifo.asp. Note that under LIFO the date acquired must still be before or on the date sold:
-# see this discussion for details,
-# https://ttlc.intuit.com/community/investments-and-rental-properties/discussion/using-lifo-method-for-cryptocurrency-or-even-stock-cost-basis/00/1433542
+# HIFO plugin. See https://www.investopedia.com/terms/h/hifo.asp. This plugin uses universal application, not per-wallet application:
+# this means there is one queue for each coin across every wallet and exchange and the accounting method is applied to each such queue.
+# More on this at https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/
 class AccountingMethod(AbstractAccountingMethod):
     def seek_non_exhausted_acquired_lot(
         self,
         lot_candidates: AcquiredLotCandidates,
         taxable_event: Optional[AbstractTransaction],
         taxable_event_amount: RP2Decimal,
     ) -> Optional[AcquiredLotAndAmount]:
@@ -47,18 +47,18 @@
                 acquired_lot_amount = acquired_lot.crypto_in
             elif lot_candidates.get_partial_amount(acquired_lot) > ZERO:
                 acquired_lot_amount = lot_candidates.get_partial_amount(acquired_lot)
             else:
                 # The acquired lot has zero partial amount
                 continue
 
-            selected_acquired_lot_amount = acquired_lot_amount
-            selected_acquired_lot = acquired_lot
-            break
+            if selected_acquired_lot is None or selected_acquired_lot.spot_price < acquired_lot.spot_price:
+                selected_acquired_lot_amount = acquired_lot_amount
+                selected_acquired_lot = acquired_lot
 
         if selected_acquired_lot_amount > ZERO and selected_acquired_lot:
             lot_candidates.clear_partial_amount(selected_acquired_lot)
             return AcquiredLotAndAmount(acquired_lot=selected_acquired_lot, amount=selected_acquired_lot_amount)
         return None
 
     def lot_candidates_order(self) -> AcquiredLotCandidatesOrder:
-        return AcquiredLotCandidatesOrder.NEWER_TO_OLDER
+        return AcquiredLotCandidatesOrder.OLDER_TO_NEWER
```

### Comparing `rp2-1.5.0/src/rp2/plugin/country/es.py` & `rp2-1.5.1/src/rp2/plugin/country/es.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/country/jp.py` & `rp2-1.5.1/src/rp2/plugin/country/jp.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/country/us.py` & `rp2-1.5.1/src/rp2/plugin/country/us.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
     # Default accounting method to use if the user doesn't specify one on the command line
     def get_default_accounting_method(self) -> str:
         return "fifo"
 
     # Set of accounting methods accepted in the country
     def get_accounting_methods(self) -> Set[str]:
-        # Temporarily removed lifo and hifo due to https://github.com/eprbell/rp2/issues/79
-        return {"fifo"}
+        return {"fifo", "lifo", "hifo"}
 
     # Default set of generators to use if the user doesn't specify them on the command line
     def get_report_generators(self) -> Set[str]:
         return {
             "open_positions",
             "rp2_full_report",
             "us.tax_report_us",
```

### Comparing `rp2-1.5.0/src/rp2/plugin/report/abstract_ods_generator.py` & `rp2-1.5.1/src/rp2/plugin/report/abstract_ods_generator.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/es/template_open_positions_es.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/es/template_open_positions_es.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_open_positions_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_kl.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_open_positions_kl.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/us/template_open_positions_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/us/template_open_positions_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods` & `rp2-1.5.1/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/jp/tax_report_jp.py` & `rp2-1.5.1/src/rp2/plugin/report/jp/tax_report_jp.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/open_positions.py` & `rp2-1.5.1/src/rp2/plugin/report/open_positions.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/rp2_full_report.py` & `rp2-1.5.1/src/rp2/plugin/report/rp2_full_report.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/plugin/report/us/tax_report_us.py` & `rp2-1.5.1/src/rp2/plugin/report/us/tax_report_us.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/rp2_configuration_translator.py` & `rp2-1.5.1/src/rp2/rp2_configuration_translator.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/rp2_decimal.py` & `rp2-1.5.1/src/rp2/rp2_decimal.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/rp2_error.py` & `rp2-1.5.1/src/rp2/rp2_error.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/rp2_main.py` & `rp2-1.5.1/src/rp2/rp2_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 )
 from rp2.input_data import InputData
 from rp2.localization import set_generation_language
 from rp2.logger import LOG_FILE, LOGGER
 from rp2.ods_parser import open_ods, parse_ods
 from rp2.tax_engine import compute_tax
 
-_VERSION: str = "1.5.0"
+_VERSION: str = "1.5.1"
 
 _ACCOUNTING_METHOD_PACKAGE = "rp2.plugin.accounting_method"
 
 
 def rp2_main(country: AbstractCountry) -> None:
     if "RP2_ENABLE_PROFILER" in os.environ:
         cProfile.runctx("_rp2_main_internal(country)", globals(), locals())
@@ -64,23 +64,31 @@
     parser = _setup_argument_parser(country)
     args = parser.parse_args()
 
     set_generation_language(args.generation_language)
 
     _setup_paths(parser=parser, configuration_file=args.configuration_file, input_file=args.input_file, output_dir=args.output_dir)
 
+    # On certain platforms the mpdecimal system library is missing (see details at: https://github.com/eprbell/rp2/issues/25).
+    try:
+        import _decimal as _  # pylint: disable=import-outside-toplevel
+    except ImportError:
+        LOGGER.error("The `mpdecimal` library is a required system dependency for RP2, but Python was not able to locate it.")
+        sys.exit(1)
+
     try:
         LOGGER.info("Country: %s", country.country_iso_code)
         LOGGER.info("Generation Language: %s", args.generation_language)
 
         configuration: Configuration = Configuration(
             configuration_path=args.configuration_file,
             country=country,
             from_date=args.from_date,
             to_date=args.to_date,
+            allow_negative_balances=args.allow_negative_balances,
         )
         LOGGER.debug("Configuration object: %s", configuration)
 
         years_2_accounting_method_names: Dict[int, str] = configuration.years_2_accounting_method_names
         if args.method and configuration.years_2_accounting_method_names:
             LOGGER.error(
                 "Accounting method cannot be defined both via -m command line option and 'accounting_methods' section in configuration file: "
@@ -301,14 +309,20 @@
         default="",
         choices=accounting_methods,
         help=f"accounting method (default: '%(default)s'). Supported values: {', '.join(accounting_methods)}",
         metavar="METHOD",
         type=str,
     )
     parser.add_argument(
+        "-n",
+        "--allow_negative_balances",
+        action="store_true",
+        help="allow exchange balances to be negative (default: '%(default)s').",
+    )
+    parser.add_argument(
         "-o",
         "--output_dir",
         action="store",
         default="output/",
         help="Write output to OUTPUT_DIR  (default: '%(default)s')",
         metavar="OUTPUT_DIR",
         type=str,
```

### Comparing `rp2-1.5.0/src/rp2/tax_engine.py` & `rp2-1.5.1/src/rp2/tax_engine.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2/transaction_set.py` & `rp2-1.5.1/src/rp2/transaction_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/src/rp2.egg-info/PKG-INFO` & `rp2-1.5.1/src/rp2.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rp2
-Version: 1.5.0
-Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
+Version: 1.5.1
+Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO, LIFO and HIFO accounting methods, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 Home-page: https://github.com/eprbell/rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/rp2/blob/main/README.md
 Project-URL: Contact, https://eprbell.github.io/eprbell/about.html
@@ -18,16 +18,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Babel>=2.10.3
+Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: prezzemolo>=0.0.4
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pyexcel-ezodf>=0.3.4
+Provides-Extra: dev
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: bandit; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pep8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-mock; extra == "dev"
+Requires-Dist: rope; extra == "dev"
+Requires-Dist: types-jsonschema; extra == "dev"
+Requires-Dist: types-python-dateutil; extra == "dev"
 
 <!--- Copyright 2021 eprbell --->
 
 <!--- Licensed under the Apache License, Version 2.0 (the "License"); --->
 <!--- you may not use this file except in compliance with the License. --->
 <!--- You may obtain a copy of the License at --->
 
@@ -37,15 +57,15 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.5.0
+# RP2 v1.5.1
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
@@ -80,15 +100,18 @@
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the following accounting methods:
+* US: [FIFO](https://www.investopedia.com/terms/f/fifo.asp), [LIFO](https://www.investopedia.com/terms/l/lifo.asp) and [HIFO](https://www.investopedia.com/terms/h/hifo.asp). Note that these methods use universal application (not per-wallet application), as explained [here](https://www.forbes.com/sites/shehanchandrasekera/2020/09/17/what-crypto-taxpayers-need-to-know-about-fifo-lifo-hifo-specific-id/);
+* Spain: FIFO;
+* Japan: Total Average Method.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
 RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
@@ -99,17 +122,17 @@
 **IMPORTANT DISCLAIMERS**:
 * RP2 offers no guarantee of correctness (read the [license](https://github.com/eprbell/rp2/tree/main/LICENSE)): always verify results with the help of a tax professional.
 * The author of RP2 is not a tax professional, but has used RP2 personally for a few years.
 
 ### How RP2 Operates
 RP2 has been designed to have expressive primitives that can be used as building blocks for most tax scenarios: complex tax events can be described with patterns, built on top of these primitives (see the [FAQ list](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#tax-scenarios) for examples).
 
-RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
+For the US case, RP2 treats virtual currency as property for tax purposes, as per [IRS Virtual Currency Guidance](https://www.irs.gov/newsroom/irs-reminds-taxpayers-to-report-virtual-currency-transactions).
 
-RP2 supports the FIFO accounting method: however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
+RP2 supports various accounting methods (e.g. FIFO, LIFO, HIFO): however, in and out lots typically don't have matching amounts, so RP2 fractions them, maps in/out lot fractions and computes the resulting cost basis and capital gains for each lot fraction.
 
 RP2 groups lot fractions into the following taxable event categories, each of which has a [specific tax treatment](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#which-crypto-tax-forms-to-file):
 * [AIRDROP](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-airdrops): gains from airdrops;
 * [DONATE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-donations): donations to charitable organizations;
 * [FEE](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#hhow-to-handle-fee-only-defi-transactions): fee-only transaction, used in some DeFi scenarios (e.g. gas fee for running certain smart contracts);
 * [GIFT](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-gifts): gifts to parties who are not charitable organizations (not tax-deductible).
 * [HARDFORK](https://github.com/eprbell/rp2/blob/main/docs/user_faq.md#how-to-handle-hard-forks): gains from hard forks;
@@ -163,15 +186,19 @@
 ```
 pip install rp2
 ```
 
 ### Installation on Other Unix-like Systems
 * install python 3.7 or greater
 * install pip3
-* `pip install rp2`
+
+Then install RP2:
+```
+pip install rp2
+```
 
 ## Running
 RP2 requires two files as input:
 * an ODS-format spreadsheet, containing crypto transactions (ODS-format files can be opened and edited with [LibreOffice](https://www.libreoffice.org/) and many other spreadsheet applications);
 * a config file, describing the format of the spreadsheet file: what value each column corresponds to (e.g. timestamp, amount, exchange, fee, etc.) and which cryptocurrencies and exchanges to expect.
 
 The two input files can either:
@@ -189,19 +216,19 @@
 To try RP2 with example files, download [crypto_example.ods](https://github.com/eprbell/rp2/tree/main/input/crypto_example.ods) and [crypto_example.ini](https://github.com/eprbell/rp2/tree/main/config/crypto_example.ini). Let's call `<download_directory>` the location of the downloaded files.
 
 The RP2 executable is country-dependent: `rp2_<country_code>`, where country code is a [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2), 2-letter identifier (e.g. `rp2_us`, `rp2_jp`, etc).
 
 To generate US tax output for the example files open a terminal window (or PowerShell if on Windows) and enter the following commands:
   ```
   cd <download_directory>
-  rp2_us -o output -p crypto_example_ crypto_example.ini crypto_example.ods
+  rp2_us -m fifo -o output -p crypto_example_ crypto_example.ini crypto_example.ods
   ```
 Results are generated in the `output` directory and logs are stored in the `log` directory.
 
-<!--- The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO). --->
+The `-m` option is particularly important, because is selects the accounting method: `rp2_us` supports FIFO, LIFO and HIFO (if `-m` is not specified it defaults to FIFO).
 
 To print full command usage information for the `rp2_us` command:
   ```
   rp2_us --help
   ```
 
 ## Input and Output Files
@@ -252,14 +279,21 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.1
+* re-enabled LIFO and HIFO accounting methods (see discussion at #79)
+* added Python 3.11 to test matrix (#107)
+* on certain Linux distribution the mpdecimal library is missing, which causes runtime errors. This is now detected and reported to the users (#108)
+* added -n CLI option to allow negative balances on exchanges (#106)
+* multiple small documentation improvements
+
 ## 1.5.0
 * added support for Spain (see #97)
 
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
```

### Comparing `rp2-1.5.0/src/rp2.egg-info/SOURCES.txt` & `rp2-1.5.1/src/rp2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/abstract_test_ods_output_diff.py` & `rp2-1.5.1/tests/abstract_test_ods_output_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     RP2_FULL_REPORT = "rp2_full_report"
     TAX_REPORT_JP = "tax_report_jp"
     TAX_REPORT_US = "tax_report_us"
 
 
 class AbstractTestODSOutputDiff(unittest.TestCase):
     # Temporarily removed lifo and hifo due to https://github.com/eprbell/rp2/issues/79
-    METHODS: List[str] = ["fifo"]
+    METHODS: List[str] = ["fifo", "lifo", "hifo"]
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     @staticmethod
     def __get_time_interval(from_date: date = MIN_DATE, to_date: date = MAX_DATE) -> str:
         time_interval: str = ""
@@ -62,14 +62,15 @@
         output_dir: Path,
         test_name: str,
         config: str,
         method: str,
         input_path: Path = INPUT_PATH,
         from_date: date = MIN_DATE,
         to_date: date = MAX_DATE,
+        allow_negative_balances: bool = False,
         generation_language: Optional[str] = None,
         country: str = "us",
     ) -> None:
         config = test_name if config is None else config
         time_interval: str = cls.__get_time_interval(from_date, to_date)
 
         arguments: List[str] = [
@@ -83,14 +84,16 @@
             arguments.extend(["-m", method])
         if generation_language:
             arguments.extend(["-g", generation_language])
         if from_date:
             arguments.extend(["-f", str(from_date)])
         if to_date:
             arguments.extend(["-t", str(to_date)])
+        if allow_negative_balances:
+            arguments.extend(["-n"])
         arguments.extend(
             [
                 str(CONFIG_PATH / Path(f"{config}.ini")),
                 str(input_path / Path(f"{test_name}.ods")),
             ]
         )
```

### Comparing `rp2-1.5.0/tests/ods_diff.py` & `rp2-1.5.1/tests/ods_diff.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/rp2_test_output.py` & `rp2-1.5.1/tests/rp2_test_output.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_configuration.py` & `rp2-1.5.1/tests/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,16 +303,15 @@
         with self.assertRaisesRegex(RP2ValueError, "invalid year value in accounting method section .*integer > 1970 was expected"):
             self._test_config(config)
 
         config[Keyword.ACCOUNTING_METHODS.value] = {"abc": "fifo"}
         with self.assertRaisesRegex(RP2ValueError, "invalid year value in accounting method section .*integer was expected"):
             self._test_config(config)
 
-        # Temporarily removed lifo and hifo due to https://github.com/eprbell/rp2/issues/79
-        # config[Keyword.ACCOUNTING_METHODS.value] = {"1970": "hifo", "2020": "lifo"}
+        config[Keyword.ACCOUNTING_METHODS.value] = {"1970": "hifo", "2020": "lifo"}
 
     def test_creation(self) -> None:
         with self.assertRaisesRegex(RP2TypeError, "Parameter 'country' is not of type AbstractCountry: .*"):
             Configuration("./config/test_data.ini", None)  # type: ignore
         with self.assertRaisesRegex(RP2TypeError, "Parameter 'configuration_path' has non-string value .*"):
             Configuration(None, self._country)  # type: ignore
         with self.assertRaisesRegex(RP2TypeError, "Parameter 'configuration_path' has non-string value .*"):
```

### Comparing `rp2-1.5.0/tests/test_gain_loss.py` & `rp2-1.5.1/tests/test_gain_loss.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_gain_loss_set.py` & `rp2-1.5.1/tests/test_gain_loss_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_in_transaction.py` & `rp2-1.5.1/tests/test_in_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_input_parser.py` & `rp2-1.5.1/tests/test_input_parser.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_intra_transaction.py` & `rp2-1.5.1/tests/test_intra_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_large_input.py` & `rp2-1.5.1/tests/test_large_input.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_localized_output.py` & `rp2-1.5.1/tests/test_localized_output.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_ods_output_diff.py` & `rp2-1.5.1/tests/test_ods_output_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,48 +29,98 @@
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
 
         for method in AbstractTestODSOutputDiff.METHODS:
-            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="crypto_example", config="crypto_example", method=method)
+            AbstractTestODSOutputDiff._generate(
+                cls.output_dir, test_name="crypto_example", config="crypto_example", method=method, allow_negative_balances=True
+            )
             AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data", config="test_data", method=method)
-            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data2", config="test_data", method=method)
+            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data2", config="test_data", method=method, allow_negative_balances=True)
             AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data3", config="test_data", method=method)
             AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data4", config="test_data4", method=method)
-            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_hifo", config="test_data", method=method)
-            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_hifo2", config="test_data", method=method)
-            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method=method)
+            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_hifo", config="test_data", method=method, allow_negative_balances=True)
+            AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_hifo2", config="test_data", method=method, allow_negative_balances=True)
+            AbstractTestODSOutputDiff._generate(
+                cls.output_dir, test_name="test_many_year_data", config="test_data", method=method, allow_negative_balances=True
+            )
             AbstractTestODSOutputDiff._generate(
-                cls.output_dir, test_name="test_data3", config="test_data", method=method, from_date=date(2019, 12, 1), to_date=date(2020, 4, 1)
+                cls.output_dir,
+                test_name="test_data3",
+                config="test_data",
+                method=method,
+                from_date=date(2019, 12, 1),
+                to_date=date(2020, 4, 1),
+                allow_negative_balances=True,
             )
 
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2016, 12, 31))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2017, 12, 31))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2018, 12, 31))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2019, 12, 31))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2020, 12, 31))
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2016, 12, 31), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2017, 12, 31), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2018, 12, 31), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2019, 12, 31), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", to_date=date(2020, 12, 31), allow_negative_balances=True
+        )
 
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2017, 1, 1))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2018, 1, 1))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2019, 1, 1))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2020, 1, 1))
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2021, 1, 1))
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2017, 1, 1), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2018, 1, 1), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2019, 1, 1), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2020, 1, 1), allow_negative_balances=True
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2021, 1, 1), allow_negative_balances=True
+        )
 
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2017, 1, 1), to_date=date(2019, 12, 31)
+            cls.output_dir,
+            test_name="test_many_year_data",
+            config="test_data",
+            method="fifo",
+            from_date=date(2017, 1, 1),
+            to_date=date(2019, 12, 31),
+            allow_negative_balances=True,
+        )
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir,
+            test_name="test_many_year_data",
+            config="test_data",
+            method="fifo",
+            from_date=date(2018, 1, 1),
+            to_date=date(2019, 12, 31),
+            allow_negative_balances=True,
         )
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2018, 1, 1), to_date=date(2019, 12, 31)
+            cls.output_dir,
+            test_name="test_many_year_data",
+            config="test_data",
+            method="fifo",
+            from_date=date(2019, 1, 1),
+            to_date=date(2019, 12, 31),
+            allow_negative_balances=True,
         )
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", from_date=date(2019, 1, 1), to_date=date(2019, 12, 31)
+            cls.output_dir, test_name="test_data_multi_method", config="test_data_multi_method", method="mixed", allow_negative_balances=True
         )
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data_multi_method", config="test_data_multi_method", method="mixed")
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     def test_crypto_example_rp2_full_report(self) -> None:
         for method in self.METHODS:
             self._compare(output_dir=self.output_dir, test_name="crypto_example", method=method, output_plugin=OutputPlugins.RP2_FULL_REPORT)
```

### Comparing `rp2-1.5.0/tests/test_ods_output_diff_es.py` & `rp2-1.5.1/tests/test_ods_output_diff_es.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,36 @@
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
 
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="crypto_example", config="crypto_example", method="fifo", country="es", generation_language="es"
+            cls.output_dir,
+            test_name="crypto_example",
+            config="crypto_example",
+            method="fifo",
+            country="es",
+            generation_language="es",
+            allow_negative_balances=True,
         )
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data", config="test_data", method="fifo", country="es", generation_language="es")
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data2", config="test_data", method="fifo", country="es", generation_language="es")
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_data2", config="test_data", method="fifo", country="es", generation_language="es", allow_negative_balances=True
+        )
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data3", config="test_data", method="fifo", country="es", generation_language="es")
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data4", config="test_data4", method="fifo", country="es", generation_language="es")
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", country="es", generation_language="es"
+            cls.output_dir,
+            test_name="test_many_year_data",
+            config="test_data",
+            method="fifo",
+            country="es",
+            generation_language="es",
+            allow_negative_balances=True,
         )
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     def test_crypto_example_rp2_full_report(self) -> None:
         self._compare(
```

### Comparing `rp2-1.5.0/tests/test_ods_output_diff_jp.py` & `rp2-1.5.1/tests/test_ods_output_diff_jp.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,22 +28,36 @@
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
 
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="crypto_example", config="crypto_example", method="fifo", country="jp", generation_language="en"
+            cls.output_dir,
+            test_name="crypto_example",
+            config="crypto_example",
+            method="fifo",
+            country="jp",
+            generation_language="en",
+            allow_negative_balances=True,
         )
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data", config="test_data", method="fifo", country="jp", generation_language="en")
-        AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data2", config="test_data", method="fifo", country="jp", generation_language="en")
+        AbstractTestODSOutputDiff._generate(
+            cls.output_dir, test_name="test_data2", config="test_data", method="fifo", country="jp", generation_language="en", allow_negative_balances=True
+        )
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data3", config="test_data", method="fifo", country="jp", generation_language="en")
         AbstractTestODSOutputDiff._generate(cls.output_dir, test_name="test_data4", config="test_data4", method="fifo", country="jp", generation_language="en")
         AbstractTestODSOutputDiff._generate(
-            cls.output_dir, test_name="test_many_year_data", config="test_data", method="fifo", country="jp", generation_language="en"
+            cls.output_dir,
+            test_name="test_many_year_data",
+            config="test_data",
+            method="fifo",
+            country="jp",
+            generation_language="en",
+            allow_negative_balances=True,
         )
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     def test_crypto_example_rp2_full_report(self) -> None:
         self._compare(
```

### Comparing `rp2-1.5.0/tests/test_out_transaction.py` & `rp2-1.5.1/tests/test_out_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_rp2_decimal.py` & `rp2-1.5.1/tests/test_rp2_decimal.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_tax_engine.py` & `rp2-1.5.1/tests/test_tax_engine.py`

 * *Files identical despite different names*

### Comparing `rp2-1.5.0/tests/test_transaction_set.py` & `rp2-1.5.1/tests/test_transaction_set.py`

 * *Files identical despite different names*

