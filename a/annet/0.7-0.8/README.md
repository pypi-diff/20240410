# Comparing `tmp/annet-0.7.tar.gz` & `tmp/annet-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annet-0.7.tar", last modified: Wed Apr  3 09:27:19 2024, max compression
+gzip compressed data, was "annet-0.8.tar", last modified: Wed Apr 10 09:06:44 2024, max compression
```

## Comparing `annet-0.7.tar` & `annet-0.8.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 09:27:12.000000 annet-0.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 09:27:12.000000 annet-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 09:27:12.000000 annet-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 09:27:19.053083 annet-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 09:27:12.000000 annet-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-03 09:27:12.000000 annet-0.7/annet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.037083 annet-0.7/annet/adapters/netbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/status_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/common/storage_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/v24/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v24/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/adapters/netbox/v37/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-03 09:27:12.000000 annet-0.7/annet/adapters/netbox/v37/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-03 09:27:12.000000 annet-0.7/annet/annet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.041083 annet-0.7/annet/annlib/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/filter_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/jsontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/devdb/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/devdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/devdb/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/devdb/data/devdb.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/netdev/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/netdev/views/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/rbparser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/deploying.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rbparser/syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/annlib/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rulebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 09:27:12.000000 annet-0.7/annet/annlib/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/api/
--rw-r--r--   0 runner    (1001) docker     (127)    33752 2024-04-03 09:27:12.000000 annet-0.7/annet/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-03 09:27:12.000000 annet-0.7/annet/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-03 09:27:12.000000 annet-0.7/annet/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-03 09:27:12.000000 annet-0.7/annet/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 09:27:12.000000 annet-0.7/annet/configs/context.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 09:27:12.000000 annet-0.7/annet/configs/logging.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-03 09:27:12.000000 annet-0.7/annet/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-04-03 09:27:12.000000 annet-0.7/annet/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-03 09:27:12.000000 annet-0.7/annet/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-03 09:27:12.000000 annet-0.7/annet/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 09:27:12.000000 annet-0.7/annet/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    31426 2024-04-03 09:27:12.000000 annet-0.7/annet/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/generators/
--rw-r--r--   0 runner    (1001) docker     (127)    33829 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/generators/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-03 09:27:12.000000 annet-0.7/annet/generators/common/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 09:27:12.000000 annet-0.7/annet/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-03 09:27:12.000000 annet-0.7/annet/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-03 09:27:12.000000 annet-0.7/annet/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-03 09:27:12.000000 annet-0.7/annet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-03 09:27:12.000000 annet-0.7/annet/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-03 09:27:12.000000 annet-0.7/annet/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-03 09:27:12.000000 annet-0.7/annet/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.045083 annet-0.7/annet/rulebook/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/arista/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/arista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/arista/iface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/aruba/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/ap_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/aruba/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/cisco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/cisco/vlandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/deploying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/huawei/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/aaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/huawei/vlandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/juniper/
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/juniper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/nexus/iface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/patching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.049083 annet-0.7/annet/rulebook/ribbon/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/ribbon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet/rulebook/texts/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.order
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/arista.rul
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.order
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/aruba.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.order
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/cisco.rul
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.deploy
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.order
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/huawei.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/juniper.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.order
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nexus.rul
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/nokia.rul
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/pc.order
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/pc.rul
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/ribbon.deploy
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/ribbon.rul
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/routeros.order
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 09:27:12.000000 annet-0.7/annet/rulebook/texts/routeros.rul
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 09:27:12.000000 annet-0.7/annet/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-03 09:27:12.000000 annet-0.7/annet/tabparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-03 09:27:12.000000 annet-0.7/annet/text_term_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 09:27:12.000000 annet-0.7/annet/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-03 09:27:12.000000 annet-0.7/annet/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 09:27:19.000000 annet-0.7/annet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:27:19.053083 annet-0.7/annet_generators/example/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 09:27:12.000000 annet-0.7/annet_generators/example/lldp.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 09:27:12.000000 annet-0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:27:19.053083 annet-0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-03 09:27:12.000000 annet-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.052765 annet-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-10 09:06:40.000000 annet-0.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 09:06:40.000000 annet-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 09:06:40.000000 annet-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 09:06:44.048766 annet-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-10 09:06:40.000000 annet-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-10 09:06:40.000000 annet-0.8/annet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/status_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/common/storage_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/v24/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v24/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.036765 annet-0.8/annet/adapters/netbox/v37/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-10 09:06:40.000000 annet-0.8/annet/adapters/netbox/v37/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      725 2024-04-10 09:06:40.000000 annet-0.8/annet/annet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/filter_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/jsontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/devdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/devdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/devdb/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/devdb/data/devdb.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/netdev/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/netdev/views/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19784 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/rbparser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/deploying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rbparser/syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/annlib/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rulebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 09:06:40.000000 annet-0.8/annet/annlib/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.040765 annet-0.8/annet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    33752 2024-04-10 09:06:40.000000 annet-0.8/annet/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-10 09:06:40.000000 annet-0.8/annet/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-10 09:06:40.000000 annet-0.8/annet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-10 09:06:40.000000 annet-0.8/annet/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 09:06:40.000000 annet-0.8/annet/configs/context.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 09:06:40.000000 annet-0.8/annet/configs/logging.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 09:06:40.000000 annet-0.8/annet/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18893 2024-04-10 09:06:40.000000 annet-0.8/annet/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-10 09:06:40.000000 annet-0.8/annet/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-10 09:06:40.000000 annet-0.8/annet/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 09:06:40.000000 annet-0.8/annet/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32336 2024-04-10 09:06:40.000000 annet-0.8/annet/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/generators/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-10 09:06:40.000000 annet-0.8/annet/generators/common/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-10 09:06:40.000000 annet-0.8/annet/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-10 09:06:40.000000 annet-0.8/annet/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-10 09:06:40.000000 annet-0.8/annet/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-10 09:06:40.000000 annet-0.8/annet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-10 09:06:40.000000 annet-0.8/annet/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 09:06:40.000000 annet-0.8/annet/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-10 09:06:40.000000 annet-0.8/annet/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/arista/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/arista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/arista/iface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/aruba/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/ap_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/aruba/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/cisco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/cisco/vlandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/deploying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/huawei/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/huawei/vlandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/juniper/
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/juniper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/nexus/iface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/patching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.044765 annet-0.8/annet/rulebook/ribbon/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/ribbon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet/rulebook/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.order
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/arista.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/aruba.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/cisco.rul
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.order
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/huawei.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/juniper.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.order
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nexus.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/nokia.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/pc.order
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/pc.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/ribbon.deploy
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/ribbon.rul
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/routeros.order
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-10 09:06:40.000000 annet-0.8/annet/rulebook/texts/routeros.rul
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-10 09:06:40.000000 annet-0.8/annet/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 09:06:40.000000 annet-0.8/annet/tabparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-10 09:06:40.000000 annet-0.8/annet/text_term_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-10 09:06:40.000000 annet-0.8/annet/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-10 09:06:40.000000 annet-0.8/annet/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 09:06:44.000000 annet-0.8/annet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.048766 annet-0.8/annet_generators/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-10 09:06:40.000000 annet-0.8/annet_generators/example/lldp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 09:06:40.000000 annet-0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:44.052765 annet-0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1283 2024-04-10 09:06:40.000000 annet-0.8/setup.py
```

### Comparing `annet-0.7/AUTHORS` & `annet-0.8/AUTHORS`

 * *Files identical despite different names*

### Comparing `annet-0.7/LICENSE` & `annet-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `annet-0.7/PKG-INFO` & `annet-0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.7
+Version: 0.8
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
```

### Comparing `annet-0.7/README.md` & `annet-0.8/README.md`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/__init__.py` & `annet-0.8/annet/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/common/client.py` & `annet-0.8/annet/adapters/netbox/common/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/common/manufacturer.py` & `annet-0.8/annet/adapters/netbox/common/manufacturer.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/common/models.py` & `annet-0.8/annet/adapters/netbox/common/models.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/common/query.py` & `annet-0.8/annet/adapters/netbox/common/query.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/common/status_client.py` & `annet-0.8/annet/adapters/netbox/common/status_client.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/provider.py` & `annet-0.8/annet/adapters/netbox/provider.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v24/api_models.py` & `annet-0.8/annet/adapters/netbox/v24/api_models.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v24/client.py` & `annet-0.8/annet/adapters/netbox/v24/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v24/storage.py` & `annet-0.8/annet/adapters/netbox/v24/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v37/api_models.py` & `annet-0.8/annet/adapters/netbox/v37/api_models.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v37/client.py` & `annet-0.8/annet/adapters/netbox/v37/client.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/adapters/netbox/v37/storage.py` & `annet-0.8/annet/adapters/netbox/v37/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annet.py` & `annet-0.8/annet/annet.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/command.py` & `annet-0.8/annet/annlib/command.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/diff.py` & `annet-0.8/annet/annlib/diff.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/filter_acl.py` & `annet-0.8/annet/annlib/filter_acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/jsontools.py` & `annet-0.8/annet/annlib/jsontools.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,7 +83,30 @@
 
     patch_data = json.loads(patch_bytes)
     patch = jsonpatch.JsonPatch(patch_data)
     new_doc = patch.apply(old_doc)
 
     new_contents = format_json(new_doc, stable=True).encode()
     return new_contents
+
+
+def apply_acl_filters(content: Dict[str, Any], filters: List[str]) -> Dict[str, Any]:
+    result = {}
+    for f in filters:
+        pointer = jsonpointer.JsonPointer(f)
+
+        try:
+            part = pointer.get(copy.deepcopy(content))
+
+            sub_tree = result
+            for i in pointer.get_parts():
+                if i not in sub_tree:
+                    sub_tree[i] = {}
+                sub_tree = sub_tree[i]
+
+            patch = jsonpatch.JsonPatch([{"op": "add", "path": f, "value": part}])
+            result = patch.apply(result)
+        except jsonpointer.JsonPointerException:
+            # no value found in new_fragment by the pointer, skip the ACL item
+            continue
+
+    return result
```

### Comparing `annet-0.7/annet/annlib/lib.py` & `annet-0.8/annet/annlib/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/netdev/db.py` & `annet-0.8/annet/annlib/netdev/db.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/netdev/devdb/__init__.py` & `annet-0.8/annet/annlib/netdev/devdb/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/netdev/devdb/data/devdb.json` & `annet-0.8/annet/annlib/netdev/devdb/data/devdb.json`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/netdev/views/dump.py` & `annet-0.8/annet/annlib/netdev/views/dump.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/netdev/views/hardware.py` & `annet-0.8/annet/annlib/netdev/views/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/output.py` & `annet-0.8/annet/annlib/output.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/patching.py` & `annet-0.8/annet/annlib/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rbparser/acl.py` & `annet-0.8/annet/annlib/rbparser/acl.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rbparser/deploying.py` & `annet-0.8/annet/annlib/rbparser/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rbparser/ordering.py` & `annet-0.8/annet/annlib/rbparser/ordering.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rbparser/platform.py` & `annet-0.8/annet/annlib/rbparser/platform.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rbparser/syntax.py` & `annet-0.8/annet/annlib/rbparser/syntax.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/rulebook/common.py` & `annet-0.8/annet/annlib/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/tabparser.py` & `annet-0.8/annet/annlib/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/annlib/types.py` & `annet-0.8/annet/annlib/types.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/api/__init__.py` & `annet-0.8/annet/api/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/argparse.py` & `annet-0.8/annet/argparse.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/cli.py` & `annet-0.8/annet/cli.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/cli_args.py` & `annet-0.8/annet/cli_args.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/configs/logging.yaml` & `annet-0.8/annet/configs/logging.yaml`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/connectors.py` & `annet-0.8/annet/connectors.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/deploy.py` & `annet-0.8/annet/deploy.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/diff.py` & `annet-0.8/annet/diff.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/executor.py` & `annet-0.8/annet/executor.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/filtering.py` & `annet-0.8/annet/filtering.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/gen.py` & `annet-0.8/annet/gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,14 +178,15 @@
             old = merge_dicts(old, implicit.config(old, implicit_rules))
             new = merge_dicts(new, implicit.config(new, implicit_rules))
             safe_new = merge_dicts(safe_new, implicit.config(safe_new, implicit_rules))
 
         if not ctx.args.no_acl:
             acl_rules = generators.compile_acl_text(res.acl_text(), device.hw.vendor)
             old = (old and patching.apply_acl(old, acl_rules))
+
             new = patching.apply_acl(
                 new,
                 acl_rules,
                 exclusive=not ctx.args.no_acl_exclusive,
                 with_annotations=ctx.add_annotations,
             )
             if ctx.args.acl_safe:
@@ -228,19 +229,37 @@
             ctx.gens.file_gens(device.fqdn),
             device,
             ctx.storage,
         )
 
         entire_results = res.entire_results
         json_fragment_results = res.json_fragment_results
+        old_json_fragment_files = old_files.json_fragment_files
+
         new_files = res.new_files()
-        new_json_fragment_files = res.new_json_fragment_files(old_files.json_fragment_files)
+        new_json_fragment_files = res.new_json_fragment_files(old_json_fragment_files)
+
         if ctx.args.acl_safe:
             safe_new_files = res.new_files(safe=True)
 
+        filters = build_filter_text(filterer, device, ctx.stdin, ctx.args, ctx.config).split("\n")
+
+        for file_name in new_json_fragment_files:
+            new_json_fragment_files = _update_json_config(
+                new_json_fragment_files,
+                file_name,
+                jsontools.apply_acl_filters(new_json_fragment_files[file_name][0], filters)
+            )
+        for file_name in old_json_fragment_files:
+            old_json_fragment_files = _update_json_config(
+                old_json_fragment_files,
+                file_name,
+                jsontools.apply_acl_filters(old_json_fragment_files[file_name][0], filters)
+            )
+
     if ctx.args.profile:
         perf = res.perf_mesures()
         combined_perf[ALL_GENS] = {"total": time.monotonic() - start}
         combined_perf.update(perf)
         if ctx.do_print_perf:
             _print_perf("ENTIRE", perf)
 
@@ -249,27 +268,34 @@
         old=old,
         new=new,
         acl_rules=acl_rules,
         old_files=old_files.entire_files,
         new_files=new_files,
         partial_result=partial_results,
         entire_result=entire_results,
-        old_json_fragment_files=old_files.json_fragment_files,
+        old_json_fragment_files=old_json_fragment_files,
         new_json_fragment_files=new_json_fragment_files,
         json_fragment_result=json_fragment_results,
         implicit_rules=implicit_rules,
         perf=combined_perf,
         acl_safe_rules=acl_safe_rules,
         safe_old=safe_old,
         safe_new=safe_new,
         safe_new_files=safe_new_files,
         filter_acl_rules=filter_acl_rules,
     )
 
 
+def _update_json_config(json_files, file_name, new_config):
+    file = list(json_files[file_name])
+    file[0] = new_config
+    json_files[file_name] = tuple(file)
+    return json_files
+
+
 @dataclasses.dataclass
 class DeviceDownloadedFiles:
     # map file path to file content for entire generators
     entire_files: Dict[str, str] = dataclasses.field(default_factory=dict)
 
     # map file path to file content for json fragment generators
     json_fragment_files: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
```

### Comparing `annet-0.7/annet/generators/__init__.py` & `annet-0.8/annet/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,16 +292,16 @@
         ret.ref_matcher.add(gen.ref(run_args.device), gen.__class__)
 
     logger.debug("Generating selected PARTIALs ...")
 
     for gen in gens:
         try:
             result = _run_partial_generator(gen, run_args)
-        except NotSupportedDevice:
-            logger.info("generator %s is not supported for this device, skip generator for this devices!", gen)
+        except NotSupportedDevice as exc:
+            logger.info("generator %s raised unsupported error: %r", gen, exc)
             continue
 
         if not result:
             continue
 
         config = result.safe_config if run_args.use_acl_safe else result.config
 
@@ -313,21 +313,25 @@
         ret.ref_track.config(gen.__class__, config)
         ret.add_partial(result)
 
     return ret
 
 
 @tracing.function(name="run_partial_generator")
-def _run_partial_generator(gen: "PartialGenerator", run_args: GeneratorPartialRunArgs) -> GeneratorPartialResult:
+def _run_partial_generator(gen: "PartialGenerator", run_args: GeneratorPartialRunArgs) -> Optional[GeneratorPartialResult]:
     logger = get_logger(generator=_make_generator_ctx(gen))
     device = run_args.device
     output = ""
     config = odict()
     safe_config = odict()
 
+    if not gen.supports_device(device):
+        logger.info("generator %s is not supported for device %s", gen, device.hostname)
+        return None
+
     span = tracing_connector.get().get_current_span()
     if span:
         tracing_connector.get().set_device_attributes(span, run_args.device)
         tracing_connector.get().set_dimensions_attributes(span, gen, run_args.device)
         span.set_attributes({
             "use_acl": run_args.use_acl,
             "use_acl_safe": run_args.use_acl_safe,
@@ -435,92 +439,95 @@
         elif gen.__class__.TYPE == "JSON_FRAGMENT":
             run_generator_fn = _run_json_fragment_generator
             add_result_fn = ret.add_json_fragment
         else:
             raise RuntimeError(f"Unknown generator class type: cls={gen.__class__} TYPE={gen.__class__.TYPE}")
         try:
             result = run_generator_fn(gen, device, storage)
-        except NotSupportedDevice:
-            logger.info("generator %s is not supported for this device", gen)
+        except NotSupportedDevice as exc:
+            logger.info("generator %s raised unsupported error: %r", gen, exc)
             continue
         if result:
             add_result_fn(result)
 
     return ret
 
 
 @tracing.function(min_duration="0.5")
 def _run_entire_generator(gen: "Entire", device: "Device", storage: Storage) -> Optional[GeneratorResult]:
+    logger = get_logger(generator=_make_generator_ctx(gen))
+    if not gen.supports_device(device):
+        logger.info("generator %s is not supported for device %s", gen, device.hostname)
+        return
+
     span = tracing_connector.get().get_current_span()
     if span:
         tracing_connector.get().set_device_attributes(span, device)
         tracing_connector.get().set_dimensions_attributes(span, gen, device)
 
-    logger = get_logger(generator=_make_generator_ctx(gen))
     path = gen.path(device)
-    if path:
-        logger.info("Generating ENTIRE ...")
-
-        with GeneratorPerfMesurer(gen, storage, trace_min_duration="0.5") as pm:
-            output = gen(device)
+    if not path:
+        raise RuntimeError("entire generator should return non-empty path")
 
-        reload_cmds = gen.get_reload_cmds(device)
-        prio = gen.prio
+    logger.info("Generating ENTIRE ...")
+    with GeneratorPerfMesurer(gen, storage, trace_min_duration="0.5") as pm:
+        output = gen(device)
 
-        return GeneratorEntireResult(
-            name=gen.__class__.__name__,
-            tags=gen.TAGS,
-            path=path,
-            output=output,
-            reload=reload_cmds,
-            prio=prio,
-            perf=pm.last_result,
-            is_safe=gen.is_safe(device),
-        )
-    return None
+    return GeneratorEntireResult(
+        name=gen.__class__.__name__,
+        tags=gen.TAGS,
+        path=path,
+        output=output,
+        reload=gen.get_reload_cmds(device),
+        prio=gen.prio,
+        perf=pm.last_result,
+        is_safe=gen.is_safe(device),
+    )
 
 
 def _make_generator_ctx(gen):
     return "%s.[%s]" % (gen.__module__, gen.__class__.__name__)
 
 
 def _run_json_fragment_generator(
         gen: "JSONFragment",
         device: "Device",
         storage: Storage,
 ) -> Optional[GeneratorResult]:
     logger = get_logger(generator=_make_generator_ctx(gen))
+    if not gen.supports_device(device):
+        logger.info("generator %s is not supported for device %s", gen, device.hostname)
+
     path = gen.path(device)
+    if not path:
+        raise RuntimeError("json fragment generator should return non-empty path")
 
     acl_item_or_list_of_items = gen.acl(device)
+    if not acl_item_or_list_of_items:
+        raise RuntimeError("json fragment generator should return non-empty acl")
     if isinstance(acl_item_or_list_of_items, list):
         acl = acl_item_or_list_of_items
     else:
         acl = [acl_item_or_list_of_items]
 
-    if path:
-        logger.info("Generating JSON_FRAGMENT ...")
-
-        with GeneratorPerfMesurer(gen, storage) as pm:
-            config = gen(device)
-
-        reload_cmds = gen.get_reload_cmds(device)
-
-        return GeneratorJSONFragmentResult(
-            name=gen.__class__.__name__,
-            tags=gen.TAGS,
-            path=path,
-            acl=acl,
-            config=config,
-            reload=reload_cmds,
-            perf=pm.last_result,
-            is_safe=gen.is_safe(device),
-            reload_prio=gen.reload_prio,
-        )
-    return None
+    logger.info("Generating JSON_FRAGMENT ...")
+    with GeneratorPerfMesurer(gen, storage) as pm:
+        config = gen(device)
+    reload_cmds = gen.get_reload_cmds(device)
+    return GeneratorJSONFragmentResult(
+        name=gen.__class__.__name__,
+        tags=gen.TAGS,
+        path=path,
+        acl=acl,
+        config=config,
+        reload=reload_cmds,
+        perf=pm.last_result,
+        is_safe=gen.is_safe(device),
+        reload_prio=gen.reload_prio,
+    )
 
 
 def _get_generators(module_paths: Union[List[str], dict], storage, device=None):
     if isinstance(module_paths, dict):
         if device is None:
             module_paths = module_paths.get("default")
         else:
@@ -583,15 +590,15 @@
 
 
 # =====
 class BaseGenerator:
     TYPE: str
     TAGS: list[str]
 
-    def supports_vendor(self, vendor: str) -> bool:  # pylint: disable=unused-argument
+    def supports_device(self, device: Device) -> bool:  # pylint: disable=unused-argument
         return True
 
 
 class TreeGenerator(BaseGenerator):
     def __init__(self, indent="  "):
         self._indents = []
         self._rows = []
@@ -677,44 +684,44 @@
         super().__init__()
         self.storage = storage
         self._annotate = False
         self._running_gen = None
         self._annotations = []
         self._annotation_module = self.__class__.__module__ or ""
 
-    def supports_vendor(self, vendor: str) -> bool:
+    def supports_device(self, device: Device) -> bool:
         if self.__class__.run is PartialGenerator.run:
-            return hasattr(self, f"run_{vendor}")
+            return bool(self._get_vendor_func(device.hw.vendor, "run"))
         else:
             return True
 
     def acl(self, device):
-        if hasattr(self, "acl_" + device.hw.vendor):
-            return getattr(self, "acl_" + device.hw.vendor)(device)
+        acl_func = self._get_vendor_func(device.hw.vendor, "acl")
+        if acl_func:
+            return acl_func(device)
 
     def acl_safe(self, device):
-        if hasattr(self, "acl_safe_" + device.hw.vendor):
-            return getattr(self, "acl_safe_" + device.hw.vendor)(device)
+        acl_func = self._get_vendor_func(device.hw.vendor, "acl_safe")
+        if acl_func:
+            return acl_func(device)
 
     def run(self, device) -> Iterable[Union[str, tuple]]:
-        if hasattr(self, "run_" + device.hw.vendor):
-            return getattr(self, "run_" + device.hw.vendor)(device)
-        logger = get_logger()
-        logger.info(
-            "generator %s is not supported for vendor %s",
-            self,
-            device.hw.vendor,
-        )
-        return iter(())
+        run_func = self._get_vendor_func(device.hw.vendor, "run")
+        if run_func:
+            return run_func(device)
 
     def get_user_runner(self, device):
         if self.__class__.run is not PartialGenerator.run:
             return self.run
-        elif hasattr(self, "run_" + device.hw.vendor):
-            return getattr(self, "run_" + device.hw.vendor)
+        return self._get_vendor_func(device.hw.vendor, "run")
+
+    def _get_vendor_func(self, vendor: str, func_name: str):
+        attr_name = f"{func_name}_{vendor}"
+        if hasattr(self, attr_name):
+            return getattr(self, attr_name)
         return None
 
     # =====
 
     @classmethod
     def get_aliases(cls) -> Set[str]:
         return {cls.__name__, *cls.TAGS}
@@ -786,14 +793,17 @@
     def __init__(self, storage):
         self.storage = storage
         # между генераторами для одного и того же path - выбирается тот что больше
         if not hasattr(self, "prio"):
             self.prio = 100
         self.__device = None
 
+    def supports_device(self, device: Device):
+        return bool(self.path(device))
+
     def run(self, device) -> Union[None, str, Iterable[Union[str, tuple]]]:
         raise NotImplementedError
 
     def reload(self, device) -> Optional[str]:  # pylint: disable=unused-argument
         return
 
     def get_reload_cmds(self, device) -> str:
@@ -903,14 +913,17 @@
         self._json_config: Dict[str, Any] = {}
         self._config_pointer: List[str] = []
 
         # if two generators edit same file, commands from generator with greater `reload_prio` will be used
         if not hasattr(self, "reload_prio"):
             self.reload_prio = 100
 
+    def supports_device(self, device: Device):
+        return bool(self.path(device))
+
     def path(self, device: Device) -> Optional[str]:
         raise NotImplementedError("Required PATH for JSON_FRAGMENT generator")
 
     @classmethod
     def get_aliases(cls) -> Set[str]:
         return {cls.__name__, *cls.TAGS}
```

### Comparing `annet-0.7/annet/generators/common/initial.py` & `annet-0.8/annet/generators/common/initial.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/hardware.py` & `annet-0.8/annet/hardware.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/implicit.py` & `annet-0.8/annet/implicit.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/lib.py` & `annet-0.8/annet/lib.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/output.py` & `annet-0.8/annet/output.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/parallel.py` & `annet-0.8/annet/parallel.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/patching.py` & `annet-0.8/annet/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/reference.py` & `annet-0.8/annet/reference.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/__init__.py` & `annet-0.8/annet/rulebook/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/arista/iface.py` & `annet-0.8/annet/rulebook/arista/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/aruba/ap_env.py` & `annet-0.8/annet/rulebook/aruba/ap_env.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/cisco/iface.py` & `annet-0.8/annet/rulebook/cisco/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/cisco/misc.py` & `annet-0.8/annet/rulebook/cisco/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/cisco/vlandb.py` & `annet-0.8/annet/rulebook/cisco/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/common.py` & `annet-0.8/annet/rulebook/common.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/deploying.py` & `annet-0.8/annet/rulebook/deploying.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/huawei/aaa.py` & `annet-0.8/annet/rulebook/huawei/aaa.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/huawei/bgp.py` & `annet-0.8/annet/rulebook/huawei/bgp.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/huawei/iface.py` & `annet-0.8/annet/rulebook/huawei/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/huawei/misc.py` & `annet-0.8/annet/rulebook/huawei/misc.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/huawei/vlandb.py` & `annet-0.8/annet/rulebook/huawei/vlandb.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/juniper/__init__.py` & `annet-0.8/annet/rulebook/juniper/__init__.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/nexus/iface.py` & `annet-0.8/annet/rulebook/nexus/iface.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/patching.py` & `annet-0.8/annet/rulebook/patching.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/arista.deploy` & `annet-0.8/annet/rulebook/texts/arista.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/arista.order` & `annet-0.8/annet/rulebook/texts/arista.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/arista.rul` & `annet-0.8/annet/rulebook/texts/arista.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/aruba.deploy` & `annet-0.8/annet/rulebook/texts/aruba.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/aruba.order` & `annet-0.8/annet/rulebook/texts/aruba.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/aruba.rul` & `annet-0.8/annet/rulebook/texts/aruba.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/cisco.deploy` & `annet-0.8/annet/rulebook/texts/cisco.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/cisco.order` & `annet-0.8/annet/rulebook/texts/cisco.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/cisco.rul` & `annet-0.8/annet/rulebook/texts/cisco.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/huawei.deploy` & `annet-0.8/annet/rulebook/texts/huawei.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/huawei.order` & `annet-0.8/annet/rulebook/texts/huawei.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/huawei.rul` & `annet-0.8/annet/rulebook/texts/huawei.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/juniper.rul` & `annet-0.8/annet/rulebook/texts/juniper.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/nexus.deploy` & `annet-0.8/annet/rulebook/texts/nexus.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/nexus.order` & `annet-0.8/annet/rulebook/texts/nexus.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/nexus.rul` & `annet-0.8/annet/rulebook/texts/nexus.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/nokia.rul` & `annet-0.8/annet/rulebook/texts/nokia.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/ribbon.deploy` & `annet-0.8/annet/rulebook/texts/ribbon.deploy`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/ribbon.rul` & `annet-0.8/annet/rulebook/texts/ribbon.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/routeros.order` & `annet-0.8/annet/rulebook/texts/routeros.order`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/rulebook/texts/routeros.rul` & `annet-0.8/annet/rulebook/texts/routeros.rul`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/storage.py` & `annet-0.8/annet/storage.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/tabparser.py` & `annet-0.8/annet/tabparser.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/text_term_format.py` & `annet-0.8/annet/text_term_format.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/tracing.py` & `annet-0.8/annet/tracing.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet/types.py` & `annet-0.8/annet/types.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet.egg-info/PKG-INFO` & `annet-0.8/annet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annet
-Version: 0.7
+Version: 0.8
 Summary: annet
 Home-page: https://github.com/annetutil/annet
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: colorama>=0.4.6
```

### Comparing `annet-0.7/annet.egg-info/SOURCES.txt` & `annet-0.8/annet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annet-0.7/annet_generators/example/lldp.py` & `annet-0.8/annet_generators/example/lldp.py`

 * *Files identical despite different names*

### Comparing `annet-0.7/setup.py` & `annet-0.8/setup.py`

 * *Files identical despite different names*

