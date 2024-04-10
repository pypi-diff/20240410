# Comparing `tmp/sts_libs-0.1.6rc0.tar.gz` & `tmp/sts_libs-0.1.7.tar.gz`

## Comparing `sts_libs-0.1.6rc0.tar` & `sts_libs-0.1.7.tar`

### file list

```diff
@@ -1,87 +1,98 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/noxfile.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/.fmf/version
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/docs/contributing.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/main.fmf
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/be2iscsi.fmf
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/bnx2i.fmf
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/cxgb4i.fmf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/local.fmf
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/qedi.fmf
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/tier0.fmf
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/plans/iscsi/libiscsi/main.fmf
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/scripts/install-python.sh
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/fixtures.py
--rw-r--r--   0        0        0    52285 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    38610 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    73771 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    41777 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/rdma.py
--rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17006 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22417 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/log.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/conftest.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/pytest.ini
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/main.fmf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/_vars/be2iscsi.yaml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/_vars/bnx2i.yaml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/_vars/cxgb4i.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/_vars/qedi.yaml
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/_vars/template_iscsi_host.yaml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/libiscsi/main.fmf
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/libiscsi/local/libiscsi-local.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/libiscsi/local/main.fmf
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/login-logout-stress/login-logout-stress.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/login-logout-stress/main.fmf
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/many-luns/main.fmf
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/many-luns/many-luns-local.py
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/parameters/iscsi_params.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/iscsi/parameters/main.fmf
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/rdma/main.fmf
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/rdma/bugs/main.fmf
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/rdma/bugs/customers/main.fmf
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/rdma/bugs/customers/issue_23967/issue_23967_verify_speed.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/tests/rdma/bugs/customers/issue_23967/main.fmf
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/LICENSE
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/pyproject.toml
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/sts_libs/README.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 sts_libs-0.1.6rc0/PKG-INFO
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sts_libs-0.1.7/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.1.7/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.fmf/version
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 sts_libs-0.1.7/docs/contributing.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/main.fmf
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/be2iscsi.fmf
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/bnx2i.fmf
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/cxgb4i.fmf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/local.fmf
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/qedi.fmf
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/tier0.fmf
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/main.fmf
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/regression.fmf
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/test_case_vars.yaml
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 sts_libs-0.1.7/scripts/install-python.sh
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    52285 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    38610 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    73771 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    41777 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/rdma.py
+-rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17006 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22417 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/iscsi_fixtures.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/rdma_fixtures.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/pytest.ini
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/main.fmf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/be2iscsi.yaml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/bnx2i.yaml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/cxgb4i.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/qedi.yaml
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/template_iscsi_host.yaml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/local/libiscsi-local.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/local/main.fmf
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/login-logout-stress/login-logout-stress.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/login-logout-stress/main.fmf
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/many-luns/main.fmf
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/many-luns/many-luns-local.py
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/parameters/iscsi_params.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/parameters/main.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/main.fmf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/main.fmf
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/main.fmf
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/customer_1/issue_23967_verify_speed.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/customer_1/main.fmf
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/others/main.fmf
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/others/reproducers.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/pyverbs-tests/core/main.fmf
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/pyverbs-tests/core/pyverbs-tests.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/sriov/core/main.fmf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/sriov/core/sriov.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 sts_libs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/README.md
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 sts_libs-0.1.7/PKG-INFO
```

### Comparing `sts_libs-0.1.6rc0/.pre-commit-config.yaml` & `sts_libs-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/README.md` & `sts_libs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/noxfile.py` & `sts_libs-0.1.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/docs/contributing.md` & `sts_libs-0.1.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/dm.py` & `sts_libs-0.1.7/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/dmpd.py` & `sts_libs-0.1.7/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/fc.py` & `sts_libs-0.1.7/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/fio.py` & `sts_libs-0.1.7/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/fixtures.py` & `sts_libs-0.1.7/sts_libs/src/sts/fixtures/iscsi_fixtures.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/iscsi.py` & `sts_libs-0.1.7/sts_libs/src/sts/iscsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/linux.py` & `sts_libs-0.1.7/sts_libs/src/sts/linux.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/lio.py` & `sts_libs-0.1.7/sts_libs/src/sts/lio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/loopdev.py` & `sts_libs-0.1.7/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/lsm.py` & `sts_libs-0.1.7/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/lvm.py` & `sts_libs-0.1.7/sts_libs/src/sts/lvm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/md.py` & `sts_libs-0.1.7/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/mp.py` & `sts_libs-0.1.7/sts_libs/src/sts/mp.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/net.py` & `sts_libs-0.1.7/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.1.7/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/scsi.py` & `sts_libs-0.1.7/sts_libs/src/sts/scsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.1.7/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/stratis.py` & `sts_libs-0.1.7/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/vdo.py` & `sts_libs-0.1.7/sts_libs/src/sts/vdo.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/logchecker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/size.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.1.7/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/cmdline_test.py` & `sts_libs-0.1.7/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/fio_test.py` & `sts_libs-0.1.7/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/iscsi_test.py` & `sts_libs-0.1.7/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/linux_test.py` & `sts_libs-0.1.7/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/logchecker_test.py` & `sts_libs-0.1.7/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/lvm_test.py` & `sts_libs-0.1.7/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/md_test.py` & `sts_libs-0.1.7/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/net_test.py` & `sts_libs-0.1.7/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.1.7/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/sts_libs/tests/scsi_test.py` & `sts_libs-0.1.7/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/conftest.py` & `sts_libs-0.1.7/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 import time
 from os import getenv
 from pathlib import Path
 from typing import cast
 
 from sts.utils.tmt import CustomResults, TmtResult, remove_nones
 
-pytest_plugins = 'sts.fixtures'
+pytest_plugins = [
+    'sts.fixtures.iscsi_fixtures',
+    'sts.fixtures.rdma_fixtures',
+]
 
 test_data_dir = getenv('TMT_TEST_DATA')
 if not test_data_dir:
     from uuid import uuid4
 
     dir_name = f'/var/tmp/{uuid4().hex[-9:]}'
```

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/_vars/template_iscsi_host.yaml` & `sts_libs-0.1.7/tests/iscsi/_vars/template_iscsi_host.yaml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/libiscsi/local/libiscsi-local.py` & `sts_libs-0.1.7/tests/iscsi/libiscsi/local/libiscsi-local.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/login-logout-stress/login-logout-stress.py` & `sts_libs-0.1.7/tests/iscsi/login-logout-stress/login-logout-stress.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/many-luns/many-luns-local.py` & `sts_libs-0.1.7/tests/iscsi/many-luns/many-luns-local.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/parameters/iscsi_params.py` & `sts_libs-0.1.7/tests/iscsi/parameters/iscsi_params.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/tests/iscsi/parameters/main.fmf` & `sts_libs-0.1.7/tests/iscsi/parameters/main.fmf`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/.gitignore` & `sts_libs-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/LICENSE` & `sts_libs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/pyproject.toml` & `sts_libs-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
   'Topic :: Software Development :: Quality Assurance',
   'Intended Audience :: Developers',
   'Operating System :: POSIX :: Linux',
   'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
   'Framework :: Hatch',
 ]
 dependencies = [
-  'pytest==7.4.3',
-  'pytest-testinfra==9.0.0',
+  'pytest~=8.0',
+  'pytest-testinfra~=10.1',
   'configobj==5.0.8',
   'six==1.16.0',
     # via configobj
 ]
 
 [project.urls]
 Repository = 'https://gitlab.com/rh-kernel-stqe/sts/'
```

### Comparing `sts_libs-0.1.6rc0/sts_libs/README.md` & `sts_libs-0.1.7/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.6rc0/PKG-INFO` & `sts_libs-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sts-libs
-Version: 0.1.6rc0
+Version: 0.1.7
 Summary: Library for pytest-based Linux storage tests
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>, Zhaojuan Guo <zguo@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
@@ -13,16 +13,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.9
 Requires-Dist: configobj==5.0.8
-Requires-Dist: pytest-testinfra==9.0.0
-Requires-Dist: pytest==7.4.3
+Requires-Dist: pytest-testinfra~=10.1
+Requires-Dist: pytest~=8.0
 Requires-Dist: six==1.16.0
 Description-Content-Type: text/markdown
 
 # sts-libs
 
 Python library for simplifying the process of writing storage tests on RPM-based Linux distributions.
```

