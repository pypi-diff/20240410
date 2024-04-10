# Comparing `tmp/RL_OM-0.7.91.tar.gz` & `tmp/RL_OM-0.7.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.7.91.tar", last modified: Wed Apr 10 15:54:03 2024, max compression
+gzip compressed data, was "RL_OM-0.7.92.tar", last modified: Wed Apr 10 15:56:33 2024, max compression
```

## Comparing `RL_OM-0.7.91.tar` & `RL_OM-0.7.92.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.238142 RL_OM-0.7.91/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.91/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.91/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 15:54:03.238005 RL_OM-0.7.91/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.91/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.229077 RL_OM-0.7.91/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.91/RL_OM/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)       23 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.91/RL_OM/_modidx 2.py
--rw-r--r--   0 magnus     (501) staff       (20)   240779 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.230149 RL_OM-0.7.91/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.232122 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/PPO_SB3.py
--rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/PPO_TEMP.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/cbs.py
--rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/eoq.py
--rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents.py
--rw-r--r--   0 magnus     (501) staff       (20)    60708 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
--rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
--rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/qr.py
--rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/saa.py
--rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/benchmark_agents/ss.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.232645 RL_OM-0.7.91/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.233028 RL_OM-0.7.91/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1162 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     6401 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.233889 RL_OM-0.7.91/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.234759 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.236070 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
--rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.236766 RL_OM-0.7.91/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    16847 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    43430 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.237058 RL_OM-0.7.91/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.237772 RL_OM-0.7.91/RL_OM/utils/
--rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/utils/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:53:52.000000 RL_OM-0.7.91/RL_OM/utils/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-04-10 15:53:51.000000 RL_OM-0.7.91/RL_OM/utils/utils.py
--rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.91/RL_OM/utils.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:54:03.230019 RL_OM-0.7.91/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.91/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2024-04-10 15:54:03.000000 RL_OM-0.7.91/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      990 2024-04-10 15:54:00.000000 RL_OM-0.7.91/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2024-04-10 15:54:03.238190 RL_OM-0.7.91/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.91/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.376027 RL_OM-0.7.92/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.92/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.92/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 15:56:33.375890 RL_OM-0.7.92/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.92/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.367049 RL_OM-0.7.92/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.92/RL_OM/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)       23 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.92/RL_OM/_modidx 2.py
+-rw-r--r--   0 magnus     (501) staff       (20)   240779 2024-04-10 15:56:16.000000 RL_OM-0.7.92/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.368175 RL_OM-0.7.92/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.370082 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/PPO_SB3.py
+-rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/PPO_TEMP.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/cbs.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents.py
+-rw-r--r--   0 magnus     (501) staff       (20)    60659 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
+-rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/qr.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/saa.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/benchmark_agents/ss.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.370643 RL_OM-0.7.92/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.371068 RL_OM-0.7.92/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1162 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6401 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.371933 RL_OM-0.7.92/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.372818 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.374175 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.374951 RL_OM-0.7.92/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16847 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    43430 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.375252 RL_OM-0.7.92/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.375695 RL_OM-0.7.92/RL_OM/utils/
+-rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/utils/MLtools.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/utils/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-04-10 15:56:15.000000 RL_OM-0.7.92/RL_OM/utils/utils.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.92/RL_OM/utils.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-10 15:56:33.368038 RL_OM-0.7.92/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.92/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2024-04-10 15:56:33.000000 RL_OM-0.7.92/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      990 2024-04-10 15:56:29.000000 RL_OM-0.7.92/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2024-04-10 15:56:33.376073 RL_OM-0.7.92/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.92/setup.py
```

### Comparing `RL_OM-0.7.91/LICENSE` & `RL_OM-0.7.92/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/PKG-INFO` & `RL_OM-0.7.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.7.91
+Version: 0.7.92
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.91/RL_OM/MLtools.py` & `RL_OM-0.7.92/RL_OM/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/_modidx 2.py` & `RL_OM-0.7.92/RL_OM/_modidx 2.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/_modidx.py` & `RL_OM-0.7.92/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/PPO_SB3.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/PPO_SB3.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/cbs.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/cbs.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/mp_agents_ERM.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/mp_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_ERM.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_ERM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1612,17 +1612,14 @@
         
         for i in X:
             if np.isnan(i).any():
                 print("nan values in input")
                 raise ValueError("NaN values in Input")
             break
 
-        print(X.shape)
-        sleep(1)
-        
         action = self.predict(X)
 
         if np.isnan(action).any():
             print("nan values in action")
             raise ValueError("NaN values in Output")
 
         return action
```

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_SAA.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_SAA.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/qr.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/qr.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/saa.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/saa.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/benchmark_agents/ss.py` & `RL_OM-0.7.92/RL_OM/agents/benchmark_agents/ss.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/networks/actors.py` & `RL_OM-0.7.92/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/networks/base.py` & `RL_OM-0.7.92/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/networks/critics.py` & `RL_OM-0.7.92/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.7.92/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/processors/processors.py` & `RL_OM-0.7.92/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.7.92/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/environments/calculation_functions.py` & `RL_OM-0.7.92/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/environments/data_generators.py` & `RL_OM-0.7.92/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/environments/feature_converters.py` & `RL_OM-0.7.92/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.7.92/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.7.92/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/utils/MLtools.py` & `RL_OM-0.7.92/RL_OM/utils/MLtools.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/utils/utils.py` & `RL_OM-0.7.92/RL_OM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM/utils.py` & `RL_OM-0.7.92/RL_OM/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.7.92/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.7.91
+Version: 0.7.92
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.91/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.7.92/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.91/settings.ini` & `RL_OM-0.7.92/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.7.91
+version = 0.7.92
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.7.91/setup.py` & `RL_OM-0.7.92/setup.py`

 * *Files identical despite different names*

