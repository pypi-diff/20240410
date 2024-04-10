# Comparing `tmp/h5py-3.8.0.tar.gz` & `tmp/h5py-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5py-3.8.0.tar", last modified: Mon Jan 23 10:21:36 2023, max compression
+gzip compressed data, was "h5py-3.9.0.tar", last modified: Tue Jun 20 09:06:12 2023, max compression
```

## Comparing `h5py-3.8.0.tar` & `h5py-3.9.0.tar`

### file list

```diff
@@ -1,249 +1,250 @@
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.019553 h5py-3.8.0/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      407 2022-12-21 16:13:47.000000 h5py-3.8.0/.gitignore
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1520 2021-05-09 11:55:36.000000 h5py-3.8.0/LICENSE
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1037 2022-12-21 16:13:47.000000 h5py-3.8.0/MANIFEST.in
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-01-23 10:21:36.018553 h5py-3.8.0/PKG-INFO
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2023-01-20 16:24:30.000000 h5py-3.8.0/README.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10725 2022-12-21 16:13:47.000000 h5py-3.8.0/api_gen.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6858 2021-05-09 11:55:36.000000 h5py-3.8.0/asv.conf.json
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.956553 h5py-3.8.0/benchmarks/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7089 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/benchmark_slicing.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1669 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/benchmarks.py
--rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)      375 2022-12-21 16:13:47.000000 h5py-3.8.0/dev-install.sh
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.963553 h5py-3.8.0/docs/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6835 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/Makefile
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9459 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/build.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8513 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/conf.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1224 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/config.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16467 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/contributing.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10212 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/faq.rst
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.965553 h5py-3.8.0/docs/high/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3972 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/high/attr.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    24278 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/dataset.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3729 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/high/dims.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23568 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/file.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20381 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/group.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1363 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/high/lowlevel.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1382 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/index.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11708 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/licenses.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5131 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/mpi.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5733 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/quick.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3985 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/refs.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4424 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/related_projects.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1201 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/release_guide.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       71 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/requirements-rtd.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7866 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/special.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6041 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/strings.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6987 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/swmr.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5811 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/vds.rst
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.970553 h5py-3.8.0/docs/whatsnew/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7122 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.0.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1832 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.1.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5438 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.10.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2625 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.2.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2608 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.3.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1436 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.4.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2460 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.5.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2591 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.6.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1753 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.7.1.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4493 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.7.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3916 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.8.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1843 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.9.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10020 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.0.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      750 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.1.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2043 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.2.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1928 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.3.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.4.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2040 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.5.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1060 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.6.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.7.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3016 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/whatsnew/3.8.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      341 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/whatsnew/index.rst
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.974553 h5py-3.8.0/docs_api/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6814 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/Makefile
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.974553 h5py-3.8.0/docs_api/_static/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/_static/.keep
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7563 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/automod.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8479 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/conf.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      428 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5a.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      114 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5ac.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      867 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5d.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5ds.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1298 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5f.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1204 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5fd.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      621 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5g.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      351 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5i.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      222 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5l.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      918 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5o.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1777 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5p.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5pl.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      521 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5r.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      933 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5s.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3796 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5t.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1099 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5z.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      663 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/index.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       96 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/objects.rst
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.977553 h5py-3.8.0/examples/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      380 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/bytesio.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1831 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/collective_io.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/dataset_concatenation.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      903 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/dual_pco_edge.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      971 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/eiger_use_case.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1308 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/excalibur_detector_modules.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1344 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/multiblockslice_interleave.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3539 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/multiprocessing_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1107 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/percival_use_case.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1339 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/store_and_retrieve_units_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/store_datetimes.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2673 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/swmr_inotify_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3865 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/swmr_multiprocess.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10795 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/threading_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1175 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/vds_simple.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1260 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/write-direct-compressed.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.995553 h5py-3.8.0/h5py/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3740 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_conv.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    35396 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_conv.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20382 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_errors.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7528 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_errors.pyx
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.999553 h5py-3.8.0/h5py/_hl/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      457 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_hl/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10694 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/attrs.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15669 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1375 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/compat.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    42162 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/dataset.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/datatype.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5407 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/dims.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23981 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/files.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13857 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/filters.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    27646 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/group.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    14478 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/selections.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/selections2.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9353 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/vds.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4571 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_locks.pxi
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      760 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_objects.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10107 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_objects.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      538 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_proxy.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10834 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_proxy.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16418 2023-01-20 16:24:30.000000 h5py-3.8.0/h5py/_selector.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/api_compat.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    34257 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/api_functions.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/api_types_ext.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    33446 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/api_types_hdf5.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      688 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6842 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      388 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5a.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12817 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5a.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      383 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ac.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5961 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ac.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      406 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5d.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    24596 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/h5d.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ds.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4802 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5ds.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      413 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5f.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18888 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5f.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      448 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5fd.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8378 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/h5fd.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      412 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5g.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15721 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5g.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      394 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5i.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4053 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5i.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      358 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5l.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10000 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5l.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5o.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10381 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5o.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2072 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5p.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    58333 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/h5p.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      667 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5pl.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2354 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5pl.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      523 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5py_warnings.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      822 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5r.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5946 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5r.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      389 2023-01-05 09:43:23.000000 h5py-3.8.0/h5py/h5s.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18189 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5s.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1460 2023-01-05 09:43:23.000000 h5py-3.8.0/h5py/h5t.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57174 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/h5t.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5z.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2970 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5z.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3642 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/ipy_completer.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.011553 h5py-3.8.0/h5py/tests/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      668 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6845 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/common.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      547 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/conftest.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.012553 h5py-3.8.0/h5py/tests/data_files/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      193 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6304 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_dset.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   169904 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_dset_utc.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9008 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_s390x.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2865 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_attribute_create.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9577 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_attrs.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7646 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_attrs_data.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3816 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1445 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_big_endian_file.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1473 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_completions.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    73292 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/tests/test_dataset.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18885 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_dataset_getitem.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5825 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_dataset_swmr.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1007 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_datatype.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8307 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_dimension_scales.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      601 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_dims_dimensionproxy.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17927 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_dtype.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2247 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_errors.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    32636 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_file.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10340 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_file2.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4404 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_file_alignment.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1524 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_file_image.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3302 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_filters.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    36053 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_group.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1216 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5358 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5d_direct_chunk.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4018 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5f.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      508 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5o.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7265 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5p.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1999 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5pl.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6582 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5t.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      911 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_objects.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1503 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_ros3.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4852 2023-01-20 16:24:30.000000 h5py-3.8.0/h5py/tests/test_selections.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13874 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_slicing.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.014553 h5py-3.8.0/h5py/tests/test_vds/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      103 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_vds/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17262 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_vds/test_highlevel_vds.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12319 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_vds/test_lowlevel_vds.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5932 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_vds/test_virtual_source.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      870 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/utils.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5396 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/utils.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1910 2023-01-23 10:18:46.000000 h5py-3.8.0/h5py/version.py
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.995553 h5py-3.8.0/h5py.egg-info/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4782 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/SOURCES.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/dependency_links.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       14 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/requires.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        5 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/top_level.txt
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.015553 h5py-3.8.0/licenses/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3766 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/hdf5.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1739 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/license.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1640 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/pytables.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2503 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/python.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1394 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/stdint.txt
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.016553 h5py-3.8.0/lzf/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1556 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/LICENSE.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3330 2022-12-21 16:13:47.000000 h5py-3.8.0/lzf/README.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2729 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/example.c
-drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.018553 h5py-3.8.0/lzf/lzf/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4406 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5445 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzfP.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9002 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf_c.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4415 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf_d.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7239 2022-12-21 16:13:47.000000 h5py-3.8.0/lzf/lzf_filter.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      861 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf_filter.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11803 2021-05-09 11:55:36.000000 h5py-3.8.0/pylintrc
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2831 2023-01-20 16:24:30.000000 h5py-3.8.0/pyproject.toml
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      171 2023-01-04 17:26:33.000000 h5py-3.8.0/pytest.ini
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       38 2023-01-23 10:21:36.019553 h5py-3.8.0/setup.cfg
--rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)     2699 2023-01-23 10:18:46.000000 h5py-3.8.0/setup.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6357 2023-01-04 17:26:33.000000 h5py-3.8.0/setup_build.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11595 2023-01-04 17:26:33.000000 h5py-3.8.0/setup_configure.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2807 2023-01-20 16:24:30.000000 h5py-3.8.0/tox.ini
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.781311 h5py-3.9.0/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1520 2021-05-09 11:55:36.000000 h5py-3.9.0/LICENSE
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1037 2022-12-21 16:13:47.000000 h5py-3.9.0/MANIFEST.in
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-06-20 09:06:12.781311 h5py-3.9.0/PKG-INFO
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2023-06-07 11:39:16.000000 h5py-3.9.0/README.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10725 2022-12-21 16:13:47.000000 h5py-3.9.0/api_gen.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6858 2021-05-09 11:55:36.000000 h5py-3.9.0/asv.conf.json
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.707311 h5py-3.9.0/benchmarks/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.9.0/benchmarks/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7089 2021-05-09 11:55:36.000000 h5py-3.9.0/benchmarks/benchmark_slicing.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1669 2021-05-09 11:55:36.000000 h5py-3.9.0/benchmarks/benchmarks.py
+-rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)      375 2022-12-21 16:13:47.000000 h5py-3.9.0/dev-install.sh
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.718310 h5py-3.9.0/docs/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6835 2023-01-04 17:26:33.000000 h5py-3.9.0/docs/Makefile
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9459 2023-01-04 17:26:33.000000 h5py-3.9.0/docs/build.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8513 2023-06-20 08:56:46.000000 h5py-3.9.0/docs/conf.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1224 2023-01-20 16:24:30.000000 h5py-3.9.0/docs/config.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16467 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/contributing.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10212 2023-01-20 16:24:30.000000 h5py-3.9.0/docs/faq.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.721310 h5py-3.9.0/docs/high/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3972 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/high/attr.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    24125 2023-04-26 15:08:31.000000 h5py-3.9.0/docs/high/dataset.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3729 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/high/dims.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23958 2023-02-17 10:43:33.000000 h5py-3.9.0/docs/high/file.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20381 2023-01-04 17:26:33.000000 h5py-3.9.0/docs/high/group.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1363 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/high/lowlevel.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1382 2023-01-20 16:24:30.000000 h5py-3.9.0/docs/index.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11708 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/licenses.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5131 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/mpi.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5733 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/quick.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3985 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/refs.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4424 2023-01-20 16:24:30.000000 h5py-3.9.0/docs/related_projects.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1201 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/release_guide.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       71 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/requirements-rtd.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7866 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/special.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6041 2023-01-04 17:26:33.000000 h5py-3.9.0/docs/strings.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6987 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/swmr.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5811 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/vds.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.727311 h5py-3.9.0/docs/whatsnew/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7122 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.0.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1832 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5438 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.10.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2625 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.2.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2608 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.3.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1436 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.4.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2460 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/2.5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2591 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/2.6.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1753 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.7.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4493 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/2.7.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3916 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.8.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1843 2021-05-09 11:55:36.000000 h5py-3.9.0/docs/whatsnew/2.9.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10020 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.0.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      750 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2043 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.2.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1928 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.3.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.4.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2040 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1060 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.6.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.9.0/docs/whatsnew/3.7.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3016 2023-01-23 10:18:46.000000 h5py-3.9.0/docs/whatsnew/3.8.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2331 2023-06-20 08:56:46.000000 h5py-3.9.0/docs/whatsnew/3.9.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      349 2023-06-20 08:56:46.000000 h5py-3.9.0/docs/whatsnew/index.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.732311 h5py-3.9.0/docs_api/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6814 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/Makefile
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.732311 h5py-3.9.0/docs_api/_static/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/_static/.keep
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7563 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/automod.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8479 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/conf.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      428 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5a.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      114 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5ac.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      867 2022-12-21 16:13:47.000000 h5py-3.9.0/docs_api/h5d.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2022-12-21 16:13:47.000000 h5py-3.9.0/docs_api/h5ds.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1298 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5f.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1204 2022-12-21 16:13:47.000000 h5py-3.9.0/docs_api/h5fd.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      621 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5g.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      351 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5i.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      222 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5l.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      918 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5o.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1777 2022-12-21 16:13:47.000000 h5py-3.9.0/docs_api/h5p.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5pl.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      521 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5r.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      933 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5s.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3796 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5t.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1099 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/h5z.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      663 2022-12-21 16:13:47.000000 h5py-3.9.0/docs_api/index.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       96 2021-05-09 11:55:36.000000 h5py-3.9.0/docs_api/objects.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.736311 h5py-3.9.0/examples/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      380 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/bytesio.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1831 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/collective_io.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/dataset_concatenation.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      903 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/dual_pco_edge.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      971 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/eiger_use_case.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1308 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/excalibur_detector_modules.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1344 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/multiblockslice_interleave.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3539 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/multiprocessing_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1107 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/percival_use_case.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1339 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/store_and_retrieve_units_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/store_datetimes.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2673 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/swmr_inotify_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3865 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/swmr_multiprocess.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10795 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/threading_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1175 2021-05-09 11:55:36.000000 h5py-3.9.0/examples/vds_simple.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1260 2022-12-21 16:13:47.000000 h5py-3.9.0/examples/write-direct-compressed.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.754311 h5py-3.9.0/h5py/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3740 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/_conv.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    35396 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_conv.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20382 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_errors.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7537 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/_errors.pyx
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.759311 h5py-3.9.0/h5py/_hl/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      457 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/_hl/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10221 2023-06-16 10:09:33.000000 h5py-3.9.0/h5py/_hl/attrs.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15788 2023-06-07 11:39:16.000000 h5py-3.9.0/h5py/_hl/base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1375 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/_hl/compat.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    41549 2023-06-16 10:09:33.000000 h5py-3.9.0/h5py/_hl/dataset.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/_hl/datatype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5407 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_hl/dims.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23981 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_hl/files.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13874 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/_hl/filters.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    27882 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/_hl/group.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    14475 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/_hl/selections.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/_hl/selections2.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9353 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/_hl/vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4571 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/_locks.pxi
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      760 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/_objects.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10107 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/_objects.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      538 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_proxy.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10834 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/_proxy.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16418 2023-01-20 16:24:30.000000 h5py-3.9.0/h5py/_selector.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/api_compat.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    34439 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/api_functions.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/api_types_ext.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    33469 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/api_types_hdf5.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      688 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6842 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      388 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5a.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12817 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5a.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      383 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5ac.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5961 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5ac.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      406 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5d.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    25454 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/h5d.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5ds.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4802 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5ds.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      413 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5f.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18888 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5f.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      448 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5fd.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8378 2023-01-10 17:06:37.000000 h5py-3.9.0/h5py/h5fd.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      412 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5g.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15721 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5g.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      394 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5i.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4053 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5i.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      358 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5l.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10000 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5l.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5o.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10381 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5o.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2072 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5p.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    58878 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/h5p.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      667 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5pl.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2354 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5pl.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      523 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/h5py_warnings.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      822 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5r.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5946 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5r.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      389 2023-01-05 09:43:23.000000 h5py-3.9.0/h5py/h5s.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18189 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5s.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1460 2023-01-05 09:43:23.000000 h5py-3.9.0/h5py/h5t.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57174 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/h5t.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/h5z.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3664 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/h5z.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3733 2023-05-16 16:24:09.000000 h5py-3.9.0/h5py/ipy_completer.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.771311 h5py-3.9.0/h5py/tests/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      668 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6845 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/common.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      547 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/conftest.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.773311 h5py-3.9.0/h5py/tests/data_files/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      193 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/data_files/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6304 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/data_files/vlen_string_dset.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)   169904 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/data_files/vlen_string_dset_utc.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9008 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/data_files/vlen_string_s390x.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2990 2023-06-07 11:39:16.000000 h5py-3.9.0/h5py/tests/test_attribute_create.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9577 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_attrs.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7646 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_attrs_data.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3816 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1445 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_big_endian_file.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1473 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_completions.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    73123 2023-06-07 11:39:16.000000 h5py-3.9.0/h5py/tests/test_dataset.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18885 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_dataset_getitem.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5825 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_dataset_swmr.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1007 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_datatype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8307 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_dimension_scales.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      601 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_dims_dimensionproxy.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17927 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_dtype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2247 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_errors.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    32636 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_file.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10340 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_file2.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4404 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_file_alignment.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1524 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_file_image.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3067 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/tests/test_filters.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    36207 2023-06-07 11:39:16.000000 h5py-3.9.0/h5py/tests/test_group.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1216 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_h5.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8233 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/tests/test_h5d_direct_chunk.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4018 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_h5f.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      508 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_h5o.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7265 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_h5p.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1999 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_h5pl.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6582 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_h5t.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1919 2023-04-26 15:08:31.000000 h5py-3.9.0/h5py/tests/test_h5z.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      911 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_objects.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1503 2023-01-04 17:26:33.000000 h5py-3.9.0/h5py/tests/test_ros3.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4852 2023-01-20 16:24:30.000000 h5py-3.9.0/h5py/tests/test_selections.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13874 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_slicing.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.775311 h5py-3.9.0/h5py/tests/test_vds/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      103 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_vds/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17262 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_vds/test_highlevel_vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12319 2022-12-21 16:13:47.000000 h5py-3.9.0/h5py/tests/test_vds/test_lowlevel_vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5932 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/tests/test_vds/test_virtual_source.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      870 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/utils.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5396 2021-05-09 11:55:36.000000 h5py-3.9.0/h5py/utils.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1910 2023-06-20 08:56:46.000000 h5py-3.9.0/h5py/version.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.755311 h5py-3.9.0/h5py.egg-info/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-06-20 09:06:12.000000 h5py-3.9.0/h5py.egg-info/PKG-INFO
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4816 2023-06-20 09:06:12.000000 h5py-3.9.0/h5py.egg-info/SOURCES.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        1 2023-06-20 09:06:12.000000 h5py-3.9.0/h5py.egg-info/dependency_links.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       14 2023-06-20 09:06:12.000000 h5py-3.9.0/h5py.egg-info/requires.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        5 2023-06-20 09:06:12.000000 h5py-3.9.0/h5py.egg-info/top_level.txt
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.777311 h5py-3.9.0/licenses/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3766 2021-05-09 11:55:36.000000 h5py-3.9.0/licenses/hdf5.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1739 2021-05-09 11:55:36.000000 h5py-3.9.0/licenses/license.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1640 2021-05-09 11:55:36.000000 h5py-3.9.0/licenses/pytables.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2503 2021-05-09 11:55:36.000000 h5py-3.9.0/licenses/python.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1394 2021-05-09 11:55:36.000000 h5py-3.9.0/licenses/stdint.txt
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.779311 h5py-3.9.0/lzf/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1556 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/LICENSE.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3330 2022-12-21 16:13:47.000000 h5py-3.9.0/lzf/README.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2729 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/example.c
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-06-20 09:06:12.780311 h5py-3.9.0/lzf/lzf/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4406 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/lzf/lzf.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5445 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/lzf/lzfP.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9002 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/lzf/lzf_c.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4415 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/lzf/lzf_d.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7239 2022-12-21 16:13:47.000000 h5py-3.9.0/lzf/lzf_filter.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      861 2021-05-09 11:55:36.000000 h5py-3.9.0/lzf/lzf_filter.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11803 2021-05-09 11:55:36.000000 h5py-3.9.0/pylintrc
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2837 2023-06-07 11:39:16.000000 h5py-3.9.0/pyproject.toml
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      171 2023-01-04 17:26:33.000000 h5py-3.9.0/pytest.ini
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       38 2023-06-20 09:06:12.781311 h5py-3.9.0/setup.cfg
+-rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)     2655 2023-06-20 08:56:46.000000 h5py-3.9.0/setup.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6357 2023-01-04 17:26:33.000000 h5py-3.9.0/setup_build.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11647 2023-06-07 11:39:16.000000 h5py-3.9.0/setup_configure.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2773 2023-06-07 11:39:16.000000 h5py-3.9.0/tox.ini
```

### Comparing `h5py-3.8.0/LICENSE` & `h5py-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/MANIFEST.in` & `h5py-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/PKG-INFO` & `h5py-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5py
-Version: 3.8.0
+Version: 3.9.0
 Summary: Read and write HDF5 files from Python
 Author-email: Andrew Collette <andrew.collette@gmail.com>
 Maintainer-email: Thomas Kluyver <thomas@kluyver.me.uk>, Thomas A Caswell <tcaswell@bnl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://www.h5py.org/
 Project-URL: Source, https://github.com/h5py/h5py
 Project-URL: Documentation, https://docs.h5py.org/en/stable/
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 The h5py package provides both a high- and low-level interface to the HDF5
 library from Python. The low-level interface is intended to be a complete
 wrapping of the HDF5 API, while the high-level component supports  access to
 HDF5 files, datasets and groups using established Python and NumPy concepts.
```

### Comparing `h5py-3.8.0/README.rst` & `h5py-3.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * Main website: https://www.h5py.org
 * Source code: https://github.com/h5py/h5py
 * Discussion forum: https://forum.hdfgroup.org/c/hdf-tools/h5py
 
 Installation
 ------------
 
-Pre-build `h5py` can either be installed via your Python Distribution (e.g.
+Pre-built `h5py` can either be installed via your Python Distribution (e.g.
 `Continuum Anaconda`_, `Enthought Canopy`_) or from `PyPI`_ via `pip`_.
 `h5py` is also distributed in many Linux Distributions (e.g. Ubuntu, Fedora),
 and in the macOS package managers `Homebrew <https://brew.sh/>`_,
 `Macports <https://www.macports.org/>`_, or `Fink <http://finkproject.org/>`_.
 
 More detailed installation instructions, including how to install `h5py` with
 MPI support, can be found at: https://docs.h5py.org/en/latest/build.html.
```

### Comparing `h5py-3.8.0/api_gen.py` & `h5py-3.9.0/api_gen.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/asv.conf.json` & `h5py-3.9.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/benchmarks/benchmark_slicing.py` & `h5py-3.9.0/benchmarks/benchmark_slicing.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/benchmarks/benchmarks.py` & `h5py-3.9.0/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/Makefile` & `h5py-3.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/build.rst` & `h5py-3.9.0/docs/build.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/conf.py` & `h5py-3.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 copyright = '2014, Andrew Collette and contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '3.8.0'
+release = '3.9.0'
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `h5py-3.8.0/docs/config.rst` & `h5py-3.9.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/contributing.rst` & `h5py-3.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/faq.rst` & `h5py-3.9.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/high/attr.rst` & `h5py-3.9.0/docs/high/attr.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/high/dataset.rst` & `h5py-3.9.0/docs/high/dataset.rst`

 * *Files 1% similar despite different names*

```diff
@@ -499,20 +499,16 @@
         type.  Conversion is handled by HDF5 directly, on the fly::
 
             >>> dset = f.create_dataset("bigint", (1000,), dtype='int64')
             >>> out = dset.astype('int16')[:]
             >>> out.dtype
             dtype('int16')
 
-        .. versionchanged:: 3.0
-           Allowed reading through the wrapper object. In earlier versions,
-           :meth:`astype` had to be used as a context manager:
-
-               >>> with dset.astype('int16'):
-               ...     out = dset[:]
+        .. versionchanged:: 3.9
+           :meth:`astype` can no longer be used as a context manager.
 
     .. method:: asstr(encoding=None, errors='strict')
 
        Only for string datasets. Returns a wrapper to read data as Python
        string objects::
 
            >>> s = dataset.asstr()[0]
```

### Comparing `h5py-3.8.0/docs/high/dims.rst` & `h5py-3.9.0/docs/high/dims.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/high/file.rst` & `h5py-3.9.0/docs/high/file.rst`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,21 @@
 
         secret_key:
           AWS secret access key. Default is ``b''``.
 
         The argument values must be ``bytes`` objects. All three arguments are
         required to activate AWS authentication.
 
+        .. note::
+           Pre-built h5py packages on PyPI do not include this S3 support. If
+           you want this feature, you could use packages from conda-forge, or
+           :ref:`build h5py from source <source_install>` against an HDF5 build
+           with S3 support. Alternatively, use the :ref:`file-like object
+           <file_fileobj>` support with a package like s3fs.
+
 
 .. _file_fileobj:
 
 Python file-like objects
 ------------------------
 
 .. versionadded:: 2.9
```

### Comparing `h5py-3.8.0/docs/high/group.rst` & `h5py-3.9.0/docs/high/group.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/high/lowlevel.rst` & `h5py-3.9.0/docs/high/lowlevel.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/index.rst` & `h5py-3.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/licenses.rst` & `h5py-3.9.0/docs/licenses.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/mpi.rst` & `h5py-3.9.0/docs/mpi.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/quick.rst` & `h5py-3.9.0/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/refs.rst` & `h5py-3.9.0/docs/refs.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/related_projects.rst` & `h5py-3.9.0/docs/related_projects.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/release_guide.rst` & `h5py-3.9.0/docs/release_guide.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/special.rst` & `h5py-3.9.0/docs/special.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/strings.rst` & `h5py-3.9.0/docs/strings.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/swmr.rst` & `h5py-3.9.0/docs/swmr.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/vds.rst` & `h5py-3.9.0/docs/vds.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.0.rst` & `h5py-3.9.0/docs/whatsnew/2.0.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.1.rst` & `h5py-3.9.0/docs/whatsnew/2.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.10.rst` & `h5py-3.9.0/docs/whatsnew/2.10.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.2.rst` & `h5py-3.9.0/docs/whatsnew/2.2.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.3.rst` & `h5py-3.9.0/docs/whatsnew/2.3.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.4.rst` & `h5py-3.9.0/docs/whatsnew/2.4.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.5.rst` & `h5py-3.9.0/docs/whatsnew/2.5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.6.rst` & `h5py-3.9.0/docs/whatsnew/2.6.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.7.1.rst` & `h5py-3.9.0/docs/whatsnew/2.7.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.7.rst` & `h5py-3.9.0/docs/whatsnew/2.7.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.8.rst` & `h5py-3.9.0/docs/whatsnew/2.8.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/2.9.rst` & `h5py-3.9.0/docs/whatsnew/2.9.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.0.rst` & `h5py-3.9.0/docs/whatsnew/3.0.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.1.rst` & `h5py-3.9.0/docs/whatsnew/3.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.2.rst` & `h5py-3.9.0/docs/whatsnew/3.2.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.3.rst` & `h5py-3.9.0/docs/whatsnew/3.3.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.4.rst` & `h5py-3.9.0/docs/whatsnew/3.4.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.5.rst` & `h5py-3.9.0/docs/whatsnew/3.5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.6.rst` & `h5py-3.9.0/docs/whatsnew/3.6.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.7.rst` & `h5py-3.9.0/docs/whatsnew/3.7.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs/whatsnew/3.8.rst` & `h5py-3.9.0/docs/whatsnew/3.8.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/Makefile` & `h5py-3.9.0/docs_api/Makefile`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/automod.py` & `h5py-3.9.0/docs_api/automod.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/conf.py` & `h5py-3.9.0/docs_api/conf.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5.rst` & `h5py-3.9.0/docs_api/h5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5d.rst` & `h5py-3.9.0/docs_api/h5d.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5f.rst` & `h5py-3.9.0/docs_api/h5f.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5fd.rst` & `h5py-3.9.0/docs_api/h5fd.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5g.rst` & `h5py-3.9.0/docs_api/h5g.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5o.rst` & `h5py-3.9.0/docs_api/h5o.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5p.rst` & `h5py-3.9.0/docs_api/h5p.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5r.rst` & `h5py-3.9.0/docs_api/h5r.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5s.rst` & `h5py-3.9.0/docs_api/h5s.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5t.rst` & `h5py-3.9.0/docs_api/h5t.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/h5z.rst` & `h5py-3.9.0/docs_api/h5z.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/docs_api/index.rst` & `h5py-3.9.0/docs_api/index.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/collective_io.py` & `h5py-3.9.0/examples/collective_io.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/dataset_concatenation.py` & `h5py-3.9.0/examples/dataset_concatenation.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/dual_pco_edge.py` & `h5py-3.9.0/examples/dual_pco_edge.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/eiger_use_case.py` & `h5py-3.9.0/examples/eiger_use_case.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/excalibur_detector_modules.py` & `h5py-3.9.0/examples/excalibur_detector_modules.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/multiblockslice_interleave.py` & `h5py-3.9.0/examples/multiblockslice_interleave.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/multiprocessing_example.py` & `h5py-3.9.0/examples/multiprocessing_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/percival_use_case.py` & `h5py-3.9.0/examples/percival_use_case.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/store_and_retrieve_units_example.py` & `h5py-3.9.0/examples/store_and_retrieve_units_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/swmr_inotify_example.py` & `h5py-3.9.0/examples/swmr_inotify_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/swmr_multiprocess.py` & `h5py-3.9.0/examples/swmr_multiprocess.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/threading_example.py` & `h5py-3.9.0/examples/threading_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/vds_simple.py` & `h5py-3.9.0/examples/vds_simple.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/examples/write-direct-compressed.py` & `h5py-3.9.0/examples/write-direct-compressed.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/__init__.py` & `h5py-3.9.0/h5py/__init__.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_conv.pyx` & `h5py-3.9.0/h5py/_conv.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_errors.pxd` & `h5py-3.9.0/h5py/_errors.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_errors.pyx` & `h5py-3.9.0/h5py/_errors.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     _minor_table[H5E_BADID] = ValueError  # Unable to find ID information
     _exact_table[(H5E_SYM, H5E_CANTCREATE)] = ValueError  # Object already exists
 
 cdef struct err_data_t:
     H5E_error_t err
     int n
 
-cdef herr_t walk_cb(unsigned int n, const H5E_error_t *desc, void *e) nogil:
+cdef herr_t walk_cb(unsigned int n, const H5E_error_t *desc, void *e) nogil noexcept:
 
     cdef err_data_t *ee = <err_data_t*>e
 
     ee[0].err.maj_num = desc[0].maj_num
     ee[0].err.min_num = desc[0].min_num
     ee[0].err.desc = desc[0].desc
     ee[0].n = n
```

### Comparing `h5py-3.8.0/h5py/_hl/attrs.py` & `h5py-3.9.0/h5py/_hl/attrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         shape
             Shape of the attribute.  Overrides data.shape if both are
             given, in which case the total number of points must be unchanged.
         dtype
             Data type of the attribute.  Overrides data.dtype if both
             are given.
         """
+        name = self._e(name)
 
         with phil:
             # First, make sure we have a NumPy array.  We leave the data type
             # conversion for HDF5 to perform.
             if not isinstance(data, Empty):
                 data = base.array_for_new_object(data, specified_dtype=dtype)
 
@@ -162,15 +163,15 @@
                 shape = shape[0:len(shape)-len(subshape)]
                 dtype = subdtype
 
             # Not an array type; make sure to check the number of elements
             # is compatible, and reshape if needed.
             else:
 
-                if shape is not None and numpy.product(shape, dtype=numpy.ulonglong) != numpy.product(data.shape, dtype=numpy.ulonglong):
+                if shape is not None and product(shape) != product(data.shape):
                     raise ValueError("Shape of new attribute conflicts with shape of data")
 
                 if shape != data.shape:
                     data = data.reshape(shape)
 
             # We need this to handle special string types.
             if not isinstance(data, Empty):
@@ -185,43 +186,32 @@
                 htype2 = None
 
             if isinstance(data, Empty):
                 space = h5s.create(h5s.NULL)
             else:
                 space = h5s.create_simple(shape)
 
-            # This mess exists because you can't overwrite attributes in HDF5.
-            # So we write to a temporary attribute first, and then rename.
-            # see issue 1385
-            # if track_order is enabled new attributes (which exceed the
-            # max_compact range, 8 is default) cannot be created as temporary
-            # attributes with subsequent rename, doing that would trigger
-            # the error discussed in the above issue
-            attr_exists = False
-            if h5a.exists(self._id, self._e(name)):
-                attr_exists = True
-                tempname = uuid.uuid4().hex
-            else:
-                tempname = name
+            # For a long time, h5py would create attributes with a random name
+            # and then rename them, imitating how you can atomically replace
+            # a file in a filesystem. But HDF5 does not offer atomic replacement
+            # (you have to delete the existing attribute first), and renaming
+            # exposes some bugs - see https://github.com/h5py/h5py/issues/1385
+            # So we've gone back to the simpler delete & recreate model.
+            if h5a.exists(self._id, name):
+                h5a.delete(self._id, name)
 
-            attr = h5a.create(self._id, self._e(tempname), htype, space)
+            attr = h5a.create(self._id, name, htype, space)
             try:
                 if not isinstance(data, Empty):
                     attr.write(data, mtype=htype2)
-                if attr_exists:
-                    # Rename temp attribute to proper name
-                    # No atomic rename in HDF5 :(
-                    h5a.delete(self._id, self._e(name))
-                    h5a.rename(self._id, self._e(tempname), self._e(name))
             except:
                 attr.close()
-                h5a.delete(self._id, self._e(tempname))
+                h5a.delete(self._id, name)
                 raise
-            finally:
-                attr.close()
+            attr.close()
 
     def modify(self, name, value):
         """ Change the value of an attribute while preserving its type.
 
         Differs from __setitem__ in that if the attribute already exists, its
         type is preserved.  This can be very useful for interacting with
         externally generated files.
```

### Comparing `h5py-3.8.0/h5py/_hl/base.py` & `h5py-3.9.0/h5py/_hl/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,21 +191,23 @@
             return lcpl
 
         if name is None:
             return (None, None) if lcpl else None
 
         if isinstance(name, bytes):
             coding = h5t.CSET_ASCII
-        else:
+        elif isinstance(name, str):
             try:
                 name = name.encode('ascii')
                 coding = h5t.CSET_ASCII
             except UnicodeEncodeError:
                 name = name.encode('utf8')
                 coding = h5t.CSET_UTF8
+        else:
+            raise TypeError(f"A name should be string or bytes, not {type(name)}")
 
         if lcpl:
             return name, get_lcpl(coding)
         return name
 
     def _d(self, name):
         """ Decode a name according to the current file settings.
```

### Comparing `h5py-3.8.0/h5py/_hl/compat.py` & `h5py-3.9.0/h5py/_hl/compat.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_hl/dataset.py` & `h5py-3.9.0/h5py/_hl/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 
 """
     Implements support for high-level dataset access.
 """
 
 import posixpath as pp
 import sys
-from warnings import warn
-
-from threading import local
 
 import numpy
 
 from .. import h5, h5s, h5t, h5r, h5d, h5p, h5fd, h5ds, _selector
-from ..h5py_warnings import H5pyDeprecationWarning
-from .base import HLObject, phil, with_phil, Empty, cached_property, find_item_type
+from .base import (
+    array_for_new_object, cached_property, Empty, find_item_type, HLObject,
+    phil, product, with_phil,
+)
 from . import filters
 from . import selections as sel
 from . import selections2 as sel2
 from .datatype import Datatype
 from .compat import filename_decode
 from .vds import VDSmap, vds_support
 
@@ -40,27 +39,26 @@
                   external=None, track_order=None, dcpl=None, dapl=None,
                   efile_prefix=None, virtual_prefix=None, allow_unknown_filter=False,
                   rdcc_nslots=None, rdcc_nbytes=None, rdcc_w0=None):
     """ Return a new low-level dataset identifier """
 
     # Convert data to a C-contiguous ndarray
     if data is not None and not isinstance(data, Empty):
-        from . import base
-        data = base.array_for_new_object(data, specified_dtype=dtype)
+        data = array_for_new_object(data, specified_dtype=dtype)
 
     # Validate shape
     if shape is None:
         if data is None:
             if dtype is None:
                 raise TypeError("One of data, shape or dtype must be specified")
             data = Empty(dtype)
         shape = data.shape
     else:
         shape = (shape,) if isinstance(shape, int) else tuple(shape)
-        if data is not None and (numpy.product(shape, dtype=numpy.ulonglong) != numpy.product(data.shape, dtype=numpy.ulonglong)):
+        if data is not None and (product(shape) != product(data.shape)):
             raise ValueError("Shape tuple is incompatible with data")
 
     if isinstance(maxshape, int):
         maxshape = (maxshape,)
     tmp_shape = maxshape if maxshape is not None else shape
 
     # Validate chunk shape
@@ -204,35 +202,27 @@
     def __init__(self, dset, dtype):
         self._dset = dset
         self._dtype = numpy.dtype(dtype)
 
     def __getitem__(self, args):
         return self._dset.__getitem__(args, new_dtype=self._dtype)
 
-    def __enter__(self):
-        # pylint: disable=protected-access
-        warn(
-            "Using astype() as a context manager is deprecated. "
-            "Slice the returned object instead, like: ds.astype(np.int32)[:10]",
-            category=H5pyDeprecationWarning, stacklevel=2,
-        )
-        self._dset._local.astype = self._dtype
-        return self
-
-    def __exit__(self, *args):
-        # pylint: disable=protected-access
-        self._dset._local.astype = None
-
     def __len__(self):
         """ Get the length of the underlying dataset
 
         >>> length = len(dataset.astype('f8'))
         """
         return len(self._dset)
 
+    def __array__(self, dtype=None):
+        data = self[:]
+        if dtype is not None:
+            data = data.astype(dtype)
+        return data
+
 
 class AsStrWrapper:
     """Wrapper to decode strings on reading the dataset"""
     def __init__(self, dset, encoding, errors='strict'):
         self._dset = dset
         if encoding is None:
             encoding = h5t.check_string_dtype(dset.dtype).encoding
@@ -257,14 +247,19 @@
     def __len__(self):
         """ Get the length of the underlying dataset
 
         >>> length = len(dataset.asstr())
         """
         return len(self._dset)
 
+    def __array__(self):
+        return numpy.array([
+            b.decode(self.encoding, self.errors) for b in self._dset
+        ], dtype=object).reshape(self._dset.shape)
+
 
 class FieldsWrapper:
     """Wrapper to extract named fields from a dataset with a struct dtype"""
     extract_field = None
 
     def __init__(self, dset, prior_dtype, names):
         self._dset = dset
@@ -490,15 +485,15 @@
         """Numpy-style attribute giving the total dataset size"""
         if 'size' in self._cache_props:
             return self._cache_props['size']
 
         if self._is_empty:
             size = None
         else:
-            size = numpy.prod(self.shape, dtype=numpy.intp)
+            size = product(self.shape)
 
         # If the file is read-only, cache the size to speed-up future uses.
         # This cache is invalidated by .refresh() when using SWMR.
         if self._readonly:
             self._cache_props['size'] = size
         return size
 
@@ -647,16 +642,14 @@
         super().__init__(bind)
 
         self._dcpl = self.id.get_create_plist()
         self._dxpl = h5p.create(h5p.DATASET_XFER)
         self._filters = filters.get_filters(self._dcpl)
         self._readonly = readonly
         self._cache_props = {}
-        self._local = local()
-        self._local.astype = None
 
     def resize(self, size, axis=None):
         """ Resize the dataset, or the specified axis.
 
         The dataset must be stored in chunked format; it can be resized up to
         the "maximum shape" (keyword maxshape) specified at creation time.
         The rank of the dataset cannot be changed.
@@ -756,17 +749,14 @@
 
         Also supports:
 
         * Boolean "mask" array indexing
         """
         args = args if isinstance(args, tuple) else (args,)
 
-        if new_dtype is None:
-            new_dtype = getattr(self._local, 'astype', None)
-
         if self._fast_read_ok and (new_dtype is None):
             try:
                 return self._fast_reader.read(args)
             except TypeError:
                 pass  # Fall back to Python read pathway below
 
         if self._is_empty:
@@ -881,15 +871,16 @@
                                        for x in val], dtype=self.dtype)
                 except ValueError:
                     pass
             if vlen == val.dtype:
                 if val.ndim > 1:
                     tmp = numpy.empty(shape=val.shape[:-1], dtype=object)
                     tmp.ravel()[:] = [i for i in val.reshape(
-                        (numpy.product(val.shape[:-1], dtype=numpy.ulonglong), val.shape[-1]))]
+                        (product(val.shape[:-1]), val.shape[-1])
+                    )]
                 else:
                     tmp = numpy.array([None], dtype=object)
                     tmp[0] = val
                 val = tmp
         elif self.dtype.kind == "O" or \
           (self.dtype.kind == 'V' and \
           (not isinstance(val, numpy.ndarray) or val.dtype.kind != 'V') and \
@@ -990,16 +981,15 @@
         # the dataset used an appropriate chunk size according the available
         # memory. In any case, if we cannot afford to create an intermediate
         # array of the same size as the dataset chunk size, the user program has
         # little hope to go much further. Solves h5py issue #1067
         if mshape == () and selection.array_shape != ():
             if self.dtype.subdtype is not None:
                 raise TypeError("Scalar broadcasting is not supported for array dtypes")
-            if self.chunks and (numpy.prod(self.chunks, dtype=numpy.float64) >=
-                                numpy.prod(selection.array_shape, dtype=numpy.float64)):
+            if self.chunks and (product(self.chunks) >= product(selection.array_shape)):
                 val2 = numpy.empty(selection.array_shape, dtype=val.dtype)
             else:
                 val2 = numpy.empty(selection.array_shape[-1], dtype=val.dtype)
             val2[...] = val
             val = val2
             mshape = val.shape
 
@@ -1063,15 +1053,15 @@
         """ Create a Numpy array containing the whole dataset.  DON'T THINK
         THIS MEANS DATASETS ARE INTERCHANGEABLE WITH ARRAYS.  For one thing,
         you have to read the whole dataset every time this method is called.
         """
         arr = numpy.zeros(self.shape, dtype=self.dtype if dtype is None else dtype)
 
         # Special case for (0,)*-shape datasets
-        if numpy.product(self.shape, dtype=numpy.ulonglong) == 0:
+        if self.size == 0:
             return arr
 
         self.read_direct(arr)
         return arr
 
     @with_phil
     def __repr__(self):
```

### Comparing `h5py-3.8.0/h5py/_hl/datatype.py` & `h5py-3.9.0/h5py/_hl/datatype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_hl/dims.py` & `h5py-3.9.0/h5py/_hl/dims.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_hl/files.py` & `h5py-3.9.0/h5py/_hl/files.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_hl/filters.py` & `h5py-3.9.0/h5py/_hl/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     encode
         Tuple of available filter names for encoding
 """
 from collections.abc import Mapping
 import operator
 
 import numpy as np
+from .base import product
 from .compat import filename_encode
 from .. import h5z, h5p, h5d, h5f
 
 
 _COMP_FILTERS = {'gzip': h5z.FILTER_DEFLATE,
                 'szip': h5z.FILTER_SZIP,
                 'lzf': h5z.FILTER_LZF,
@@ -354,36 +355,36 @@
 
     chunks = np.array(shape, dtype='=f8')
     if not np.all(np.isfinite(chunks)):
         raise ValueError("Illegal value in chunk tuple")
 
     # Determine the optimal chunk size in bytes using a PyTables expression.
     # This is kept as a float.
-    dset_size = np.product(chunks)*typesize
+    dset_size = product(chunks)*typesize
     target_size = CHUNK_BASE * (2**np.log10(dset_size/(1024.*1024)))
 
     if target_size > CHUNK_MAX:
         target_size = CHUNK_MAX
     elif target_size < CHUNK_MIN:
         target_size = CHUNK_MIN
 
     idx = 0
     while True:
         # Repeatedly loop over the axes, dividing them by 2.  Stop when:
         # 1a. We're smaller than the target chunk size, OR
         # 1b. We're within 50% of the target chunk size, AND
         #  2. The chunk is smaller than the maximum chunk size
 
-        chunk_bytes = np.product(chunks)*typesize
+        chunk_bytes = product(chunks)*typesize
 
         if (chunk_bytes < target_size or \
          abs(chunk_bytes-target_size)/target_size < 0.5) and \
          chunk_bytes < CHUNK_MAX:
             break
 
-        if np.product(chunks) == 1:
+        if product(chunks) == 1:
             break  # Element size larger than CHUNK_MAX
 
         chunks[idx%ndims] = np.ceil(chunks[idx%ndims] / 2.0)
         idx += 1
 
     return tuple(int(x) for x in chunks)
```

### Comparing `h5py-3.8.0/h5py/_hl/group.py` & `h5py-3.9.0/h5py/_hl/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,36 +401,36 @@
                 except KeyError:
                     return default
 
             if name not in self:
                 return default
 
             elif getclass and not getlink:
-                typecode = h5o.get_info(self.id, self._e(name)).type
+                typecode = h5o.get_info(self.id, self._e(name), lapl=self._lapl).type
 
                 try:
                     return {h5o.TYPE_GROUP: Group,
                             h5o.TYPE_DATASET: dataset.Dataset,
                             h5o.TYPE_NAMED_DATATYPE: datatype.Datatype}[typecode]
                 except KeyError:
                     raise TypeError("Unknown object type")
 
             elif getlink:
-                typecode = self.id.links.get_info(self._e(name)).type
+                typecode = self.id.links.get_info(self._e(name), lapl=self._lapl).type
 
                 if typecode == h5l.TYPE_SOFT:
                     if getclass:
                         return SoftLink
-                    linkbytes = self.id.links.get_val(self._e(name))
+                    linkbytes = self.id.links.get_val(self._e(name), lapl=self._lapl)
                     return SoftLink(self._d(linkbytes))
 
                 elif typecode == h5l.TYPE_EXTERNAL:
                     if getclass:
                         return ExternalLink
-                    filebytes, linkbytes = self.id.links.get_val(self._e(name))
+                    filebytes, linkbytes = self.id.links.get_val(self._e(name), lapl=self._lapl)
                     return ExternalLink(
                         filename_decode(filebytes), self._d(linkbytes)
                     )
 
                 elif typecode == h5l.TYPE_HARD:
                     return HardLink if getclass else HardLink()
 
@@ -504,14 +504,18 @@
         """ Iterate over member names in reverse order. """
         for x in self.id.__reversed__():
             yield self._d(x)
 
     @with_phil
     def __contains__(self, name):
         """ Test if a member name exists """
+        if hasattr(h5g, "_path_valid"):
+            if not self.id:
+                return False
+            return h5g._path_valid(self.id, self._e(name), self._lapl)
         return self._e(name) in self.id
 
     def copy(self, source, dest, name=None,
              shallow=False, expand_soft=False, expand_external=False,
              expand_refs=False, without_attrs=False):
         """Copy an object or group.
```

### Comparing `h5py-3.8.0/h5py/_hl/selections.py` & `h5py-3.9.0/h5py/_hl/selections.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,13 +423,13 @@
         N_leftover = masked_sid.get_select_npoints()
 
         return N//N_leftover
 
 
     shape = tuple(get_n_axis(sid, x) for x in range(rank))
 
-    if np.product(shape) != N:
+    if product(shape) != N:
         # This means multiple hyperslab selections are in effect,
         # so we fall back to a 1D shape
         return (N,)
 
     return shape
```

### Comparing `h5py-3.8.0/h5py/_hl/selections2.py` & `h5py-3.9.0/h5py/_hl/selections2.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_hl/vds.py` & `h5py-3.9.0/h5py/_hl/vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_locks.pxi` & `h5py-3.9.0/h5py/_locks.pxi`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_objects.pxd` & `h5py-3.9.0/h5py/_objects.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_objects.pyx` & `h5py-3.9.0/h5py/_objects.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_proxy.pxd` & `h5py-3.9.0/h5py/_proxy.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_proxy.pyx` & `h5py-3.9.0/h5py/_proxy.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/_selector.pyx` & `h5py-3.9.0/h5py/_selector.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/api_compat.h` & `h5py-3.9.0/h5py/api_compat.h`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/api_functions.txt` & `h5py-3.9.0/h5py/api_functions.txt`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,16 @@
 
   herr_t    H5Pset_nlinks(hid_t plist_id, size_t nlinks)
   herr_t    H5Pget_nlinks(hid_t plist_id, size_t *nlinks)
   herr_t    H5Pset_elink_prefix(hid_t plist_id, char *prefix)
   ssize_t   H5Pget_elink_prefix(hid_t plist_id, char *prefix, size_t size)
   hid_t     H5Pget_elink_fapl(hid_t lapl_id)
   herr_t    H5Pset_elink_fapl(hid_t lapl_id, hid_t fapl_id)
+  herr_t    H5Pget_elink_acc_flags(hid_t lapl_id, unsigned int *flags)
+  herr_t    H5Pset_elink_acc_flags(hid_t lapl_id, unsigned int flags)
 
   herr_t    H5Pset_create_intermediate_group(hid_t plist_id, unsigned crt_intmd)
   herr_t    H5Pget_create_intermediate_group(hid_t plist_id, unsigned *crt_intmd)
 
   herr_t    H5Pset_copy_object(hid_t plist_id, unsigned crt_intmd)
   herr_t    H5Pget_copy_object(hid_t plist_id, unsigned *crt_intmd)
 
@@ -582,14 +584,15 @@
   char*     H5Tget_tag(hid_t type_id)
 
 
   # === H5Z - Filters =========================================================
 
   htri_t    H5Zfilter_avail(H5Z_filter_t id_)
   herr_t    H5Zget_filter_info(H5Z_filter_t filter_, unsigned int *filter_config_flags)
+  herr_t    H5Zregister(const void *cls)
   herr_t    H5Zunregister(H5Z_filter_t id_)
 
 hdf5_hl:
 
   # === H5DS - Dimension Scales API =============================================
 
   herr_t  H5DSattach_scale(hid_t did, hid_t dsid, unsigned int idx)
```

### Comparing `h5py-3.8.0/h5py/api_types_ext.pxd` & `h5py-3.9.0/h5py/api_types_ext.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/api_types_hdf5.pxd` & `h5py-3.9.0/h5py/api_types_hdf5.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -772,14 +772,15 @@
       size_t nelmts, size_t buf_stride, size_t bkg_stride, void *buf,
       void *bkg, hid_t dset_xfer_plist) except -1
 
 # === H5Z - Filters ===========================================================
 
   ctypedef int H5Z_filter_t
 
+  int H5Z_CLASS_T_VERS
   int H5Z_FILTER_ERROR
   int H5Z_FILTER_NONE
   int H5Z_FILTER_ALL
   int H5Z_FILTER_DEFLATE
   int H5Z_FILTER_SHUFFLE
   int H5Z_FILTER_FLETCHER32
   int H5Z_FILTER_SZIP
```

### Comparing `h5py-3.8.0/h5py/h5.pxd` & `h5py-3.9.0/h5py/h5.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5.pyx` & `h5py-3.9.0/h5py/h5.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5a.pyx` & `h5py-3.9.0/h5py/h5a.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5ac.pyx` & `h5py-3.9.0/h5py/h5ac.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5d.pyx` & `h5py-3.9.0/h5py/h5d.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 """
 
 include "config.pxi"
 
 # Compile-time imports
 
 from collections import namedtuple
+cimport cython
 from ._objects cimport pdefault
 from numpy cimport ndarray, import_array, PyArray_DATA
 from .utils cimport  check_numpy_read, check_numpy_write, \
                      convert_tuple, convert_dims, emalloc, efree
 from .h5t cimport TypeID, typewrap, py_create
 from .h5s cimport SpaceID
 from .h5p cimport PropID, propwrap
 from ._proxy cimport dset_rw
 
 from ._objects import phil, with_phil
-from cpython cimport PyObject_GetBuffer, \
-                     PyBUF_ANY_CONTIGUOUS, \
-                     PyBuffer_Release
+from cpython cimport PyBUF_ANY_CONTIGUOUS, \
+                     PyBuffer_Release, \
+                     PyBytes_AsString, \
+                     PyBytes_FromStringAndSize, \
+                     PyObject_GetBuffer
 
 
 # Initialization
 import_array()
 
 # === Public constants and data structures ====================================
 
@@ -512,73 +515,87 @@
                 efree(offset)
                 PyBuffer_Release(&view)
                 if space_id:
                     H5Sclose(space_id)
 
     IF HDF5_VERSION >= (1, 10, 2):
 
-        def read_direct_chunk(self, offsets, PropID dxpl=None):
-            """ (offsets, PropID dxpl=None)
+        @cython.boundscheck(False)
+        @cython.wraparound(False)
+        def read_direct_chunk(self, offsets, PropID dxpl=None, unsigned char[::1] out=None):
+            """ (offsets, PropID dxpl=None, out=None)
 
             Reads data to a bytes array directly from a chunk at position
             specified by the `offsets` argument and bypasses any filters HDF5
             would normally apply to the written data. However, the written data
             may be compressed or not.
 
-            Returns a tuple containing the `filter_mask` and the bytes data
-            which are the raw data storing this chuck.
+            Returns a tuple containing the `filter_mask` and the raw data
+            storing this chunk as bytes if `out` is None, else as a memoryview.
 
             `filter_mask` is a bit field of up to 32 values. It records which
             filters have been applied to this chunk, of the filter pipeline
             defined for that dataset. Each bit set to `1` means that the filter
             in the corresponding position in the pipeline was not applied to
             compute the raw data. So the default value of `0` means that all
             defined filters have been applied to the raw data.
 
+            If the `out` argument is not None, it must be a writeable
+            contiguous 1D array-like of bytes (e.g., `bytearray` or
+            `numpy.ndarray`) and large enough to contain the whole chunk.
+
             Feature requires: 1.10.2 HDF5
             """
-
             cdef hid_t dset_id
             cdef hid_t dxpl_id
-            cdef hid_t space_id = 0
+            cdef hid_t space_id
             cdef hsize_t *offset = NULL
-            cdef size_t data_size
             cdef int rank
             cdef uint32_t filters
-            cdef hsize_t read_chunk_nbytes
-            cdef char *data = NULL
-            cdef bytes ret
+            cdef hsize_t chunk_bytes, out_bytes
+            cdef int nb_offsets = len(offsets)
+            cdef void * chunk_buffer
 
             dset_id = self.id
             dxpl_id = pdefault(dxpl)
-            space_id = H5Dget_space(self.id)
+            space_id = H5Dget_space(dset_id)
             rank = H5Sget_simple_extent_ndims(space_id)
+            H5Sclose(space_id)
 
-            if len(offsets) != rank:
-                raise TypeError("offset length (%d) must match dataset rank (%d)" % (len(offsets), rank))
+            if nb_offsets != rank:
+                raise TypeError(
+                    f"offsets length ({nb_offsets}) must match dataset rank ({rank})"
+                )
 
+            offset = <hsize_t*>emalloc(sizeof(hsize_t)*rank)
             try:
-                offset = <hsize_t*>emalloc(sizeof(hsize_t)*rank)
                 convert_tuple(offsets, offset, rank)
-                H5Dget_chunk_storage_size(dset_id, offset, &read_chunk_nbytes)
-                data = <char *>emalloc(read_chunk_nbytes)
+                H5Dget_chunk_storage_size(dset_id, offset, &chunk_bytes)
+
+                if out is None:
+                    retval = PyBytes_FromStringAndSize(NULL, chunk_bytes)
+                    chunk_buffer = PyBytes_AsString(retval)
+                else:
+                    out_bytes = out.shape[0]  # Fast way to get out length
+                    if out_bytes < chunk_bytes:
+                        raise ValueError(
+                            f"out buffer is only {out_bytes} bytes, {chunk_bytes} bytes required"
+                        )
+                    retval = memoryview(out[:chunk_bytes])
+                    chunk_buffer = &out[0]
 
                 IF HDF5_VERSION >= (1, 10, 3):
-                    H5Dread_chunk(dset_id, dxpl_id, offset, &filters, data)
+                    H5Dread_chunk(dset_id, dxpl_id, offset, &filters, chunk_buffer)
                 ELSE:
-                    H5DOread_chunk(dset_id, dxpl_id, offset, &filters, data)
-                ret = data[:read_chunk_nbytes]
+                    H5DOread_chunk(dset_id, dxpl_id, offset, &filters, chunk_buffer)
             finally:
                 efree(offset)
-                if data:
-                    efree(data)
-                if space_id:
-                    H5Sclose(space_id)
 
-            return filters, ret
+            return filters, retval
+
 
     IF HDF5_VERSION >= (1, 10, 5):
 
         @with_phil
         def get_num_chunks(self, SpaceID space=None):
             """ (SpaceID space=None) => INT num_chunks
```

### Comparing `h5py-3.8.0/h5py/h5ds.pyx` & `h5py-3.9.0/h5py/h5ds.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5f.pyx` & `h5py-3.9.0/h5py/h5f.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5fd.pyx` & `h5py-3.9.0/h5py/h5fd.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5g.pyx` & `h5py-3.9.0/h5py/h5g.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5i.pyx` & `h5py-3.9.0/h5py/h5i.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5l.pyx` & `h5py-3.9.0/h5py/h5l.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5o.pyx` & `h5py-3.9.0/h5py/h5o.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5p.pxd` & `h5py-3.9.0/h5py/h5p.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5p.pyx` & `h5py-3.9.0/h5py/h5p.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1640,14 +1640,35 @@
         """
         cdef hid_t fid
         fid = H5Pget_elink_fapl(self.id)
         if H5Iget_ref(fid) > 1:
             H5Idec_ref(fid)
         return propwrap(fid)
 
+
+    @with_phil
+    def set_elink_acc_flags(self, unsigned int flags):
+        """ (UNIT flags)
+
+        Sets the external link traversal file access flag in a link access property list.
+        """
+        H5Pset_elink_acc_flags(self.id, flags)
+
+
+    @with_phil
+    def get_elink_acc_flags(self):
+        """() => UINT
+
+        Retrieves the external link traversal file access flag from the specified link access property list.
+        """
+        cdef unsigned int flags
+        H5Pget_elink_acc_flags(self.id, &flags)
+        return flags
+
+
 # Datatype creation
 cdef class PropTCID(PropOCID):
     """ Datatype creation property list
 
     No methods yet.
     """
```

### Comparing `h5py-3.8.0/h5py/h5pl.pxd` & `h5py-3.9.0/h5py/h5pl.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5pl.pyx` & `h5py-3.9.0/h5py/h5pl.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5py_warnings.py` & `h5py-3.9.0/h5py/h5py_warnings.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5r.pxd` & `h5py-3.9.0/h5py/h5r.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5r.pyx` & `h5py-3.9.0/h5py/h5r.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5s.pyx` & `h5py-3.9.0/h5py/h5s.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5t.pxd` & `h5py-3.9.0/h5py/h5t.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5t.pyx` & `h5py-3.9.0/h5py/h5t.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/h5z.pyx` & `h5py-3.9.0/h5py/h5z.pyx`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 """
 
 from ._objects import phil, with_phil
 
 
 # === Public constants and data structures ====================================
 
+CLASS_T_VERS = H5Z_CLASS_T_VERS
+
 FILTER_LZF = H5PY_FILTER_LZF
 
 FILTER_ERROR    = H5Z_FILTER_ERROR
 FILTER_NONE     = H5Z_FILTER_NONE
 FILTER_ALL      = H5Z_FILTER_ALL
 FILTER_DEFLATE  = H5Z_FILTER_DEFLATE
 FILTER_SHUFFLE  = H5Z_FILTER_SHUFFLE
@@ -93,14 +95,35 @@
     """
     cdef unsigned int flags
     H5Zget_filter_info(<H5Z_filter_t>filter_code, &flags)
     return flags
 
 
 @with_phil
+def register_filter(Py_ssize_t cls_pointer_address):
+    '''(INT cls_pointer_address) => BOOL
+
+    Register a new filter from the memory address of a buffer containing a
+    ``H5Z_class1_t`` or ``H5Z_class2_t`` data structure describing the filter.
+
+    `cls_pointer_address` can be retrieved from a HDF5 filter plugin dynamic
+    library::
+
+        import ctypes
+
+        filter_clib = ctypes.CDLL("/path/to/my_hdf5_filter_plugin.so")
+        filter_clib.H5PLget_plugin_info.restype = ctypes.c_void_p
+
+        h5py.h5z.register_filter(filter_clib.H5PLget_plugin_info())
+
+    '''
+    return <int>H5Zregister(<const void *>cls_pointer_address) >= 0
+
+
+@with_phil
 def unregister_filter(int filter_code):
     '''(INT filter_code) => BOOL
 
     Unregister a filter
 
     '''
     return <int>H5Zunregister(<H5Z_filter_t>filter_code) >= 0
```

### Comparing `h5py-3.8.0/h5py/ipy_completer.py` & `h5py-3.9.0/h5py/ipy_completer.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,20 @@
     return ["%s.%s" % (base, a) for a in attrs if a[:len(attr)] == attr]
 
 
 def h5py_completer(self, event):
     """ Completer function to be loaded into IPython """
     base = re_object_match.split(event.line)[1]
 
-    if not isinstance(self._ofind(base).get('obj'), (AttributeManager, HLObject)):
+    try:
+        obj = self._ofind(base).obj
+    except AttributeError:
+        obj = self._ofind(base).get('obj')
+
+    if not isinstance(obj, (AttributeManager, HLObject)):
         raise TryNext
 
     try:
         return h5py_attr_completer(self, event.line)
     except ValueError:
         pass
```

### Comparing `h5py-3.8.0/h5py/tests/__init__.py` & `h5py-3.9.0/h5py/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/common.py` & `h5py-3.9.0/h5py/tests/common.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/conftest.py` & `h5py-3.9.0/h5py/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/data_files/vlen_string_dset.h5` & `h5py-3.9.0/h5py/tests/data_files/vlen_string_dset.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/data_files/vlen_string_dset_utc.h5` & `h5py-3.9.0/h5py/tests/data_files/vlen_string_dset_utc.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/data_files/vlen_string_s390x.h5` & `h5py-3.9.0/h5py/tests/data_files/vlen_string_s390x.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_attribute_create.py` & `h5py-3.9.0/h5py/tests/test_attribute_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,7 +85,11 @@
         array = np.arange(4, dtype='i')
         with self.assertRaises(ValueError):
             self.f.attrs.create('x', data=array, dtype=dt)
         # Shape of new attribute conflicts with shape of data
         dt = np.dtype('()i')
         with self.assertRaises(ValueError):
             self.f.attrs.create('x', data=array, shape=(5,), dtype=dt)
+
+    def test_key_type(self):
+        with self.assertRaises(TypeError):
+            self.f.attrs.create(1, data=('a', 'b'))
```

### Comparing `h5py-3.8.0/h5py/tests/test_attrs.py` & `h5py-3.9.0/h5py/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_attrs_data.py` & `h5py-3.9.0/h5py/tests/test_attrs_data.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_base.py` & `h5py-3.9.0/h5py/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_big_endian_file.py` & `h5py-3.9.0/h5py/tests/test_big_endian_file.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_completions.py` & `h5py-3.9.0/h5py/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_dataset.py` & `h5py-3.9.0/h5py/tests/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import platform
 import pytest
 import warnings
 
 from .common import ut, TestCase
 from .data_files import get_data_file_path
 from h5py import File, Group, Dataset
-from h5py._hl.base import is_empty_dataspace
+from h5py._hl.base import is_empty_dataspace, product
 from h5py import h5f, h5t
 from h5py.h5py_warnings import H5pyDeprecationWarning
 from h5py import version
 import h5py
 import h5py._hl.selections as sel
 
 
@@ -227,15 +227,15 @@
         [
             ((100,), (100,), np.s_[0:10], np.s_[50:60]),
             ((70,), (100,), np.s_[50:60], np.s_[90:]),
             ((30, 10), (20, 20), np.s_[:20, :], np.s_[:, :10]),
             ((5, 7, 9), (6,), np.s_[2, :6, 3], np.s_[:]),
         ])
     def test_read_direct(self, writable_file, source_shape, dest_shape, source_sel, dest_sel):
-        source_values = np.arange(np.product(source_shape), dtype="int64").reshape(source_shape)
+        source_values = np.arange(product(source_shape), dtype="int64").reshape(source_shape)
         dset = writable_file.create_dataset("dset", source_shape, data=source_values)
         arr = np.full(dest_shape, -1, dtype="int64")
         expected = arr.copy()
         expected[dest_sel] = source_values[source_sel]
 
         dset.read_direct(arr, source_sel, dest_sel)
         np.testing.assert_array_equal(arr, expected)
@@ -276,15 +276,15 @@
             ((100,), (100,), np.s_[0:10], np.s_[50:60]),
             ((70,), (100,), np.s_[50:60], np.s_[90:]),
             ((30, 10), (20, 20), np.s_[:20, :], np.s_[:, :10]),
             ((5, 7, 9), (6,), np.s_[2, :6, 3], np.s_[:]),
         ])
     def test_write_direct(self, writable_file, source_shape, dest_shape, source_sel, dest_sel):
         dset = writable_file.create_dataset('dset', dest_shape, dtype='int32', fillvalue=-1)
-        arr = np.arange(np.product(source_shape)).reshape(source_shape)
+        arr = np.arange(product(source_shape)).reshape(source_shape)
         expected = np.full(dest_shape, -1, dtype='int32')
         expected[dest_sel] = arr[source_sel]
         dset.write_direct(arr, source_sel, dest_sel)
         np.testing.assert_array_equal(dset[:], expected)
 
     def test_empty(self, writable_file):
         empty_dset = writable_file.create_dataset("edset", dtype='int64')
@@ -1253,20 +1253,23 @@
 
         # latin-1 will decode it but give the wrong text
         self.assertNotEqual(ds.asstr('latin-1')[0], data)
 
         # len of ds
         self.assertEqual(10, len(ds.asstr()))
 
-
         # Array output
         np.testing.assert_array_equal(
             ds.asstr()[:1], np.array([data], dtype=object)
         )
 
+        np.testing.assert_array_equal(
+            np.asarray(ds.asstr())[:1], np.array([data], dtype=object)
+        )
+
     def test_asstr_fixed(self):
         dt = h5py.string_dtype(length=5)
         ds = self.f.create_dataset('x', (10,), dtype=dt)
         data = 'cù'
         ds[0] = np.array(data.encode('utf-8'), dtype=dt)
 
         self.assertIsInstance(ds[0], np.bytes_)
@@ -1565,41 +1568,32 @@
         self.assertEqual(self.dset.regionref.shape(ref), self.dset.shape)
         self.assertEqual(self.dset.regionref.selection(ref), (10, 18))
 
 
 class TestAstype(BaseDataset):
     """.astype() wrapper & context manager
     """
-    def test_astype_ctx(self):
-        dset = self.f.create_dataset('x', (100,), dtype='i2')
-        dset[...] = np.arange(100)
-
-        with warnings.catch_warnings(record=True) as warn_rec:
-            warnings.simplefilter("always")
-
-            with dset.astype('f8'):
-                self.assertArrayEqual(dset[...], np.arange(100, dtype='f8'))
-
-            with dset.astype('f4') as f4ds:
-                self.assertArrayEqual(f4ds[...], np.arange(100, dtype='f4'))
-
-        assert [w.category for w in warn_rec] == [H5pyDeprecationWarning] * 2
-
     def test_astype_wrapper(self):
         dset = self.f.create_dataset('x', (100,), dtype='i2')
         dset[...] = np.arange(100)
         arr = dset.astype('f4')[:]
         self.assertArrayEqual(arr, np.arange(100, dtype='f4'))
 
 
     def test_astype_wrapper_len(self):
         dset = self.f.create_dataset('x', (100,), dtype='i2')
         dset[...] = np.arange(100)
         self.assertEqual(100, len(dset.astype('f4')))
 
+    def test_astype_wrapper_asarray(self):
+        dset = self.f.create_dataset('x', (100,), dtype='i2')
+        dset[...] = np.arange(100)
+        arr = np.asarray(dset.astype('f4'), dtype='i2')
+        self.assertArrayEqual(arr, np.arange(100, dtype='i2'))
+
 
 class TestScalarCompound(BaseDataset):
 
     """
         Retrieval of a single field from a scalar compound dataset should
         strip the field info
     """
```

### Comparing `h5py-3.8.0/h5py/tests/test_dataset_getitem.py` & `h5py-3.9.0/h5py/tests/test_dataset_getitem.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_dataset_swmr.py` & `h5py-3.9.0/h5py/tests/test_dataset_swmr.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_datatype.py` & `h5py-3.9.0/h5py/tests/test_datatype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_dimension_scales.py` & `h5py-3.9.0/h5py/tests/test_dimension_scales.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_dims_dimensionproxy.py` & `h5py-3.9.0/h5py/tests/test_dims_dimensionproxy.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_dtype.py` & `h5py-3.9.0/h5py/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_errors.py` & `h5py-3.9.0/h5py/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_file.py` & `h5py-3.9.0/h5py/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_file2.py` & `h5py-3.9.0/h5py/tests/test_file2.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_file_alignment.py` & `h5py-3.9.0/h5py/tests/test_file_alignment.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_file_image.py` & `h5py-3.9.0/h5py/tests/test_file_image.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_filters.py` & `h5py-3.9.0/h5py/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 """
     Tests the h5py._hl.filters module.
 
 """
 import os
 import numpy as np
 import h5py
-import pytest
 
-from .common import ut, TestCase, insubprocess
+from .common import ut, TestCase
 
 
 class TestFilters(TestCase):
 
     def setUp(self):
         """ like TestCase.setUp but also store the file path """
         self.path = self.mktemp()
@@ -83,21 +82,13 @@
 def test_filter_ref_obj_eq():
     gzip8 = h5py.filters.Gzip(level=8)
 
     assert gzip8 == h5py.filters.Gzip(level=8)
     assert gzip8 != h5py.filters.Gzip(level=7)
 
 
-@pytest.mark.mpi_skip
-@insubprocess
-def test_unregister_filter(request):
-    if h5py.h5z.filter_avail(h5py.h5z.FILTER_LZF):
-        res = h5py.h5z.unregister_filter(h5py.h5z.FILTER_LZF)
-        assert res
-
-
 @ut.skipIf(not os.getenv('H5PY_TEST_CHECK_FILTERS'),  "H5PY_TEST_CHECK_FILTERS not set")
 def test_filters_available():
     assert 'gzip' in h5py.filters.decode
     assert 'gzip' in h5py.filters.encode
     assert 'lzf' in h5py.filters.decode
     assert 'lzf' in h5py.filters.encode
```

### Comparing `h5py-3.8.0/h5py/tests/test_group.py` & `h5py-3.9.0/h5py/tests/test_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,19 @@
         """ Unicode names convertible to ASCII are stored as ASCII (issue 239)
         """
         name = u"/Hello, this is a name"
         group = self.f.create_group(name)
         self.assertEqual(group.name, name)
         self.assertEqual(group.id.links.get_info(name.encode('utf8')).cset, h5t.CSET_ASCII)
 
+    def test_type(self):
+        """ Names should be strings or bytes """
+        with self.assertRaises(TypeError):
+            self.f.create_group(1.)
+
     def test_appropriate_low_level_id(self):
         " Binding a group to a non-group identifier fails with ValueError "
         dset = self.f.create_dataset('foo', [1])
         with self.assertRaises(ValueError):
             Group(dset.id)
 
 class TestDatasetAssignment(BaseGroup):
```

### Comparing `h5py-3.8.0/h5py/tests/test_h5.py` & `h5py-3.9.0/h5py/tests/test_h5.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_h5f.py` & `h5py-3.9.0/h5py/tests/test_h5f.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_h5p.py` & `h5py-3.9.0/h5py/tests/test_h5p.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_h5pl.py` & `h5py-3.9.0/h5py/tests/test_h5pl.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_h5t.py` & `h5py-3.9.0/h5py/tests/test_h5t.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_objects.py` & `h5py-3.9.0/h5py/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_ros3.py` & `h5py-3.9.0/h5py/tests/test_ros3.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_selections.py` & `h5py-3.9.0/h5py/tests/test_selections.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_slicing.py` & `h5py-3.9.0/h5py/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_vds/test_highlevel_vds.py` & `h5py-3.9.0/h5py/tests/test_vds/test_highlevel_vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_vds/test_lowlevel_vds.py` & `h5py-3.9.0/h5py/tests/test_vds/test_lowlevel_vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/tests/test_vds/test_virtual_source.py` & `h5py-3.9.0/h5py/tests/test_vds/test_virtual_source.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/utils.pxd` & `h5py-3.9.0/h5py/utils.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/utils.pyx` & `h5py-3.9.0/h5py/utils.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/h5py/version.py` & `h5py-3.9.0/h5py/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # All should be integers, except pre, as validating versions is more than is
 # needed for our use case
 _H5PY_VERSION_CLS = namedtuple("_H5PY_VERSION_CLS",
                                "major minor bugfix pre post dev")
 
 hdf5_built_version_tuple = _h5.HDF5_VERSION_COMPILED_AGAINST
 
-version_tuple = _H5PY_VERSION_CLS(3, 8, 0, None, None, None)
+version_tuple = _H5PY_VERSION_CLS(3, 9, 0, None, None, None)
 
 version = "{0.major:d}.{0.minor:d}.{0.bugfix:d}".format(version_tuple)
 if version_tuple.pre is not None:
     version += version_tuple.pre
 if version_tuple.post is not None:
     version += ".post{0.post:d}".format(version_tuple)
 if version_tuple.dev is not None:
```

### Comparing `h5py-3.8.0/h5py.egg-info/PKG-INFO` & `h5py-3.9.0/h5py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5py
-Version: 3.8.0
+Version: 3.9.0
 Summary: Read and write HDF5 files from Python
 Author-email: Andrew Collette <andrew.collette@gmail.com>
 Maintainer-email: Thomas Kluyver <thomas@kluyver.me.uk>, Thomas A Caswell <tcaswell@bnl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://www.h5py.org/
 Project-URL: Source, https://github.com/h5py/h5py
 Project-URL: Documentation, https://docs.h5py.org/en/stable/
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 The h5py package provides both a high- and low-level interface to the HDF5
 library from Python. The low-level interface is intended to be a complete
 wrapping of the HDF5 API, while the high-level component supports  access to
 HDF5 files, datasets and groups using established Python and NumPy concepts.
```

### Comparing `h5py-3.8.0/h5py.egg-info/SOURCES.txt` & `h5py-3.9.0/h5py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.gitignore
 LICENSE
 MANIFEST.in
 README.rst
 api_gen.py
 asv.conf.json
 dev-install.sh
 pylintrc
@@ -56,14 +55,15 @@
 docs/whatsnew/3.2.rst
 docs/whatsnew/3.3.rst
 docs/whatsnew/3.4.rst
 docs/whatsnew/3.5.rst
 docs/whatsnew/3.6.rst
 docs/whatsnew/3.7.rst
 docs/whatsnew/3.8.rst
+docs/whatsnew/3.9.rst
 docs/whatsnew/index.rst
 docs_api/Makefile
 docs_api/automod.py
 docs_api/conf.py
 docs_api/h5.rst
 docs_api/h5a.rst
 docs_api/h5ac.rst
@@ -198,14 +198,15 @@
 h5py/tests/test_h5.py
 h5py/tests/test_h5d_direct_chunk.py
 h5py/tests/test_h5f.py
 h5py/tests/test_h5o.py
 h5py/tests/test_h5p.py
 h5py/tests/test_h5pl.py
 h5py/tests/test_h5t.py
+h5py/tests/test_h5z.py
 h5py/tests/test_objects.py
 h5py/tests/test_ros3.py
 h5py/tests/test_selections.py
 h5py/tests/test_slicing.py
 h5py/tests/data_files/__init__.py
 h5py/tests/data_files/vlen_string_dset.h5
 h5py/tests/data_files/vlen_string_dset_utc.h5
```

### Comparing `h5py-3.8.0/licenses/hdf5.txt` & `h5py-3.9.0/licenses/hdf5.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/licenses/license.txt` & `h5py-3.9.0/licenses/license.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/licenses/pytables.txt` & `h5py-3.9.0/licenses/pytables.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/licenses/python.txt` & `h5py-3.9.0/licenses/python.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/licenses/stdint.txt` & `h5py-3.9.0/licenses/stdint.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/LICENSE.txt` & `h5py-3.9.0/lzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/README.txt` & `h5py-3.9.0/lzf/README.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/example.c` & `h5py-3.9.0/lzf/example.c`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf/lzf.h` & `h5py-3.9.0/lzf/lzf/lzf.h`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf/lzfP.h` & `h5py-3.9.0/lzf/lzf/lzfP.h`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf/lzf_c.c` & `h5py-3.9.0/lzf/lzf/lzf_c.c`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf/lzf_d.c` & `h5py-3.9.0/lzf/lzf/lzf_d.c`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf_filter.c` & `h5py-3.9.0/lzf/lzf_filter.c`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/lzf/lzf_filter.h` & `h5py-3.9.0/lzf/lzf_filter.h`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/pylintrc` & `h5py-3.9.0/pylintrc`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/pyproject.toml` & `h5py-3.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "Cython ~=0.29",
+    "Cython >=0.29.31,<1",
     "oldest-supported-numpy",
     "pkgconfig",
     "setuptools >=61",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -32,15 +32,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Database",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["dependencies", "version"]
 
 [project.readme]
 text = """\
 The h5py package provides both a high- and low-level interface to the HDF5
 library from Python. The low-level interface is intended to be a complete
 wrapping of the HDF5 API, while the high-level component supports  access to
```

### Comparing `h5py-3.8.0/setup.py` & `h5py-3.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 # path, add it back if needed.
 if '' not in sys.path:
     sys.path.insert(0, '')
 
 import setup_build, setup_configure
 
 
-VERSION = '3.8.0'
+VERSION = '3.9.0'
 
 
 # these are required to use h5py
 RUN_REQUIRES = [
     # We only really aim to support NumPy & Python combinations for which
-    # there are wheels on PyPI (e.g. NumPy >=1.17.5 for Python 3.8).
+    # there are wheels on PyPI (e.g. NumPy >=1.23.2 for Python 3.11).
     # But we don't want to duplicate the information in oldest-supported-numpy
     # here, and if you can build an older NumPy on a newer Python, h5py probably
     # works (assuming you build it from source too).
-    # NumPy 1.14.5 is the first with wheels for Python 3.7, our minimum Python.
-    "numpy >=1.14.5",
+    # NumPy 1.17.3 is the first with wheels for Python 3.8, our minimum Python.
+    "numpy >=1.17.3",
 ]
 
 # Packages needed to build h5py (in addition to static list in pyproject.toml)
 # For packages we link to (numpy, mpi4py), we build against the oldest
 # supported version; h5py wheels should then work with newer versions of these.
 # Downstream packagers - e.g. Linux distros - can safely build with newer
 # versions.
 # TODO: setup_requires is deprecated in setuptools.
 SETUP_REQUIRES = []
 
 if setup_configure.mpi_enabled():
-    RUN_REQUIRES.append('mpi4py >=3.0.2')
-    SETUP_REQUIRES.append("mpi4py ==3.0.2; python_version<'3.8'")
-    SETUP_REQUIRES.append("mpi4py ==3.0.3; python_version=='3.8.*'")
-    SETUP_REQUIRES.append("mpi4py ==3.1.0; python_version=='3.9.*' or python_version=='3.10.*'")
+    # mpi4py 3.1.1 fixed a typo in python_requires, which made older versions
+    # incompatible with newer setuptools.
+    RUN_REQUIRES.append('mpi4py >=3.1.1')
+    SETUP_REQUIRES.append("mpi4py ==3.1.1; python_version<'3.11'")
     SETUP_REQUIRES.append("mpi4py ==3.1.4; python_version>='3.11'")
 
 # Set the environment variable H5PY_SETUP_REQUIRES=0 if we need to skip
 # setup_requires for any reason.
 if os.environ.get('H5PY_SETUP_REQUIRES', '1') == '0':
     SETUP_REQUIRES = []
```

### Comparing `h5py-3.8.0/setup_build.py` & `h5py-3.9.0/setup_build.py`

 * *Files identical despite different names*

### Comparing `h5py-3.8.0/setup_configure.py` & `h5py-3.9.0/setup_configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
         if op.isabs(path) and not op.exists(path):
             raise FileNotFoundError(f"{path} is missing")
 
         try:
             lib = ctypes.CDLL(path, **load_kw)
         except Exception:
             print("error: Unable to load dependency HDF5, make sure HDF5 is installed properly")
+            print("Library dirs checked:", libdirs)
             raise
 
         self._lib = lib
 
     def autodetect_version(self):
         """
         Detect the current version of HDF5, and return X.Y.Z version string.
```

### Comparing `h5py-3.8.0/tox.ini` & `h5py-3.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tox]
 # We want an envlist like
 # envlist = {py36,py37,pypy3}-{test}-{deps,mindeps}-{,mpi4py}-{,pre},nightly,docs,checkreadme,pre-commit
 # but we want to skip mpi and pre by default, so this envlist is below
-envlist = {py37,py38,py39,py310,py311,pypy3}-{test}-{deps,mindeps},nightly,docs,apidocs,checkreadme,pre-commit,rever
+envlist = {py38,py39,py310,py311,pypy3}-{test}-{deps,mindeps},nightly,docs,apidocs,checkreadme,pre-commit,rever
 isolated_build = True
 
 [testenv]
 deps =
     test: pytest
     test: pytest-cov
     test: pytest-mpi>=0.2
 
-    py37-deps: numpy>=1.14.5
     py38-deps: numpy>=1.17.5
     py39-deps: numpy>=1.19.3
     py310-deps: numpy>=1.21.3
     py311-deps: numpy>=1.23.2
 
     mindeps: oldest-supported-numpy
 
-    mpi4py: mpi4py>=3.0.2
+    mpi4py: mpi4py>=3.1.1
 
     tables-deps: tables>=3.4.4
     tables-mindeps: tables==3.4.4
 
 # see pytest.ini for additional common options to pytest
 commands =
     test: python -c "import sys; print('64 bit?', sys.maxsize > 2**32)"
```

