# Comparing `tmp/experiment-lab-1.0.5.tar.gz` & `tmp/experiment-lab-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-lab-1.0.5.tar", last modified: Sun Apr  7 19:19:33 2024, max compression
+gzip compressed data, was "experiment-lab-1.0.6.tar", last modified: Tue Apr  9 22:28:40 2024, max compression
```

## Comparing `experiment-lab-1.0.5.tar` & `experiment-lab-1.0.6.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.509651 experiment-lab-1.0.5/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.0.5/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-07 19:19:33.509432 experiment-lab-1.0.5/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.502873 experiment-lab-1.0.5/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-07 19:18:36.000000 experiment-lab-1.0.5/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.503692 experiment-lab-1.0.5/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.504147 experiment-lab-1.0.5/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.0.5/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6734 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.504572 experiment-lab-1.0.5/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.504708 experiment-lab-1.0.5/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.0.5/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.504828 experiment-lab-1.0.5/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.504931 experiment-lab-1.0.5/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.0.5/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.505137 experiment-lab-1.0.5/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.505710 experiment-lab-1.0.5/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      312 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.505952 experiment-lab-1.0.5/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.506410 experiment-lab-1.0.5/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      206 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      898 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.0.5/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1981 2024-04-03 18:52:52.000000 experiment-lab-1.0.5/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.506502 experiment-lab-1.0.5/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.0.5/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.506819 experiment-lab-1.0.5/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.507195 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.507751 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.508313 experiment-lab-1.0.5/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.0.5/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.0.5/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10429 2024-03-24 16:11:49.000000 experiment-lab-1.0.5/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.0.5/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      565 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.508702 experiment-lab-1.0.5/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.0.5/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.0.5/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-07 19:19:33.508874 experiment-lab-1.0.5/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2422 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-07 19:19:33.000000 experiment-lab-1.0.5/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.0.5/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-07 19:19:33.509685 experiment-lab-1.0.5/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.0.5/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.702095 experiment-lab-1.0.6/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.0.6/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-09 22:28:40.701917 experiment-lab-1.0.6/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.695268 experiment-lab-1.0.6/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.696107 experiment-lab-1.0.6/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.696572 experiment-lab-1.0.6/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.0.6/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6734 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.696984 experiment-lab-1.0.6/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.697106 experiment-lab-1.0.6/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.0.6/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.697214 experiment-lab-1.0.6/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.697307 experiment-lab-1.0.6/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.0.6/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.697516 experiment-lab-1.0.6/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.698077 experiment-lab-1.0.6/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      444 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.698291 experiment-lab-1.0.6/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.698811 experiment-lab-1.0.6/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      206 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3331 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1249 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.0.6/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.698912 experiment-lab-1.0.6/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.0.6/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.699220 experiment-lab-1.0.6/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.699658 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.700184 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.700776 experiment-lab-1.0.6/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10429 2024-03-24 16:11:49.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.0.6/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.701197 experiment-lab-1.0.6/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.0.6/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.0.6/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:28:40.701355 experiment-lab-1.0.6/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-09 22:28:40.000000 experiment-lab-1.0.6/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.0.6/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-09 22:28:40.702130 experiment-lab-1.0.6/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.0.6/setup.py
```

### Comparing `experiment-lab-1.0.5/LICENCE` & `experiment-lab-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/PKG-INFO` & `experiment-lab-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.5
+Version: 1.0.6
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.5/README.md` & `experiment-lab-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/networks/blocks.py` & `experiment-lab-1.0.6/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/networks/mlp.py` & `experiment-lab-1.0.6/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/networks/network.py` & `experiment-lab-1.0.6/experiment_lab/common/networks/network.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/resolvers/__init__.py` & `experiment-lab-1.0.6/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/resolvers/list_resolvers.py` & `experiment-lab-1.0.6/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/common/utils/__init__.py` & `experiment-lab-1.0.6/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment-lab-1.0.6/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/configs/rl/walker.yaml` & `experiment-lab-1.0.6/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment-lab-1.0.6/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/core/base_experiment.py` & `experiment-lab-1.0.6/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/core/runner.py` & `experiment-lab-1.0.6/experiment_lab/core/runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 from typing import Any, Callable, Type, Sequence
 import hydra
 from omegaconf import DictConfig, OmegaConf
 
 import experiment_lab
 from experiment_lab.common.resolvers import register_resolvers
+from experiment_lab.core.base_analysis import BaseAnalysis
 from experiment_lab.core.base_config import BaseConfig, register_configs
 from experiment_lab.core.base_experiment import BaseExperiment
 
 root_config_folder = f"{os.path.dirname(experiment_lab.__file__)}/configs"
 
 
 def run_experiment(
     experiment_cls: Type[BaseExperiment],
     config_cls: Type[BaseConfig] = BaseConfig,
+    analysis_cls: Type[BaseAnalysis] | None = None,
     register_configs: Callable[[], None] = register_configs,
     register_resolvers: Callable[[], None] = register_resolvers,
     config_path: str = root_config_folder,
     config_name: str = "config",
-) -> Sequence[Any]:
+) -> Any:
     """The main entrypoint to collect all the hydra config and run the experiment.
 
     Args:
         experiment_cls (Type[BaseExperiment]): The experiment class.
         config_cls (Type[BaseConfig], optional): The config class. Defaults to BaseConfig.
         register_configs (Callable[[], None], optional): The function to register any configs. Defaults to register_configs.
         register_resolvers (Callable[[], None], optional): The function to register any resolvers. Defaults to register_resolvers.
@@ -37,14 +39,20 @@
     """
     register_resolvers()
     register_configs()
 
     config_path = os.path.join(os.getcwd(), config_path)
 
     @hydra.main(config_path=config_path, config_name=config_name, version_base=None)
-    def main(dict_cfg: DictConfig) -> Sequence[Any]:
+    def main(dict_cfg: DictConfig) -> Any:
         OmegaConf.resolve(dict_cfg)
         cfg: config_cls = OmegaConf.to_object(dict_cfg)  # type: ignore
-        e = experiment_cls(cfg)
-        return e.run()
+        if cfg.run_analysis:
+            if analysis_cls is None:
+                raise ValueError("Analysis class not provided!")
+            a = analysis_cls(cfg)
+            return a._analyze_wrapper()
+        else:
+            e = experiment_cls(cfg)
+            return e.run()
 
     return main()
```

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment-lab-1.0.6/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/examples/random_waits.py` & `experiment-lab-1.0.6/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/config.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/monte_carlo/main.py` & `experiment-lab-1.0.6/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/rl/config.py` & `experiment-lab-1.0.6/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/rl/environment.py` & `experiment-lab-1.0.6/experiment_lab/experiments/rl/environment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/rl/experiment.py` & `experiment-lab-1.0.6/experiment_lab/experiments/rl/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/supervised/config.py` & `experiment-lab-1.0.6/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/supervised/experiment.py` & `experiment-lab-1.0.6/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab/experiments/supervised/main.py` & `experiment-lab-1.0.6/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/experiment_lab.egg-info/PKG-INFO` & `experiment-lab-1.0.6/experiment_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.5
+Version: 1.0.6
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.5/experiment_lab.egg-info/SOURCES.txt` & `experiment-lab-1.0.6/experiment_lab.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 experiment_lab/configs/rl/cartpole.yaml
 experiment_lab/configs/rl/config.yaml
 experiment_lab/configs/rl/crossing.yaml
 experiment_lab/configs/rl/walker.yaml
 experiment_lab/configs/supervised/config.yaml
 experiment_lab/configs/supervised/fashion_mnist.yaml
 experiment_lab/core/__init__.py
+experiment_lab/core/base_analysis.py
 experiment_lab/core/base_config.py
 experiment_lab/core/base_experiment.py
 experiment_lab/core/runner.py
 experiment_lab/experiments/__init__.py
 experiment_lab/experiments/examples/__init__.py
 experiment_lab/experiments/examples/mc_pi_estimate.py
 experiment_lab/experiments/examples/random_waits.py
@@ -44,14 +45,15 @@
 experiment_lab/experiments/monte_carlo/main.py
 experiment_lab/experiments/monte_carlo/components/__init__.py
 experiment_lab/experiments/monte_carlo/components/aggregators.py
 experiment_lab/experiments/monte_carlo/components/post_processors.py
 experiment_lab/experiments/monte_carlo/components/sample_filters.py
 experiment_lab/experiments/monte_carlo/components/samplers.py
 experiment_lab/experiments/rl/__init__.py
+experiment_lab/experiments/rl/analysis.py
 experiment_lab/experiments/rl/config.py
 experiment_lab/experiments/rl/environment.py
 experiment_lab/experiments/rl/experiment.py
 experiment_lab/experiments/rl/main.py
 experiment_lab/experiments/supervised/__init__.py
 experiment_lab/experiments/supervised/config.py
 experiment_lab/experiments/supervised/experiment.py
```

### Comparing `experiment-lab-1.0.5/pyproject.toml` & `experiment-lab-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.5/setup.py` & `experiment-lab-1.0.6/setup.py`

 * *Files identical despite different names*

