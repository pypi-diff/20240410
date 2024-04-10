# Comparing `tmp/dpgen-0.9.0.tar.gz` & `tmp/dpgen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpgen-0.9.0.tar", last modified: Sun Mar 28 00:43:38 2021, max compression
+gzip compressed data, was "dpgen-0.9.1.tar", last modified: Sat Mar 27 23:34:34 2021, max compression
```

## Comparing `dpgen-0.9.0.tar` & `dpgen-0.9.1.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.809576 dpgen-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-28 00:42:54.000000 dpgen-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-03-28 00:42:54.000000 dpgen-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-03-28 00:42:54.000000 dpgen-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    66034 2021-03-28 00:43:38.929576 dpgen-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    55746 2021-03-28 00:42:54.000000 dpgen-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.809576 dpgen-0.9.0/dpgen/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen/_date.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.817576 dpgen-0.9.0/dpgen/auto_test/
--rw-r--r--   0 runner    (1001) docker     (121)     9270 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/EOS.py
--rw-r--r--   0 runner    (1001) docker     (121)    10134 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12729 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Interstitial.py
--rw-r--r--   0 runner    (1001) docker     (121)    21493 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Property.py
--rw-r--r--   0 runner    (1001) docker     (121)    10211 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Task.py
--rw-r--r--   0 runner    (1001) docker     (121)     9363 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/VASP.py
--rw-r--r--   0 runner    (1001) docker     (121)     9507 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/Vacancy.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/common_equi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8982 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/common_prop.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4355 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/gen_confs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.817576 dpgen-0.9.0/dpgen/auto_test/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/BatchJob.py
--rw-r--r--   0 runner    (1001) docker     (121)    19814 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/RemoteJob.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/SlurmJob.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/crys.py
--rw-r--r--   0 runner    (1001) docker     (121)    17558 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/lmp.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/localhost.json
--rwxr-xr-x   0 runner    (1001) docker     (121)    45430 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/mfp_eosfit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/pwscf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/siesta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14835 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/lib/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/mpdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/refine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/dpgen/auto_test/template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/dpgen/auto_test/template/elastic/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.817576 dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/displace.mod
--rw-r--r--   0 runner    (1001) docker     (121)     8724 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/in.elastic
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/init.mod
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/potential.mod
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.821575 dpgen-0.9.0/dpgen/auto_test/template/incars/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/incars/INCAR.relax
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/auto_test/template/incars/INCAR.static
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.821575 dpgen-0.9.0/dpgen/collect/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/collect/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.821575 dpgen-0.9.0/dpgen/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25596 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.829576 dpgen-0.9.0/dpgen/data/jsons/
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.diamond.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.diamond.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.fcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.fcc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.hcp.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.hcp.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.hcp.332.json
--rw-r--r--   0 runner    (1001) docker     (121)      556 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/al.sc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.diamond.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.diamond.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.fcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.fcc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.hcp.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.hcp.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.hcp.332.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.sc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/almg.sc.333.json
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.diamond.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.diamond.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.fcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.fcc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.hcp.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.hcp.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.hcp.332.json
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/mg.sc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/param.json
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.diamond.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.diamond.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.fcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.fcc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.hcp.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.hcp.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/si.sc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.al.fcc.json
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.al.hcp.json
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.almg.fcc.json
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.almg.hcp.json
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.mg.fcc.json
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.mg.hcp.json
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/surf.si.diamond.json
--rw-r--r--   0 runner    (1001) docker     (121)      602 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/w.bcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/w.bcc.222.json
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/w.diamond.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/w.fcc.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/w.hcp.111.json
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/jsons/water.111.json
--rw-r--r--   0 runner    (1001) docker     (121)     7338 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)    21785 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/surf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.829576 dpgen-0.9.0/dpgen/data/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/bcc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12048 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/cessp2force_lin.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      255 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/clean.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     8314 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/create_random_disturb.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/diamond.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/fcc.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/hcp.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7636 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/io_lammps.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1438 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/ovito_file_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1133 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/poscar_copy.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/sc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       96 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/data/tools/test.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.829576 dpgen-0.9.0/dpgen/database/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/database/entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5262 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/database/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/database/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.833576 dpgen-0.9.0/dpgen/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (121)    23016 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/ALI.py
--rw-r--r--   0 runner    (1001) docker     (121)     6307 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/AWS.py
--rw-r--r--   0 runner    (1001) docker     (121)     6706 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/Batch.py
--rw-r--r--   0 runner    (1001) docker     (121)    14600 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/Dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    13513 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/DispatcherList.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/JobStatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     7306 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/LSF.py
--rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/LazyLocalContext.py
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/LocalContext.py
--rw-r--r--   0 runner    (1001) docker     (121)     5238 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/PBS.py
--rw-r--r--   0 runner    (1001) docker     (121)    10809 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/SSHContext.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/Shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     7693 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/Slurm.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/dispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.833576 dpgen-0.9.0/dpgen/generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.833576 dpgen-0.9.0/dpgen/generator/ch4/
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/ch4/machine.json
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/ch4/param.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/dpgen/generator/lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6244 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/cp2k.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/cvasp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/ele_temp.py
--rw-r--r--   0 runner    (1001) docker     (121)    10483 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     5996 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/pwmat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8367 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/pwscf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/siesta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/lib/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)    96512 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/generator/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     7443 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/dpgen/remote/
--rw-r--r--   0 runner    (1001) docker     (121)    35697 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/remote/RemoteJob.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13830 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/remote/decide_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)    18343 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/remote/group_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/remote/localhost.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/dpgen/simplify/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/simplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27485 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/simplify/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/dpgen/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10381 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/auto_gen_param.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4041 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/collect_data.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11504 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/relabel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      764 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/run_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/stat_iter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/stat_sys.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5502 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/tools/stat_time.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-03-28 00:42:54.000000 dpgen-0.9.0/dpgen/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.809576 dpgen-0.9.0/dpgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    66034 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25450 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-03-28 00:43:38.000000 dpgen-0.9.0/dpgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/examples/database/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/database/param_Ti.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.837576 dpgen-0.9.0/examples/init/
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/CH4.POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/al.POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/al.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/al.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/ch4.json
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/ch4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      372 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/reaction.json
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/surf.json
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/init/surf.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/machine/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/
--rw-r--r--   0 runner    (1001) docker     (121)     5800 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-aws.json
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-local.json
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-lsf.json
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.json
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.json
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-ali.json
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-local.json
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-pbs-gaussian.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/machine/bk/
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/bk/machine-hnu.json
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/bk/machine-tiger-pwscf-della.json
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/bk/machine-tiger-vasp-della.json
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/bk/machine-tiger.json
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/machine/bk/machine-ucloud.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/run/bk/
--rw-r--r--   0 runner    (1001) docker     (121)    10838 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/bk/param-h2oscan-vasp.json
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/bk/param-mg-vasp-ucloud.json
--rw-r--r--   0 runner    (1001) docker     (121)     8201 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/bk/param-mg-vasp.json
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/bk/param-pyridine-pwscf.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/dp-lammps-cp2k/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/run/dp-lammps-cp2k/CH4/
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-cp2k/CH4/param_CH4.json
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-cp2k/CH4/param_CH4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/run/dp-lammps-pwmat/
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-pwmat/machine-slurm-pwmat-single.json
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-pwmat/param_CH4.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/dp-lammps-siesta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.841575 dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.json
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/dp-lammps-vasp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu-deepmd-kit-1.1.0.json
--rw-r--r--   0 runner    (1001) docker     (121)     9068 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.json
--rw-r--r--   0 runner    (1001) docker     (121)     7022 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/INCAR_methane
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/POT_C
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/POT_H
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4.json
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4_deepmd-kit-1.1.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/run/dp-lammps-vasp-et/
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp-lammps-vasp-et/param_elet.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.797576 dpgen-0.9.0/examples/run/dp_lammps_gaussian/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/run/dp_lammps_gaussian/dodecane/
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/run/dp_lammps_gaussian/dodecane/dodecane.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/simplify/
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/simplify/qm7.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/examples/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/test/deepmd_param.json
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/test/meam_param.json
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/test/vasp_param.json
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-03-28 00:42:54.000000 dpgen-0.9.0/examples/test/vasp_param_from_incar.json
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-03-28 00:42:54.000000 dpgen-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-28 00:43:38.929576 dpgen-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1954 2021-03-28 00:42:54.000000 dpgen-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.845576 dpgen-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/auto_test/confs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/confs/hp-Li/
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/confs/hp-Li/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/confs/mp-141/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/confs/mp-141/mp-141.cif
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/make_kp_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.000/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.000/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.000/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.001/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.001/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.002/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.002/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.002/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.003/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.003/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.003/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.004/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.004/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.004/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.005/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.005/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.005/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.849576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.006/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.006/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.006/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.007/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.007/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.007/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.008/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.008/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.008/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.009/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.009/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.009/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.010/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.010/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.010/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.011/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.011/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.011/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.012/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.012/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.012/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.013/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.013/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.013/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.014/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.014/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.014/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.015/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.015/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.015/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.016/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.016/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.016/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.017/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.017/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.017/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.018/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.018/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.018/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.853576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.019/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.019/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.019/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.020/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.020/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.020/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.021/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.021/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.021/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.022/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.022/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.022/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.023/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.023/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.023/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.024/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.024/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.024/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.025/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.025/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.025/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.026/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.026/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.026/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.857576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.027/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.027/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.027/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.028/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.028/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.028/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.029/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.029/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/test.029/kp.ref
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/auto_test/equi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/equi/lammps/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/lammps/Al-fcc.vasp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/equi/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)     7761 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/Al-fcc.json
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/CONTCAR
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/CONTCAR_Al_fcc
--rw-r--r--   0 runner    (1001) docker     (121)  1223831 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/mp-141.vasp
--rw-r--r--   0 runner    (1001) docker     (121)   132959 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/equi/vasp/outcar.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/lammps_input/
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/lammps_input/in.lammps_high
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_eos.py
--rw-r--r--   0 runner    (1001) docker     (121)     3596 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_make_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_mpdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3362 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_vacancy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_vasp_equi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_vasp_equi_std.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/test_vasp_kspacing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.873576 dpgen-0.9.0/tests/auto_test/vasp_input/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/vasp_input/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/vasp_input/INCAR.md
--rw-r--r--   0 runner    (1001) docker     (121)      484 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/vasp_input/INCAR.rlx
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/vasp_input/POTCAR
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/auto_test/vasp_input/POT_Al
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.877575 dpgen-0.9.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/INCAR_metal_rlx_low
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/POTCAR
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/al.json
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/alloy.json
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/context_bulk.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/context_surf.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/context_surf_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/data/out_data_02_md/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/data/out_data_02_md/02.md/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.877575 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/
--rw-r--r--   0 runner    (1001) docker     (121)    39103 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/OUTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.877575 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/
--rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/surf-100.POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      586 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/surf.json
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/surf_poscar.json
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/test_coll_vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/test_gen_bulk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/test_gen_surf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/test_gen_surf_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.877575 dpgen-0.9.0/tests/data/vasp.in/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/data/vasp.in/INCAR.rlx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.881576 dpgen-0.9.0/tests/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/context.py
--rw-r--r--   0 runner    (1001) docker     (121)  1413120 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/data.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)  2395367 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/init.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)   269213 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/iter.000000.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)      559 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/param_Al.json
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/database/test_db_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.885576 dpgen-0.9.0/tests/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.885576 dpgen-0.9.0/tests/dispatcher/lsf/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/lsf/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/lsf/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5928 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/lsf/test_lsf_local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.885576 dpgen-0.9.0/tests/dispatcher/pbs/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/pbs/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/pbs/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5767 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/pbs/test_pbs_local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.885576 dpgen-0.9.0/tests/dispatcher/shell/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/shell/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/shell/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     6851 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/shell/test_shell_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     6497 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/shell/test_shell_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.885576 dpgen-0.9.0/tests/dispatcher/slurm/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/test_dispatcher_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_ssh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/test_dispatcher_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    15449 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/test_local_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/test_local_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    10373 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/dispatcher/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/C.SG15.PBE.UPF
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/C.psf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/C_HSCV_PBE-1.0.UPF
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/H.SG15.PBE.UPF
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/H.psf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/H_HSCV_PBE-1.0.UPF
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/KNOWN_ISSUES
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/N.SG15.PBE.UPF
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/N.psf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/N_HSCV_PBE-1.0.UPF
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/POSCAR_Au_cluster
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/check_bad_box/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/check_bad_box/bad.height.POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/check_bad_box/bad.length.lammpstrj
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/check_bad_box/good.lammpstrj
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)    95736 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cluster/14400.lammpstrj
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cluster/cluster1.json
--rw-r--r--   0 runner    (1001) docker     (121)    63261 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cluster/input0_new.gaussianlog
--rw-r--r--   0 runner    (1001) docker     (121)     6112 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/comp_sys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/cp2k_basis_pp_file/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_basis_pp_file/BASIS_MOLOPT
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_basis_pp_file/GTH_POTENTIALS
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_basis_pp_file/dftd3.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/generator/cp2k_make_fp_files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/cp2k_make_fp_files/exinput/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_make_fp_files/exinput/template.inp
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_test_exref.inp
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/cp2k_test_ref.inp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.801576 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.897575 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/data/deepmd/
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      920 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/force.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/data/deepmd/set.000/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/set.000/box.npy
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/set.000/coord.npy
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/set.000/energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/set.000/force.npy
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/set.000/virial.npy
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/data/deepmd/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/lmp/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/lmp/input.lammps
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/lmp/input.plumed
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/machine-local-v1.json
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/machine-local.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/POTCAR
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/POTCAR.dbl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.000300K/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.000300K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.000300K/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.001000K/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.001000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.001000K/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.901576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.005000K/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.005000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.005000K/POSCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.010000K/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.010000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.010000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.010000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.020000K/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.020000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.020000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.020000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.040000K/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.040000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.040000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.040000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.080000K/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.080000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.080000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.080000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.160000K/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.160000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.160000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.160000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.240000K/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.240000K/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.240000K/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.240000K/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_nbands_esti/mgal/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/mgal/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/mgal/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_nbands_esti/mgal/POTCAR
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.905576 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/coord.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/input.inp
--rw-r--r--   0 runner    (1001) docker     (121)    71826 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.909576 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/orig/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.909576 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/info
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/input
--rw-r--r--   0 runner    (1001) docker     (121)    18377 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.909576 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/orig/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.909576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/OUT.MLMD
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/etot.input
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/info
--rwxr-xr-x   0 runner    (1001) docker     (121)   937024 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/poscar2config.x
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.913576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/OUT.MLMD
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/etot.input
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/info
--rwxr-xr-x   0 runner    (1001) docker     (121)   937024 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/poscar2config.x
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.913576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/type_map.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.913576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/info
--rw-r--r--   0 runner    (1001) docker     (121)     5782 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/input
--rw-r--r--   0 runner    (1001) docker     (121)    46235 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/info
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/input
--rw-r--r--   0 runner    (1001) docker     (121)    46235 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)    26401 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)    26939 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/info
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/input
--rw-r--r--   0 runner    (1001) docker     (121)    26683 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/output
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/box.raw
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/coord.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/energy.raw
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/force.raw
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/type.raw
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/orig/virial.raw
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)    39103 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.917576 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/
--rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/
--rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/
--rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/job.json
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mg-vasp-diy.json
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mg-vasp-old.json
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mg-vasp-v1-et.json
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mg-vasp-v1.json
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mg-vasp.json
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-mgo-cp2k-exinput.json
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-cp2k.json
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-gaussian.json
--rw-r--r--   0 runner    (1001) docker     (121)     4795 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-pwmat.json
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-pwscf-old.json
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-pwscf.json
--rw-r--r--   0 runner    (1001) docker     (121)     4443 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/param-pyridine-siesta.json
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_check_bad_box.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_check_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_concat_fp_vasp_pp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_make_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    29339 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_make_fp.py
--rw-r--r--   0 runner    (1001) docker     (121)    21392 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_make_md.py
--rw-r--r--   0 runner    (1001) docker     (121)    13398 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_make_train.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_nbands_esti.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_parse_cur_job.py
--rw-r--r--   0 runner    (1001) docker     (121)    10194 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/test_post_fp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/generator/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/INCAR.diy
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/POSCAR.ch4
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/POSCAR.oh
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/nbands_esti.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/generator/vasp/potcars/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/potcars/POTCAR.C
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/potcars/POTCAR.H
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/potcars/POTCAR.O
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/potcars/POTCAR.al
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/generator/vasp/potcars/POTCAR.mg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.805575 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.809576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.921576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.925576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 00:43:38.929576 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/input.lammps
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/run_report_test_output/param.json
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-03-28 00:42:54.000000 dpgen-0.9.0/tests/tools/test_run_report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.048391 dpgen-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.944388 dpgen-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.964389 dpgen-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-27 23:33:40.000000 dpgen-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-03-27 23:33:40.000000 dpgen-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-03-27 23:33:40.000000 dpgen-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    66034 2021-03-27 23:34:34.044391 dpgen-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    55746 2021-03-27 23:33:40.000000 dpgen-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.964389 dpgen-0.9.1/dpgen/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen/_date.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/auto_test/
+-rw-r--r--   0 runner    (1001) docker     (121)     9270 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/EOS.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10134 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Elastic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12729 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Interstitial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21493 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Property.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10211 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9363 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/VASP.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9507 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/Vacancy.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7240 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/common_equi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8982 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/common_prop.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4355 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/gen_confs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/auto_test/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)     3306 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/BatchJob.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19814 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/RemoteJob.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/SlurmJob.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2677 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/crys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17558 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5219 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/lmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/localhost.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)    45430 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/mfp_eosfit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4456 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/pwscf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/siesta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14835 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/lib/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/mpdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/refine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.948388 dpgen-0.9.1/dpgen/auto_test/template/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.948388 dpgen-0.9.1/dpgen/auto_test/template/elastic/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/displace.mod
+-rw-r--r--   0 runner    (1001) docker     (121)     8724 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/in.elastic
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/init.mod
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/potential.mod
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/auto_test/template/incars/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/incars/INCAR.relax
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/auto_test/template/incars/INCAR.static
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/collect/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4496 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/collect/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.968389 dpgen-0.9.1/dpgen/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25601 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.976389 dpgen-0.9.1/dpgen/data/jsons/
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.diamond.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.diamond.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.fcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.fcc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.hcp.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.hcp.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.hcp.332.json
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/al.sc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.diamond.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.diamond.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.fcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.fcc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.hcp.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.hcp.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.hcp.332.json
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.sc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/almg.sc.333.json
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.diamond.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.diamond.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.fcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.fcc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.hcp.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.hcp.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.hcp.332.json
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/mg.sc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/param.json
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.diamond.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.diamond.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.fcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.fcc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.hcp.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.hcp.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/si.sc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.al.fcc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.al.hcp.json
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.almg.fcc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.almg.hcp.json
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.mg.fcc.json
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.mg.hcp.json
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/surf.si.diamond.json
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/w.bcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/w.bcc.222.json
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/w.diamond.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/w.fcc.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/w.hcp.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/jsons/water.111.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7338 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21791 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/surf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.976389 dpgen-0.9.1/dpgen/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/bcc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12048 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/cessp2force_lin.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      255 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/clean.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8314 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/create_random_disturb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/diamond.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/hcp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7636 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/io_lammps.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1438 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/ovito_file_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1133 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/poscar_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/sc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)       96 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/data/tools/test.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.980389 dpgen-0.9.1/dpgen/database/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4191 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/database/entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5262 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/database/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6663 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/database/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.980389 dpgen-0.9.1/dpgen/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (121)    23016 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/ALI.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6307 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/AWS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6706 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/Batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14600 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/Dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13513 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/DispatcherList.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/JobStatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7311 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/LSF.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/LazyLocalContext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7226 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/LocalContext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5238 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/PBS.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10809 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/SSHContext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/Shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7693 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/Slurm.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/dispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.980389 dpgen-0.9.1/dpgen/generator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.980389 dpgen-0.9.1/dpgen/generator/ch4/
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/ch4/machine.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3580 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/ch4/param.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.980389 dpgen-0.9.1/dpgen/generator/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6244 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/cp2k.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/cvasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/ele_temp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10483 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5996 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/pwmat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8367 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/pwscf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/siesta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/lib/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96512 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7443 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/dpgen/remote/
+-rw-r--r--   0 runner    (1001) docker     (121)    35697 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/remote/RemoteJob.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13830 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/remote/decide_machine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18343 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/remote/group_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/remote/localhost.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/dpgen/simplify/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/simplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27485 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/simplify/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/dpgen/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10381 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/auto_gen_param.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4041 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/collect_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11504 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/relabel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      764 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/run_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/stat_iter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/stat_sys.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5502 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/tools/stat_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-03-27 23:33:40.000000 dpgen-0.9.1/dpgen/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.964389 dpgen-0.9.1/dpgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    66034 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    25450 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-03-27 23:34:33.000000 dpgen-0.9.1/dpgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/examples/database/
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/database/param_Ti.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/examples/init/
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/CH4.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/al.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/al.json
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/al.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/ch4.json
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/ch4.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/reaction.json
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/surf.json
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/init/surf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.952389 dpgen-0.9.1/examples/machine/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.984389 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/
+-rw-r--r--   0 runner    (1001) docker     (121)     5800 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-aws.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-local.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-lsf.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3273 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-ali.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-local.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2228 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-pbs-gaussian.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/machine/bk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/bk/machine-hnu.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1911 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/bk/machine-tiger-pwscf-della.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/bk/machine-tiger-vasp-della.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/bk/machine-tiger.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2623 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/machine/bk/machine-ucloud.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/run/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/bk/
+-rw-r--r--   0 runner    (1001) docker     (121)    10838 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/bk/param-h2oscan-vasp.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/bk/param-mg-vasp-ucloud.json
+-rw-r--r--   0 runner    (1001) docker     (121)     8201 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/bk/param-mg-vasp.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4589 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/bk/param-pyridine-pwscf.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.952389 dpgen-0.9.1/examples/run/dp-lammps-cp2k/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-cp2k/CH4/
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-cp2k/CH4/param_CH4.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-cp2k/CH4/param_CH4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-pwmat/
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-pwmat/machine-slurm-pwmat-single.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-pwmat/param_CH4.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/run/dp-lammps-siesta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/
+-rw-r--r--   0 runner    (1001) docker     (121)     3162 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/run/dp-lammps-vasp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/
+-rw-r--r--   0 runner    (1001) docker     (121)     8804 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu-deepmd-kit-1.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9068 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.json
+-rw-r--r--   0 runner    (1001) docker     (121)     7022 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/INCAR_methane
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/POT_C
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/POT_H
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3502 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4_deepmd-kit-1.1.0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp-lammps-vasp-et/
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp-lammps-vasp-et/param_elet.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/examples/run/dp_lammps_gaussian/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/run/dp_lammps_gaussian/dodecane/
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/run/dp_lammps_gaussian/dodecane/dodecane.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.988389 dpgen-0.9.1/examples/simplify/
+-rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/simplify/qm7.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/examples/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/test/deepmd_param.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/test/meam_param.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/test/vasp_param.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-03-27 23:33:40.000000 dpgen-0.9.1/examples/test/vasp_param_from_incar.json
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-03-27 23:33:40.000000 dpgen-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-27 23:34:34.048391 dpgen-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1954 2021-03-27 23:33:40.000000 dpgen-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/auto_test/confs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/confs/hp-Li/
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/confs/hp-Li/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/confs/mp-141/
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/confs/mp-141/mp-141.cif
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/make_kp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.000/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.000/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.001/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.001/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.002/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.002/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.002/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.992390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.003/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.003/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.003/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.004/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.004/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.004/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.005/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.005/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.005/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.006/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.006/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.006/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.007/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.007/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.007/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.008/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.008/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.008/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.009/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.009/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.009/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.010/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.010/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.010/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.011/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.011/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.011/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.012/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.012/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.012/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.013/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.013/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.013/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.014/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.014/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.014/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.015/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.015/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.015/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.016/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.016/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.016/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.017/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.017/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.017/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.018/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.018/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.018/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.996390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.019/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.019/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.019/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.020/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.020/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.020/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.021/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.021/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.021/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.022/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.022/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.022/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.023/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.023/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.023/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.024/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.024/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.024/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.025/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.025/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.025/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.026/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.026/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.026/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.027/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.027/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.027/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.028/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.028/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.028/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.029/
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.029/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/test.029/kp.ref
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/auto_test/equi/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.000390 dpgen-0.9.1/tests/auto_test/equi/lammps/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/lammps/Al-fcc.vasp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/auto_test/equi/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)     7761 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/Al-fcc.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4692 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/CONTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/CONTCAR_Al_fcc
+-rw-r--r--   0 runner    (1001) docker     (121)  1223831 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/mp-141.vasp
+-rw-r--r--   0 runner    (1001) docker     (121)   132959 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/equi/vasp/outcar.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/auto_test/lammps_input/
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/lammps_input/in.lammps_high
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3890 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_eos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3596 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3733 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_make_prop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_mpdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3738 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3948 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_vacancy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5584 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_vasp_equi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_vasp_equi_std.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/test_vasp_kspacing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/auto_test/vasp_input/
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/vasp_input/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/vasp_input/INCAR.md
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/vasp_input/INCAR.rlx
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/vasp_input/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/auto_test/vasp_input/POT_Al
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/INCAR_metal_rlx_low
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/al.json
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/alloy.json
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/context_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/context_surf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/context_surf_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/data/out_data_02_md/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/data/out_data_02_md/02.md/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/
+-rw-r--r--   0 runner    (1001) docker     (121)    39103 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/OUTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.004390 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/
+-rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/surf-100.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/surf.json
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/surf_poscar.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/test_coll_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/test_gen_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/test_gen_surf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/test_gen_surf_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.008390 dpgen-0.9.1/tests/data/vasp.in/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/data/vasp.in/INCAR.rlx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.012390 dpgen-0.9.1/tests/database/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1413120 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/data.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)  2395367 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/init.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)   269213 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/iter.000000.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/param_Al.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/database/test_db_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.012390 dpgen-0.9.1/tests/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.012390 dpgen-0.9.1/tests/dispatcher/lsf/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/lsf/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/lsf/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5928 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/lsf/test_lsf_local.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.012390 dpgen-0.9.1/tests/dispatcher/pbs/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/pbs/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/pbs/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5767 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/pbs/test_pbs_local.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.012390 dpgen-0.9.1/tests/dispatcher/shell/
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/shell/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/shell/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6851 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/shell/test_shell_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6497 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/shell/test_shell_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.016390 dpgen-0.9.1/tests/dispatcher/slurm/
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/test_dispatcher_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6197 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5840 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6102 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/test_dispatcher_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7583 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15449 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/test_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/test_local_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10373 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/dispatcher/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/C.SG15.PBE.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/C.psf
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/C_HSCV_PBE-1.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/H.SG15.PBE.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/H.psf
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/H_HSCV_PBE-1.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/KNOWN_ISSUES
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/N.SG15.PBE.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/N.psf
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/N_HSCV_PBE-1.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/POSCAR_Au_cluster
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/check_bad_box/
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/check_bad_box/bad.height.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/check_bad_box/bad.length.lammpstrj
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/check_bad_box/good.lammpstrj
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/cluster/
+-rw-r--r--   0 runner    (1001) docker     (121)    95736 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cluster/14400.lammpstrj
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cluster/cluster1.json
+-rw-r--r--   0 runner    (1001) docker     (121)    63261 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cluster/input0_new.gaussianlog
+-rw-r--r--   0 runner    (1001) docker     (121)     6112 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/comp_sys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/cp2k_basis_pp_file/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_basis_pp_file/BASIS_MOLOPT
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_basis_pp_file/GTH_POTENTIALS
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_basis_pp_file/dftd3.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.956389 dpgen-0.9.1/tests/generator/cp2k_make_fp_files/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/cp2k_make_fp_files/exinput/
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_make_fp_files/exinput/template.inp
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_test_exref.inp
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/cp2k_test_ref.inp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.020390 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/data/deepmd/
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/force.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/data/deepmd/set.000/
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/set.000/box.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/set.000/coord.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/set.000/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/set.000/force.npy
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/set.000/virial.npy
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/data/deepmd/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/lmp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/lmp/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/lmp/input.plumed
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/machine-local-v1.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/machine-local.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/POTCAR.dbl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.000300K/
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.000300K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.000300K/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.001000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.001000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.001000K/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.005000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.005000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.005000K/POSCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.010000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.010000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.010000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.010000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.020000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.020000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.020000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.020000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.024390 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.040000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.040000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.040000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.040000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.080000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.080000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.080000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.080000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.160000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.160000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.160000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.160000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.240000K/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.240000K/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.240000K/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.240000K/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_nbands_esti/mgal/
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/mgal/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/mgal/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_nbands_esti/mgal/POTCAR
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/coord.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/input.inp
+-rw-r--r--   0 runner    (1001) docker     (121)    71826 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/orig/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/info
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/input
+-rw-r--r--   0 runner    (1001) docker     (121)    18377 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/orig/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.028391 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/OUT.MLMD
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/etot.input
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/info
+-rwxr-xr-x   0 runner    (1001) docker     (121)   937024 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/poscar2config.x
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.032390 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/OUT.MLMD
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/etot.input
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/info
+-rwxr-xr-x   0 runner    (1001) docker     (121)   937024 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/poscar2config.x
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.032390 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/type_map.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.032390 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/info
+-rw-r--r--   0 runner    (1001) docker     (121)     5782 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/input
+-rw-r--r--   0 runner    (1001) docker     (121)    46235 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.032390 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/info
+-rw-r--r--   0 runner    (1001) docker     (121)     5786 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/input
+-rw-r--r--   0 runner    (1001) docker     (121)    46235 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    26401 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)    26939 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/info
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/input
+-rw-r--r--   0 runner    (1001) docker     (121)    26683 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/output
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/box.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/force.raw
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/type.raw
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/orig/virial.raw
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)    39103 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/job.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/job.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/job.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)    41068 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/job.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2444 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mg-vasp-diy.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mg-vasp-old.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mg-vasp-v1-et.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mg-vasp-v1.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mg-vasp.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4358 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-mgo-cp2k-exinput.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-cp2k.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4369 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-gaussian.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4795 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-pwmat.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-pwscf-old.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4852 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-pwscf.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4443 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/param-pyridine-siesta.json
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_check_bad_box.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_check_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1332 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2735 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_concat_fp_vasp_pp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_make_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29339 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_make_fp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21392 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_make_md.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13398 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_make_train.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3656 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_nbands_esti.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_parse_cur_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10194 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/test_post_fp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.036391 dpgen-0.9.1/tests/generator/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/INCAR.diy
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/POSCAR.ch4
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/POSCAR.oh
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/nbands_esti.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/generator/vasp/potcars/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/potcars/POTCAR.C
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/potcars/POTCAR.H
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/potcars/POTCAR.O
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/potcars/POTCAR.al
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/generator/vasp/potcars/POTCAR.mg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.960389 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:33.964389 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.040391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-27 23:34:34.044391 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (121)     2517 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/run_report_test_output/param.json
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2021-03-27 23:33:40.000000 dpgen-0.9.1/tests/tools/test_run_report.py
```

### Comparing `dpgen-0.9.0/.github/workflows/test.yml` & `dpgen-0.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/LICENSE` & `dpgen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/PKG-INFO` & `dpgen-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpgen
-Version: 0.9.0
+Version: 0.9.1
 Summary: DPGen: The deep potential generator
 Home-page: https://github.com/deepmodeling/dpgen
 Author: Han Wang
 Author-email: wang_han@iapcm.ac.cn
 License: UNKNOWN
 Description: # DP-GEN Manual
```

### Comparing `dpgen-0.9.0/README.md` & `dpgen-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/__init__.py` & `dpgen-0.9.1/dpgen/__init__.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/EOS.py` & `dpgen-0.9.1/dpgen/auto_test/EOS.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Elastic.py` & `dpgen-0.9.1/dpgen/auto_test/Elastic.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Interstitial.py` & `dpgen-0.9.1/dpgen/auto_test/Interstitial.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Lammps.py` & `dpgen-0.9.1/dpgen/auto_test/Lammps.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Property.py` & `dpgen-0.9.1/dpgen/auto_test/Property.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Surface.py` & `dpgen-0.9.1/dpgen/auto_test/Surface.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Task.py` & `dpgen-0.9.1/dpgen/auto_test/Task.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/VASP.py` & `dpgen-0.9.1/dpgen/auto_test/VASP.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/Vacancy.py` & `dpgen-0.9.1/dpgen/auto_test/Vacancy.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/calculator.py` & `dpgen-0.9.1/dpgen/auto_test/calculator.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/common_equi.py` & `dpgen-0.9.1/dpgen/auto_test/common_equi.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/common_prop.py` & `dpgen-0.9.1/dpgen/auto_test/common_prop.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/gen_confs.py` & `dpgen-0.9.1/dpgen/auto_test/gen_confs.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/BatchJob.py` & `dpgen-0.9.1/dpgen/auto_test/lib/BatchJob.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/RemoteJob.py` & `dpgen-0.9.1/dpgen/auto_test/lib/RemoteJob.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/SlurmJob.py` & `dpgen-0.9.1/dpgen/auto_test/lib/SlurmJob.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/crys.py` & `dpgen-0.9.1/dpgen/auto_test/lib/crys.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/lammps.py` & `dpgen-0.9.1/dpgen/auto_test/lib/lammps.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/lmp.py` & `dpgen-0.9.1/dpgen/auto_test/lib/lmp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/mfp_eosfit.py` & `dpgen-0.9.1/dpgen/auto_test/lib/mfp_eosfit.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/pwscf.py` & `dpgen-0.9.1/dpgen/auto_test/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/siesta.py` & `dpgen-0.9.1/dpgen/auto_test/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/util.py` & `dpgen-0.9.1/dpgen/auto_test/lib/util.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/utils.py` & `dpgen-0.9.1/dpgen/auto_test/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/lib/vasp.py` & `dpgen-0.9.1/dpgen/auto_test/lib/vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/mpdb.py` & `dpgen-0.9.1/dpgen/auto_test/mpdb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from dpgen import dlog
-from pymatgen import MPRester,Structure
-from pymatgen.ext.matproj import MPRestError 
+from pymatgen.ext.matproj import MPRester, MPRestError
+from pymatgen.core import Structure
 
 web="materials.org"
 
 def check_apikey():
     try:
       apikey=os.environ['MAPI_KEY']
     except KeyError:
```

### Comparing `dpgen-0.9.0/dpgen/auto_test/refine.py` & `dpgen-0.9.1/dpgen/auto_test/refine.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/reproduce.py` & `dpgen-0.9.1/dpgen/auto_test/reproduce.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/run.py` & `dpgen-0.9.1/dpgen/auto_test/run.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/displace.mod` & `dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/displace.mod`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/in.elastic` & `dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/in.elastic`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/init.mod` & `dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/init.mod`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/auto_test/template/elastic/lmp/potential.mod` & `dpgen-0.9.1/dpgen/auto_test/template/elastic/lmp/potential.mod`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/collect/collect.py` & `dpgen-0.9.1/dpgen/collect/collect.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/gen.py` & `dpgen-0.9.1/dpgen/data/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import subprocess as sp
 import dpgen.data.tools.hcp as hcp
 import dpgen.data.tools.fcc as fcc
 import dpgen.data.tools.bcc as bcc
 import dpgen.data.tools.diamond as diamond
 import dpgen.data.tools.sc as sc
 from dpgen.generator.lib.vasp import incar_upper
-from pymatgen import Structure
+from pymatgen.core import Structure
 from pymatgen.io.vasp import Incar
 from dpgen.remote.decide_machine import  decide_fp_machine
 from dpgen import ROOT_PATH
 from dpgen.dispatcher.Dispatcher import Dispatcher, make_dispatcher
```

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.diamond.111.json` & `dpgen-0.9.1/dpgen/data/jsons/al.diamond.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.diamond.222.json` & `dpgen-0.9.1/dpgen/data/jsons/al.diamond.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.fcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/al.fcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.fcc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/al.fcc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.hcp.111.json` & `dpgen-0.9.1/dpgen/data/jsons/al.hcp.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.hcp.222.json` & `dpgen-0.9.1/dpgen/data/jsons/al.hcp.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.hcp.332.json` & `dpgen-0.9.1/dpgen/data/jsons/al.hcp.332.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/al.sc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/al.sc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.diamond.111.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.diamond.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.diamond.222.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.diamond.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.fcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.fcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.fcc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.fcc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.hcp.111.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.hcp.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.hcp.222.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.hcp.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.hcp.332.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.hcp.332.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.sc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.sc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/almg.sc.333.json` & `dpgen-0.9.1/dpgen/data/jsons/almg.sc.333.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.diamond.111.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.diamond.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.diamond.222.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.diamond.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.fcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.fcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.fcc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.fcc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.hcp.111.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.hcp.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/mg.sc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/mg.sc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/param.json` & `dpgen-0.9.1/dpgen/data/jsons/param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.diamond.111.json` & `dpgen-0.9.1/dpgen/data/jsons/si.diamond.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.diamond.222.json` & `dpgen-0.9.1/dpgen/data/jsons/si.diamond.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.fcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/si.fcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.fcc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/si.fcc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.hcp.111.json` & `dpgen-0.9.1/dpgen/data/jsons/si.hcp.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.hcp.222.json` & `dpgen-0.9.1/dpgen/data/jsons/si.hcp.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/si.sc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/si.sc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.al.fcc.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.al.fcc.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.al.hcp.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.al.hcp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.almg.fcc.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.almg.fcc.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.almg.hcp.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.almg.hcp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.mg.fcc.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.mg.fcc.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.mg.hcp.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.mg.hcp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/surf.si.diamond.json` & `dpgen-0.9.1/dpgen/data/jsons/surf.si.diamond.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/w.bcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/w.bcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/w.bcc.222.json` & `dpgen-0.9.1/dpgen/data/jsons/w.bcc.222.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/w.diamond.111.json` & `dpgen-0.9.1/dpgen/data/jsons/w.diamond.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/w.fcc.111.json` & `dpgen-0.9.1/dpgen/data/jsons/w.fcc.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/w.hcp.111.json` & `dpgen-0.9.1/dpgen/data/jsons/w.hcp.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/jsons/water.111.json` & `dpgen-0.9.1/dpgen/data/jsons/water.111.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/reaction.py` & `dpgen-0.9.1/dpgen/data/reaction.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/surf.py` & `dpgen-0.9.1/dpgen/data/surf.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import dpgen.data.tools.bcc as bcc
 from dpgen import dlog
 from dpgen import ROOT_PATH
 from dpgen.remote.decide_machine import  decide_fp_machine
 from dpgen.dispatcher.Dispatcher import Dispatcher, make_dispatcher
 #-----PMG---------
 from pymatgen.io.vasp import Poscar
-from pymatgen import Structure,Element
+from pymatgen.core import Structure, Element
 from pymatgen.io.ase import AseAtomsAdaptor
 #-----ASE-------
 from ase.io import read
 from ase.build import general_surface
 
 
 def create_path (path) :
```

### Comparing `dpgen-0.9.0/dpgen/data/tools/bcc.py` & `dpgen-0.9.1/dpgen/data/tools/bcc.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/cessp2force_lin.py` & `dpgen-0.9.1/dpgen/data/tools/cessp2force_lin.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/create_random_disturb.py` & `dpgen-0.9.1/dpgen/data/tools/create_random_disturb.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/diamond.py` & `dpgen-0.9.1/dpgen/data/tools/diamond.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/fcc.py` & `dpgen-0.9.1/dpgen/data/tools/fcc.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/hcp.py` & `dpgen-0.9.1/dpgen/data/tools/hcp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/io_lammps.py` & `dpgen-0.9.1/dpgen/data/tools/io_lammps.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/ovito_file_convert.py` & `dpgen-0.9.1/dpgen/data/tools/ovito_file_convert.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/poscar_copy.py` & `dpgen-0.9.1/dpgen/data/tools/poscar_copy.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/data/tools/sc.py` & `dpgen-0.9.1/dpgen/data/tools/sc.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/database/entry.py` & `dpgen-0.9.1/dpgen/database/entry.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/database/run.py` & `dpgen-0.9.1/dpgen/database/run.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/database/vasp.py` & `dpgen-0.9.1/dpgen/database/vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/ALI.py` & `dpgen-0.9.1/dpgen/dispatcher/ALI.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/AWS.py` & `dpgen-0.9.1/dpgen/dispatcher/AWS.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/Batch.py` & `dpgen-0.9.1/dpgen/dispatcher/Batch.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/Dispatcher.py` & `dpgen-0.9.1/dpgen/dispatcher/Dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/DispatcherList.py` & `dpgen-0.9.1/dpgen/dispatcher/DispatcherList.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/LSF.py` & `dpgen-0.9.1/dpgen/dispatcher/LSF.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     
     def check_status(self):
         try:
             job_id = self._get_job_id()
         except:
             return JobStatus.terminated
         if job_id == "" :
-            raise RuntimeError("job %s is has not been submitted" % self.remote_root)
+            raise RuntimeError("job %s has not been submitted" % self.context.remote_root)
         ret, stdin, stdout, stderr\
             = self.context.block_call ("bjobs " + job_id)
         err_str = stderr.read().decode('utf-8')
         if ("Job <%s> is not found" % job_id) in err_str :
             if self.check_finish_tag() :
                 return JobStatus.finished
             else :
```

### Comparing `dpgen-0.9.0/dpgen/dispatcher/LazyLocalContext.py` & `dpgen-0.9.1/dpgen/dispatcher/LazyLocalContext.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/LocalContext.py` & `dpgen-0.9.1/dpgen/dispatcher/LocalContext.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/PBS.py` & `dpgen-0.9.1/dpgen/dispatcher/PBS.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/SSHContext.py` & `dpgen-0.9.1/dpgen/dispatcher/SSHContext.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/Shell.py` & `dpgen-0.9.1/dpgen/dispatcher/Shell.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/dispatcher/Slurm.py` & `dpgen-0.9.1/dpgen/dispatcher/Slurm.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/ch4/machine.json` & `dpgen-0.9.1/dpgen/generator/ch4/machine.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/ch4/param.json` & `dpgen-0.9.1/dpgen/generator/ch4/param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/cp2k.py` & `dpgen-0.9.1/dpgen/generator/lib/cp2k.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/cvasp.py` & `dpgen-0.9.1/dpgen/generator/lib/cvasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/ele_temp.py` & `dpgen-0.9.1/dpgen/generator/lib/ele_temp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/gaussian.py` & `dpgen-0.9.1/dpgen/generator/lib/gaussian.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/lammps.py` & `dpgen-0.9.1/dpgen/generator/lib/lammps.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/pwmat.py` & `dpgen-0.9.1/dpgen/generator/lib/pwmat.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/pwscf.py` & `dpgen-0.9.1/dpgen/generator/lib/pwscf.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/siesta.py` & `dpgen-0.9.1/dpgen/generator/lib/siesta.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/utils.py` & `dpgen-0.9.1/dpgen/generator/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/lib/vasp.py` & `dpgen-0.9.1/dpgen/generator/lib/vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/generator/run.py` & `dpgen-0.9.1/dpgen/generator/run.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/main.py` & `dpgen-0.9.1/dpgen/main.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/remote/RemoteJob.py` & `dpgen-0.9.1/dpgen/remote/RemoteJob.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/remote/decide_machine.py` & `dpgen-0.9.1/dpgen/remote/decide_machine.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/remote/group_jobs.py` & `dpgen-0.9.1/dpgen/remote/group_jobs.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/simplify/simplify.py` & `dpgen-0.9.1/dpgen/simplify/simplify.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/auto_gen_param.py` & `dpgen-0.9.1/dpgen/tools/auto_gen_param.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/collect_data.py` & `dpgen-0.9.1/dpgen/tools/collect_data.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/relabel.py` & `dpgen-0.9.1/dpgen/tools/relabel.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/run_report.py` & `dpgen-0.9.1/dpgen/tools/run_report.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/stat_iter.py` & `dpgen-0.9.1/dpgen/tools/stat_iter.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/stat_sys.py` & `dpgen-0.9.1/dpgen/tools/stat_sys.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/tools/stat_time.py` & `dpgen-0.9.1/dpgen/tools/stat_time.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen/util.py` & `dpgen-0.9.1/dpgen/util.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/dpgen.egg-info/PKG-INFO` & `dpgen-0.9.1/dpgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpgen
-Version: 0.9.0
+Version: 0.9.1
 Summary: DPGen: The deep potential generator
 Home-page: https://github.com/deepmodeling/dpgen
 Author: Han Wang
 Author-email: wang_han@iapcm.ac.cn
 License: UNKNOWN
 Description: # DP-GEN Manual
```

### Comparing `dpgen-0.9.0/dpgen.egg-info/SOURCES.txt` & `dpgen-0.9.1/dpgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/database/param_Ti.json` & `dpgen-0.9.1/examples/database/param_Ti.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/init/CH4.POSCAR` & `dpgen-0.9.1/examples/init/CH4.POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/init/al.json` & `dpgen-0.9.1/examples/init/al.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/init/surf.json` & `dpgen-0.9.1/examples/init/surf.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-aws.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-aws.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-local.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-local.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-lsf.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-lsf.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.yaml` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-multi.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.yaml` & `dpgen-0.9.1/examples/machine/DeePMD-kit-0.12/machine-slurm-vasp-single.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-ali.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-ali.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-local.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-local.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/DeePMD-kit-1.0/machine-pbs-gaussian.json` & `dpgen-0.9.1/examples/machine/DeePMD-kit-1.0/machine-pbs-gaussian.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/bk/machine-hnu.json` & `dpgen-0.9.1/examples/machine/bk/machine-hnu.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/bk/machine-tiger-pwscf-della.json` & `dpgen-0.9.1/examples/machine/bk/machine-tiger-pwscf-della.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/bk/machine-tiger-vasp-della.json` & `dpgen-0.9.1/examples/machine/bk/machine-tiger-vasp-della.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/bk/machine-tiger.json` & `dpgen-0.9.1/examples/machine/bk/machine-tiger.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/machine/bk/machine-ucloud.json` & `dpgen-0.9.1/examples/machine/bk/machine-ucloud.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/bk/param-h2oscan-vasp.json` & `dpgen-0.9.1/examples/run/bk/param-h2oscan-vasp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/bk/param-mg-vasp-ucloud.json` & `dpgen-0.9.1/examples/run/bk/param-mg-vasp-ucloud.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/bk/param-mg-vasp.json` & `dpgen-0.9.1/examples/run/bk/param-mg-vasp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/bk/param-pyridine-pwscf.json` & `dpgen-0.9.1/examples/run/bk/param-pyridine-pwscf.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-cp2k/CH4/param_CH4.json` & `dpgen-0.9.1/examples/run/dp-lammps-cp2k/CH4/param_CH4.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-cp2k/CH4/param_CH4.yaml` & `dpgen-0.9.1/examples/run/dp-lammps-cp2k/CH4/param_CH4.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-pwmat/machine-slurm-pwmat-single.json` & `dpgen-0.9.1/examples/run/dp-lammps-pwmat/machine-slurm-pwmat-single.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-pwmat/param_CH4.json` & `dpgen-0.9.1/examples/run/dp-lammps-pwmat/param_CH4.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.json` & `dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.yaml` & `dpgen-0.9.1/examples/run/dp-lammps-siesta/dp-lammps-siesta/CH4/param_CH4.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu-deepmd-kit-1.1.0.json` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu-deepmd-kit-1.1.0.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.json` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.yaml` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/Al/param_al_all_gpu.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4.json` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4.yaml` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4.yaml`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp/CH4/param_CH4_deepmd-kit-1.1.0.json` & `dpgen-0.9.1/examples/run/dp-lammps-vasp/CH4/param_CH4_deepmd-kit-1.1.0.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp-lammps-vasp-et/param_elet.json` & `dpgen-0.9.1/examples/run/dp-lammps-vasp-et/param_elet.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/run/dp_lammps_gaussian/dodecane/dodecane.json` & `dpgen-0.9.1/examples/run/dp_lammps_gaussian/dodecane/dodecane.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/simplify/qm7.json` & `dpgen-0.9.1/examples/simplify/qm7.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/test/deepmd_param.json` & `dpgen-0.9.1/examples/test/deepmd_param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/test/meam_param.json` & `dpgen-0.9.1/examples/test/meam_param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/test/vasp_param.json` & `dpgen-0.9.1/examples/test/vasp_param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/examples/test/vasp_param_from_incar.json` & `dpgen-0.9.1/examples/test/vasp_param_from_incar.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/setup.py` & `dpgen-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/confs/hp-Li/POSCAR` & `dpgen-0.9.1/tests/auto_test/confs/hp-Li/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/confs/mp-141/mp-141.cif` & `dpgen-0.9.1/tests/auto_test/confs/mp-141/mp-141.cif`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/data.vasp.kp.gf/make_kp_test.py` & `dpgen-0.9.1/tests/auto_test/data.vasp.kp.gf/make_kp_test.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/equi/vasp/Al-fcc.json` & `dpgen-0.9.1/tests/auto_test/equi/vasp/Al-fcc.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/equi/vasp/CONTCAR` & `dpgen-0.9.1/tests/auto_test/equi/vasp/CONTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/equi/vasp/OUTCAR` & `dpgen-0.9.1/tests/auto_test/equi/vasp/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/equi/vasp/outcar.json` & `dpgen-0.9.1/tests/auto_test/equi/vasp/outcar.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/lammps_input/in.lammps_high` & `dpgen-0.9.1/tests/auto_test/lammps_input/in.lammps_high`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_elastic.py` & `dpgen-0.9.1/tests/auto_test/test_elastic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, sys, json, glob, shutil
 import dpdata
 import numpy as np
 import unittest
 import dpdata
 from monty.serialization import loadfn, dumpfn
 from pymatgen.analysis.elasticity.strain import Strain, Deformation
-from pymatgen import Structure
+from pymatgen.core import Structure
 from pymatgen.io.vasp import Incar
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'auto_test'
 
 from .context import make_kspacing_kpoints
 from .context import setUpModule
```

### Comparing `dpgen-0.9.0/tests/auto_test/test_eos.py` & `dpgen-0.9.1/tests/auto_test/test_eos.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_lammps.py` & `dpgen-0.9.1/tests/auto_test/test_lammps.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_make_prop.py` & `dpgen-0.9.1/tests/auto_test/test_make_prop.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_mpdb.py` & `dpgen-0.9.1/tests/auto_test/test_mpdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 import unittest
-from pymatgen import Structure
+from pymatgen.core import Structure
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from monty.serialization import loadfn,dumpfn
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'auto_test'
 from .context import make_kspacing_kpoints
 from .context import setUpModule
```

### Comparing `dpgen-0.9.0/tests/auto_test/test_refine.py` & `dpgen-0.9.1/tests/auto_test/test_refine.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_surface.py` & `dpgen-0.9.1/tests/auto_test/test_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys, json, glob, shutil
 import dpdata
 import numpy as np
 import unittest
 import dpdata
 from monty.serialization import loadfn, dumpfn
-from pymatgen import Structure
+from pymatgen.core import Structure
 from pymatgen.io.vasp import Incar
 from pymatgen.core.surface import SlabGenerator
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'auto_test'
 
 from .context import make_kspacing_kpoints
```

### Comparing `dpgen-0.9.0/tests/auto_test/test_vacancy.py` & `dpgen-0.9.1/tests/auto_test/test_vacancy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys, json, glob, shutil
 import dpdata
 import numpy as np
 import unittest
 import dpdata
 from monty.serialization import loadfn, dumpfn
-from pymatgen import Structure
+from pymatgen.core import Structure
 from pymatgen.io.vasp import Incar
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.analysis.defects.core import Vacancy as pmg_Vacancy
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'auto_test'
```

### Comparing `dpgen-0.9.0/tests/auto_test/test_vasp.py` & `dpgen-0.9.1/tests/auto_test/test_vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_vasp_equi.py` & `dpgen-0.9.1/tests/auto_test/test_vasp_equi.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_vasp_equi_std.py` & `dpgen-0.9.1/tests/auto_test/test_vasp_equi_std.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/test_vasp_kspacing.py` & `dpgen-0.9.1/tests/auto_test/test_vasp_kspacing.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/auto_test/vasp_input/INCAR.md` & `dpgen-0.9.1/tests/auto_test/vasp_input/INCAR.md`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/OUTCAR` & `dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000000/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/OUTCAR` & `dpgen-0.9.1/tests/data/out_data_02_md/02.md/sys-004/scale-1.000/000001/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/surf-100.POSCAR` & `dpgen-0.9.1/tests/data/surf-100.POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/surf.json` & `dpgen-0.9.1/tests/data/surf.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/surf_poscar.json` & `dpgen-0.9.1/tests/data/surf_poscar.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/test_coll_vasp.py` & `dpgen-0.9.1/tests/data/test_coll_vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/data/test_gen_bulk.py` & `dpgen-0.9.1/tests/data/test_gen_bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os,sys,json,glob,shutil
 import unittest
-from pymatgen import Structure,Composition
+from pymatgen.core import Structure, Composition
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'data'
 from .context import setUpModule
 from .context_bulk import *
 
 class TestGenBulk(unittest.TestCase):
```

### Comparing `dpgen-0.9.0/tests/data/test_gen_surf.py` & `dpgen-0.9.1/tests/data/test_gen_surf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os,sys,json,glob,shutil
 import unittest
-from pymatgen import Structure,Element
+from pymatgen.core import Structure, Element
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'data'
 from .context import setUpModule
 from .context_surf import *
 
 class TestGenSurf(unittest.TestCase):
```

### Comparing `dpgen-0.9.0/tests/data/test_gen_surf_poscar.py` & `dpgen-0.9.1/tests/data/test_gen_surf_poscar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os,sys,json,glob,shutil
 import unittest
-from pymatgen import Structure,Element
+from pymatgen.core import Structure, Element
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 __package__ = 'data'
 from .context import setUpModule
 from .context_surf_poscar import *
 
 class TestGenSurfPOSCAR(unittest.TestCase):
```

### Comparing `dpgen-0.9.0/tests/database/data.tar.gz` & `dpgen-0.9.1/tests/database/data.tar.gz`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/database/init.tar.gz` & `dpgen-0.9.1/tests/database/init.tar.gz`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/database/iter.000000.tar.gz` & `dpgen-0.9.1/tests/database/iter.000000.tar.gz`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/database/param_Al.json` & `dpgen-0.9.1/tests/database/param_Al.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/database/test_db_vasp.py` & `dpgen-0.9.1/tests/database/test_db_vasp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/context.py` & `dpgen-0.9.1/tests/dispatcher/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/lsf/context.py` & `dpgen-0.9.1/tests/dispatcher/lsf/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/lsf/test_dispatcher.py` & `dpgen-0.9.1/tests/dispatcher/lsf/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/lsf/test_lsf_local.py` & `dpgen-0.9.1/tests/dispatcher/lsf/test_lsf_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/pbs/context.py` & `dpgen-0.9.1/tests/dispatcher/pbs/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/pbs/test_dispatcher.py` & `dpgen-0.9.1/tests/dispatcher/pbs/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/pbs/test_pbs_local.py` & `dpgen-0.9.1/tests/dispatcher/pbs/test_pbs_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/shell/context.py` & `dpgen-0.9.1/tests/dispatcher/shell/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/shell/test_dispatcher.py` & `dpgen-0.9.1/tests/dispatcher/shell/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/shell/test_shell_local.py` & `dpgen-0.9.1/tests/dispatcher/shell/test_shell_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/shell/test_shell_ssh.py` & `dpgen-0.9.1/tests/dispatcher/shell/test_shell_ssh.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/context.py` & `dpgen-0.9.1/tests/dispatcher/slurm/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/test_dispatcher.py` & `dpgen-0.9.1/tests/dispatcher/slurm/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/test_dispatcher_lazy_local.py` & `dpgen-0.9.1/tests/dispatcher/slurm/test_dispatcher_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_lazy_local.py` & `dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_local.py` & `dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_local.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/slurm/test_slurm_ssh.py` & `dpgen-0.9.1/tests/dispatcher/slurm/test_slurm_ssh.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/test_dispatcher_utils.py` & `dpgen-0.9.1/tests/dispatcher/test_dispatcher_utils.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/test_lazy_local_context.py` & `dpgen-0.9.1/tests/dispatcher/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/test_local_context.py` & `dpgen-0.9.1/tests/dispatcher/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/dispatcher/test_ssh_context.py` & `dpgen-0.9.1/tests/dispatcher/test_ssh_context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/POSCAR_Au_cluster` & `dpgen-0.9.1/tests/generator/POSCAR_Au_cluster`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/check_bad_box/bad.height.POSCAR` & `dpgen-0.9.1/tests/generator/check_bad_box/bad.height.POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/check_bad_box/bad.length.lammpstrj` & `dpgen-0.9.1/tests/generator/check_bad_box/bad.length.lammpstrj`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/check_bad_box/good.lammpstrj` & `dpgen-0.9.1/tests/generator/check_bad_box/good.lammpstrj`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cluster/14400.lammpstrj` & `dpgen-0.9.1/tests/generator/cluster/14400.lammpstrj`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cluster/cluster1.json` & `dpgen-0.9.1/tests/generator/cluster/cluster1.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cluster/input0_new.gaussianlog` & `dpgen-0.9.1/tests/generator/cluster/input0_new.gaussianlog`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/comp_sys.py` & `dpgen-0.9.1/tests/generator/comp_sys.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/context.py` & `dpgen-0.9.1/tests/generator/context.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cp2k_make_fp_files/exinput/template.inp` & `dpgen-0.9.1/tests/generator/cp2k_make_fp_files/exinput/template.inp`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cp2k_test_exref.inp` & `dpgen-0.9.1/tests/generator/cp2k_test_exref.inp`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/cp2k_test_ref.inp` & `dpgen-0.9.1/tests/generator/cp2k_test_ref.inp`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000000/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000001/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.040/000002/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000000/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000001/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/POSCAR` & `dpgen-0.9.1/tests/generator/data/al.fcc.02x02x02/01.scale_pert/sys-0032/scale-1.060/000002/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/deepmd/box.raw` & `dpgen-0.9.1/tests/generator/data/deepmd/box.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/deepmd/coord.raw` & `dpgen-0.9.1/tests/generator/data/deepmd/coord.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/deepmd/force.raw` & `dpgen-0.9.1/tests/generator/data/deepmd/force.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/data/deepmd/virial.raw` & `dpgen-0.9.1/tests/generator/data/deepmd/virial.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/lmp/input.lammps` & `dpgen-0.9.1/tests/generator/lmp/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/machine-local-v1.json` & `dpgen-0.9.1/tests/generator/machine-local-v1.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/machine-local.json` & `dpgen-0.9.1/tests/generator/machine-local.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.000300K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.000300K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.001000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.001000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.005000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.005000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.010000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.010000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.020000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.020000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.040000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.040000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.080000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.080000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.160000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.160000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/md.240000K/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/md.240000K/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_nbands_esti/mgal/POSCAR` & `dpgen-0.9.1/tests/generator/out_data_nbands_esti/mgal/POSCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/input.inp` & `dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/input.inp`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/output` & `dpgen-0.9.1/tests/generator/out_data_post_fp_cp2k/02.fp/task.000.000000/output`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/output` & `dpgen-0.9.1/tests/generator/out_data_post_fp_gaussian/02.fp/task.000.000000/output`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/OUT.MLMD` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/OUT.MLMD`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/poscar2config.x` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000000/poscar2config.x`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/OUT.MLMD` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/OUT.MLMD`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/poscar2config.x` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/02.fp/task.000.000001/poscar2config.x`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwmat/orig/coord.raw` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwmat/orig/coord.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/input` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/input`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/output` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000000/output`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/input` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/input`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/output` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/02.fp/task.000.000001/output`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/coord.raw` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/coord.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_pwscf/orig/force.raw` & `dpgen-0.9.1/tests/generator/out_data_post_fp_pwscf/orig/force.raw`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/input` & `dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/input`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/output` & `dpgen-0.9.1/tests/generator/out_data_post_fp_siesta/02.fp/task.000.000000/output`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/OUTCAR` & `dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000000/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/OUTCAR` & `dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.000.000001/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/OUTCAR` & `dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000000/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/OUTCAR` & `dpgen-0.9.1/tests/generator/out_data_post_fp_vasp/02.fp/task.001.000001/OUTCAR`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mg-vasp-diy.json` & `dpgen-0.9.1/tests/generator/param-mg-vasp-diy.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mg-vasp-old.json` & `dpgen-0.9.1/tests/generator/param-mg-vasp-old.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mg-vasp-v1-et.json` & `dpgen-0.9.1/tests/generator/param-mg-vasp-v1-et.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mg-vasp-v1.json` & `dpgen-0.9.1/tests/generator/param-mg-vasp-v1.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mg-vasp.json` & `dpgen-0.9.1/tests/generator/param-mg-vasp.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-mgo-cp2k-exinput.json` & `dpgen-0.9.1/tests/generator/param-mgo-cp2k-exinput.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-cp2k.json` & `dpgen-0.9.1/tests/generator/param-pyridine-cp2k.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-gaussian.json` & `dpgen-0.9.1/tests/generator/param-pyridine-gaussian.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-pwmat.json` & `dpgen-0.9.1/tests/generator/param-pyridine-pwmat.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-pwscf-old.json` & `dpgen-0.9.1/tests/generator/param-pyridine-pwscf-old.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-pwscf.json` & `dpgen-0.9.1/tests/generator/param-pyridine-pwscf.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/param-pyridine-siesta.json` & `dpgen-0.9.1/tests/generator/param-pyridine-siesta.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_check_bad_box.py` & `dpgen-0.9.1/tests/generator/test_check_bad_box.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_check_cluster.py` & `dpgen-0.9.1/tests/generator/test_check_cluster.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_cluster.py` & `dpgen-0.9.1/tests/generator/test_cluster.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_concat_fp_vasp_pp.py` & `dpgen-0.9.1/tests/generator/test_concat_fp_vasp_pp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_make_dispatcher.py` & `dpgen-0.9.1/tests/generator/test_make_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_make_fp.py` & `dpgen-0.9.1/tests/generator/test_make_fp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_make_md.py` & `dpgen-0.9.1/tests/generator/test_make_md.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_make_train.py` & `dpgen-0.9.1/tests/generator/test_make_train.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_nbands_esti.py` & `dpgen-0.9.1/tests/generator/test_nbands_esti.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_parse_cur_job.py` & `dpgen-0.9.1/tests/generator/test_parse_cur_job.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/generator/test_post_fp.py` & `dpgen-0.9.1/tests/generator/test_post_fp.py`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000000/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000001/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000002/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000003/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000004/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000005/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000006/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000007/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000008/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000009/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000010/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000011/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000012/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000013/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000014/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000015/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000016/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000017/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000018/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.000.000019/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000000/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000001/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000002/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000003/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000004/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000005/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000006/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000007/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000008/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000009/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000010/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000011/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000012/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000013/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000014/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000015/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000016/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000017/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000018/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/input.lammps` & `dpgen-0.9.1/tests/tools/run_report_test_output/iter.000000/01.model_devi/task.001.000019/input.lammps`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/run_report_test_output/param.json` & `dpgen-0.9.1/tests/tools/run_report_test_output/param.json`

 * *Files identical despite different names*

### Comparing `dpgen-0.9.0/tests/tools/test_run_report.py` & `dpgen-0.9.1/tests/tools/test_run_report.py`

 * *Files identical despite different names*

