# Comparing `tmp/experiment-lab-1.0.7.tar.gz` & `tmp/experiment-lab-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-lab-1.0.7.tar", last modified: Tue Apr  9 22:35:58 2024, max compression
+gzip compressed data, was "experiment-lab-1.0.8.tar", last modified: Wed Apr 10 14:32:33 2024, max compression
```

## Comparing `experiment-lab-1.0.7.tar` & `experiment-lab-1.0.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.458776 experiment-lab-1.0.7/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.0.7/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-09 22:35:58.458545 experiment-lab-1.0.7/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.452201 experiment-lab-1.0.7/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-09 22:35:22.000000 experiment-lab-1.0.7/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.453004 experiment-lab-1.0.7/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.453425 experiment-lab-1.0.7/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.0.7/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6734 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.453749 experiment-lab-1.0.7/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.453855 experiment-lab-1.0.7/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.0.7/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.453948 experiment-lab-1.0.7/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.454061 experiment-lab-1.0.7/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.0.7/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.454267 experiment-lab-1.0.7/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.454763 experiment-lab-1.0.7/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      444 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.454951 experiment-lab-1.0.7/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.455454 experiment-lab-1.0.7/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-09 22:35:13.000000 experiment-lab-1.0.7/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3331 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/core/base_analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1249 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.0.7/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.455562 experiment-lab-1.0.7/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.0.7/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.455846 experiment-lab-1.0.7/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.456269 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.456796 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.457424 experiment-lab-1.0.7/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10429 2024-03-24 16:11:49.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.0.7/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.457851 experiment-lab-1.0.7/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.0.7/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.0.7/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-09 22:35:58.457988 experiment-lab-1.0.7/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-09 22:35:58.000000 experiment-lab-1.0.7/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.0.7/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-09 22:35:58.458816 experiment-lab-1.0.7/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.0.7/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.091386 experiment-lab-1.0.8/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.0.8/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-10 14:32:33.091168 experiment-lab-1.0.8/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.084476 experiment-lab-1.0.8/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-10 14:31:57.000000 experiment-lab-1.0.8/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.085310 experiment-lab-1.0.8/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.085809 experiment-lab-1.0.8/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.0.8/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6734 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.086174 experiment-lab-1.0.8/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.086289 experiment-lab-1.0.8/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.0.8/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.086392 experiment-lab-1.0.8/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.086507 experiment-lab-1.0.8/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.0.8/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.086709 experiment-lab-1.0.8/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.087390 experiment-lab-1.0.8/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      472 2024-04-10 14:31:57.000000 experiment-lab-1.0.8/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.087634 experiment-lab-1.0.8/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.088152 experiment-lab-1.0.8/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-09 22:37:45.000000 experiment-lab-1.0.8/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3727 2024-04-10 14:31:57.000000 experiment-lab-1.0.8/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1285 2024-04-10 14:31:57.000000 experiment-lab-1.0.8/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.0.8/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.0.8/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.088247 experiment-lab-1.0.8/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.0.8/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.088552 experiment-lab-1.0.8/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.088949 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.089424 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.090034 experiment-lab-1.0.8/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10429 2024-03-24 16:11:49.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.0.8/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.090410 experiment-lab-1.0.8/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.0.8/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.0.8/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:32:33.090543 experiment-lab-1.0.8/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-10 14:32:33.000000 experiment-lab-1.0.8/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.0.8/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-10 14:32:33.091421 experiment-lab-1.0.8/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.0.8/setup.py
```

### Comparing `experiment-lab-1.0.7/LICENCE` & `experiment-lab-1.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/PKG-INFO` & `experiment-lab-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.7
+Version: 1.0.8
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.7/README.md` & `experiment-lab-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/networks/blocks.py` & `experiment-lab-1.0.8/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/networks/mlp.py` & `experiment-lab-1.0.8/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/networks/network.py` & `experiment-lab-1.0.8/experiment_lab/common/networks/network.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/resolvers/__init__.py` & `experiment-lab-1.0.8/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/resolvers/list_resolvers.py` & `experiment-lab-1.0.8/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/common/utils/__init__.py` & `experiment-lab-1.0.8/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment-lab-1.0.8/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/configs/rl/walker.yaml` & `experiment-lab-1.0.8/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment-lab-1.0.8/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/core/base_analysis.py` & `experiment-lab-1.0.8/experiment_lab/core/base_analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,17 +64,25 @@
         )
 
         full_df = []
 
         configs = {}
 
         for wandb_run in tqdm.tqdm(wandb_runs):
-            df = pd.DataFrame(
-                wandb_run.scan_history(keys=self.cfg.analysis.wandb_keys),
-            )
+            if self.cfg.analysis.all_keys_per_step:
+                df = pd.DataFrame(
+                    wandb_run.scan_history(keys=self.cfg.analysis.wandb_keys),
+                )
+            else:
+                df = pd.DataFrame()
+                for key in self.cfg.analysis.wandb_keys:
+                    temp_df = pd.DataFrame(
+                        wandb_run.scan_history(keys=[key]),
+                    )
+                    df = pd.merge(df, temp_df, left_index=True, right_index=True, how='outer')
             df["experiment_id"] = wandb_run.config["experiment_id"]
             df["run_id"] = wandb_run.id
             if wandb_run.config["experiment_id"] not in configs:
                 configs[wandb_run.config["experiment_id"]] = wandb_run.config
             if self.cfg.analysis.index is not None:
                 df.set_index(
                     ["experiment_id", "run_id", self.cfg.analysis.index], inplace=True
```

### Comparing `experiment-lab-1.0.7/experiment_lab/core/base_config.py` & `experiment-lab-1.0.8/experiment_lab/core/base_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @dataclass
 class AnalysisConfig:
     """Config for analysis of this experiment."""
 
     filters: List[Dict] = field(default_factory=lambda: [])
     wandb_keys: List[str] = field(default_factory=lambda: [])
     index: str | None = None
+    all_keys_per_step: bool = False
 
 
 @dataclass
 class BaseConfig:
     """Basic configuration for general experiment runs."""
 
     experiment_name: str | None = None
```

### Comparing `experiment-lab-1.0.7/experiment_lab/core/base_experiment.py` & `experiment-lab-1.0.8/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/core/runner.py` & `experiment-lab-1.0.8/experiment_lab/core/runner.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment-lab-1.0.8/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/examples/random_waits.py` & `experiment-lab-1.0.8/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/config.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/monte_carlo/main.py` & `experiment-lab-1.0.8/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/rl/analysis.py` & `experiment-lab-1.0.8/experiment_lab/experiments/rl/analysis.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/rl/config.py` & `experiment-lab-1.0.8/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/rl/environment.py` & `experiment-lab-1.0.8/experiment_lab/experiments/rl/environment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/rl/experiment.py` & `experiment-lab-1.0.8/experiment_lab/experiments/rl/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/rl/main.py` & `experiment-lab-1.0.8/experiment_lab/experiments/rl/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/supervised/config.py` & `experiment-lab-1.0.8/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/supervised/experiment.py` & `experiment-lab-1.0.8/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab/experiments/supervised/main.py` & `experiment-lab-1.0.8/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/experiment_lab.egg-info/PKG-INFO` & `experiment-lab-1.0.8/experiment_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.7
+Version: 1.0.8
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.7/experiment_lab.egg-info/SOURCES.txt` & `experiment-lab-1.0.8/experiment_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/pyproject.toml` & `experiment-lab-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.7/setup.py` & `experiment-lab-1.0.8/setup.py`

 * *Files identical despite different names*

