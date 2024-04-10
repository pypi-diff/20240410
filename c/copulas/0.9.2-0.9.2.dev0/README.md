# Comparing `tmp/copulas-0.9.2.tar.gz` & `tmp/copulas-0.9.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copulas-0.9.2.tar", last modified: Thu Oct 12 18:34:32 2023, max compression
+gzip compressed data, was "copulas-0.9.2.dev0.tar", last modified: Thu Oct 12 00:26:42 2023, max compression
```

## Comparing `copulas-0.9.2.tar` & `copulas-0.9.2.dev0.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.307235 copulas-0.9.2/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       77 2023-08-10 21:03:13.000000 copulas-0.9.2/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6960 2023-10-12 18:34:29.000000 copulas-0.9.2/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11342 2023-10-12 18:34:29.000000 copulas-0.9.2/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4822 2023-01-06 19:54:16.000000 copulas-0.9.2/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2023-01-05 18:17:33.000000 copulas-0.9.2/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17478 2023-10-12 18:34:32.307353 copulas-0.9.2/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5194 2023-10-12 18:34:29.000000 copulas-0.9.2/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6612 2023-10-12 18:34:29.000000 copulas-0.9.2/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.261891 copulas-0.9.2/copulas/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9280 2023-10-12 18:34:29.000000 copulas-0.9.2/copulas/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.263921 copulas-0.9.2/copulas/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5087 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13952 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4536 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/clayton.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4641 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/frank.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4216 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/gumbel.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2069 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/independence.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/bivariate/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6831 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/datasets.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.264591 copulas-0.9.2/copulas/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      362 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5600 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/multivariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11140 2023-10-12 18:34:29.000000 copulas-0.9.2/copulas/multivariate/gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22020 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/multivariate/tree.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12882 2023-08-10 21:03:13.000000 copulas-0.9.2/copulas/multivariate/vine.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.264721 copulas-0.9.2/copulas/optimize/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4927 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/optimize/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.266264 copulas-0.9.2/copulas/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      825 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19976 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1016 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      906 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      728 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6093 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      921 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/log_laplace.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      944 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/selection.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1932 2023-08-02 16:17:09.000000 copulas-0.9.2/copulas/univariate/truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      754 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/univariate/uniform.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4665 2023-01-05 18:17:33.000000 copulas-0.9.2/copulas/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.263035 copulas-0.9.2/copulas.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17478 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7597 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1637 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        8 2023-10-12 18:34:32.000000 copulas-0.9.2/copulas.egg-info/top_level.txt
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.268799 copulas-0.9.2/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      608 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/Makefile
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/authors.rst
--rwxr-xr-x   0 andrewmontanez   (501) staff       (20)     5850 2023-10-12 18:34:29.000000 copulas-0.9.2/docs/conf.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.273743 copulas-0.9.2/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15307 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/copulas-200.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    26688 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/copulas.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52079 2023-01-06 19:54:16.000000 copulas-0.9.2/docs/images/copulas_sample_dataset.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   886153 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/dai-logo-white.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/dice_cdf.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23772 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/pdf_cdf.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9447 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/pit.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   128308 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/images/quickstart.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      651 2023-08-10 21:03:13.000000 copulas-0.9.2/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      769 2023-01-05 18:17:33.000000 copulas-0.9.2/docs/make.bat
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1441 2023-10-12 18:34:32.307867 copulas-0.9.2/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3940 2023-10-12 18:34:29.000000 copulas-0.9.2/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.274503 copulas-0.9.2/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4710 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.275539 copulas-0.9.2/tests/end-to-end/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1663 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.275824 copulas-0.9.2/tests/end-to-end/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       51 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1301 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/bivariate/test_base.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.276355 copulas-0.9.2/tests/end-to-end/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1146 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/multivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7040 2023-10-12 18:34:29.000000 copulas-0.9.2/tests/end-to-end/multivariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1910 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/multivariate/test_vine.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1670 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/test_visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.277315 copulas-0.9.2/tests/end-to-end/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5170 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5090 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5032 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5576 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5210 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5276 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/end-to-end/univariate/test_truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9510 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/large_scale_evaluation.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.278031 copulas-0.9.2/tests/numerical/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3795 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.278368 copulas-0.9.2/tests/numerical/cdf/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.278513 copulas-0.9.2/tests/numerical/cdf/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/input/bivariate_cdf_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.285245 copulas-0.9.2/tests/numerical/cdf/output/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.286392 copulas-0.9.2/tests/numerical/cdf/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_input.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2090 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1678 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.257079 copulas-0.9.2/tests/numerical/cdf/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.287884 copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      808 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.288945 copulas-0.9.2/tests/numerical/cdf/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.289592 copulas-0.9.2/tests/numerical/cdf/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1077 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/cdf/test_cdf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.290240 copulas-0.9.2/tests/numerical/fit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.290765 copulas-0.9.2/tests/numerical/fit/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       72 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.291499 copulas-0.9.2/tests/numerical/fit/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1008 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/scripts/bivariate_fit_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      780 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/scripts/bivariate_fit_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.257595 copulas-0.9.2/tests/numerical/fit/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.292128 copulas-0.9.2/tests/numerical/fit/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      826 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      828 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.292775 copulas-0.9.2/tests/numerical/fit/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.293230 copulas-0.9.2/tests/numerical/fit/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      966 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/fit/test_fit.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.293728 copulas-0.9.2/tests/numerical/pdf/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.293888 copulas-0.9.2/tests/numerical/pdf/input/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/input/bivariate_pdf_input.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.298706 copulas-0.9.2/tests/numerical/pdf/output/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.299563 copulas-0.9.2/tests/numerical/pdf/scripts/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      603 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_input.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2070 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_output.R
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1694 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_output.m
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.258164 copulas-0.9.2/tests/numerical/pdf/test_cases/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.300552 copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.301834 copulas-0.9.2/tests/numerical/pdf/test_cases/frank/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.302459 copulas-0.9.2/tests/numerical/pdf/test_cases/gumbel/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1086 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/numerical/pdf/test_pdf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.303195 copulas-0.9.2/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.304622 copulas-0.9.2/tests/unit/bivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      490 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3907 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3549 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test_clayton.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3583 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test_frank.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3567 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test_gumbel.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/bivariate/test_independence.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.305342 copulas-0.9.2/tests/unit/multivariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       48 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/multivariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/multivariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18825 2023-10-12 18:34:29.000000 copulas-0.9.2/tests/unit/multivariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24177 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/multivariate/test_tree.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6015 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/multivariate/test_vine.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.305592 copulas-0.9.2/tests/unit/optimize/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       53 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/optimize/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      899 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/optimize/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    17715 2023-10-12 18:34:29.000000 copulas-0.9.2/tests/unit/test___init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 18:34:32.307097 copulas-0.9.2/tests/unit/univariate/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7497 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2432 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_beta.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1428 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_gamma.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6788 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_gaussian_kde.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_log_laplace.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3059 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_selection.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1197 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_student_t.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1532 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_truncated_gaussian.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1387 2023-01-05 18:17:33.000000 copulas-0.9.2/tests/unit/univariate/test_uniform.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.642320 copulas-0.9.2.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       77 2023-08-10 21:03:13.000000 copulas-0.9.2.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6960 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10765 2023-08-10 21:03:13.000000 copulas-0.9.2.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4822 2023-01-06 19:54:16.000000 copulas-0.9.2.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    16906 2023-10-12 00:26:42.642439 copulas-0.9.2.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5194 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6612 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.592010 copulas-0.9.2.dev0/copulas/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9285 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/copulas/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.595759 copulas-0.9.2.dev0/copulas/bivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5087 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13952 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4536 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/clayton.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4641 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/frank.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4216 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/gumbel.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2069 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/independence.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/bivariate/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6831 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/datasets.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.597651 copulas-0.9.2.dev0/copulas/multivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      362 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/multivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5600 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/multivariate/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11140 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/copulas/multivariate/gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22020 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/multivariate/tree.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12882 2023-08-10 21:03:13.000000 copulas-0.9.2.dev0/copulas/multivariate/vine.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.597997 copulas-0.9.2.dev0/copulas/optimize/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4927 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/optimize/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.601237 copulas-0.9.2.dev0/copulas/univariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      825 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19976 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1016 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/beta.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      906 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/gamma.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      728 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6093 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/gaussian_kde.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      921 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/log_laplace.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      944 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/selection.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/student_t.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1932 2023-08-02 16:17:09.000000 copulas-0.9.2.dev0/copulas/univariate/truncated_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      754 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/univariate/uniform.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4665 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/copulas/visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.593349 copulas-0.9.2.dev0/copulas.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    16906 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7597 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1637 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        8 2023-10-12 00:26:42.000000 copulas-0.9.2.dev0/copulas.egg-info/top_level.txt
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.603478 copulas-0.9.2.dev0/docs/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      608 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/Makefile
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       28 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/authors.rst
+-rwxr-xr-x   0 andrewmontanez   (501) staff       (20)     5850 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/docs/conf.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/contributing.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/history.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.607317 copulas-0.9.2.dev0/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15307 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/copulas-200.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    26688 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/copulas.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52079 2023-01-06 19:54:16.000000 copulas-0.9.2.dev0/docs/images/copulas_sample_dataset.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   886153 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/dai-logo-white.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/dice_cdf.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23772 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/pdf_cdf.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9447 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/pit.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   128308 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/images/quickstart.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      651 2023-08-10 21:03:13.000000 copulas-0.9.2.dev0/docs/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      769 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/docs/make.bat
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1446 2023-10-12 00:26:42.642969 copulas-0.9.2.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3945 2023-08-10 21:03:37.000000 copulas-0.9.2.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.608080 copulas-0.9.2.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4710 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.609295 copulas-0.9.2.dev0/tests/end-to-end/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1663 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.610158 copulas-0.9.2.dev0/tests/end-to-end/bivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       51 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/bivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1301 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/bivariate/test_base.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.611395 copulas-0.9.2.dev0/tests/end-to-end/multivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/multivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1146 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7040 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1910 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_vine.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1670 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/test_visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.613173 copulas-0.9.2.dev0/tests/end-to-end/univariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5170 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_beta.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5090 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gamma.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5032 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5576 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gaussian_kde.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5210 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_student_t.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5276 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9510 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/large_scale_evaluation.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.613714 copulas-0.9.2.dev0/tests/numerical/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3795 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.614298 copulas-0.9.2.dev0/tests/numerical/cdf/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.614605 copulas-0.9.2.dev0/tests/numerical/cdf/input/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/input/bivariate_cdf_input.csv
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.618789 copulas-0.9.2.dev0/tests/numerical/cdf/output/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_2_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/clayton_cdf_test_case_3_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      220 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_2_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/frank_cdf_test_case_3_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      217 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/output/gumbel_cdf_test_case_2_output_R.csv
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.619639 copulas-0.9.2.dev0/tests/numerical/cdf/scripts/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2090 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1678 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.586492 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.620809 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      808 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.621766 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.622385 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/gumbel/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1077 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/cdf/test_cdf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.623031 copulas-0.9.2.dev0/tests/numerical/fit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.623659 copulas-0.9.2.dev0/tests/numerical/fit/input/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/input/bivariate_fit_test_case_1_input.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       72 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/input/bivariate_fit_test_case_2_input.csv
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.624309 copulas-0.9.2.dev0/tests/numerical/fit/scripts/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1008 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      780 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.587191 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.624890 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/clayton/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      826 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      828 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.625361 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/frank/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      820 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.625827 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/gumbel/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      823 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      966 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/fit/test_fit.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.626381 copulas-0.9.2.dev0/tests/numerical/pdf/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       44 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.626672 copulas-0.9.2.dev0/tests/numerical/pdf/input/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/input/bivariate_pdf_input.csv
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.630760 copulas-0.9.2.dev0/tests/numerical/pdf/output/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_2_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/clayton_pdf_test_case_3_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_2_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      208 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/frank_pdf_test_case_3_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_1_output_R.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_Matlab.csv
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/output/gumbel_pdf_test_case_2_output_R.csv
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.631641 copulas-0.9.2.dev0/tests/numerical/pdf/scripts/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      603 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2070 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1694 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.588158 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.632699 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      744 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      743 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.633957 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      737 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      733 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.634492 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/gumbel/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      738 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1086 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/numerical/pdf/test_pdf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.635010 copulas-0.9.2.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.637247 copulas-0.9.2.dev0/tests/unit/bivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      490 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3907 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3549 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test_clayton.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3583 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test_frank.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3567 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test_gumbel.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/bivariate/test_independence.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.638834 copulas-0.9.2.dev0/tests/unit/multivariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       48 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/multivariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      382 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/multivariate/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18825 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/tests/unit/multivariate/test_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24177 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/multivariate/test_tree.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6015 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/multivariate/test_vine.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.639420 copulas-0.9.2.dev0/tests/unit/optimize/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       53 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/optimize/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      899 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/optimize/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17715 2023-10-12 00:24:56.000000 copulas-0.9.2.dev0/tests/unit/test___init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-10-12 00:26:42.642107 copulas-0.9.2.dev0/tests/unit/univariate/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       46 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7497 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2432 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_beta.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1428 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_gamma.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1305 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6788 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_gaussian_kde.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1412 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_log_laplace.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3059 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_selection.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1197 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_student_t.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1532 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_truncated_gaussian.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1387 2023-01-05 18:17:33.000000 copulas-0.9.2.dev0/tests/unit/univariate/test_uniform.py
```

### Comparing `copulas-0.9.2/CONTRIBUTING.rst` & `copulas-0.9.2.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/HISTORY.md` & `copulas-0.9.2.dev0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,9 @@
 # History
 
-## v0.9.2 - 2023-10-12
-
-This release removes a warning that was being raised when univariate distributions failed to fit and logs the message instead.
-
-### New Features
-
-* When Copulas univariate fit fails, produce a log instead of a warning - Issue [#359](https://github.com/sdv-dev/Copulas/issues/359) by @R-Palazzo
-
-### Maintenance
-
-* Switch default branch from master to main - Issue [#360](https://github.com/sdv-dev/Copulas/issues/360) by @amontanez24
-* Update add-on detection for Copulas - Issue [#362](https://github.com/sdv-dev/Copulas/issues/362) by @pvk-developer
-
 ## v0.9.1 - 2023-08-10
 
 This release fixes problems with the documentation site and drops support for Python 3.7.
 
 ### Maintenance
 
 * Drop support for Python 3.7 - Issue [#355](https://github.com/sdv-dev/Copulas/issues/355) by @amontanez24
```

### Comparing `copulas-0.9.2/LICENSE` & `copulas-0.9.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/PKG-INFO` & `copulas-0.9.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.9.2
+Version: 0.9.2.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: copulas
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -158,27 +158,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.9.2 - 2023-10-12
-
-This release removes a warning that was being raised when univariate distributions failed to fit and logs the message instead.
-
-### New Features
-
-* When Copulas univariate fit fails, produce a log instead of a warning - Issue [#359](https://github.com/sdv-dev/Copulas/issues/359) by @R-Palazzo
-
-### Maintenance
-
-* Switch default branch from master to main - Issue [#360](https://github.com/sdv-dev/Copulas/issues/360) by @amontanez24
-* Update add-on detection for Copulas - Issue [#362](https://github.com/sdv-dev/Copulas/issues/362) by @pvk-developer
-
 ## v0.9.1 - 2023-08-10
 
 This release fixes problems with the documentation site and drops support for Python 3.7.
 
 ### Maintenance
 
 * Drop support for Python 3.7 - Issue [#355](https://github.com/sdv-dev/Copulas/issues/355) by @amontanez24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.9.2 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.9.2.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -75,47 +75,40 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.2 - 2023-10-12 This release
-removes a warning that was being raised when univariate distributions failed to
-fit and logs the message instead. ### New Features * When Copulas univariate
-fit fails, produce a log instead of a warning - Issue [#359](https://
-github.com/sdv-dev/Copulas/issues/359) by @R-Palazzo ### Maintenance * Switch
-default branch from master to main - Issue [#360](https://github.com/sdv-dev/
-Copulas/issues/360) by @amontanez24 * Update add-on detection for Copulas -
-Issue [#362](https://github.com/sdv-dev/Copulas/issues/362) by @pvk-developer
-## v0.9.1 - 2023-08-10 This release fixes problems with the documentation site
-and drops support for Python 3.7. ### Maintenance * Drop support for Python 3.7
-- Issue [#355](https://github.com/sdv-dev/Copulas/issues/355) by @amontanez24
-### Documentation * Formatting is broken on the main docs page - Issue [#341]
-(https://github.com/sdv-dev/Copulas/issues/341) by @amontanez24 ## v0.9.0 -
-2023-04-26 This release adds support for pandas 2.0 and above. Additionally
-adds a functionality to find version add-ons and renames ``covariance`` to
-``correlation``. ### Maintenance * Remove upper bound for pandas - Issue[#349]
-(https://github.com/sdv-dev/Copulas/issues/349) by @pvk-developer * Rename
-covariance to correlation - PR[#346](https://github.com/sdv-dev/Copulas/pull/
-346) by @frances-h * Add functionality to find version add-on - Issue[#349]
-(https://github.com/sdv-dev/Copulas/issues/349) by @frances-h ## v0.8.0 - 2023-
-01-06 This release adds support for python 3.10 and 3.11. Additionally, it
-drops support for python 3.6. ### Maintenance * Support python 3.10 and above -
-PR[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer *
-Copulas Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/
-Copulas/issues/336) by @pvk-developer * Add support for python 3.10 - PR[#329]
-(https://github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-
-10 This release adds `gaussian` as a fallback distribution in case the user
-specified one fails. It also improves the `fit` of the `beta` distribution by
-properly estimating the `loc` and `scale` parameters. ### General Improvements
-* Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/
-issues/320) by @fealho * Improve the fit of the Beta distribution: Use the new
-loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by
-@pvk-developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
+libraries for specific needs. # History ## v0.9.1 - 2023-08-10 This release
+fixes problems with the documentation site and drops support for Python 3.7.
+### Maintenance * Drop support for Python 3.7 - Issue [#355](https://
+github.com/sdv-dev/Copulas/issues/355) by @amontanez24 ### Documentation *
+Formatting is broken on the main docs page - Issue [#341](https://github.com/
+sdv-dev/Copulas/issues/341) by @amontanez24 ## v0.9.0 - 2023-04-26 This release
+adds support for pandas 2.0 and above. Additionally adds a functionality to
+find version add-ons and renames ``covariance`` to ``correlation``. ###
+Maintenance * Remove upper bound for pandas - Issue[#349](https://github.com/
+sdv-dev/Copulas/issues/349) by @pvk-developer * Rename covariance to
+correlation - PR[#346](https://github.com/sdv-dev/Copulas/pull/346) by
+@frances-h * Add functionality to find version add-on - Issue[#349](https://
+github.com/sdv-dev/Copulas/issues/349) by @frances-h ## v0.8.0 - 2023-01-06
+This release adds support for python 3.10 and 3.11. Additionally, it drops
+support for python 3.6. ### Maintenance * Support python 3.10 and above - PR
+[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer * Copulas
+Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/
+issues/336) by @pvk-developer * Add support for python 3.10 - PR[#329](https://
+github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-10 This
+release adds `gaussian` as a fallback distribution in case the user specified
+one fails. It also improves the `fit` of the `beta` distribution by properly
+estimating the `loc` and `scale` parameters. ### General Improvements * Add
+gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/
+320) by @fealho * Improve the fit of the Beta distribution: Use the new loc and
+scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-
+developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
 functionality by taking in RandomState objects in addition to random seeds. ###
 General Improvements * Use random_state instead of random_seed - Issue[#113]
 (https://github.com/sdv-dev/Copulas/issues/113) by @katxiao ## v0.6.0 - 2021-
 05-13 This release makes Copulas compatible with Python 3.9! It also improves
 library maintenance by updating dependencies, reorganizing the CI workflows,
 adding pip check to the workflows and removing unused files. ### General
 Improvements * Add support for Python 3.9 - Issue[#282](https://github.com/sdv-
```

### Comparing `copulas-0.9.2/README.md` & `copulas-0.9.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/RELEASE.md` & `copulas-0.9.2.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/__init__.py` & `copulas-0.9.2.dev0/copulas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for Copulas."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '0.9.2'
+__version__ = '0.9.2.dev0'
 
 import contextlib
 import importlib
 import sys
 import warnings
 from copy import deepcopy
 from operator import attrgetter
```

### Comparing `copulas-0.9.2/copulas/bivariate/__init__.py` & `copulas-0.9.2.dev0/copulas/bivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/bivariate/base.py` & `copulas-0.9.2.dev0/copulas/bivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/bivariate/clayton.py` & `copulas-0.9.2.dev0/copulas/bivariate/clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/bivariate/frank.py` & `copulas-0.9.2.dev0/copulas/bivariate/frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/bivariate/gumbel.py` & `copulas-0.9.2.dev0/copulas/bivariate/gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/bivariate/independence.py` & `copulas-0.9.2.dev0/copulas/bivariate/independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/datasets.py` & `copulas-0.9.2.dev0/copulas/datasets.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/multivariate/base.py` & `copulas-0.9.2.dev0/copulas/multivariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/multivariate/gaussian.py` & `copulas-0.9.2.dev0/copulas/multivariate/gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/multivariate/tree.py` & `copulas-0.9.2.dev0/copulas/multivariate/tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/multivariate/vine.py` & `copulas-0.9.2.dev0/copulas/multivariate/vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/optimize/__init__.py` & `copulas-0.9.2.dev0/copulas/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/__init__.py` & `copulas-0.9.2.dev0/copulas/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/base.py` & `copulas-0.9.2.dev0/copulas/univariate/base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/beta.py` & `copulas-0.9.2.dev0/copulas/univariate/beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/gamma.py` & `copulas-0.9.2.dev0/copulas/univariate/gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/gaussian.py` & `copulas-0.9.2.dev0/copulas/univariate/gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/gaussian_kde.py` & `copulas-0.9.2.dev0/copulas/univariate/gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/log_laplace.py` & `copulas-0.9.2.dev0/copulas/univariate/log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/selection.py` & `copulas-0.9.2.dev0/copulas/univariate/selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/student_t.py` & `copulas-0.9.2.dev0/copulas/univariate/student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/truncated_gaussian.py` & `copulas-0.9.2.dev0/copulas/univariate/truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/univariate/uniform.py` & `copulas-0.9.2.dev0/copulas/univariate/uniform.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas/visualization.py` & `copulas-0.9.2.dev0/copulas/visualization.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas.egg-info/PKG-INFO` & `copulas-0.9.2.dev0/copulas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copulas
-Version: 0.9.2
+Version: 0.9.2.dev0
 Summary: Create tabular synthetic data using copulas-based modeling.
 Home-page: https://github.com/sdv-dev/Copulas
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: copulas
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -158,27 +158,14 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.9.2 - 2023-10-12
-
-This release removes a warning that was being raised when univariate distributions failed to fit and logs the message instead.
-
-### New Features
-
-* When Copulas univariate fit fails, produce a log instead of a warning - Issue [#359](https://github.com/sdv-dev/Copulas/issues/359) by @R-Palazzo
-
-### Maintenance
-
-* Switch default branch from master to main - Issue [#360](https://github.com/sdv-dev/Copulas/issues/360) by @amontanez24
-* Update add-on detection for Copulas - Issue [#362](https://github.com/sdv-dev/Copulas/issues/362) by @pvk-developer
-
 ## v0.9.1 - 2023-08-10
 
 This release fixes problems with the documentation site and drops support for Python 3.7.
 
 ### Maintenance
 
 * Drop support for Python 3.7 - Issue [#355](https://github.com/sdv-dev/Copulas/issues/355) by @amontanez24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copulas Version: 0.9.2 Summary: Create tabular
+Metadata-Version: 2.1 Name: copulas Version: 0.9.2.dev0 Summary: Create tabular
 synthetic data using copulas-based modeling. Home-page: https://github.com/sdv-
 dev/Copulas Author: DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1
 Keywords: copulas Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -75,47 +75,40 @@
 including: * ð Data discovery & transformation. Reverse the transforms to
 reproduce realistic data. * ð§  Multiple machine learning models -- ranging
 from Copulas to Deep Learning -- to create tabular, multi table and time series
 data. * ð Measuring quality and privacy of synthetic data, and comparing
 different synthetic data generation models. [Get started using the SDV package]
 (https://sdv.dev/SDV/getting_started/install.html) -- a fully integrated
 solution and your one-stop shop for synthetic data. Or, use the standalone
-libraries for specific needs. # History ## v0.9.2 - 2023-10-12 This release
-removes a warning that was being raised when univariate distributions failed to
-fit and logs the message instead. ### New Features * When Copulas univariate
-fit fails, produce a log instead of a warning - Issue [#359](https://
-github.com/sdv-dev/Copulas/issues/359) by @R-Palazzo ### Maintenance * Switch
-default branch from master to main - Issue [#360](https://github.com/sdv-dev/
-Copulas/issues/360) by @amontanez24 * Update add-on detection for Copulas -
-Issue [#362](https://github.com/sdv-dev/Copulas/issues/362) by @pvk-developer
-## v0.9.1 - 2023-08-10 This release fixes problems with the documentation site
-and drops support for Python 3.7. ### Maintenance * Drop support for Python 3.7
-- Issue [#355](https://github.com/sdv-dev/Copulas/issues/355) by @amontanez24
-### Documentation * Formatting is broken on the main docs page - Issue [#341]
-(https://github.com/sdv-dev/Copulas/issues/341) by @amontanez24 ## v0.9.0 -
-2023-04-26 This release adds support for pandas 2.0 and above. Additionally
-adds a functionality to find version add-ons and renames ``covariance`` to
-``correlation``. ### Maintenance * Remove upper bound for pandas - Issue[#349]
-(https://github.com/sdv-dev/Copulas/issues/349) by @pvk-developer * Rename
-covariance to correlation - PR[#346](https://github.com/sdv-dev/Copulas/pull/
-346) by @frances-h * Add functionality to find version add-on - Issue[#349]
-(https://github.com/sdv-dev/Copulas/issues/349) by @frances-h ## v0.8.0 - 2023-
-01-06 This release adds support for python 3.10 and 3.11. Additionally, it
-drops support for python 3.6. ### Maintenance * Support python 3.10 and above -
-PR[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer *
-Copulas Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/
-Copulas/issues/336) by @pvk-developer * Add support for python 3.10 - PR[#329]
-(https://github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-
-10 This release adds `gaussian` as a fallback distribution in case the user
-specified one fails. It also improves the `fit` of the `beta` distribution by
-properly estimating the `loc` and `scale` parameters. ### General Improvements
-* Add gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/
-issues/320) by @fealho * Improve the fit of the Beta distribution: Use the new
-loc and scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by
-@pvk-developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
+libraries for specific needs. # History ## v0.9.1 - 2023-08-10 This release
+fixes problems with the documentation site and drops support for Python 3.7.
+### Maintenance * Drop support for Python 3.7 - Issue [#355](https://
+github.com/sdv-dev/Copulas/issues/355) by @amontanez24 ### Documentation *
+Formatting is broken on the main docs page - Issue [#341](https://github.com/
+sdv-dev/Copulas/issues/341) by @amontanez24 ## v0.9.0 - 2023-04-26 This release
+adds support for pandas 2.0 and above. Additionally adds a functionality to
+find version add-ons and renames ``covariance`` to ``correlation``. ###
+Maintenance * Remove upper bound for pandas - Issue[#349](https://github.com/
+sdv-dev/Copulas/issues/349) by @pvk-developer * Rename covariance to
+correlation - PR[#346](https://github.com/sdv-dev/Copulas/pull/346) by
+@frances-h * Add functionality to find version add-on - Issue[#349](https://
+github.com/sdv-dev/Copulas/issues/349) by @frances-h ## v0.8.0 - 2023-01-06
+This release adds support for python 3.10 and 3.11. Additionally, it drops
+support for python 3.6. ### Maintenance * Support python 3.10 and above - PR
+[#338](https://github.com/sdv-dev/Copulas/pull/338) by @pvk-developer * Copulas
+Package Maintenance Updates - Issue[#336](https://github.com/sdv-dev/Copulas/
+issues/336) by @pvk-developer * Add support for python 3.10 - PR[#329](https://
+github.com/sdv-dev/Copulas/pull/329) by @katxiao ## v0.7.0 - 2022-05-10 This
+release adds `gaussian` as a fallback distribution in case the user specified
+one fails. It also improves the `fit` of the `beta` distribution by properly
+estimating the `loc` and `scale` parameters. ### General Improvements * Add
+gaussian as fallback - Issue[#320](https://github.com/sdv-dev/Copulas/issues/
+320) by @fealho * Improve the fit of the Beta distribution: Use the new loc and
+scale - Issue[#317](https://github.com/sdv-dev/Copulas/issues/317) by @pvk-
+developer ## v0.6.1 - 2022-02-25 This release improves the `random_state`
 functionality by taking in RandomState objects in addition to random seeds. ###
 General Improvements * Use random_state instead of random_seed - Issue[#113]
 (https://github.com/sdv-dev/Copulas/issues/113) by @katxiao ## v0.6.0 - 2021-
 05-13 This release makes Copulas compatible with Python 3.9! It also improves
 library maintenance by updating dependencies, reorganizing the CI workflows,
 adding pip check to the workflows and removing unused files. ### General
 Improvements * Add support for Python 3.9 - Issue[#282](https://github.com/sdv-
```

### Comparing `copulas-0.9.2/copulas.egg-info/SOURCES.txt` & `copulas-0.9.2.dev0/copulas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/copulas.egg-info/requires.txt` & `copulas-0.9.2.dev0/copulas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/Makefile` & `copulas-0.9.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/conf.py` & `copulas-0.9.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/copulas-200.png` & `copulas-0.9.2.dev0/docs/images/copulas-200.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/copulas.png` & `copulas-0.9.2.dev0/docs/images/copulas.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/copulas_sample_dataset.png` & `copulas-0.9.2.dev0/docs/images/copulas_sample_dataset.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/dai-logo-white.png` & `copulas-0.9.2.dev0/docs/images/dai-logo-white.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/dice_cdf.png` & `copulas-0.9.2.dev0/docs/images/dice_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/pdf_cdf.png` & `copulas-0.9.2.dev0/docs/images/pdf_cdf.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/pit.png` & `copulas-0.9.2.dev0/docs/images/pit.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/images/quickstart.png` & `copulas-0.9.2.dev0/docs/images/quickstart.png`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/index.rst` & `copulas-0.9.2.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/docs/make.bat` & `copulas-0.9.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/setup.cfg` & `copulas-0.9.2.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.2
+current_version = 0.9.2.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `copulas-0.9.2/setup.py` & `copulas-0.9.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,10 +132,10 @@
     name='copulas',
     packages=find_packages(include=['copulas', 'copulas.*']),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/Copulas',
-    version='0.9.2',
+    version='0.9.2.dev0',
     zip_safe=False,
 )
```

### Comparing `copulas-0.9.2/tests/__init__.py` & `copulas-0.9.2.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/README.md` & `copulas-0.9.2.dev0/tests/end-to-end/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/bivariate/test_base.py` & `copulas-0.9.2.dev0/tests/end-to-end/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/multivariate/test_base.py` & `copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/multivariate/test_gaussian.py` & `copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/multivariate/test_vine.py` & `copulas-0.9.2.dev0/tests/end-to-end/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/test___init__.py` & `copulas-0.9.2.dev0/tests/end-to-end/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_beta.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_gamma.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_gaussian.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_gaussian_kde.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_student_t.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/end-to-end/univariate/test_truncated_gaussian.py` & `copulas-0.9.2.dev0/tests/end-to-end/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/large_scale_evaluation.py` & `copulas-0.9.2.dev0/tests/large_scale_evaluation.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/README.md` & `copulas-0.9.2.dev0/tests/numerical/README.md`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_input.py` & `copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_output.R` & `copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/scripts/bivariate_cdf_output.m` & `copulas-0.9.2.dev0/tests/numerical/cdf/scripts/bivariate_cdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/clayton/clayton_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/frank/frank_cdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cases/gumbel/gumbel_cdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/cdf/test_cdf.py` & `copulas-0.9.2.dev0/tests/numerical/cdf/test_cdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/scripts/bivariate_fit_output.R` & `copulas-0.9.2.dev0/tests/numerical/fit/scripts/bivariate_fit_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/scripts/bivariate_fit_output.m` & `copulas-0.9.2.dev0/tests/numerical/fit/scripts/bivariate_fit_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/clayton/clayton_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/frank/frank_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/fit/test_cases/gumbel/gumbel_fit_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/fit/test_fit.py` & `copulas-0.9.2.dev0/tests/numerical/fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_input.py` & `copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_input.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_output.R` & `copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.R`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/scripts/bivariate_pdf_output.m` & `copulas-0.9.2.dev0/tests/numerical/pdf/scripts/bivariate_pdf_output.m`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/clayton/clayton_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/frank/frank_pdf_test_case_3.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_1.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_cases/gumbel/gumbel_pdf_test_case_2.json`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/numerical/pdf/test_pdf.py` & `copulas-0.9.2.dev0/tests/numerical/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/bivariate/test_base.py` & `copulas-0.9.2.dev0/tests/unit/bivariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/bivariate/test_clayton.py` & `copulas-0.9.2.dev0/tests/unit/bivariate/test_clayton.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/bivariate/test_frank.py` & `copulas-0.9.2.dev0/tests/unit/bivariate/test_frank.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/bivariate/test_gumbel.py` & `copulas-0.9.2.dev0/tests/unit/bivariate/test_gumbel.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/bivariate/test_independence.py` & `copulas-0.9.2.dev0/tests/unit/bivariate/test_independence.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/multivariate/test_gaussian.py` & `copulas-0.9.2.dev0/tests/unit/multivariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/multivariate/test_tree.py` & `copulas-0.9.2.dev0/tests/unit/multivariate/test_tree.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/multivariate/test_vine.py` & `copulas-0.9.2.dev0/tests/unit/multivariate/test_vine.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/optimize/test___init__.py` & `copulas-0.9.2.dev0/tests/unit/optimize/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/test___init__.py` & `copulas-0.9.2.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_base.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_base.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_beta.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_beta.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_gamma.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_gamma.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_gaussian.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_gaussian_kde.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_log_laplace.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_log_laplace.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_selection.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_selection.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_student_t.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_student_t.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_truncated_gaussian.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_truncated_gaussian.py`

 * *Files identical despite different names*

### Comparing `copulas-0.9.2/tests/unit/univariate/test_uniform.py` & `copulas-0.9.2.dev0/tests/unit/univariate/test_uniform.py`

 * *Files identical despite different names*

