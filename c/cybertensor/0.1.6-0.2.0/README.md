# Comparing `tmp/cybertensor-0.1.6.tar.gz` & `tmp/cybertensor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybertensor-0.1.6.tar", last modified: Tue Mar 26 06:39:28 2024, max compression
+gzip compressed data, was "cybertensor-0.2.0.tar", last modified: Wed Apr 10 05:27:10 2024, max compression
```

## Comparing `cybertensor-0.1.6.tar` & `cybertensor-0.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.276966 cybertensor-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-26 06:39:22.000000 cybertensor-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 06:39:22.000000 cybertensor-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-26 06:39:28.276966 cybertensor-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-26 06:39:22.000000 cybertensor-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.264966 cybertensor-0.1.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1996 2024-03-26 06:39:22.000000 cybertensor-0.1.6/bin/ctcli
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.268966 cybertensor-0.1.6/cybertensor/
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67642 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/axon.py
--rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/chain_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.268966 cybertensor-0.1.6/cybertensor/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/delegates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/metagraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    33693 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    29100 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    28434 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/stake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/unstake.py
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42803 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/commands/wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/ctlogging.py
--rw-r--r--   0 runner    (1001) docker     (127)   107683 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/cwtensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    36471 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/dendrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    30758 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/keyfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.272966 cybertensor-0.1.6/cybertensor/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/delegation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)    13263 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/root.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/serving.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/set_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/staking.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/messages/unstaking.py
--rw-r--r--   0 runner    (1001) docker     (127)    22578 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/metagraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.272966 cybertensor-0.1.6/cybertensor/mock/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49856 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/mock/cwtensor_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/mock/keyfile_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/mock/wallet_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)    35287 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/synapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.276966 cybertensor-0.1.6/cybertensor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/_register_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    38150 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/wallet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/utils/weight_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-03-26 06:39:22.000000 cybertensor-0.1.6/cybertensor/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.276966 cybertensor-0.1.6/cybertensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-03-26 06:39:28.000000 cybertensor-0.1.6/cybertensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-26 06:39:28.000000 cybertensor-0.1.6/cybertensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 06:39:28.000000 cybertensor-0.1.6/cybertensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-26 06:39:28.000000 cybertensor-0.1.6/cybertensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 06:39:28.000000 cybertensor-0.1.6/cybertensor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 06:39:28.276966 cybertensor-0.1.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 06:39:22.000000 cybertensor-0.1.6/requirements/cubit.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-26 06:39:22.000000 cybertensor-0.1.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-26 06:39:22.000000 cybertensor-0.1.6/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 06:39:28.276966 cybertensor-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-26 06:39:22.000000 cybertensor-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.049584 cybertensor-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 05:27:04.000000 cybertensor-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 05:27:04.000000 cybertensor-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-10 05:27:10.049584 cybertensor-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 05:27:04.000000 cybertensor-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.033583 cybertensor-0.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1996 2024-04-10 05:27:04.000000 cybertensor-0.2.0/bin/ctcli
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.037583 cybertensor-0.2.0/cybertensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67743 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/axon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26316 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/chain_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.041583 cybertensor-0.2.0/cybertensor/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/delegates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/metagraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33693 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29100 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28434 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/stake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/unstake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42803 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/commands/wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14076 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/ctlogging.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108267 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/cwtensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36538 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/dendrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30758 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/keyfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.045584 cybertensor-0.2.0/cybertensor/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/delegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/set_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/staking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/messages/unstaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22578 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/metagraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.045584 cybertensor-0.2.0/cybertensor/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49856 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/mock/cwtensor_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/mock/keyfile_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/mock/wallet_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.045584 cybertensor-0.2.0/cybertensor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/_register_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38150 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/wallet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/utils/weight_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-04-10 05:27:04.000000 cybertensor-0.2.0/cybertensor/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.045584 cybertensor-0.2.0/cybertensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-10 05:27:10.000000 cybertensor-0.2.0/cybertensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-10 05:27:10.000000 cybertensor-0.2.0/cybertensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:27:10.000000 cybertensor-0.2.0/cybertensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-10 05:27:10.000000 cybertensor-0.2.0/cybertensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 05:27:10.000000 cybertensor-0.2.0/cybertensor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:27:10.045584 cybertensor-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 05:27:04.000000 cybertensor-0.2.0/requirements/cubit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-10 05:27:04.000000 cybertensor-0.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 05:27:04.000000 cybertensor-0.2.0/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:27:10.049584 cybertensor-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-10 05:27:04.000000 cybertensor-0.2.0/setup.py
```

### Comparing `cybertensor-0.1.6/LICENSE` & `cybertensor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/PKG-INFO` & `cybertensor-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybertensor
-Version: 0.1.6
+Version: 0.2.0
 Summary: cybertensor
 Home-page: https://github.com/cybercongress/cybertensor
 Author: cyberhead
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -58,14 +58,16 @@
 Requires-Dist: tqdm
 Requires-Dist: uvicorn==0.22.0
 Requires-Dist: wheel
 Requires-Dist: cosmpy>=0.9.1
 Requires-Dist: ecdsa<0.15
 Requires-Dist: py-bip39-bindings
 Requires-Dist: urllib3==1.26.15
+Requires-Dist: websocket>=0.2.1
+Requires-Dist: websocket-client==1.7.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.2.0; extra == "dev"
 Requires-Dist: pytest-mock==3.12.0; extra == "dev"
 Requires-Dist: pytest-split==0.8.0; extra == "dev"
 Requires-Dist: pytest-xdist==3.0.2; extra == "dev"
 Requires-Dist: pytest-rerunfailures==10.2; extra == "dev"
 Requires-Dist: coveralls==3.3.1; extra == "dev"
```

### Comparing `cybertensor-0.1.6/README.md` & `cybertensor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/bin/ctcli` & `cybertensor-0.2.0/bin/ctcli`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/__init__.py` & `cybertensor-0.2.0/cybertensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from cosmpy.aerial.config import NetworkConfig
 from rich.console import Console
 from rich.traceback import install
 
 nest_asyncio.apply()
 
 # Cybertensor code and protocol version.
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 version_split = __version__.split(".")
 __version_as_int__ = (
     (100 * int(version_split[0]))
     + (10 * int(version_split[1]))
     + (1 * int(version_split[2]))
 )
 
@@ -61,23 +61,14 @@
     __use_console__ = True
     __console__ = Console()
 
 
 turn_console_on()
 
 
-# Logging helpers.
-def trace(on: bool = True):
-    logging.set_trace(on)
-
-
-def debug(on: bool = True):
-    logging.set_debug(on)
-
-
 class NetworkConfigCwTensor(NetworkConfig):
     def __init__(
         self,
         chain_id: str,
         fee_minimum_gas_price: Union[int, float],
         fee_denomination: str,
         staking_denomination: str,
@@ -192,15 +183,14 @@
 from cybertensor.synapse import TerminalInfo, Synapse
 from cybertensor.stream import StreamingSynapse
 from cybertensor.tensor import tensor, Tensor
 from cybertensor.axon import axon
 from cybertensor.dendrite import dendrite
 from cybertensor.config import Config
 from cybertensor.mock import MockCwtensor, MockWallet
-# from .subnets import SubnetsAPI
 
 configs = [
     axon.config(),
     Config(),
     PriorityThreadPoolExecutor.config(),
     Wallet.config(),
     logging.config(),
```

### Comparing `cybertensor-0.1.6/cybertensor/axon.py` & `cybertensor-0.2.0/cybertensor/axon.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from fastapi import FastAPI, APIRouter, Depends
 from fastapi.responses import JSONResponse
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 
 import cybertensor
+import cybertensor.utils.networking as net
 from cybertensor.config import Config
 from cybertensor.errors import *
 from cybertensor.keypair import Keypair
 from cybertensor.threadpool import PriorityThreadPoolExecutor
 from cybertensor.wallet import Wallet
 
 """ Create and init Axon, which services Forward and Backward requests from other neurons.
@@ -180,48 +181,48 @@
         import cybertensor
         # Define your custom synapse class
         class MySynapse( cybertensor.Synapse ):
             input: int = 1
             output: int = None
 
         # Define a custom request forwarding function
-        def forward( synapse: MySynapse ) -> MySynapse:
+        def forward_my_synapse( synapse: MySynapse ) -> MySynapse:
             # Apply custom logic to synapse and return it
             synapse.output = 2
             return synapse
 
         # Define a custom request verification function
         def verify_my_synapse( synapse: MySynapse ):
             # Apply custom verification logic to synapse
             # Optionally raise Exception
 
-        # Define a custom request blacklist fucntion
+        # Define a custom request blacklist function
         def blacklist_my_synapse( synapse: MySynapse ) -> bool:
             # Apply custom blacklist
             # return False ( if non blacklisted ) or True ( if blacklisted )
 
-        # Define a custom request priority fucntion
-        def prioritize_my_synape( synapse: MySynapse ) -> float:
+        # Define a custom request priority function
+        def prioritize_my_synapse( synapse: MySynapse ) -> float:
             # Apply custom priority
             return 1.0
 
         # Initialize Axon object with a custom configuration
         my_axon = cybertensor.axon(config=my_config, wallet=my_wallet, port=9090, ip="192.0.2.0", external_ip="203.0.113.0", external_port=7070)
 
         # Attach the endpoint with the specified verification and forwarding functions
         my_axon.attach(
             forward_fn = forward_my_synapse,
             verify_fn = verify_my_synapse,
             blacklist_fn = blacklist_my_synapse,
-            priority_fn = prioritize_my_synape
+            priority_fn = prioritize_my_synapse
         ).attach(
             forward_fn = forward_my_synapse_2,
             verify_fn = verify_my_synapse_2,
             blacklist_fn = blacklist_my_synapse_2,
-            priority_fn = prioritize_my_synape_2
+            priority_fn = prioritize_my_synapse_2
         ).serve(
             netuid = ...
             cwtensor = ...
         ).start()
 
    Args:
         wallet (cybertensor.wallet, optional): Wallet with hotkey and coldkeypub.
@@ -305,24 +306,16 @@
         # Get wallet or use default.
         self.wallet = wallet or Wallet()
 
         # Build axon objects.
         self.uuid = str(uuid.uuid1())
         self.ip = self.config.axon.ip
         self.port = self.config.axon.port
-        self.external_ip = (
-            self.config.axon.external_ip
-            if self.config.axon.external_ip is not None
-            else cybertensor.utils.networking.get_external_ip()
-        )
-        self.external_port = (
-            self.config.axon.external_port
-            if self.config.axon.external_port is not None
-            else self.config.axon.port
-        )
+        self.external_ip = self.config.axon.external_ip or net.get_external_ip()
+        self.external_port = self.config.axon.external_port or self.config.axon.port
         self.full_address = str(self.config.axon.ip) + ":" + str(self.config.axon.port)
         self.started = False
 
         # Build middleware
         self.thread_pool = cybertensor.PriorityThreadPoolExecutor(
             max_workers=self.config.axon.max_workers
         )
@@ -683,20 +676,20 @@
 
         Args:
             config (Config): The config object holding axon settings.
 
         Raises:
             AssertionError: If the axon or external ports are not in range [1024, 65535]
         """
-        assert (
-            config.axon.port > 1024 and config.axon.port < 65535
+        assert config.axon.port is None or (
+                1024 < config.axon.port < 65535
         ), "Axon port must be in range [1024, 65535]"
 
         assert config.axon.external_port is None or (
-            config.axon.external_port > 1024 and config.axon.external_port < 65535
+                1024 < config.axon.external_port < 65535
         ), "External port must be in range [1024, 65535]"
 
     def to_string(self):
         """
         Provides a human-readable representation of the AxonInfo for this Axon.
         """
         return self.info().to_string()
@@ -843,15 +836,18 @@
 
         Note:
             The verification process assumes the use of an asymmetric encryption algorithm, where the sender signs the
             message with their private key and the receiver verifies the signature using the sender's public key.
         """
         # Build the keypair from the dendrite_hotkey
         if synapse.dendrite is not None:
-            keypair = Keypair(address=synapse.dendrite.hotkey)  # type: ignore
+            cybertensor.logging.info(f"dendrite: {synapse.dendrite}")
+            # NOTE added public key to the synapese for correct keypair initialization
+            # keypair = Keypair(address=synapse.dendrite.hotkey)
+            keypair = Keypair(address=synapse.dendrite.hotkey, public_key=synapse.dendrite.pubkey)
             # Build the signature messages.
             message = (f"{synapse.dendrite.nonce}.{synapse.dendrite.hotkey}.{self.wallet.hotkey.address}."
                        f"{synapse.dendrite.uuid}.{synapse.computed_body_hash}")
 
             # Build the unique endpoint key.
             endpoint_key = f"{synapse.dendrite.hotkey}:{synapse.dendrite.uuid}"
 
@@ -860,15 +856,15 @@
                     endpoint_key in self.nonces.keys()
                     and self.nonces[endpoint_key] is not None
                     and synapse.dendrite.nonce is not None
                     and synapse.dendrite.nonce <= self.nonces[endpoint_key]
             ):
                 raise Exception("Nonce is too small")
 
-            if not keypair.verify(message, synapse.dendrite.signature):  # type: ignore
+            if not keypair.verify(message, synapse.dendrite.signature):
                 raise Exception(
                     f"Signature mismatch with {message} and {synapse.dendrite.signature}"
                 )
 
             # Success
             self.nonces[endpoint_key] = synapse.dendrite.nonce  # type: ignore
         else:
@@ -977,19 +973,21 @@
         try:
             # Set up the synapse from its headers.
             synapse: cybertensor.Synapse = await self.preprocess(request)
 
             # Logs the start of the request processing
             if synapse.dendrite is not None:
                 cybertensor.logging.trace(
-                    f"axon     | <-- | {request.headers.get('content-length', -1)} B | {synapse.name} | {synapse.dendrite.hotkey} | {synapse.dendrite.ip}:{synapse.dendrite.port} | 200 | Success "
+                    f"axon     | <-- | {request.headers.get('content-length', -1)} B | {synapse.name} | "
+                    f"{synapse.dendrite.hotkey} | {synapse.dendrite.ip}:{synapse.dendrite.port} | 200 | Success "
                 )
             else:
                 cybertensor.logging.trace(
-                    f"axon     | <-- | {request.headers.get('content-length', -1)} B | {synapse.name} | None | None | 200 | Success "
+                    f"axon     | <-- | {request.headers.get('content-length', -1)} B | {synapse.name} | "
+                    f"None | None | 200 | Success "
                 )
 
             # Call the blacklist function
             await self.blacklist(synapse)
 
             # Call verify and return the verified request
             await self.verify(synapse)
```

### Comparing `cybertensor-0.1.6/cybertensor/chain_data.py` & `cybertensor-0.2.0/cybertensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/cli.py` & `cybertensor-0.2.0/cybertensor/cli.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/__init__.py` & `cybertensor-0.2.0/cybertensor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/delegates.py` & `cybertensor-0.2.0/cybertensor/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/identity.py` & `cybertensor-0.2.0/cybertensor/commands/identity.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/inspect.py` & `cybertensor-0.2.0/cybertensor/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/list.py` & `cybertensor-0.2.0/cybertensor/commands/list.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/metagraph.py` & `cybertensor-0.2.0/cybertensor/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/network.py` & `cybertensor-0.2.0/cybertensor/commands/network.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/overview.py` & `cybertensor-0.2.0/cybertensor/commands/overview.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/register.py` & `cybertensor-0.2.0/cybertensor/commands/register.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/root.py` & `cybertensor-0.2.0/cybertensor/commands/root.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/stake.py` & `cybertensor-0.2.0/cybertensor/commands/stake.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/transfer.py` & `cybertensor-0.2.0/cybertensor/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/unstake.py` & `cybertensor-0.2.0/cybertensor/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/utils.py` & `cybertensor-0.2.0/cybertensor/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/commands/wallets.py` & `cybertensor-0.2.0/cybertensor/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/config.py` & `cybertensor-0.2.0/cybertensor/config.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/ctlogging.py` & `cybertensor-0.2.0/cybertensor/ctlogging.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,26 +96,26 @@
 
             cls.set_debug(cls.__debug_on__)
             cls.set_trace(cls.__trace_on__)
 
     def __new__(
         cls,
         config: Optional["Config"] = None,
-        level: Optional[int] = 40,
+        level: Optional[int] = None,
         debug: Optional[bool] = None,
         trace: Optional[bool] = None,
         record_log: Optional[bool] = None,
         logging_dir: Optional[str] = None,
     ):
         r"""Instantiate cybertensor logging system backend.
         Args:
             config (Config, optional):
                 cybertensor.logging.config()
             level (int, optional):
-                logger level (default: 40).
+                logger level in numeric value.
             debug (bool, optional):
                 Turn on debug.
             trace (bool, optional):
                 Turn on trace.
             record_log (bool, optional):
                 If ``True``, logs are saved to logging dir.
             logging_dir (str, optional):
@@ -125,14 +125,17 @@
         cls.__has_been_inited__ = True
 
         if config is None:
             config = logging.config()
         config = copy.deepcopy(config)
         config.logging.debug = debug if debug is not None else config.logging.debug
         config.logging.trace = trace if trace is not None else config.logging.trace
+        config.logging.level = (
+            level if level is not None else config.logging.level if config.logging.level is not None else 20
+        )
         config.logging.record_log = (
             record_log if record_log is not None else config.logging.record_log
         )
         config.logging.logging_dir = (
             logging_dir if logging_dir is not None else config.logging.logging_dir
         )
 
@@ -147,15 +150,15 @@
             logger.remove(cls.__std_sink__)
         if cls.__file_sink__ is not None:
             logger.remove(cls.__file_sink__)
 
         # Add filtered sys.stdout.
         cls.__std_sink__ = logger.add(
             sys.stdout,
-            level=level,
+            level=config.logging.level,
             filter=cls.log_filter,
             colorize=True,
             enqueue=True,
             backtrace=True,
             diagnose=True,
             format=cls.log_formatter,
         )
@@ -206,33 +209,39 @@
             default_logging_record_log = os.getenv("CT_LOGGING_RECORD_LOG") or False
             default_logging_logging_dir = (
                 os.getenv("CT_LOGGING_LOGGING_DIR") or "~/.cybertensor/miners"
             )
             parser.add_argument(
                 "--" + prefix_str + "logging.debug",
                 action="store_true",
-                help="""Turn on cybertensor debugging information""",
+                help="""Turn on cybertensor debugging information.""",
                 default=default_logging_debug,
             )
             parser.add_argument(
                 "--" + prefix_str + "logging.trace",
                 action="store_true",
-                help="""Turn on cybertensor trace level information""",
+                help="""Turn on cybertensor trace level information.""",
                 default=default_logging_trace,
             )
             parser.add_argument(
+                "--" + prefix_str + "logging.level",
+                type=int,
+                help="""The default logging level in numeric values.""",
+                default=None,
+            )
+            parser.add_argument(
                 "--" + prefix_str + "logging.record_log",
                 action="store_true",
                 help="""Turns on logging to file.""",
                 default=default_logging_record_log,
             )
             parser.add_argument(
                 "--" + prefix_str + "logging.logging_dir",
                 type=str,
-                help="Logging default root directory.",
+                help="""Logging default root directory.""",
                 default=default_logging_logging_dir,
             )
         except argparse.ArgumentError:
             # re-parsing arguments.
             pass
 
     @classmethod
```

### Comparing `cybertensor-0.1.6/cybertensor/cwtensor.py` & `cybertensor-0.2.0/cybertensor/cwtensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,19 +341,23 @@
                              error,
                              gas: Optional[int] = cybertensor.__default_gas__,
                              funds: Optional[str] = None) -> Optional[bool]:
         if not wait_for_finalization:
             self.contract.execute(msg, signer_wallet, gas, funds=funds)
             return True
         else:
-            tx = self.contract.execute(msg, signer_wallet, gas, funds=funds)
+            try:
+                # NOTE will raise exception if tx simulation is not successful, need to catch it
+                tx = self.contract.execute(msg, signer_wallet, gas, funds=funds)
+            except Exception as e:
+                raise error(e.__str__())
             try:
                 tx.wait_to_complete()
                 if tx.response.is_successful():
-                    print(f'Gas used: {tx.response.gas_used}')
+                    cybertensor.logging.trace(f'Gas used: {tx.response.gas_used}')
                     return True
                 else:
                     raise error(tx.response.logs)
             except Exception as e:
                 raise error(e.__str__())
 
     def _execute_contract(self, wait_for_finalization: bool,
@@ -367,14 +371,15 @@
                           gas: Optional[int] = cybertensor.__default_gas__,
                           funds: Optional[str] = None) -> [bool, Optional[str]]:
         try:
             _private_key = wallet.hotkey.private_key if use_hotkey else wallet.coldkey.private_key
             signer_wallet = LocalWallet(
                 PrivateKey(_private_key), self.address_prefix
             )
+            cybertensor.logging.trace(f'tx msg {msg}\tsigner_wallet {signer_wallet}')
             res = self.make_call_with_retry(
                 wait_for_finalization=wait_for_finalization,
                 msg=msg,
                 signer_wallet=signer_wallet,
                 error=error,
                 gas=gas,
                 funds=funds)
@@ -398,32 +403,38 @@
             return False, f"[red]{exception_text}[/red]: error:{e}"
         return False, None
 
     @retry(delay=3, tries=3, backoff=2, max_delay=8)
     def make_call_with_retry_2(self, wait_for_finalization: bool,
                                msg: dict, signer_wallet: LocalWallet, gas: Optional[int] = cybertensor.__default_gas__,
                                funds: Optional[str] = None) -> [bool, Optional[str]]:
+        cybertensor.logging.trace(f'tx msg {msg}\tsigner_wallet {signer_wallet}')
         if not wait_for_finalization:
             self.contract.execute(msg, signer_wallet, gas, funds=funds)
             return True, None
         else:
-            tx = self.contract.execute(msg, signer_wallet, gas, funds=funds)
+            try:
+                # NOTE will raise exception if tx simulation is not successful, need to catch it
+                tx = self.contract.execute(msg, signer_wallet, gas, funds=funds)
+            except Exception as e:
+                return False, e.__str__()
+
             try:
                 tx.wait_to_complete()
                 if tx.response.is_successful():
                     print(f'Gas used: {tx.response.gas_used}')
                     return True, None
                 else:
                     return False, tx.response.code
             except Exception as e:
                 return False, e.__str__()
 
-    ####################
-    #### Websocket Interface related
-    ####################
+    #####################################
+    #### Websocket Interface related ####
+    #####################################
     def connect_websocket(self):
         """
         (Re)creates the websocket connection, if the URL contains a 'ws' or 'wss' scheme
         """
         pass
 
     def close(self):
@@ -1453,17 +1464,17 @@
             netuids=netuids,
             weights=weights,
             version_key=version_key,
             wait_for_finalization=wait_for_finalization,
             prompt=prompt,
         )
 
-    #####################################
-    #### Hyper parameter calls. ####
-    #####################################
+    ###############################
+    #### Hyper parameter calls ####
+    ###############################
 
     def difficulty(self, netuid: int, block: Optional[int] = None) -> Optional[int]:
         """
         Retrieves the 'Difficulty' hyperparameter for a specified subnet in the cybertensor network.
         This parameter is instrumental in determining the computational challenge required for neurons
         to participate in consensus and validation processes.
         Args:
@@ -1745,17 +1756,17 @@
         
         The transaction rate limit is an essential parameter for ensuring the stability and scalability
         of the cybertensor network. It helps in managing network load and preventing congestion, thereby
         maintaining efficient and timely transaction processing.
         """
         return self.contract.query({"get_tx_rate_limit": {}})
 
-    #####################################
+    ############################
     #### Network Parameters ####
-    #####################################
+    ############################
 
     def get_subnet_burn_cost(self, block: Optional[int] = None) -> Optional[int]:
         lock_cost = self.contract.query({"get_network_registration_cost": {}})
 
         if lock_cost is None:
             return None
 
@@ -2088,17 +2099,17 @@
         """
         result = self.contract.query(
             {"get_stake_info_for_coldkeys": {"coldkeys": coldkey_list}}
         )
 
         return StakeInfo.list_of_tuple_from_list_any(result)
 
-    ########################################
+    #######################################
     #### Neuron information per subnet ####
-    ########################################
+    #######################################
 
     def is_hotkey_registered_any(
         self, hotkey: str, block: Optional[int] = None
     ) -> bool:
         """
         Checks if a neuron's hotkey is registered on any subnet within the cybertensor network.
         Args:
```

### Comparing `cybertensor-0.1.6/cybertensor/dendrite.py` & `cybertensor-0.2.0/cybertensor/dendrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,21 +616,23 @@
         # Build the Dendrite headers using the local system's details
         synapse.dendrite = cybertensor.TerminalInfo(
             ip=self.external_ip,
             version=cybertensor.__version_as_int__,
             nonce=time.monotonic_ns(),
             uuid=self.uuid,
             hotkey=self.keypair.address,
+            pubkey=self.keypair.public_key
         )
 
         # Build the Axon headers using the target axon's details
         synapse.axon = cybertensor.TerminalInfo(
             ip=target_axon_info.ip,
             port=target_axon_info.port,
             hotkey=target_axon_info.hotkey,
+            pubkey=None
         )
 
         # Sign the request using the dendrite, axon info, and the synapse body hash
         message = f"{synapse.dendrite.nonce}.{synapse.dendrite.hotkey}.{synapse.axon.hotkey}.{synapse.dendrite.uuid}.{synapse.body_hash}"
         synapse.dendrite.signature = f"0x{self.keypair.sign(message).hex()}"
 
         return synapse
```

### Comparing `cybertensor-0.1.6/cybertensor/errors.py` & `cybertensor-0.2.0/cybertensor/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,22 +101,27 @@
 
 
 class KeyFileError(Exception):
     r"""Error thrown when the keyfile is corrupt, non-writable, non-readable or the password used to decrypt is invalid."""
     pass
 
 
+class ConfigurationError(Exception):
+    r"""Error raised when a private key is not found."""
+    pass
+
+
 class MetadataError(ChainTransactionError):
     r"""Error raised when metadata commitment transaction fails."""
 
     pass
 
 
 class InvalidRequestNameError(Exception):
-    r"""This exception is raised when the request name is invalid. Ususally indicates a broken URL."""
+    r"""This exception is raised when the request name is invalid. Usually indicates a broken URL."""
 
     pass
 
 
 class UnknownSynapseError(Exception):
     r"""This exception is raised when the request name is not found in the Axon's forward_fns dictionary."""
 
@@ -142,14 +147,15 @@
 
 
 class PriorityException(Exception):
     r"""This exception is raised when the request priority is not met."""
 
     pass
 
+
 class PostProcessException(Exception):
     r"""This exception is raised when the response headers cannot be updated."""
 
     pass
 
 
 class RunException(Exception):
```

### Comparing `cybertensor-0.1.6/cybertensor/keyfile.py` & `cybertensor-0.2.0/cybertensor/keyfile.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/keypair.py` & `cybertensor-0.2.0/cybertensor/keypair.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,35 +11,49 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+import base64
+import hashlib
 from typing import Optional, Union
 
+from bech32 import (  # pylint: disable=wrong-import-order
+    bech32_encode,
+    convertbits,
+)
 from bip39 import bip39_generate, bip39_validate
+from ecdsa import (  # type: ignore # pylint: disable=wrong-import-order
+    SECP256k1,
+    SigningKey,
+    VerifyingKey,
+)
 from cosmpy.crypto.address import Address
+from cosmpy.crypto.hashfuncs import ripemd160
 from cosmpy.crypto.keypairs import PrivateKey, PublicKey
 from cosmpy.mnemonic import (
     derive_child_key_from_mnemonic,
     COSMOS_HD_PATH,
     validate_mnemonic_and_normalise,
 )
 
+import cybertensor as ct
 from cybertensor import __chain_address_prefix__
+from cybertensor.errors import ConfigurationError
 
 
 class Keypair:
     def __init__(
-        self,
-        address: str = None,
-        public_key: Union[bytes, str] = None,
-        private_key: Union[bytes, str] = None,
-        prefix: Optional[str] = None,
+            self,
+            address: str = None,
+            public_key: Union[bytes, str] = None,
+            private_key: Union[bytes, str] = None,
+            prefix: Optional[str] = None,
     ):
         """
         Allows generation of Keypairs from a variety of input combination, such as a public/private key combination,
         mnemonic or URI containing soft and hard derivation paths. With these Keypairs data can be signed and verified
 
         Parameters
         ----------
@@ -57,18 +71,21 @@
             if type(private_key) is str:
                 private_key = bytes.fromhex(private_key.replace("0x", ""))
 
             private_key_obj = PrivateKey(private_key)
             public_key = private_key_obj.public_key.public_key
             address = Address(PublicKey(private_key_obj.public_key), prefix).__str__()
 
-        if not public_key:
-            raise ValueError("No public key provided")
+        if isinstance(public_key, str):
+            self.public_key = public_key
+        else:
+            self.public_key: str = public_key.decode("utf-8")
 
-        self.public_key: bytes = public_key
+        if not self.public_key:
+            raise ValueError("No public key provided")
 
         self.address: str = address
 
         self.private_key: bytes = private_key
 
         self.mnemonic = None
 
@@ -100,15 +117,15 @@
         -------
         bool
         """
         return bip39_validate(mnemonic, "en")
 
     @classmethod
     def create_from_mnemonic(
-        cls, mnemonic: str, prefix: Optional[str] = None
+            cls, mnemonic: str, prefix: Optional[str] = None
     ) -> "Keypair":
         """
         Create a Keypair for given mnemonic
 
         Parameters
         ----------
         mnemonic: Seed phrase
@@ -130,15 +147,15 @@
 
         keypair.mnemonic = mnemonic
 
         return keypair
 
     @classmethod
     def create_from_private_key(
-        cls, private_key: Union[bytes, str], prefix: Optional[str] = None
+            cls, private_key: Union[bytes, str], prefix: Optional[str] = None
     ) -> "Keypair":
         """
         Creates Keypair for specified public/private keys
         Parameters
         ----------
         private_key: hex string or bytes of private key
         prefix: prefix, defaults to None
@@ -153,14 +170,81 @@
 
         return cls(
             public_key=PrivateKey(private_key).public_key.public_key,
             private_key=private_key,
             prefix=prefix,
         )
 
+    def get_address_from_public_key(self, public_key: str) -> str:
+        """
+        Get the address from the public key.
+
+        :param public_key: the public key
+        :return: str
+        """
+        public_key_bytes = bytes.fromhex(public_key)
+        s = hashlib.new("sha256", public_key_bytes).digest()
+        r = ripemd160(s)
+        five_bit_r = convertbits(r, 8, 5)
+        if five_bit_r is None:  # pragma: nocover
+            raise TypeError("Unsuccessful bech32.convertbits call")
+
+        ## TODO add configuration for chain prefix
+        address = bech32_encode(__chain_address_prefix__, five_bit_r)
+        return address
+
+    def recover_message(self, message: bytes, signature: str) -> tuple[Address, ...]:
+        public_keys = self.recover_public_keys_from_message(message, signature)
+        addresses = [
+            self.get_address_from_public_key(public_key) for public_key in public_keys
+        ]
+        return tuple(addresses)
+
+    def recover_public_keys_from_message(self, message: bytes, signature: str) -> tuple[str, ...]:
+        signature_b64 = base64.b64decode(signature)
+        verifying_keys = VerifyingKey.from_public_key_recovery(
+            signature_b64,
+            message,
+            SECP256k1,
+            hashfunc=hashlib.sha256,
+        )
+        public_keys = [
+            verifying_key.to_string("compressed").hex()
+            for verifying_key in verifying_keys
+        ]
+        return tuple(public_keys)
+
+    def sign(self, data: Union[bytes, str]) -> bytes:
+        """
+        Creates a signature for given data
+
+        Parameters
+        ----------
+        data: data to sign in bytes or hex string format
+
+        Returns
+        -------
+        signature in bytes
+
+        """
+        if data[0:2] == '0x':
+            data = bytes.fromhex(data[2:])
+        elif type(data) is str:
+            data = data.encode()
+        elif type(data) is not bytes:
+            raise TypeError(f"Signed data should be of type bytes or hex-string, given data type is {type(data)}")
+
+        if not self.private_key:
+            raise ConfigurationError("No private key set to create signatures")
+
+        signature_compact = PrivateKey(self.private_key).sign(message=data, deterministic=True)
+        signature_base64_str = base64.b64encode(signature_compact).decode("utf-8").encode()
+
+        return signature_base64_str
+
     def verify(self, data: Union[bytes, str], signature: Union[bytes, str]) -> bool:
         """
         Verifies data with specified signature
 
         Parameters
         ----------
         data: data to be verified in bytes or hex string format
@@ -171,28 +255,23 @@
         True if data is signed with this Keypair, otherwise False
         """
 
         if data[0:2] == "0x":
             data = bytes.fromhex(data[2:])
         elif type(data) is str:
             data = data.encode()
+        elif type(data) is not bytes:
+            raise TypeError(f"Signed data should be of type bytes or hex-string, given data type is {type(data)}")
 
         if type(signature) is str and signature[0:2] == "0x":
             signature = bytes.fromhex(signature[2:])
 
-        if type(signature) is not bytes:
-            raise TypeError("Signature should be of type bytes or a hex-string")
-
-        # TODO replace verify function to correct
-        verified = True
-        # verified = crypto_verify_fn(signature, data, self.public_key)
-        #
-        # if not verified:
-        #     verified = crypto_verify_fn(signature, b'<Bytes>' + data + b'</Bytes>', self.public_key)
-        #
-        return verified
+        for address in self.recover_message(message=data, signature=signature):
+            if self.address == address:
+                return True
+        return False
 
     def __repr__(self):
         if self.address:
             return f"<Keypair (address={self.address})>"
         else:
             return f"<Keypair (public_key={self.public_key})>"
```

### Comparing `cybertensor-0.1.6/cybertensor/messages/__init__.py` & `cybertensor-0.2.0/cybertensor/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/delegation.py` & `cybertensor-0.2.0/cybertensor/messages/delegation.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/network.py` & `cybertensor-0.2.0/cybertensor/messages/network.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/prometheus.py` & `cybertensor-0.2.0/cybertensor/messages/prometheus.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,22 @@
         netuid (int):
             network uid to serve on.
         wait_for_finalization (bool):
             If set, waits for the extrinsic to be finalized on the chain before returning ``true``,
             or returns ``false`` if the extrinsic fails to be finalized within the timeout.
     Returns:
         success (bool):
-            Flag is ``true`` if extrinsic was finalized or uncluded in the block.
+            Flag is ``true`` if extrinsic was finalized or included in the block.
             If we did not wait for finalization / inclusion, the response is ``true``.
     """
 
     # ---- Get external ip ----
     if ip is None:
         try:
-            external_ip = net.get_external_ip()
+            external_ip = cwtensor.config.axon.external_ip or net.get_external_ip()
             console.print(
                 f":white_heavy_check_mark: [green]Found external ip: {external_ip}[/green]"
             )
             cybertensor.logging.success(
                 prefix="External IP", sufix=f"<blue>{external_ip}</blue>"
             )
         except Exception as e:
```

### Comparing `cybertensor-0.1.6/cybertensor/messages/registration.py` & `cybertensor-0.2.0/cybertensor/messages/registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         f":satellite: Checking Account on [bold]subnet:{netuid}[/bold]..."
     ):
         neuron = cwtensor.get_neuron_for_pubkey_and_subnet(
             wallet.hotkey.address, netuid=netuid
         )
         if not neuron.is_null:
             cybertensor.logging.debug(
-                f"Wallet {wallet} is already registered on {neuron.netuid} with {neuron.uid}"
+                f"Wallet {wallet} is already registered on network: {neuron.netuid} with user id: {neuron.uid}"
             )
             return True
 
     if prompt:
         if not Confirm.ask(
             f"Continue Registration?\n"
             f"  hotkey:     [bold white]{wallet.hotkey.address}[/bold white]\n"
@@ -262,14 +262,15 @@
             return True
 
     if prompt:
         # Prompt user for confirmation.
         if not Confirm.ask(f"Recycle {recycle_amount} to register on subnet:{netuid}?"):
             return False
 
+    # TODO Update to configured token
     with console.status(":satellite: Recycling BOOT for Registration..."):
         success, err_msg = cwtensor._do_burned_register(
             netuid=netuid,
             burn=recycle_amount.__int__(),
             wallet=wallet,
             wait_for_finalization=wait_for_finalization,
         )
```

### Comparing `cybertensor-0.1.6/cybertensor/messages/root.py` & `cybertensor-0.2.0/cybertensor/messages/root.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/serving.py` & `cybertensor-0.2.0/cybertensor/messages/serving.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,22 @@
     )
     neuron_up_to_date = not neuron.is_null and params == {
         "version": neuron.axon_info.version,
         "ip": net.ip_to_int(neuron.axon_info.ip),
         "port": neuron.axon_info.port,
         "ip_type": neuron.axon_info.ip_type,
         "netuid": neuron.netuid,
-        "hotkey": neuron.hotkey,
-        "coldkey": neuron.coldkey,
+        # "hotkey": neuron.hotkey,
+        # "coldkey": neuron.coldkey,
         "protocol": neuron.axon_info.protocol,
         "placeholder1": neuron.axon_info.placeholder1,
         "placeholder2": neuron.axon_info.placeholder2,
     }
-    output = params.copy()
-    output["coldkey"] = wallet.coldkeypub.address
-    output["hotkey"] = wallet.hotkey.address
     if neuron_up_to_date:
-        cybertensor.logging.debug(
+        cybertensor.logging.info(
             f"Axon already served on: AxonInfo({wallet.hotkey.address},{ip}:{port}) "
         )
         return True
 
     if prompt:
         output = params.copy()
         output["coldkey"] = wallet.coldkeypub.address
@@ -131,16 +128,16 @@
             )
             return True
         else:
             cybertensor.logging.debug(
                 f"Axon failed to served with error: {error_message} "
             )
             return False
-    else:
-        return True
+
+    return True
 
 
 def serve_axon_message(
     cwtensor: "cybertensor.cwtensor",
     netuid: int,
     axon: "cybertensor.axon",
     wait_for_finalization: bool = True,
@@ -165,15 +162,15 @@
     axon.wallet.hotkey
     axon.wallet.coldkeypub
     external_port = axon.external_port
 
     # ---- Get external ip ----
     if axon.external_ip is None:
         try:
-            external_ip = net.get_external_ip()
+            external_ip = cwtensor.config.axon.external_ip or net.get_external_ip()
             console.print(
                 f":white_heavy_check_mark: [green]Found external ip: {external_ip}[/green]"
             )
             cybertensor.logging.success(
                 prefix="External IP", sufix=f"<blue>{external_ip}</blue>"
             )
         except Exception as e:
```

### Comparing `cybertensor-0.1.6/cybertensor/messages/set_weights.py` & `cybertensor-0.2.0/cybertensor/messages/set_weights.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/staking.py` & `cybertensor-0.2.0/cybertensor/messages/staking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/transfer.py` & `cybertensor-0.2.0/cybertensor/messages/transfer.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/messages/unstaking.py` & `cybertensor-0.2.0/cybertensor/messages/unstaking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/metagraph.py` & `cybertensor-0.2.0/cybertensor/metagraph.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/mock/__init__.py` & `cybertensor-0.2.0/cybertensor/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/mock/cwtensor_mock.py` & `cybertensor-0.2.0/cybertensor/mock/cwtensor_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/mock/keyfile_mock.py` & `cybertensor-0.2.0/cybertensor/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/mock/wallet_mock.py` & `cybertensor-0.2.0/cybertensor/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/stream.py` & `cybertensor-0.2.0/cybertensor/stream.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/subnets.py` & `cybertensor-0.2.0/cybertensor/subnets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # The MIT License (MIT)
 # Copyright © 2021 Yuma Rao
 # Copyright © 2023 Opentensor Foundation
 # Copyright © 2023 Opentensor Technologies Inc
+# Copyright © 2024 cyber~Congress
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 # documentation files (the “Software”), to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
 # and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all copies or substantial portions of
@@ -64,15 +65,15 @@
             uid (int, optional): The specific UID of the API node to query. Defaults to None.
             **kwargs: Keyword arguments for the prepare_synapse_fn.
 
         Returns:
             Any: The result of the process_responses_fn.
         """
         synapse = self.prepare_synapse(**kwargs)
-        cybertensor.logging.debug(f"Quering valdidator axons with synapse {synapse.name}...")
+        cybertensor.logging.debug(f"Querying validator axons with synapse {synapse.name}...")
         responses = await self.dendrite(
             axons=axons,
             synapse=synapse,
             deserialize=deserialize,
             timeout=timeout,
         )
         return self.process_responses(responses)
```

### Comparing `cybertensor-0.1.6/cybertensor/synapse.py` & `cybertensor-0.2.0/cybertensor/synapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,17 @@
             status_message="Success",
             process_time=0.1,
             ip="198.123.23.1",
             port=9282,
             version=111,
             nonce=111111,
             uuid="5ecbd69c-1cec-11ee-b0dc-e29ce36fec1a",
-            hotkey="5EnjDGNqqWnuL2HCAdxeEtN2oqtXZw6BMBe936Kfy2PFz1J1",
-            signature="0x0813029319030129u4120u10841824y0182u091u230912u"
+            hotkey="pussy1tqhv59nmdwls2263gtwc86swgte20mtsqvhtrd",
+            signature="0x657a43695079644639586631434c4570593844337262684432436e3776503741495870626e656f4d6e4878426e566d61464854347274686142313155377865376d4f4e385057587856523746567a5169442f6d5757513d3d",
+            pubkey="AmET/9CWsKo3TWCg2zsaldtdgr2MLug4/yZQfxQiZafJ"
         )
 
         # Accessing TerminalInfo attributes
         ip_address = terminal_info.ip
         processing_duration = terminal_info.process_time
 
         # TerminalInfo can be used to monitor and verify network interactions, ensuring proper communication and
@@ -188,15 +189,15 @@
     _extract_process_time = pydantic.validator(
         "process_time", pre=True, allow_reuse=True
     )(cast_float)
 
     # The terminal ip.
     ip: Optional[str] = pydantic.Field(
         title="ip",
-        description="The ip of the axon recieving the request.",
+        description="The ip of the axon receiving the request.",
         examples="198.123.23.1",
         default=None,
         allow_mutation=True,
     )
 
     # The host port of the terminal.
     port: Optional[int] = pydantic.Field(
@@ -239,24 +240,33 @@
         allow_mutation=True,
     )
 
     # The cybertensor version on the terminal as an int.
     hotkey: Optional[str] = pydantic.Field(
         title="hotkey",
         description="The hotkey string of the terminal wallet.",
-        examples="5EnjDGNqqWnuL2HCAdxeEtN2oqtXZw6BMBe936Kfy2PFz1J1",
+        examples="pussy1tqhv59nmdwls2263gtwc86swgte20mtsqvhtrd",
         default=None,
         allow_mutation=True,
     )
 
     # A signature verifying the tuple (axon_nonce, axon_hotkey, dendrite_hotkey, axon_uuid)
     signature: Optional[str] = pydantic.Field(
         title="signature",
         description="A signature verifying the tuple (nonce, axon_hotkey, dendrite_hotkey, uuid)",
-        examples="0x0813029319030129u4120u10841824y0182u091u230912u",
+        examples="0x657a43695079644639586631434c4570593844337262684432436e3776503741495870626e656f4d6e4878426e566d61464854347274686142313155377865376d4f4e385057587856523746567a5169442f6d5757513d3d",
+        default=None,
+        allow_mutation=True,
+    )
+
+    # The cybertensor version on the terminal as an int.
+    pubkey: Optional[str] = pydantic.Field(
+        title="pubkey",
+        description="The hotkey pubkey string of the terminal wallet.",
+        examples="AmET/9CWsKo3TWCg2zsaldtdgr2MLug4/yZQfxQiZafJ",
         default=None,
         allow_mutation=True,
     )
 
 
 class Synapse(pydantic.BaseModel):
     """
```

### Comparing `cybertensor-0.1.6/cybertensor/tensor.py` & `cybertensor-0.2.0/cybertensor/tensor.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/threadpool.py` & `cybertensor-0.2.0/cybertensor/threadpool.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/types.py` & `cybertensor-0.2.0/cybertensor/types.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/__init__.py` & `cybertensor-0.2.0/cybertensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/_register_cuda.py` & `cybertensor-0.2.0/cybertensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/balance.py` & `cybertensor-0.2.0/cybertensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/formatting.py` & `cybertensor-0.2.0/cybertensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/networking.py` & `cybertensor-0.2.0/cybertensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/registration.py` & `cybertensor-0.2.0/cybertensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/wallet_utils.py` & `cybertensor-0.2.0/cybertensor/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/utils/weight_utils.py` & `cybertensor-0.2.0/cybertensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor/wallet.py` & `cybertensor-0.2.0/cybertensor/wallet.py`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor.egg-info/PKG-INFO` & `cybertensor-0.2.0/cybertensor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybertensor
-Version: 0.1.6
+Version: 0.2.0
 Summary: cybertensor
 Home-page: https://github.com/cybercongress/cybertensor
 Author: cyberhead
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -58,14 +58,16 @@
 Requires-Dist: tqdm
 Requires-Dist: uvicorn==0.22.0
 Requires-Dist: wheel
 Requires-Dist: cosmpy>=0.9.1
 Requires-Dist: ecdsa<0.15
 Requires-Dist: py-bip39-bindings
 Requires-Dist: urllib3==1.26.15
+Requires-Dist: websocket>=0.2.1
+Requires-Dist: websocket-client==1.7.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.2.0; extra == "dev"
 Requires-Dist: pytest-mock==3.12.0; extra == "dev"
 Requires-Dist: pytest-split==0.8.0; extra == "dev"
 Requires-Dist: pytest-xdist==3.0.2; extra == "dev"
 Requires-Dist: pytest-rerunfailures==10.2; extra == "dev"
 Requires-Dist: coveralls==3.3.1; extra == "dev"
```

### Comparing `cybertensor-0.1.6/cybertensor.egg-info/SOURCES.txt` & `cybertensor-0.2.0/cybertensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybertensor-0.1.6/cybertensor.egg-info/requires.txt` & `cybertensor-0.2.0/cybertensor.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 tqdm
 uvicorn==0.22.0
 wheel
 cosmpy>=0.9.1
 ecdsa<0.15
 py-bip39-bindings
 urllib3==1.26.15
+websocket>=0.2.1
+websocket-client==1.7.0
 
 [dev]
 pytest==7.2.0
 pytest-mock==3.12.0
 pytest-split==0.8.0
 pytest-xdist==3.0.2
 pytest-rerunfailures==10.2
```

### Comparing `cybertensor-0.1.6/requirements/prod.txt` & `cybertensor-0.2.0/requirements/prod.txt`

 * *Files 16% similar despite different names*

```diff
@@ -33,7 +33,9 @@
 tqdm
 uvicorn==0.22.0
 wheel
 cosmpy>=0.9.1
 ecdsa<0.15
 py-bip39-bindings
 urllib3==1.26.15
+websocket>=0.2.1
+websocket-client==1.7.0
```

### Comparing `cybertensor-0.1.6/setup.py` & `cybertensor-0.2.0/setup.py`

 * *Files identical despite different names*

