# Comparing `tmp/mrQA-0.2.4.tar.gz` & `tmp/mrQA-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrQA-0.2.4.tar", last modified: Wed Jun  7 17:33:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mrQA-0.2.4.tar` & `mrQA-0.3.tar`

### file list

```diff
@@ -1,64 +1,43 @@
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.256268 mrQA-0.2.4/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      170 2023-06-07 17:11:42.000000 mrQA-0.2.4/AUTHORS.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3491 2022-11-07 22:31:28.000000 mrQA-0.2.4/CONTRIBUTING.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       89 2022-11-07 22:31:28.000000 mrQA-0.2.4/HISTORY.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      583 2022-11-07 22:31:28.000000 mrQA-0.2.4/LICENSE
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      335 2023-06-07 17:23:37.000000 mrQA-0.2.4/MANIFEST.in
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2423 2023-06-07 17:33:05.256268 mrQA-0.2.4/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1559 2023-06-07 17:11:42.000000 mrQA-0.2.4/README.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/docs/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      496 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/API.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      604 2022-11-07 22:31:28.000000 mrQA-0.2.4/docs/Makefile
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       28 2022-11-07 22:31:28.000000 mrQA-0.2.4/docs/authors.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/docs/build/
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/docs/build/html/
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/docs/build/html/_images/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)   144544 2023-03-13 20:29:31.000000 mrQA-0.2.4/docs/build/html/_images/schematic_mrQA.png
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/docs/build/html/_static/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      286 2022-07-14 07:38:19.000000 mrQA-0.2.4/docs/build/html/_static/file.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 mrQA-0.2.4/docs/build/html/_static/minus.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       90 2022-07-14 07:38:19.000000 mrQA-0.2.4/docs/build/html/_static/plus.png
--rwxrwxr-x   0 sinhah    (1000) sinhah    (1000)     4987 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/conf.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       33 2022-11-07 22:31:28.000000 mrQA-0.2.4/docs/contributing.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     8176 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/examples.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1818 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/index.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1114 2022-11-07 22:31:28.000000 mrQA-0.2.4/docs/installation.rst
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      765 2022-11-07 22:31:28.000000 mrQA-0.2.4/docs/make.bat
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)   144544 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/schematic_mrQA.png
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      831 2023-06-07 17:11:42.000000 mrQA-0.2.4/docs/usage.rst
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.256268 mrQA-0.2.4/mrQA/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      336 2022-11-07 22:31:28.000000 mrQA-0.2.4/mrQA/__compliance__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      272 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      497 2023-06-07 17:33:05.256268 mrQA-0.2.4/mrQA/_version.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5204 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/cli.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      451 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/common.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2552 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4140 2023-06-07 17:25:13.000000 mrQA-0.2.4/mrQA/formatter.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    11696 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/layout.html
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     7852 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/monitor.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     9861 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/parallel_utils.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     6481 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/project.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     3987 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/run_merge.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    13002 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/run_parallel.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4148 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/run_subset.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.256268 mrQA-0.2.4/mrQA/tests/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       34 2022-11-07 22:31:28.000000 mrQA-0.2.4/mrQA/tests/__init__.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1097 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/config.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      141 2023-02-22 17:41:50.000000 mrQA-0.2.4/mrQA/tests/conftest.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    11070 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/test_compliance.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     7155 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/test_monitor.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     5688 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/test_parallel.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     8959 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/unit_tests.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     4336 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/tests/utils.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    30481 2023-06-07 17:11:42.000000 mrQA-0.2.4/mrQA/utils.py
-drwxrwxr-x   0 sinhah    (1000) sinhah    (1000)        0 2023-06-07 17:33:05.252268 mrQA-0.2.4/mrQA.egg-info/
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     2423 2023-06-07 17:33:04.000000 mrQA-0.2.4/mrQA.egg-info/PKG-INFO
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1089 2023-06-07 17:33:05.000000 mrQA-0.2.4/mrQA.egg-info/SOURCES.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:33:04.000000 mrQA-0.2.4/mrQA.egg-info/dependency_links.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      146 2023-06-07 17:33:05.000000 mrQA-0.2.4/mrQA.egg-info/entry_points.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        1 2023-06-07 17:33:04.000000 mrQA-0.2.4/mrQA.egg-info/not-zip-safe
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)       51 2023-06-07 17:33:05.000000 mrQA-0.2.4/mrQA.egg-info/requires.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)        5 2023-06-07 17:33:05.000000 mrQA-0.2.4/mrQA.egg-info/top_level.txt
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)      575 2023-06-07 17:33:05.256268 mrQA-0.2.4/setup.cfg
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)     1792 2023-06-07 17:23:54.000000 mrQA-0.2.4/setup.py
--rw-rw-r--   0 sinhah    (1000) sinhah    (1000)    81180 2023-03-16 21:25:02.000000 mrQA-0.2.4/versioneer.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/__compliance__.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/_version.py
+-rw-r--r--   0        0        0    26401 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/base.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/cli.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/config.py
+-rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/formatter.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/monitor.py
+-rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/parallel_utils.py
+-rw-r--r--   0        0        0    23049 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/plotting.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/project.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/run_merge.py
+-rw-r--r--   0        0        0    15495 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/run_parallel.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/run_subset.py
+-rw-r--r--   0        0        0    47393 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/check_status.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/conftest.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/simulate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_base.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_common.py
+-rw-r--r--   0        0        0    13130 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_compliance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_formatter.py
+-rw-r--r--   0        0        0     9771 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_majority.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_monitor.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_parallel.py
+-rw-r--r--   0        0        0    13181 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/test_utils.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/utils.py
+-rw-r--r--   0        0        0  5566627 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/compliant_dicom_data.zip
+-rw-r--r--   0        0        0  5376332 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/example_dicom_data.zip
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/invalid-json.json
+-rw-r--r--   0        0        0   647462 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/invalid.dcm
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/mri-config.json
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/test-config.json
+-rw-r--r--   0        0        0    21128 2020-02-02 00:00:00.000000 mrQA-0.3/mrQA/tests/resources/valid.dcm
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 mrQA-0.3/.gitignore
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mrQA-0.3/AUTHORS.rst
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 mrQA-0.3/LICENSE
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 mrQA-0.3/README.rst
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 mrQA-0.3/pyproject.toml
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 mrQA-0.3/PKG-INFO
```

### Comparing `mrQA-0.2.4/PKG-INFO` & `mrQA-0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,72 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mrQA
-Version: 0.2.4
-Summary: mrQA suite of tools offering automatic evaluation of protocol compliance
-Home-page: https://github.com/Open-Minds-Lab/mrQA
-Author: Pradeep Raamana
-Author-email: raamana@gmail.com
-License: Apache Software License 2.0
-Keywords: mrQA
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Version: 0.3
+Summary: rQA suite of tools offering automatic evaluation of protocol compliance
+Project-URL: Homepage, https://github.com/Open-Minds-Lab/mrQA
+Project-URL: Documentation, https://open-minds-lab.github.io/mrQA/
+Author-email: Pradeep Reddy Raamana <raamana@gmail.com>, Harsh Sinha <harsh.sinha@pitt.edu>
+License-Expression: Apache-2.0
+License-File: AUTHORS.rst
+License-File: LICENSE
+Keywords: protocol compliance, quality assurance
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
+Requires-Python: >=3.8
+Requires-Dist: bokeh
+Requires-Dist: dictdiffer
+Requires-Dist: jinja2>=3.0.3
+Requires-Dist: mrdataset
+Requires-Dist: nibabel
+Requires-Dist: protocol
+Requires-Dist: pydicom
+Requires-Dist: tqdm
+Provides-Extra: test
+Requires-Dist: coverage; extra == 'test'
+Requires-Dist: flake8; extra == 'test'
+Requires-Dist: hypothesis>=6.97.1; extra == 'test'
+Requires-Dist: pytest~=7.1.2; extra == 'test'
+Requires-Dist: requests; extra == 'test'
+Description-Content-Type: text/x-rst
 
 mrQA : automatic protocol compliance checks on MR datasets
 =============================================================
 
 .. image:: https://img.shields.io/pypi/v/mrQA.svg
         :target: https://pypi.python.org/pypi/mrQA
 
-.. image:: https://img.shields.io/travis/Open-Minds-Lab/mrQA.svg
-        :target: https://travis-ci.com/Open-Minds-Lab/mrQA
+.. image:: https://app.codacy.com/project/badge/Grade/8cd263e1eaa0480d8fac50eba0094401
+        :target: https://app.codacy.com/gh/sinhaharsh/mrQA/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+.. image:: https://github.com/sinhaharsh/mrQA/actions/workflows/continuous-integration.yml/badge.svg
+        :target: https://github.com/sinhaharsh/mrQA/actions/workflows/continuous-integration.yml
+
 
 .. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
         :target: https://nbviewer.org/github/Open-Minds-Lab/mrQA/blob/master/examples/usage.ipynb
 
 
-* Documentation: https://open-minds-lab.github.io/mrQA/
+----
 
-A tool for automatic evaluation of protocol compliance in MRI datasets. The tool analyzes MR acquisition data from DICOM headers and compares it against protocol to determine the level of compliance. It takes as input a dataset in DICOM/BIDS format. The tool outputs a compliance report in HTML format, with a percent compliance score for each protocol. The tool also outputs a JSON file with the compliance scores for each modality. In addition, it highlights any deviations from the protocol. The tool has been specifically created keeping radiologists in mind, but can be used by anyone who wants to evaluate that MR scans are acquired according to the pre-defined protocol and to minimize errors in acquisition process.
+Documentation: https://open-minds-lab.github.io/mrQA/
 
-Simple schematic of the library:
-
-.. image:: ./docs/schematic_mrQA.png
+----
 
+``mrQA`` is a tool developed for automatic evaluation of protocol compliance in MRI datasets. The tool analyzes MR acquisition data from DICOM headers and compares it against protocol to determine the level of compliance. It takes as input a dataset in DICOM/BIDS format. The tool outputs a compliance report in HTML format, with a percent compliance score for each sequence/modality in a dataset. The tool also outputs a JSON file with the compliance scores for each modality. In addition, it highlights any deviations from the protocol. The tool has been specifically created keeping in mind those who directly acquired the data such as MR Physicists and Technologists, but can be used by anyone who wants to evaluate that MR scans are acquired according to a pre-defined protocol and to minimize errors in acquisition process.
 
 ``mrQA`` uses ``MRDataset`` to efficiently parse various neuroimaging dataset formats, which is available `here <github.com/Open-Minds-Lab/MRdataset>`_.
 
+Key features:
 
+- evaluation of protocol compliance (within-sequence across-dataset) in an existing dataset
+- continuous monitoring of incoming data (hourly or daily on XNAT server or similar)
+- parallel processing of very large datasets (like ABCD or UK Biobank) on a HPC cluster
+- few more to be released soon including vertical audit within-session across-sequence checks
 
+Simple schematic of the library:
 
+.. image:: ./docs/schematic_mrQA.png
 
-=======
-History
-=======
 
-0.1.0 (2022-05-20)
-------------------
 
-* First release on PyPI.
```

### Comparing `mrQA-0.2.4/docs/index.rst` & `mrQA-0.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 mrQA : automatic protocol compliance checks on MR datasets
 =============================================================
 
-
 .. image:: https://img.shields.io/pypi/v/mrQA.svg
         :target: https://pypi.python.org/pypi/mrQA
 
-.. image:: https://img.shields.io/travis/Open-Minds-Lab/mrQA.svg
-        :target: https://travis-ci.com/Open-Minds-Lab/mrQA
+.. image:: https://app.codacy.com/project/badge/Grade/8cd263e1eaa0480d8fac50eba0094401
+        :target: https://app.codacy.com/gh/sinhaharsh/mrQA/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+.. image:: https://github.com/sinhaharsh/mrQA/actions/workflows/continuous-integration.yml/badge.svg
+        :target: https://github.com/sinhaharsh/mrQA/actions/workflows/continuous-integration.yml
+
 
 .. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
         :target: https://nbviewer.org/github/Open-Minds-Lab/mrQA/blob/master/examples/usage.ipynb
 
 
-* Documentation: https://open-minds-lab.github.io/mrQA/
+----
 
-A tool for automatic evaluation of protocol compliance in MRI datasets. The tool analyzes MR acquisition data from DICOM headers and compares it against protocol to determine the level of compliance. It takes as input a dataset in DICOM/BIDS format. The tool outputs a compliance report in HTML format, with a percent compliance score for each protocol. The tool also outputs a JSON file with the compliance scores for each modality. In addition, it highlights any deviations from the protocol. The tool has been specifically created keeping radiologists in mind, but can be used by anyone who wants to evaluate that MR scans are acquired according to the pre-defined protocol and to minimize errors in acquisition process.
+Documentation: https://open-minds-lab.github.io/mrQA/
 
-Simple schematic of the library:
-
-.. image:: ./schematic_mrQA.png
+----
 
+``mrQA`` is a tool developed for automatic evaluation of protocol compliance in MRI datasets. The tool analyzes MR acquisition data from DICOM headers and compares it against protocol to determine the level of compliance. It takes as input a dataset in DICOM/BIDS format. The tool outputs a compliance report in HTML format, with a percent compliance score for each sequence/modality in a dataset. The tool also outputs a JSON file with the compliance scores for each modality. In addition, it highlights any deviations from the protocol. The tool has been specifically created keeping in mind those who directly acquired the data such as MR Physicists and Technologists, but can be used by anyone who wants to evaluate that MR scans are acquired according to a pre-defined protocol and to minimize errors in acquisition process.
 
 ``mrQA`` uses ``MRDataset`` to efficiently parse various neuroimaging dataset formats, which is available `here <github.com/Open-Minds-Lab/MRdataset>`_.
 
-.. include:: ./usage.rst
+Key features:
 
-Further
--------
-.. toctree::
-    :hidden:
+- evaluation of protocol compliance (within-sequence across-dataset) in an existing dataset
+- continuous monitoring of incoming data (hourly or daily on XNAT server or similar)
+- parallel processing of very large datasets (like ABCD or UK Biobank) on a HPC cluster
+- few more to be released soon including vertical audit within-session across-sequence checks
 
-    self
+Simple schematic of the library:
 
-.. toctree::
-   :maxdepth: 1
+.. image:: ./docs/schematic_mrQA.png
 
 
-   installation
-   examples
-   API
-   contributing
-   authors
 
 
 
-Indices and tables
-------------------
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
```

### Comparing `mrQA-0.2.4/mrQA/cli.py` & `mrQA-0.3/mrQA/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,116 @@
 """Console script for mrQA."""
 import argparse
 import sys
 from pathlib import Path
 
-from MRdataset import import_dataset
-from MRdataset.utils import is_writable, valid_dirs
-from MRdataset.log import logger
+from MRdataset import import_dataset, load_mr_dataset, valid_dirs, \
+    DatasetEmptyException
 
 from mrQA import check_compliance
-from mrQA.config import PATH_CONFIG
+from mrQA import logger
+from mrQA.config import PATH_CONFIG, THIS_DIR
+from mrQA.utils import is_writable
 
 
 def get_parser():
-    """Console script for mrQA."""
+    """Parser for command line interface."""
     parser = argparse.ArgumentParser(
         description='Protocol Compliance of MRI scans',
         add_help=False
     )
 
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
 
     # Add help
     required.add_argument('-d', '--data-source', nargs='+', required=True,
                           help='directory containing downloaded dataset with '
                                'dicom files, supports nested hierarchies')
+    required.add_argument('--config', type=str,
+                          help='path to config file',
+                          default=THIS_DIR / 'resources/mri-config.json')
     optional.add_argument('-o', '--output-dir', type=str,
                           help='specify the directory where the report'
                                ' would be saved. By default, the --data_source '
                                'directory will be used to save reports')
     optional.add_argument('-f', '--format', type=str, default='dicom',
-                          help='type of dataset, one of [dicom|bids|pybids]')
+                          help='type of dataset, one of [dicom|bids]')
     optional.add_argument('-n', '--name', type=str,
                           help='provide a identifier/name for the dataset')
     optional.add_argument('-h', '--help', action='help',
                           default=argparse.SUPPRESS,
                           help='show this help message and exit')
     optional.add_argument('--decimals', type=int, default=3,
                           help='number of decimal places to round to '
                                '(default:0). If decimals are negative it '
                                'specifies the number of positions to the left'
                                'of the decimal point.')
     optional.add_argument('-t', '--tolerance', type=float, default=0,
                           help='tolerance for checking against reference '
-                               'protocol. Default is 0.1')
+                               'protocol. Default is 0')
     # TODO: use this flag to store cache
     optional.add_argument('-v', '--verbose', action='store_true',
                           help='allow verbose output on console')
-    optional.add_argument('-ref', '--reference_path', type=str,
-                          help='.yaml file containing protocol specification')
-    optional.add_argument('--strategy', type=str, default='majority',
-                          help='how to examine parameters [majority|reference].'
-                               '--reference_path required if using reference')
-    optional.add_argument('--include-phantom', action='store_true',
-                          help='whether to include phantom, localizer, '
-                               'aahead_scout')
-    optional.add_argument('--include-nifti-header', action='store_true',
-                          help='whether to check nifti headers for compliance,'
-                               'only used when --format==bids')
-    # Experimental features, not implemented yet.
-    optional.add_argument('-l', '--logging', type=int, default=40,
-                          help='set logging to appropriate level')
-    optional.add_argument('--skip', nargs='+',
-                          help='skip these parameters')
-
+    optional.add_argument('-ref', '--ref-protocol-path', type=str,
+                          help='XML file containing desired protocol. If not '
+                               'provided, the protocol will be inferred from '
+                               'the dataset.')
+    optional.add_argument('-pkl', '--mrds-pkl-path', type=str,
+                          help='.mrds.pkl file can be provided to facilitate '
+                               'faster re-runs.')
     if len(sys.argv) < 2:
         logger.critical('Too few arguments!')
         parser.print_help()
         parser.exit(1)
 
     return parser
 
 
-def main():
+def cli():
+    """
+    Console script for mrQA.
+    """
     args = parse_args()
-
-    dataset = import_dataset(data_source=args.data_source,
-                             ds_format=args.format,
-                             name=args.name,
-                             verbose=args.verbose,
-                             include_phantom=args.include_phantom,
-                             include_nifti_header=args.include_nifti_header)
-
-    check_compliance(dataset=dataset,
-                     strategy=args.strategy,
-                     output_dir=args.output_dir,
-                     decimals=args.decimals,
-                     verbose=args.verbose,
-                     tolerance=args.tolerance,)
+    if args.mrds_pkl_path:
+        dataset = load_mr_dataset(args.mrds_pkl_path)
+    else:
+        dataset = import_dataset(data_source=args.data_source,
+                                 ds_format=args.format,
+                                 name=args.name,
+                                 verbose=args.verbose,
+                                 config_path=args.config,
+                                 output_dir=args.output_dir)
+
+    try:
+        check_compliance(dataset=dataset,
+                         output_dir=args.output_dir,
+                         decimals=args.decimals,
+                         verbose=args.verbose,
+                         tolerance=args.tolerance,
+                         config_path=args.config,
+                         reference_path=args.ref_protocol_path, )
+    except DatasetEmptyException:
+        logger.error("Cannot check compliance if the dataset doesn't have "
+                     "any scans. Please check the dataset.")
+    except NotADirectoryError:
+        logger.error('Provided output directory for saving reports is invalid.'
+                     'Either it is not a directory or it does not exist. ')
     return 0
 
 
 def parse_args():
+    """Validates command line arguments and returns parsed arguments"""
     parser = get_parser()
     args = parser.parse_args()
 
     if args.verbose:
-        logger.setLevel('INFO')
-    else:
         logger.setLevel('WARNING')
+    else:
+        logger.setLevel('ERROR')
 
     if not valid_dirs(args.data_source):
         raise OSError('Expected valid directory for --data_source argument, '
                       'Got {0}'.format(args.data_source))
 
     if args.output_dir is None:
         logger.info('Use --output-dir to specify dir for final directory. '
@@ -110,16 +118,30 @@
         args.output_dir = PATH_CONFIG['output_dir'] / args.name.lower()
         args.output_dir.mkdir(exist_ok=True, parents=True)
     else:
         if not Path(args.output_dir).is_dir():
             try:
                 Path(args.output_dir).mkdir(parents=True, exist_ok=True)
             except OSError as exc:
+                logger.error(f'Unable to create folder {args.output_dir} for '
+                             f'saving reports')
                 raise exc
 
     if not is_writable(args.output_dir):
         raise OSError(f'Output Folder {args.output_dir} is not writable')
+
+    check_path(args.config, '--config')
+    check_path(args.ref_protocol_path, '--ref-protocol-path')
+    check_path(args.mrds_pkl_path, '--mrds-pkl-path')
     return args
 
 
+def check_path(path, arg_name):
+    """Validates if the path is a valid file"""
+    if path is not None:
+        if not Path(path).is_file():
+            raise OSError(
+                f'Expected valid file for {arg_name} argument, Got {path}')
+
+
 if __name__ == "__main__":
-    sys.exit(main())  # pragma: no cover
+    cli()
```

### Comparing `mrQA-0.2.4/mrQA/parallel_utils.py` & `mrQA-0.3/mrQA/parallel_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import math
 import os
 import subprocess
 from pathlib import Path
+from time import sleep
 from typing import Union, Iterable
 
-from MRdataset.log import logger
-from MRdataset.utils import valid_dirs
+from MRdataset import valid_dirs
 
-from mrQA.utils import is_integer_number, execute_local, list2txt
+from mrQA import logger
+from mrQA.utils import is_integer_number, execute_local, list2txt, \
+    folders_with_min_files
 
 
 def _check_args(data_source: Union[str, Path, Iterable] = None,
                 ds_format: str = 'dicom',
                 output_dir: Union[str, Path] = None,
                 debug: bool = False,
                 subjects_per_job: int = None,
                 hpc: bool = False,
                 conda_dist: str = None,
-                conda_env: str = None):
+                conda_env: str = None,
+                config_path: Union[str, Path] = None):
     # It is not possible to submit jobs while debugging, why would you submit
     # a job, if code is still being debugged
     if debug and hpc:
         raise AttributeError('Dont debug on hpc!')
     if ds_format != 'dicom':
         raise NotImplementedError(f'Expects dicom, Got {ds_format}')
     if not is_integer_number(subjects_per_job):
@@ -29,73 +31,76 @@
                            f'Got {subjects_per_job}')
     if subjects_per_job < 1:
         raise RuntimeError('subjects_per_job cannot be less than 1')
 
     # Check if data_source is a valid directory, or list of valid directories
     data_source = valid_dirs(data_source)
 
-    # RULE : If output_dir not provided, output wil be saved in 'mrqa_files'
+    # RULE : If output_dir not provided, output will be saved in 'mrqa_files'
     # created in the parent folder of data_source
     if not output_dir:
         if isinstance(data_source, Iterable):
             # If data_source is a bunch of directories, the above RULE cannot
             # be followed, just pass a directory to save the file.
             raise RuntimeError('Need an output directory to store files')
 
         # Didn't find a good alternative to os.access
-        # in pathlib, please raise a issue if you know one, happy to incorporate
-        output_dir = data_source.parent / (
-            data_source.name + '_mrqa_files')
+        # in pathlib, please raise an issue if you know one,
+        # happy to incorporate
+        parent_dir = Path(data_source[0]).parent
+        output_dir = parent_dir / (data_source[0].name + '_mrqa_files')
 
         # Check if permission to create a folder in data_source.parent
-        if os.access(data_source.parent, os.W_OK):
+        if os.access(parent_dir, os.W_OK):
             logger.warning('Expected a directory to save job scripts. Using '
                            'parent folder of --data_source instead.')
         else:
-            raise PermissionError(f'You do not have write permission to'
-                                  f'create a folder in '
-                                  f'{data_source.parent}'
-                                  f'Please provide output_dir')
+            raise PermissionError('You do not have write permission to'
+                                  'create a folder in '
+                                  f'{parent_dir}'
+                                  'Please provide output_dir')
     else:
         output_dir = Path(output_dir)
     # Information about conda env is required for creating slurm scripts
     # The snippet below sets some defaults, may not be true for everyone.
     # The user can use the arguments to specify
     if not conda_env:
         conda_env = 'mrqa' if hpc else 'mrcheck'
     if not conda_dist:
         conda_dist = 'miniconda3' if hpc else 'anaconda3'
+    if not Path(config_path).exists():
+        raise FileNotFoundError(f'Config file not found at {config_path}')
     return data_source, output_dir, conda_env, conda_dist
 
 
 def _make_file_folders(output_dir):
     output_dir.mkdir(parents=True, exist_ok=True)
     # Create a folder id_lists for saving list of subject ids for each job
     # in a separate txt file.
     # Create a folder bash_scripts for saving bash_script for each job
     # Create a folder 'partial_mrds' for saving partial mrds pkl file
     # created by the corresponding bash script
 
     folder_paths = {
-        'ids': output_dir / 'id_lists',
+        'fnames': output_dir / 'fname_lists',
         'scripts': output_dir / 'bash_scripts',
         'mrds': output_dir / 'partial_mrds'
     }
     files_per_batch = {
-        'ids': output_dir / 'per_batch_id_list.txt',
+        'fnames': output_dir / 'per_batch_folders_list.txt',
         'scripts': output_dir / 'per_batch_script_list.txt',
         'mrds': output_dir / 'per_batch_partial_mrds_list.txt'
     }
 
     for path in folder_paths.values():
         path.mkdir(parents=True, exist_ok=True)
 
     # And store the original complete list (contains all
     # subject ids) in "complete_id_list.txt"
-    all_ids_path = output_dir / 'complete_id_list.txt'
+    all_ids_path = output_dir / 'complete_fname_list.txt'
     return folder_paths, files_per_batch, all_ids_path
 
 
 def _run_single_batch(script_path: Union[str, Path],
                       hpc: bool,
                       output_mrds_path: Union[str, Path]):
     """
@@ -115,14 +120,16 @@
 
     if not output_mrds_path.exists():
         if hpc:
             # If running on a hpc, use the sbatch command
             # to submit the script
             # TODO: Add try/except block here
             subprocess.run(['sbatch', script_path], check=True, shell=True)
+            # Without any delay, you may receive NODE_FAIL error
+            sleep(2)
             # print(out.stdout)
             # some way to check was submitted/accepted
 
         else:
             # If running locally, and the user does not want to
             # submit the job, run the script using the bash command
             execute_local(script_path)
@@ -130,130 +137,127 @@
 
     else:
         logger.warning('%s already exists, skipping.  Use sbatch %s to'
                        ' overwrite', output_mrds_path, script_path)
 
 
 def _create_slurm_script(output_script_path: Union[str, Path],
-                         ids_filepath: Union[str, Path],
+                         fnames_filepath: Union[str, Path],
                          env: str = 'mrqa',
                          conda_dist: str = 'anaconda3',
-                         num_subj_per_job: int = 50,
+                         folders_per_job: int = 50,
                          verbose: bool = False,
-                         include_phantom: bool = False,
-                         output_mrds_path: bool = None) -> None:
+                         config_path: Union[str, Path] = None,
+                         output_mrds_path: bool = None,
+                         email='mail.sinha.harsh@gmail.com') -> None:
     """
     Creates a slurm script file which can be submitted to a hpc.
 
     Parameters
     ----------
     output_script_path : str
         Path to slurm script file
-    ids_filepath : str
+    fnames_filepath : str
         Path to text file containing list of subject ids
     env : str
         Conda environment name
     conda_dist : str
         Conda distribution
-    num_subj_per_job : int
+    folders_per_job : int
         Number of subjects to process in each slurm job
     verbose : bool
         If True, prints the output of the script
-    include_phantom : bool
-        If True, includes phantom, localizer and calibration studies
     output_mrds_path : str
         Path to the partial mrds pickle file
     """
 
     # Memory and CPU time :  typical usage observed locally
 
     # For subjects_per_job = 50             100
     # Max RSS Size (Memory) ~150 MB,        ~160 MB
     # Sys Time (CPU Time) : 10 minutes      20 minutes
 
     # Set the memory and cpu time limits
-    mem_reqd = 2000  # MB;
-    num_mins_per_subject = 1  # minutes
-    num_hours = int(math.ceil(num_subj_per_job * num_mins_per_subject / 60))
+    mem_required = 2000  # MB;
+    # num_mins_per_subject = 1  # minutes
     # Set the number of hours to 3 if less than 3
-    time_limit = 3 if num_hours < 3 else num_hours
+    time_limit = 24
     # Setup python command to run
-    python_cmd = f'mrpc_subset -o {output_mrds_path} -b {ids_filepath}'
+    python_cmd = (f'mrqa_subset -o {output_mrds_path} -b {fnames_filepath} '
+                  f'--config {config_path}')
 
     # Add flags to python command
     if verbose:
         python_cmd += ' --verbose'
-    if include_phantom:
-        python_cmd += ' --include_phantom'
-    python_cmd += ' --is_partial'
+    python_cmd += ' --is-partial'
 
     # Create the slurm script file
     with open(output_script_path, 'w', encoding='utf-8') as fp:
         fp.writelines('\n'.join([
             '#!/bin/bash',
             '#SBATCH -A med220005p',
             '#SBATCH -N 1',
             '#SBATCH -p RM-shared',
-            f'#SBATCH --mem-per-cpu={mem_reqd}M #memory per cpu-core',
+            f'#SBATCH --mem-per-cpu={mem_required}M #memory per cpu-core',
             f'#SBATCH --time={time_limit}:00:00',
             '#SBATCH --ntasks-per-node=1',
-            f'#SBATCH --error={ids_filepath.stem}.%J.err',
-            f'#SBATCH --output={ids_filepath.stem}.%J.out',
+            f'#SBATCH --error={fnames_filepath.stem}.%J.err',
+            f'#SBATCH --output={fnames_filepath.stem}.%J.out',
             '#SBATCH --mail-type=end          # send email when job ends',
             '#SBATCH --mail-type=fail         # send email if job fails',
-            '#SBATCH --mail-user=mail.sinha.harsh@gmail.com',
+            f'#SBATCH --mail-user={email}',
             '#Clear the environment from any previously loaded modules',
             'module purge > /dev/null 2>&1',
             f'source  ${{HOME}}/{conda_dist}/etc/profile.d/conda.sh',
             f'conda activate {env}',
             python_cmd,
             'date\n',
         ])
         )
 
 
-def _get_num_workers(subjects_per_job, subject_list):
-    if subjects_per_job > len(subject_list):
+def _get_num_workers(folders_per_job, folder_list):
+    if folders_per_job > len(folder_list):
         # If subjects_per_job is greater than the number of subjects,
         # process all subjects in a single job. Stop execution.
         raise RuntimeError('Trying to create more jobs than total number of '
-                           'subjects in the directory. Why?')
+                           'folders in the directory. Why?')
 
     # Get the number of jobs
-    workers = len(subject_list) // subjects_per_job
+    workers = len(folder_list) // folders_per_job
     if workers == 1:
         # If there is only one job, process all subjects in a single job
-        raise RuntimeError('Decrease number of subjects per job. Expected'
+        raise RuntimeError('Decrease number of folders per job. Expected'
                            'workers > 1 for parallel processing. Got 1')
 
     return workers
 
 
-def _get_subject_ids(data_source: Union[str, Path],
-                     all_ids_path: Union[str, Path]) -> list:
+def _get_terminal_folders(data_source: Union[str, Path],
+                          all_ids_path: Union[str, Path],
+                          pattern='*',
+                          min_count=1) -> Iterable:
     """
     Get the list of subject ids from the data source folder
 
     Parameters
     ----------
     data_source : Union[str, Path]
         Path to the root directory of the data
     all_ids_path : Union[str, Path]
         Path to the output directory
 
     Returns
     -------
-    subject_list : list
+    subject_list : Iterable
         List of subject ids
     """
-    subject_list = []
+    terminal_folder_list = []
     # Get the list of subject ids
-    for root, _, _ in os.walk(data_source):
-        if 'sub-' in Path(root).name:
-            # Get the subject id
-            num_files_in_root = len(list(Path(root).rglob('*/*')))
-            if num_files_in_root > 0:
-                subject_list.append(root)
+    for directory in valid_dirs(data_source):
+        sub_folders = folders_with_min_files(directory, pattern,
+                                             min_count)
+        terminal_folder_list.extend(sub_folders)
     # Store the list of unique subject ids to a text file given by
     # output_path
-    list2txt(all_ids_path, list(set(subject_list)))
-    return subject_list
+    list2txt(all_ids_path, list(set(terminal_folder_list)))
+    return terminal_folder_list
```

### Comparing `mrQA-0.2.4/mrQA/run_merge.py` & `mrQA-0.3/mrQA/run_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,15 @@
     complete_dataset = _merge_from_disk(mrds_path_list)
     complete_dataset.is_complete = True
     if name:
         complete_dataset.name = name
     save_mr_dataset(output_path, complete_dataset)
 
 
-def _merge_from_disk(mrds_path_list: Union[List[Path], List[str]]) \
-                    -> BaseDataset:
+def _merge_from_disk(mrds_path_list: List) -> BaseDataset:
     """
     Given a list of paths to partial mrds datasets, read and merge
     Keep aggregating along with the loop.
 
     Parameters
     ----------
     mrds_path_list : List[Path]
```

### Comparing `mrQA-0.2.4/mrQA/run_parallel.py` & `mrQA-0.3/mrQA/run_parallel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,117 @@
 """ This module contains functions to run the compliance checks in parallel"""
 import argparse
 import sys
 import time
 from pathlib import Path
 from typing import Iterable, Union
 
-from MRdataset import load_mr_dataset
-from MRdataset.config import MRDS_EXT
-from MRdataset.log import logger
-from MRdataset.utils import valid_paths, is_writable
+from MRdataset import load_mr_dataset, MRDS_EXT, DatasetEmptyException
 
-from mrQA.config import PATH_CONFIG
+from mrQA import check_compliance
+from mrQA import logger
+from mrQA.config import PATH_CONFIG, THIS_DIR
 from mrQA.parallel_utils import _check_args, _make_file_folders, \
-    _run_single_batch, _create_slurm_script, _get_num_workers, _get_subject_ids
+    _run_single_batch, _create_slurm_script, _get_num_workers, \
+    _get_terminal_folders
 from mrQA.run_merge import check_and_merge
 from mrQA.utils import list2txt, split_list, \
     txt2list
-from mrQA import check_compliance
+from mrQA.utils import valid_paths, is_writable
 
 
 def get_parser():
+    """Parser for the CLI"""
     parser = argparse.ArgumentParser(
         description='Parallelize the mrQA compliance checks',
         add_help=False
     )
 
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
 
     # Add help
     optional.add_argument('-h', '--help', action='help',
                           help='show this help message and exit')
     required.add_argument('-d', '--data-source', type=str, required=True,
                           help='directory containing downloaded dataset with '
                                'dicom files, supports nested hierarchies')
+    required.add_argument('--config', type=str,
+                          help='path to config file',
+                          default=THIS_DIR / 'resources/mri-config.json')
     optional.add_argument('-o', '--output-dir', type=str,
                           help='specify the directory where the report'
                                ' would be saved. By default, the --data_source '
                                'directory will be used to save reports')
     optional.add_argument('-p', '--out-mrds-path', type=str,
                           help='specify the path to the output mrds file. ')
     optional.add_argument('-n', '--name', type=str,
                           help='provide a identifier/name for the dataset')
-    optional.add_argument('-s', '--subjects-per-job', type=int, default=5,
-                          help='number of subjects to process per job')
+    optional.add_argument('-j', '--job-size', type=int, default=5,
+                          help='number of folders to process per job')
     optional.add_argument('-e', '--conda-env', type=str, default='mrcheck',
                           help='name of conda environment to use')
     optional.add_argument('-c', '--conda-dist', type=str, default='anaconda3',
                           help='name of conda distribution to use')
     optional.add_argument('-H', '--hpc', action='store_true',
                           help='flag to run on HPC')
     optional.add_argument('-v', '--verbose', action='store_true',
                           help='allow verbose output on console')
+    optional.add_argument('-ref', '--ref-protocol-path', type=str,
+                          help='XML file containing desired protocol. If not '
+                               'provided, the protocol will be inferred from '
+                               'the dataset.')
+    optional.add_argument('--decimals', type=int, default=3,
+                          help='number of decimal places to round to '
+                               '(default:0). If decimals are negative it '
+                               'specifies the number of positions to the left'
+                               'of the decimal point.')
+    optional.add_argument('-t', '--tolerance', type=float, default=0,
+                          help='tolerance for checking against reference '
+                               'protocol. Default is 0')
+
     if len(sys.argv) < 2:
         logger.critical('Too few arguments!')
         parser.print_help()
         parser.exit(1)
 
     return parser
 
 
-def main():
+def cli():
+    """Console script for mrQA."""
     args = parse_args()
     process_parallel(data_source=args.data_source,
                      output_dir=args.output_dir,
                      out_mrds_path=args.out_mrds_path,
                      name=args.name,
-                     subjects_per_job=args.subjects_per_job,
+                     job_size=args.job_size,
                      conda_env=args.conda_env,
                      conda_dist=args.conda_dist,
+                     config_path=args.config,
                      hpc=args.hpc)
     dataset = load_mr_dataset(args.out_mrds_path)
-    check_compliance(dataset=dataset,
-                     output_dir=args.output_dir)
+    try:
+        check_compliance(dataset=dataset,
+                         output_dir=args.output_dir,
+                         decimals=args.decimals,
+                         verbose=args.verbose,
+                         tolerance=args.tolerance,
+                         config_path=args.config,
+                         reference_path=args.ref_protocol_path, )
+    except DatasetEmptyException:
+        logger.error("Cannot check compliance if the dataset doesn't have "
+                     "any scans. Please check the dataset.")
+    except NotADirectoryError:
+        logger.error('Provided output directory for saving reports is invalid.'
+                     'Either it is not a directory or it does not exist. ')
 
 
 def parse_args():
+    """Argument parser for the CLI"""
     parser = get_parser()
     args = parser.parse_args()
 
     if args.verbose:
         logger.setLevel('INFO')
     else:
         logger.setLevel('WARNING')
@@ -91,56 +123,73 @@
     else:
         if not Path(args.output_dir).is_dir():
             try:
                 Path(args.output_dir).mkdir(parents=True, exist_ok=True)
             except OSError as exc:
                 raise exc
 
+    if args.ref_protocol_path is not None:
+        if not Path(args.ref_protocol_path).is_file():
+            raise OSError(
+                'Expected valid file for --ref-protocol-path argument, '
+                'Got {0}'.format(args.ref_protocol_path))
+
     if not is_writable(args.output_dir):
         raise OSError(f'Output Folder {args.output_dir} is not writable')
+
+    if not Path(args.config).is_file():
+        raise FileNotFoundError(f'Expected valid config file, '
+                                f'Got {args.config}')
     return args
 
 
 def process_parallel(data_source: Union[str, Path],
                      output_dir: Union[str, Path],
                      out_mrds_path: Union[str, Path],
                      name: str = None,
-                     subjects_per_job: int = 5,
+                     job_size: int = 5,
                      conda_env: str = 'mrcheck',
                      conda_dist: str = 'anaconda3',
+                     config_path: Union[str, Path] = None,
                      hpc: bool = False):
     """
     Given a folder(or List[folder]) it will divide the work into smaller
-    jobs. Each job will contain a fixed number of subjects. These jobs can be
+    jobs. Each job will contain a fixed number of folders. These jobs can be
     executed in parallel to save time.
 
     Parameters
     ----------
-    data_source: str or Path
-        Path to the folder containing the subject folders
-    output_dir: str or Path
-        Path to the folder where the output will be saved
-    out_mrds_path: str or Path
-        Path to the final output mrds file
+    data_source: str | Path
+        Valid path to the folder containing the multiple folders
+    output_dir: str | Path
+        Valid path to the folder where the output will be saved
+    out_mrds_path: str | Path
+        Valid path to the final output .mrds.pkl file
     name: str
         Name of the final output file
-    subjects_per_job: int
-        Number of subjects to be processed in each job
+    job_size: int
+        Number of folders to be processed in each job
     conda_env: str
         Name of the conda environment to be used
     conda_dist: str
         Name of the conda distribution to be used
     hpc: bool
         Whether to use HPC or not
+    config_path: str
+        Path to the config file
     """
     # One function to process them all!
     # note that it will generate scripts only
     script_list_filepath, mrds_list_filepath = create_script(
+        ds_format='dicom',
+        verbose=False,
+        debug=False,
+        config_path=config_path,
         data_source=data_source,
-        subjects_per_job=subjects_per_job,
+        folders_per_job=job_size,
         conda_env=conda_env,
         conda_dist=conda_dist,
         output_dir=output_dir,
         hpc=hpc,
     )
     # Generate slurm scripts and submit jobs, for local parallel processing
     submit_job(scripts_list_filepath=script_list_filepath,
@@ -161,15 +210,15 @@
 
 
 def submit_job(scripts_list_filepath: Union[str, Path],
                mrds_list_filepath: Union[str, Path],
                hpc: bool = False) -> None:
     """
     Given a folder(or List[folder]) it will divide the work into smaller
-    jobs. Each job will contain a fixed number of subjects. These jobs can be
+    jobs. Each job will contain a fixed number of folders. These jobs can be
     executed in parallel to save time.
 
     Parameters
     ----------
     scripts_list_filepath: str
         Path to the file containing list of bash scripts to be executed
     mrds_list_filepath: str
@@ -188,144 +237,146 @@
         _run_single_batch(script_path=script_path,
                           hpc=hpc,
                           output_mrds_path=output_mrds_path)
 
 
 def create_script(data_source: Union[str, Path, Iterable] = None,
                   ds_format: str = 'dicom',
-                  include_phantom: bool = False,
                   verbose: bool = False,
                   output_dir: Union[str, Path] = None,
                   debug: bool = False,
-                  subjects_per_job: int = None,
+                  folders_per_job: int = None,
                   hpc: bool = False,
                   conda_dist: str = None,
-                  conda_env: str = None):
+                  conda_env: str = None,
+                  config_path: Union[str, Path] = None):
     """
     Given a folder(or List[folder]) it will divide the work into smaller
-    jobs. Each job will contain a fixed number of subjects. These jobs can be
+    jobs. Each job will contain a fixed number of folders. These jobs can be
     executed in parallel to save time.
 
     Parameters
     ----------
     data_source: str or List[str]
         /path/to/my/dataset containing files
     ds_format: str
         Specify dataset type. Use one of [dicom]
-    include_phantom: bool
-        Include phantom scans in the dataset
     verbose: bool
         Print progress
     output_dir: str
         Path to save the output dataset
     debug: bool
         If True, the dataset will be created locally. This is useful for testing
-    subjects_per_job: int
-        Number of subjects per job. Recommended value is 50 or 100
+    folders_per_job: int
+        Number of folders per job. Recommended value is 50 or 100
     hpc: bool
         If True, the scripts will be generated for HPC, not for local execution
     conda_dist: str
         Name of conda distribution
     conda_env: str
         Name of conda environment
+    config_path: str
+        Path to the config file
     """
 
     data_src, output_dir, env, dist = _check_args(data_source, ds_format,
                                                   output_dir, debug,
-                                                  subjects_per_job, hpc,
-                                                  conda_dist, conda_env)
-    folder_paths, files_per_batch, all_ids_path = _make_file_folders(output_dir)
-    ids_path_list = split_ids_list(
+                                                  folders_per_job, hpc,
+                                                  conda_dist, conda_env,
+                                                  config_path)
+    folder_paths, files_per_batch, all_fnames_path = _make_file_folders(
+        output_dir)
+    fnames_path_list = split_folders_list(
         data_src,
-        all_ids_path=all_ids_path,
-        per_batch_ids=files_per_batch['ids'],
-        output_dir=folder_paths['ids'],
-        subjects_per_job=subjects_per_job
+        all_fnames_path=all_fnames_path,
+        per_batch_ids=files_per_batch['fnames'],
+        output_dir=folder_paths['fnames'],
+        folders_per_job=folders_per_job
     )
 
     scripts_path_list = []
     mrds_path_list = []
-    # create a slurm job script for each sub_group of subject ids
-    for ids_filepath in ids_path_list:
+    # create a slurm job script for each sub_group of folders
+    for fnames_filepath in fnames_path_list:
         # Filename of the bash script should be same as text file.
-        # Say batch0000.txt points to set of 10 subjects. Then create a
-        # slurm script file batch0000.sh which will run for these 10 subjects,
+        # Say batch0000.txt points to set of 10 folders. Then create a
+        # slurm script file batch0000.sh which will run for these 10 folders,
         # and the final partial mrds pickle file will have the name
         # batch0000.mrds.pkl
-        script_filename = ids_filepath.stem + '.sh'
-        partial_mrds_filename = ids_filepath.stem + MRDS_EXT
+        script_filename = fnames_filepath.stem + '.sh'
+        partial_mrds_filename = fnames_filepath.stem + MRDS_EXT
         script_filepath = folder_paths['scripts'] / script_filename
         partial_mrds_filepath = folder_paths['mrds'] / partial_mrds_filename
 
         # Keep storing the filenames. The entire list would be saved at the end
         scripts_path_list.append(script_filepath)
         mrds_path_list.append(partial_mrds_filepath)
 
         # Finally create the slurm script and save to disk
         _create_slurm_script(output_script_path=script_filepath,
-                             ids_filepath=ids_filepath,
+                             fnames_filepath=fnames_filepath,
                              env=conda_env,
                              conda_dist=conda_dist,
-                             num_subj_per_job=subjects_per_job,
+                             folders_per_job=folders_per_job,
                              verbose=verbose,
-                             include_phantom=include_phantom,
+                             config_path=config_path,
                              output_mrds_path=partial_mrds_filepath)
 
     # Finally, save the all the paths to create mrds pickle files and all the
     # paths to generated scripts in a text file for reference.
     list2txt(fpath=files_per_batch['mrds'], list_=mrds_path_list)
     list2txt(fpath=files_per_batch['scripts'], list_=scripts_path_list)
     return files_per_batch['scripts'], files_per_batch['mrds']
 
 
-def split_ids_list(data_source: Union[str, Path],
-                   all_ids_path: Union[str, Path],
-                   per_batch_ids: Union[str, Path],
-                   output_dir: Union[str, Path],
-                   subjects_per_job: int = 50):
+def split_folders_list(data_source: Union[str, Path],
+                       all_fnames_path: Union[str, Path],
+                       per_batch_ids: Union[str, Path],
+                       output_dir: Union[str, Path],
+                       folders_per_job: int = 50):
     """
-    Splits a given set of subjects into multiple jobs and creates separate
-    text files containing the list of subjects. Each text file
-    contains the list of subjects to be processed in a single job.
+    Splits a given set of folders into multiple jobs and creates separate
+    text files containing the list of folders. Each text file
+    contains the list of folders to be processed in a single job.
 
     Parameters
     ----------
     data_source : Union[str, Path]
         Path to the root directory of the data
-    all_ids_path : Union[str, Path]
+    all_fnames_path : Union[str, Path]
         Path to the output directory
     per_batch_ids : Union[str, Path]
         filepath to a file which has paths to all txt files for all jobs.
-        Each of these txt files contains a list of subject ids for
+        Each of these txt files contains a list of folder ids for
         corresponding job.
     output_dir : Union[str, Path]
         Name of the output directory
-    subjects_per_job : int
-        Number of subjects to process in each job
+    folders_per_job : int
+        Number of folders to process in each job
 
     Returns
     -------
-    batch_ids_path_list : list
-        Paths to the text files, each containing a list of subjects
+    batch_ids_path_list : Sized
+        Paths to the text files, each containing a list of folders
     """
 
-    all_ids_path = Path(all_ids_path)
+    all_fnames_path = Path(all_fnames_path)
     # List of paths to the txt files,
-    # each containing the list of subjects per job
-    batch_ids_path_list = []
+    # each containing the list of folders per job
+    batch_fnames_path_list = []
 
-    subject_list = _get_subject_ids(data_source, all_ids_path)
-    # Get the list of subjects for each job
-    workers = _get_num_workers(subjects_per_job, subject_list)
-    subject_subsets = split_list(subject_list, num_chunks=workers)
+    folder_list = _get_terminal_folders(data_source, all_fnames_path)
+    # Get the list of folders for each job
+    workers = _get_num_workers(folders_per_job, folder_list)
+    folder_subsets = split_list(folder_list, num_chunks=workers)
 
     # Create a text file for each job
-    for i, subset in enumerate(subject_subsets):
-        # Create a text file containing the list of subjects for each job
+    for i, subset in enumerate(folder_subsets):
+        # Create a text file containing the list of folders for each job
         batch_filepath = output_dir / f'batch{i:04}.txt'
         # Store to the path given to the text file
         list2txt(batch_filepath, subset)
         # Add the path to the text file ( containing the
-        # list of subjects for each job) to a list, return the list
-        batch_ids_path_list.append(batch_filepath)
-    list2txt(fpath=per_batch_ids, list_=batch_ids_path_list)
-    return batch_ids_path_list
+        # list of folders for each job) to a list, return the list
+        batch_fnames_path_list.append(batch_filepath)
+    list2txt(fpath=per_batch_ids, list_=batch_fnames_path_list)
+    return batch_fnames_path_list
```

### Comparing `mrQA-0.2.4/mrQA/run_subset.py` & `mrQA-0.3/mrQA/run_subset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,141 @@
 """ Console script for running subset of dataset, a part of parallel
 processing"""
 import argparse
 import sys
 from pathlib import Path
+from typing import Union
 
-from MRdataset import import_dataset, save_mr_dataset
-from MRdataset.base import BaseDataset
-from MRdataset.log import logger
+from MRdataset import import_dataset, save_mr_dataset, BaseDataset
 
+from mrQA import logger
+from mrQA.config import THIS_DIR
 from mrQA.utils import txt2list
 
 
-def main():
+def parse_args():
+    parser = get_parser()
+    args = parser.parse_args()
+
+    if args.verbose:
+        logger.setLevel('WARNING')
+    else:
+        logger.setLevel('ERROR')
+
+    return args
+
+
+def get_parser():
     """Console script for mrQA."""
     parser = argparse.ArgumentParser(
         description='Protocol Compliance of MRI scans',
         add_help=False
     )
 
     required = parser.add_argument_group('required arguments')
     optional = parser.add_argument_group('optional arguments')
 
-    required.add_argument('-o', '--output_path', type=str, required=True,
+    required.add_argument('-o', '--output-path', type=str,
+                          required=True,
                           help='complete path to pickle file for storing '
                                'partial dataset')
-    required.add_argument('-b', '--batch_ids_file', type=str, required=True,
+    required.add_argument('-b', '--batch-ids-file', type=str,
+                          required=True,
                           help='text file path specifying the folders to read')
     optional.add_argument('-h', '--help', action='help',
                           default=argparse.SUPPRESS,
                           help='show this help message and exit')
-    optional.add_argument('--is_partial', action='store_true',
+    optional.add_argument('--is-partial', action='store_true',
                           help='flag dataset as a partial dataset')
     # TODO: use this flag to store cache
     optional.add_argument('-v', '--verbose', action='store_true',
                           help='allow verbose output on console')
-    optional.add_argument('--include_phantom', action='store_true',
-                          help='whether to include phantom, localizer, '
-                               'aahead_scout')
+    required.add_argument('--config', type=str,
+                          help='path to config file',
+                          default=THIS_DIR / 'resources/mri-config.json')
 
     if len(sys.argv) < 2:
         logger.critical('Too few arguments!')
         parser.print_help()
         parser.exit(1)
 
-    args = parser.parse_args()
-    output_path = Path(args.output_path).resolve()
+    return parser
 
-    if args.verbose:
-        logger.setLevel('INFO')
-    else:
-        logger.setLevel('WARNING')
+
+def cli():
+    """Console script for mrQA subset."""
+    args = parse_args()
+    output_path = Path(args.output_path).resolve()
 
     if not output_path.exists():
-        partial_dataset = read_subset(output_path=args.output_path,
+        partial_dataset = read_subset(output_dir=Path(args.output_path).parent,
                                       batch_ids_file=args.batch_ids_file,
                                       ds_format='dicom',
                                       verbose=args.verbose,
-                                      include_phantom=args.include_phantom,
+                                      config_path=args.config,
                                       is_complete=not args.is_partial)
 
         partial_dataset.is_complete = False
         save_mr_dataset(args.output_path, partial_dataset)
 
 
-def read_subset(batch_ids_file: str,
+def read_subset(output_dir: Union[str, Path],
+                batch_ids_file: str,
                 ds_format: str,
                 verbose: bool,
-                include_phantom: bool,
+                config_path: str = None,
+                is_complete: bool = True,
                 **kwargs) -> BaseDataset:
     """
     Given a list of folder paths, reads all dicom files in those folders
     and returns a MRdataset object. In context, when this function was created,
     each folder corresponds to a different subject.
 
     Parameters
     ----------
+    output_dir : Path | str
+        path to a folder where the partial dataset will be saved
     batch_ids_file : str
         path to a text file containing a list of paths (to several folders)
     ds_format : str
         what kind of MRdataset to create, dicom, bids etc.
     verbose : bool
         print more while doing the job
-    include_phantom : bool
-        whether to include phantom files in processing
+    config_path : str
+        path to config file
+    is_complete : bool
+        whether the dataset is subset of a larger dataset. It is useful for
+        parallel processing of large datasets.
     **kwargs: dict
         additional arguments to pass to import_dataset
 
+
     Returns
     -------
     BaseDataset
 
     Raises
     ------
     NotImplementedError
         if ds_format is not dicom
     """
     # Supports only dicom for now
     if ds_format != 'dicom':
-        raise NotImplementedError(f'Expected ds_format as dicom, Got {ds_format}')
+        raise NotImplementedError(
+            f'Expected ds_format as dicom, Got {ds_format}')
 
     subset = txt2list(batch_ids_file)
     identifier = Path(batch_ids_file).stem
     partial_dataset = import_dataset(data_source=subset,
                                      ds_format=ds_format,
                                      name=identifier,
                                      verbose=verbose,
-                                     include_phantom=include_phantom,
+                                     config_path=config_path,
+                                     output_dir=output_dir,
+                                     is_complete=is_complete,
                                      **kwargs)
-    # partial_dataset.walk(), import_dataset already does this
+    # partial_dataset.load(), import_dataset already does this
     return partial_dataset
 
 
 if __name__ == '__main__':
-    sys.exit(main())  # pragma: no cover
+    sys.exit(cli())  # pragma: no cover
```

### Comparing `mrQA-0.2.4/mrQA/tests/test_compliance.py` & `mrQA-0.3/mrQA/tests/test_compliance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,252 +1,271 @@
+import tempfile
 from collections import defaultdict
 from pathlib import Path
 
-import MRdataset.config
 import hypothesis.strategies as st
 from MRdataset import import_dataset
-from MRdataset.simulate import make_compliant_test_dataset, \
-    make_test_dataset, make_bids_test_dataset
-from bids import BIDSLayout
 from hypothesis import given, settings, assume
-
 from mrQA import check_compliance
-from mrQA.tests.config import const_bids
+from mrQA.tests.simulate import make_test_dataset
+from mrQA.utils import get_config_from_file
 
+THIS_DIR = Path(__file__).parent.resolve()
 
-@settings(max_examples=50, deadline=None)
-@given(st.integers(min_value=0, max_value=10),
-       st.floats(allow_nan=False,
-                 allow_infinity=False),
-       st.integers(min_value=-10000000, max_value=10000000),
-       st.floats(allow_nan=False,
-                 allow_infinity=False))
-def test_compliance_all_clean(num_subjects,
-                              repetition_time,
-                              echo_train_length,
-                              flip_angle):
-    """pass compliant datasets, and make sure library recognizes them as such"""
-    dest_dir = make_compliant_test_dataset(num_subjects,
-                                           repetition_time,
-                                           echo_train_length,
-                                           flip_angle)
-    fake_mrd_dataset = import_dataset(dest_dir, include_phantom=True)
-    checked_dataset = check_compliance(dataset=fake_mrd_dataset)
-
-    sub_names_by_modality = defaultdict(list)
-    for modality_pat in Path(dest_dir).iterdir():
-        if modality_pat.is_dir() and ('.mrdataset' not in str(modality_pat)):
-            for subject_path in modality_pat.iterdir():
-                sub_names_by_modality[modality_pat.name].append(
-                    subject_path.name)
-
-    for modality in checked_dataset.modalities:
-        percent_compliant = len(modality.compliant_subject_names) / len(
-            modality.subjects)
-        assert percent_compliant == 1.
-
-        percent_non_compliant = len(modality.non_compliant_subject_names) / len(
-            modality.subjects)
-        assert percent_non_compliant == 0
-
-        assert len(modality.non_compliant_subject_names) == 0
-        assert len(modality.compliant_subject_names) == len(
-            modality._children.keys())
-
-        assert set(sub_names_by_modality[modality.name]) == set(
-            modality.compliant_subject_names)
-        assert len(modality.non_compliant_params) == 0
-
-        assert modality.compliant
-        assert not modality.is_multi_echo()
-
-        for subject in modality.subjects:
-            for session in subject.sessions:
-                for run in session.runs:
-                    assert not run.delta
-                    assert run.params['tr'] == repetition_time
-                    assert run.params[
-                               'echo_train_length'] == echo_train_length
-                    assert run.params['flip_angle'] == flip_angle
-                    assert modality.reference[run.echo_time]['tr'] == \
-                           repetition_time
-                    assert modality.reference[run.echo_time][
-                               'echo_train_length'] == \
-                           echo_train_length
-                    assert modality.reference[run.echo_time][
-                               'flip_angle'] == flip_angle
+
+# @settings(max_examples=50, deadline=None)
+# @given(st.integers(min_value=0, max_value=10),
+#        st.floats(allow_nan=False,
+#                  allow_infinity=False),
+#        st.integers(min_value=-10000000, max_value=10000000),
+#        st.floats(allow_nan=False,
+#                  allow_infinity=False))
+# def test_compliance_all_clean(num_subjects,
+#                               repetition_time,
+#                               echo_train_length,
+#                               flip_angle):
+#     """pass compliant datasets, and make sure library recognizes them as such"""
+#     dest_dir = make_compliant_test_dataset(num_subjects,
+#                                            repetition_time,
+#                                            echo_train_length,
+#                                            flip_angle)
+#     fake_mrd_dataset = import_dataset(dest_dir, output_dir=tempdir)
+#     checked_dataset = check_compliance(dataset=fake_mrd_dataset)
+#
+#     sub_names_by_modality = defaultdict(list)
+#     for modality_pat in Path(dest_dir).iterdir():
+#         if modality_pat.is_dir() and ('.mrdataset' not in str(modality_pat)):
+#             for subject_path in modality_pat.iterdir():
+#                 sub_names_by_modality[modality_pat.name].append(
+#                     subject_path.name)
+#
+#     for modality in checked_dataset.modalities:
+#         percent_compliant = len(modality.compliant_subject_names) / len(
+#             modality.subjects)
+#         assert percent_compliant == 1.
+#
+#         percent_non_compliant = len(modality.non_compliant_subject_names) / len(
+#             modality.subjects)
+#         assert percent_non_compliant == 0
+#
+#         assert len(modality.non_compliant_subject_names) == 0
+#         assert len(modality.compliant_subject_names) == len(
+#             modality._children.keys())
+#
+#         assert set(sub_names_by_modality[modality.name]) == set(
+#             modality.compliant_subject_names)
+#         assert len(modality.non_compliant_params) == 0
+#
+#         assert modality.compliant
+#         assert not modality.is_multi_echo()
+#
+#         for subject in modality.subjects:
+#             for session in subject.sessions:
+#                 for run in session.runs:
+#                     assert not run.delta
+#                     assert run.params['tr'] == repetition_time
+#                     assert run.params[
+#                                'echo_train_length'] == echo_train_length
+#                     assert run.params['flip_angle'] == flip_angle
+#                     assert modality.reference[run.echo_time]['tr'] == \
+#                            repetition_time
+#                     assert modality.reference[run.echo_time][
+#                                'echo_train_length'] == \
+#                            echo_train_length
+#                     assert modality.reference[run.echo_time][
+#                                'flip_angle'] == flip_angle
 
 
 def assert_list(list1, list2):
     if set(list1) == set(list2):
         if len(list1) == len(list2):
             return True
     return False
 
 
-@settings(max_examples=100, deadline=None)
+@settings(max_examples=5, deadline=None)
 @given(st.lists(st.integers(min_value=0, max_value=3), min_size=15,
                 max_size=15),
        st.floats(allow_nan=False, allow_infinity=False),
        st.integers(min_value=-10000000, max_value=10000000),
        st.floats(allow_nan=False, allow_infinity=False)
        )
 def test_non_compliance(num_noncompliant_subjects,
                         repetition_time,
                         echo_train_length,
                         flip_angle):
     """pass non-compliant ds, and ensure library recognizes them as such"""
-    assume(repetition_time != 200)
-    assume(echo_train_length != 4000)
-    assume(flip_angle != 80)
-
-    fake_ds_dir, dataset_info = \
-        make_test_dataset(num_noncompliant_subjects,
-                          repetition_time,
-                          echo_train_length,
-                          flip_angle)
-    mrd = import_dataset(fake_ds_dir, include_phantom=True)
-    checked_dataset = check_compliance(dataset=mrd)
-
-    # Check on disk, basically the truth
-    sub_names_by_modality = defaultdict(list)
-    for modality_path in Path(fake_ds_dir).iterdir():
-        if modality_path.is_dir() and ('.mrdataset' not in str(modality_path)):
-            for subject_path in modality_path.iterdir():
-                sub_names_by_modality[modality_path.name].append(
-                    subject_path.name)
-
-    # Check if modalities are equal
-    non_compliant_modality_names = [m for m in dataset_info if dataset_info[m]]
-    assert assert_list(sub_names_by_modality.keys(),
-                       checked_dataset._children.keys())
-
-    assert assert_list(checked_dataset.non_compliant_modality_names,
-                       non_compliant_modality_names)
-
-    assert assert_list(checked_dataset.compliant_modality_names,
-                       set(checked_dataset._children.keys()) - set(
-                           non_compliant_modality_names))
-
-    for modality in checked_dataset.modalities:
-        # GT
-        all_subjects = sub_names_by_modality[modality.name]
-        non_compliant_subjects = dataset_info[modality.name]
-        compliant_subjects = set(all_subjects) - set(non_compliant_subjects)
-
-        # What did you parse
-        assert assert_list(all_subjects, modality._children.keys())
-        assert assert_list(non_compliant_subjects,
-                           modality.non_compliant_subject_names)
-        assert assert_list(compliant_subjects, modality.compliant_subject_names)
-
-        # Check if reference has the right values
-        echo_time = list(modality.reference.keys())[0]
-        assert modality.reference[echo_time]['tr'] == 200
-        assert modality.reference[echo_time]['echo_train_length'] == 4000
-        assert modality.reference[echo_time]['flip_angle'] == 80
-
-        for subject in modality.subjects:
-            for session in subject.sessions:
-                for run in session.runs:
-                    if run.delta:
-                        assert run.params['tr'] == repetition_time
-                        assert run.params[
-                                   'echo_train_length'] == echo_train_length
-                        assert run.params['flip_angle'] == flip_angle
-                    else:
-                        assert run.params['tr'] == 200
-                        assert run.params[
-                                   'echo_train_length'] == 4000
-                        assert run.params['flip_angle'] == 80
-
-
-@settings(max_examples=30, deadline=None)
-@given(st.lists(st.integers(min_value=0, max_value=2), min_size=11,
-                max_size=11),
-       st.floats(allow_nan=False, allow_infinity=False),
-       st.floats(allow_nan=False, allow_infinity=False),
-       st.floats(allow_nan=False, allow_infinity=False)
-       )
-def test_non_compliance_bids(num_noncompliant_subjects,
-                             repetition_time,
-                             magnetic_field_strength,
-                             flip_angle):
-    """pass non-compliant ds, and ensure library recognizes them as such"""
-    assume(repetition_time != const_bids['tr'])
-    assume(magnetic_field_strength != const_bids['b0'])
-    assume(flip_angle != const_bids['fa'])
-
-    fake_dir, dataset_info = make_bids_test_dataset(num_noncompliant_subjects,
-                                                    repetition_time,
-                                                    magnetic_field_strength,
-                                                    flip_angle)
-    mrd = import_dataset(fake_dir, include_phantom=True, ds_format='bids')
-    checked_dataset = check_compliance(dataset=mrd, output_dir=mrd.data_source)
-
-    # Check on disk, basically the truth
-    layout = BIDSLayout(fake_dir)
-    sub_names_by_modality = defaultdict(set)
-    subjects = layout.get_subjects()
-
-    for modality in MRdataset.config.datatypes:
-        for sub in subjects:
-            filters = {'datatype': modality,
-                       'subject': sub,
-                       'extension': 'json'}
-            files = layout.get(**filters)
-            if files:
-                sub_names_by_modality[modality].add(sub)
-
-    # Check if modalities are equal
-    non_compliant_modality_names = [m for m in dataset_info if dataset_info[m]]
-    assert assert_list(sub_names_by_modality.keys(),
-                       checked_dataset._children.keys())
-
-    assert assert_list(checked_dataset.non_compliant_modality_names,
-                       non_compliant_modality_names)
-
-    assert assert_list(checked_dataset.compliant_modality_names,
-                       set(checked_dataset._children.keys()) - set(
-                           non_compliant_modality_names))
-
-    for modality in checked_dataset.modalities:
-        # GT
-        all_subjects = sub_names_by_modality[modality.name]
-        non_compliant_subjects = dataset_info[modality.name]
-        compliant_subjects = set(all_subjects) - set(non_compliant_subjects)
-
-        # What did you parse
-        assert assert_list(all_subjects, modality._children.keys())
-        assert assert_list(non_compliant_subjects,
-                           modality.non_compliant_subject_names)
-        assert assert_list(compliant_subjects, modality.compliant_subject_names)
-
-        # Check if reference has the right values
-        echo_times = modality.get_echo_times()
-        for te in echo_times:
-            reference = modality.get_reference(te)
-            assert reference['RepetitionTime'] == const_bids['tr']
-            assert reference['MagneticFieldStrength'] == const_bids['b0']
-            assert reference['FlipAngle'] == const_bids['fa']
-
-        for subject in modality.subjects:
-            for session in subject.sessions:
-                for run in session.runs:
-                    if run.delta:
-                        assert run.params['RepetitionTime'] == repetition_time
-                        assert run.params['MagneticFieldStrength'] == \
-                               magnetic_field_strength
-                        assert run.params['FlipAngle'] == flip_angle
-                    else:
-                        assert run.params['RepetitionTime'] == const_bids['tr']
-                        assert run.params['MagneticFieldStrength'] == \
-                               const_bids['b0']
-                        assert run.params['FlipAngle'] == const_bids['fa']
-
-
-if __name__ == '__main__':
-    test_non_compliance_bids(num_noncompliant_subjects=[1, 0, 0, 2, 0, 0, 1, 0,
-                                                        0, 2, 2],
-                             repetition_time=0.0,
-                             magnetic_field_strength=0.0,
-                             flip_angle=0.0)
+    with tempfile.TemporaryDirectory() as tempdir:
+        assume(repetition_time != 200)
+        assume(echo_train_length != 4000)
+        assume(flip_angle != 80)
+
+        fake_ds_dir, dataset_info = \
+            make_test_dataset(num_noncompliant_subjects,
+                              repetition_time,
+                              echo_train_length,
+                              flip_angle)
+        mrd = import_dataset(fake_ds_dir,
+                             config_path=THIS_DIR / 'resources/mri-config.json',
+                             output_dir=tempdir)
+        hz_audit_results, vt_audit_results, report_path = check_compliance(
+            dataset=mrd,
+            output_dir=tempdir,
+            config_path=THIS_DIR / 'resources/mri-config.json')
+        config_dict = get_config_from_file(
+            THIS_DIR / 'resources/mri-config.json')
+        # include_params = config_dict['include_parameters']
+        stratify_by = config_dict.get('stratify_by', None)
+
+        if hz_audit_results is not None:
+            # Check on disk, basically the truth
+            sub_names_by_modality = defaultdict(list)
+            for modality_path in Path(fake_ds_dir).iterdir():
+                if modality_path.is_dir() and (
+                    '.mrdataset' not in str(modality_path)):
+                    for subject_path in modality_path.iterdir():
+                        sub_names_by_modality[modality_path.name].append(
+                            subject_path.name)
+
+            fully_compliant_ds = hz_audit_results['compliant']
+            non_compliant_ds = hz_audit_results['non_compliant']
+            reference = hz_audit_results['reference']
+            non_compliant_sequences = non_compliant_ds.get_sequence_ids()
+            # non_compliant_sequences = [f.split(ATTRIBUTE_SEPARATOR)[0] for f in non_compliant_sequences]
+            fully_compliant_sequences = fully_compliant_ds.get_sequence_ids()
+            # fully_compliant_sequences = [f.split(ATTRIBUTE_SEPARATOR)[0] for f in fully_compliant_sequences]
+            all_sequences = mrd.get_sequence_ids()
+
+            # Check if modalities are   equal
+            all_modalities_on_disk = [m for m in sub_names_by_modality.keys() if
+                                      not m.startswith('local')]
+            non_compliant_modality_on_disk = [m for m in dataset_info if
+                                              dataset_info[m] if
+                                              not m.startswith('local')]
+            compliant_modalities_on_disk = set(all_modalities_on_disk) - set(
+                non_compliant_modality_on_disk)
+
+            assert assert_list(all_modalities_on_disk, all_sequences)
+            assert assert_list(non_compliant_sequences,
+                               non_compliant_modality_on_disk)
+            assert assert_list(fully_compliant_sequences,
+                               compliant_modalities_on_disk)
+
+            for seq_id in mrd.get_sequence_ids():
+                all_subjects = mrd.get_subject_ids(seq_id)
+                non_compliant_subjects = non_compliant_ds.get_subject_ids(
+                    seq_id)
+                compliant_subjects = set(all_subjects) - set(
+                    non_compliant_subjects)
+                # On diskplu
+                all_subjects_on_disk = sub_names_by_modality[seq_id]
+                non_compliant_subjects_on_disk = dataset_info[seq_id]
+                compliant_subjects_on_disk = set(all_subjects_on_disk) - set(
+                    non_compliant_subjects_on_disk)
+
+                # What did you parse
+                assert assert_list(all_subjects, all_subjects_on_disk)
+                assert assert_list(non_compliant_subjects,
+                                   non_compliant_subjects_on_disk)
+                assert assert_list(compliant_subjects,
+                                   compliant_subjects_on_disk)
+
+                # Check if reference has the right values
+                assert reference[seq_id]['RepetitionTime'].get_value() == 200
+                assert reference[seq_id]['EchoTrainLength'].get_value() == 4000
+                assert reference[seq_id]['FlipAngle'].get_value() == 80
+
+                for subject, session, run, seq in non_compliant_ds.traverse_horizontal(
+                    seq_id):
+                    assert seq['RepetitionTime'].get_value() == repetition_time
+                    assert seq[
+                               'EchoTrainLength'].get_value() == echo_train_length
+                    assert seq['FlipAngle'].get_value() == flip_angle
+
+                for subject, session, run, seq in fully_compliant_ds.traverse_horizontal(
+                    seq_id):
+                    assert seq['RepetitionTime'].get_value() == 200
+                    assert seq['EchoTrainLength'].get_value() == 4000
+                    assert seq['FlipAngle'].get_value() == 80
+
+    # @settings(max_examples=30, deadline=None)
+    # @given(st.lists(st.integers(min_value=0, max_value=2), min_size=11,
+    #                 max_size=11),
+    #        st.floats(allow_nan=False, allow_infinity=False),
+    #        st.floats(allow_nan=False, allow_infinity=False),
+    #        st.floats(allow_nan=False, allow_infinity=False)
+    #        )
+    # def modify_test_non_compliance_bids(num_noncompliant_subjects,
+    #                                     repetition_time,
+    #                                     magnetic_field_strength,
+    #                                     flip_angle):
+    #     """pass non-compliant ds, and ensure library recognizes them as such"""
+    #     assume(repetition_time != const_bids['tr'])
+    #     assume(magnetic_field_strength != const_bids['b0'])
+    #     assume(flip_angle != const_bids['fa'])
+    #
+    #     fake_dir, dataset_info = make_bids_test_dataset(num_noncompliant_subjects,
+    #                                                     repetition_time,
+    #                                                     magnetic_field_strength,
+    #                                                     flip_angle)
+    #     mrd = import_dataset(fake_dir, include_phantom=True, ds_format='bids')
+    #     checked_dataset = check_compliance(dataset=mrd, output_dir=mrd.data_source)
+    #
+    #     # Check on disk, basically the truth
+    #     layout = BIDSLayout(fake_dir)
+    #     sub_names_by_modality = defaultdict(set)
+    #     subjects = layout.get_subjects()
+
+    # for modality in MRdataset.config.datatypes:
+    #     for sub in subjects:
+    #         filters = {'datatype': modality,
+    #                    'subject': sub,
+    #                    'extension': 'json'}
+    #         files = layout.get(**filters)
+    #         if files:
+    #             sub_names_by_modality[modality].add(sub)
+    #
+    # # Check if modalities are equal
+    # non_compliant_modality_names = [m for m in dataset_info if dataset_info[m]]
+    # assert assert_list(sub_names_by_modality.keys(),
+    #                    checked_dataset._children.keys())
+    #
+    # assert assert_list(checked_dataset.non_compliant_modality_names,
+    #                    non_compliant_modality_names)
+    #
+    # assert assert_list(checked_dataset.compliant_modality_names,
+    #                    set(checked_dataset._children.keys()) - set(
+    #                        non_compliant_modality_names))
+    #
+    # for modality in checked_dataset.modalities:
+    #     # GT
+    #     all_subjects = sub_names_by_modality[modality.name]
+    #     non_compliant_subjects = dataset_info[modality.name]
+    #     compliant_subjects = set(all_subjects) - set(non_compliant_subjects)
+    #
+    #     # What did you parse
+    #     assert assert_list(all_subjects, modality._children.keys())
+    #     assert assert_list(non_compliant_subjects,
+    #                        modality.non_compliant_subject_names)
+    #     assert assert_list(compliant_subjects, modality.compliant_subject_names)
+    #
+    #     # Check if reference has the right values
+    #     echo_times = modality.get_echo_times()
+    #     for te in echo_times:
+    #         reference = modality.get_reference(te)
+    #         assert reference['RepetitionTime'] == const_bids['tr']
+    #         assert reference['MagneticFieldStrength'] == const_bids['b0']
+    #         assert reference['FlipAngle'] == const_bids['fa']
+    #
+    #     for subject in modality.subjects:
+    #         for session in subject.sessions:
+    #             for run in session.runs:
+    #                 if run.delta:
+    #                     assert run.params['RepetitionTime'] == repetition_time
+    #                     assert run.params['MagneticFieldStrength'] == \
+    #                            magnetic_field_strength
+    #                     assert run.params['FlipAngle'] == flip_angle
+    #                 else:
+    #                     assert run.params['RepetitionTime'] == const_bids['tr']
+    #                     assert run.params['MagneticFieldStrength'] == \
+    #                            const_bids['b0']
+    #                     assert run.params['FlipAngle'] == const_bids['fa']
```

### Comparing `mrQA-0.2.4/mrQA/tests/unit_tests.py` & `mrQA-0.3/mrQA/tests/test_majority.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-from mrQA.utils import majority_attribute_values, files_modified_since
+import shutil
+from subprocess import CalledProcessError
+
+from protocol import UnspecifiedType
+
+from mrQA.config import EqualCountType, CannotComputeMajority
+from mrQA.tests.conftest import THIS_DIR
+from mrQA.utils import majority_values, folders_modified_since
 from mrQA.utils import list2txt, txt2list
 import unittest
 import tempfile
 from pathlib import Path
 from MRdataset.utils import random_name
 from datetime import datetime, timezone
 
@@ -17,44 +24,48 @@
             {'species': 'lion', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'puma', 'color': 'yellow', 'habitat': 'city'},
             {'species': 'cougar', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'lion', 'color': 'yellow', 'habitat': 'savanna'},
             {'species': 'panther', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'lion', 'color': 'brown', 'habitat': 'savanna'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
+        maj_attr_vals = majority_values(
+            animals,
+            include_params=['species', 'color', 'habitat'])
         self.assertEqual(maj_attr_vals['species'], 'lion')
         self.assertEqual(maj_attr_vals['habitat'], 'jungle')
         self.assertEqual(maj_attr_vals['color'], 'orange')
 
     def test_empty_list(self):
         animals = []
         with self.assertRaises(ValueError):
-            majority_attribute_values(animals)
+            majority_values(animals)
 
     def test_list_empty_dicts(self):
         animals = [{}, {}, {}, {}]
         with self.assertRaises(ValueError):
-            majority_attribute_values(animals)
+            majority_values(animals)
 
     def test_equal_count(self):
         animals = [
             {'species': 'lion', 'color': 'orange', 'habitat': 'savanna'},
             {'species': 'tiger', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'lion', 'color': 'yellow', 'habitat': 'jungle'},
             {'species': 'tiger', 'color': 'brown', 'habitat': 'savanna'},
             {'species': 'lion', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'tiger', 'color': 'yellow', 'habitat': 'city'},
             {'species': 'tiger', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'lion', 'color': 'yellow', 'habitat': 'savanna'},
             {'species': 'tiger', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'lion', 'color': 'brown', 'habitat': 'savanna'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
-        self.assertIsNone(maj_attr_vals['species'])
+        maj_attr_vals = majority_values(
+            animals,
+            include_params=['species', 'color', 'habitat'])
+        self.assertIsInstance(maj_attr_vals['species'], EqualCountType)
         self.assertEqual(maj_attr_vals['habitat'], 'jungle')
         self.assertEqual(maj_attr_vals['color'], 'orange')
 
     def test_single_key_equal_count(self):
         animals = [
             {'species': 'lion'},
             {'species': 'tiger'},
@@ -63,31 +74,34 @@
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'tiger'},
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'lion'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
-        self.assertIsNone(maj_attr_vals['species'])
+        maj_attr_vals = majority_values(
+            animals,
+            include_params=['species'])
+        self.assertIsInstance(maj_attr_vals['species'], EqualCountType)
 
     def test_single_key_majority(self):
         animals = [
             {'species': 'lion'},
             {'species': 'lion'},
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'tiger'},
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'lion'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
+        maj_attr_vals = majority_values(animals,
+                                        include_params=['species'])
         self.assertEqual(maj_attr_vals['species'], 'lion')
 
     def test_none_majority(self):
         animals = [
             {'species': None},
             {'species': None},
             {'species': None},
@@ -95,15 +109,17 @@
             {'species': None},
             {'species': 'tiger'},
             {'species': 'tiger'},
             {'species': None},
             {'species': 'tiger'},
             {'species': None},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
+        maj_attr_vals = majority_values(
+            animals,
+            include_params=['species'])
         self.assertEqual(maj_attr_vals['species'], 'tiger')
 
     def test_all_none(self):
         animals = [
             {'species': None},
             {'species': None},
             {'species': None},
@@ -111,68 +127,70 @@
             {'species': None},
             {'species': None},
             {'species': None},
             {'species': None},
             {'species': None},
             {'species': None},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
+        maj_attr_vals = majority_values(
+            animals,
+            include_params=['species'])
         self.assertIsNone(maj_attr_vals['species'])
 
     def test_many_values_for_majority(self):
         animals = [
             {'species': 'lion'},
             {'species': 'lion'},
             {'species': 'lion'},
             {'species': 'tiger'},
             {'species': 'tiger'},
             {'species': 'tiger'},
             {'species': 'cheetah'},
             {'species': 'cheetah'},
             {'species': 'cheetah'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
-        self.assertIsNone(maj_attr_vals['species'])
+        maj_attr_vals = majority_values(animals,
+                                        include_params=['species'])
+        self.assertIsInstance(maj_attr_vals['species'], EqualCountType)
 
     def test_length_less_than_3(self):
         animals = [
             {'species': 'lion', 'color': 'orange', 'habitat': 'savanna'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
-        self.assertIsNone(maj_attr_vals['species'])
-        self.assertIsNone(maj_attr_vals['habitat'])
-        self.assertIsNone(maj_attr_vals['color'])
+        with self.assertRaises(CannotComputeMajority):
+            maj_attr_vals = majority_values(
+                animals, include_params=['species', 'color', 'habitat'])
 
         animals = [
             {'species': 'lion', 'color': 'orange', 'habitat': 'savanna'},
             {'species': 'tiger', 'color': 'yellow', 'habitat': 'jungle'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
-        self.assertIsNone(maj_attr_vals['species'])
-        self.assertIsNone(maj_attr_vals['habitat'])
-        self.assertIsNone(maj_attr_vals['color'])
+        with self.assertRaises(CannotComputeMajority):
+            maj_attr_vals = majority_values(
+                animals, include_params=['species', 'color', 'habitat'])
 
     def test_none(self):
         with self.assertRaises(ValueError):
-            majority_attribute_values(None)
+            majority_values(None)
 
     def test_different_keys(self):
         animals = [
             {'species': 'lion', 'color': 'orange'},
             {'species': 'tiger', 'color': 'orange'},
             {'species': 'lion', 'color': 'yellow'},
             {'species': 'tiger', 'color': 'brown', 'habitat': 'savanna'},
             {'species': 'lion', 'color': 'orange', 'habitat': 'savanna'},
             {'species': 'tiger', 'color': 'yellow', 'habitat': 'city'},
             {'species': 'tiger', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'jaguar', 'color': 'yellow', 'habitat': 'savanna'},
             {'species': 'tiger', 'color': 'orange', 'habitat': 'jungle'},
             {'species': 'jaguar', 'color': 'brown', 'habitat': 'savanna'},
         ]
-        maj_attr_vals = majority_attribute_values(animals)
+        maj_attr_vals = majority_values(
+            animals, include_params=['species', 'color', 'habitat'])
         self.assertEqual(maj_attr_vals['species'], 'tiger')
         self.assertEqual(maj_attr_vals['habitat'], 'savanna')
         self.assertEqual(maj_attr_vals['color'], 'orange')
 
 
 class TestTxt2List(unittest.TestCase):
     def test_valid_file(self):
@@ -191,42 +209,42 @@
 class TestModifiedTimeDirectory(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         # super().__init__()
         cls.temp_ds = cls.create_dummy_directory()
 
     def test_invalid_path(self):
-        with self.assertRaises(FileNotFoundError):
-            now = datetime.now(timezone.utc)
-            files_modified_since('/tmp/mrqa', now.strftime("%m/%d/%Y %H:%M:%S"))
+        now = datetime.now(timezone.utc)
+        folders = folders_modified_since(
+            input_dir='/tmp/mrqa',
+            last_reported_on=now.strftime("%m/%d/%Y %H:%M:%S"),
+            output_dir='/tmp/',
+            time_format='datetime'
+        )
+        self.assertEqual(len(folders), 0)
 
     @staticmethod
     def create_dummy_directory():
         temp_dir = Path(tempfile.gettempdir())
         temp_folder_name = temp_dir / random_name()
         temp_folder_name.mkdir(parents=True, exist_ok=True)
 
         num_folder = 10
         num_files = 5
         for i in range(num_folder):
             temp_subdir_path = temp_folder_name / random_name()
             temp_subdir_path.mkdir(parents=True, exist_ok=True)
             for j in range(num_files):
-                tmp = tempfile.NamedTemporaryFile(delete=False,
-                                                  dir=temp_subdir_path)
+                # copy a file from somewhere
+                temp_file_path = temp_subdir_path / random_name()
+                shutil.copy(Path(THIS_DIR / 'resources/valid.dcm'), temp_file_path)
         return temp_folder_name
 
     def test_basic(self):
         now = datetime(2023, 2, 5, 18, 00)
         # datetime.now(timezone.utc)
         date_time = now.strftime("%m/%d/%Y %H:%M:%S")
-        valid_files = files_modified_since(self.temp_ds, date_time, '/tmp/',
-                                           time_format='datetime')
-        print(valid_files)
-
-
-if __name__ == '__main__':
-    a = TestModifiedTimeDirectory()
-    # a.check_basic()
-
-
-
+        valid_files = folders_modified_since(input_dir=str(self.temp_ds),
+                                             last_reported_on=date_time,
+                                             output_dir='/tmp/',
+                                             time_format='datetime')
+        self.assertEqual(len(valid_files), 10)
```

