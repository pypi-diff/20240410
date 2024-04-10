# Comparing `tmp/seml-0.4.3.tar.gz` & `tmp/seml-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seml-0.4.3.tar", last modified: Fri Mar  1 10:42:33 2024, max compression
+gzip compressed data, was "seml-0.4.4.tar", last modified: Tue Apr  9 14:50:20 2024, max compression
```

## Comparing `seml-0.4.3.tar` & `seml-0.4.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.627721 seml-0.4.3/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1135 2023-09-19 07:51:23.000000 seml-0.4.3/LICENSE
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      183 2024-03-01 09:42:10.000000 seml-0.4.3/MANIFEST.in
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6545 2024-03-01 10:42:33.623721 seml-0.4.3/PKG-INFO
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     3892 2024-03-01 09:42:11.000000 seml-0.4.3/README.md
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1431 2024-03-01 10:41:26.000000 seml-0.4.3/pyproject.toml
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)       38 2024-03-01 10:42:33.627721 seml-0.4.3/setup.cfg
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.563722 seml-0.4.3/src/
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.607721 seml-0.4.3/src/seml/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      747 2024-02-12 17:39:39.000000 seml-0.4.3/src/seml/__init__.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    34121 2024-03-01 10:41:18.000000 seml-0.4.3/src/seml/__main__.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    13861 2024-02-27 09:49:18.000000 seml-0.4.3/src/seml/add.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    30938 2024-02-12 17:39:39.000000 seml-0.4.3/src/seml/config.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1427 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/configure.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1686 2024-02-13 07:47:05.000000 seml-0.4.3/src/seml/console.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    11781 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/database.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7327 2024-02-12 17:39:39.000000 seml-0.4.3/src/seml/description.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1030 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/errors.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2893 2024-02-27 09:35:35.000000 seml-0.4.3/src/seml/evaluation.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7975 2024-02-27 10:41:48.000000 seml-0.4.3/src/seml/experiment.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     9015 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/json.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    46116 2024-02-27 12:20:58.000000 seml-0.4.3/src/seml/manage.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    11371 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/mattermost_observer.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      635 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/module_hider.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1509 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/network.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6324 2024-02-12 17:39:39.000000 seml-0.4.3/src/seml/observers.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    10803 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/parameters.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4210 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/prepare_experiment.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6013 2024-03-01 10:41:18.000000 seml-0.4.3/src/seml/project.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     5567 2024-03-01 10:41:18.000000 seml-0.4.3/src/seml/settings.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7083 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/sources.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    42129 2024-02-29 09:55:40.000000 seml-0.4.3/src/seml/start.py
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.563722 seml-0.4.3/src/seml/templates/
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.619722 seml-0.4.3/src/seml/templates/slurm/
--rwxr-xr-x   0 gaoni    (10028) tumuser  (20909)      647 2023-09-19 07:51:24.000000 seml-0.4.3/src/seml/templates/slurm/jupyter_template.sh
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2042 2024-02-13 07:29:32.000000 seml-0.4.3/src/seml/templates/slurm/slurm_template.sh
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      253 2024-01-26 21:46:29.000000 seml-0.4.3/src/seml/typer.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    17301 2024-02-29 11:47:18.000000 seml-0.4.3/src/seml/utils.py
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-03-01 10:42:33.623721 seml-0.4.3/src/seml.egg-info/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6545 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/PKG-INFO
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      859 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/SOURCES.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)        1 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/dependency_links.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)       44 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/entry_points.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      241 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/requires.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)        5 2024-03-01 10:42:33.000000 seml-0.4.3/src/seml.egg-info/top_level.txt
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.729006 seml-0.4.4/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1135 2023-09-19 07:51:23.000000 seml-0.4.4/LICENSE
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      183 2024-03-01 09:42:10.000000 seml-0.4.4/MANIFEST.in
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6930 2024-04-09 14:50:20.729006 seml-0.4.4/PKG-INFO
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4163 2024-04-09 14:39:51.000000 seml-0.4.4/README.md
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1468 2024-04-09 14:49:42.000000 seml-0.4.4/pyproject.toml
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)       38 2024-04-09 14:50:20.729006 seml-0.4.4/setup.cfg
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.673007 seml-0.4.4/src/
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.713007 seml-0.4.4/src/seml/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1201 2024-03-19 10:39:23.000000 seml-0.4.4/src/seml/__init__.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    34241 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/__main__.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    13861 2024-03-11 16:09:35.000000 seml-0.4.4/src/seml/add.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    30912 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/config.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2220 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/configure.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     3289 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/console.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    14313 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/database.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7370 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/description.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1030 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/errors.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2892 2024-03-19 10:39:24.000000 seml-0.4.4/src/seml/evaluation.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7975 2024-02-27 10:41:48.000000 seml-0.4.4/src/seml/experiment.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     9015 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/json.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    46239 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/manage.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    11371 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/mattermost_observer.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      635 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/module_hider.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1509 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/network.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6324 2024-02-12 17:39:39.000000 seml-0.4.4/src/seml/observers.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    10803 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/parameters.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4210 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/prepare_experiment.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6020 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/project.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     5786 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/settings.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     8014 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/sources.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    43616 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/start.py
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.673007 seml-0.4.4/src/seml/templates/
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.725006 seml-0.4.4/src/seml/templates/slurm/
+-rwxr-xr-x   0 gaoni    (10028) tumuser  (20909)      647 2023-09-19 07:51:24.000000 seml-0.4.4/src/seml/templates/slurm/jupyter_template.sh
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2042 2024-02-13 07:29:32.000000 seml-0.4.4/src/seml/templates/slurm/slurm_template.sh
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      253 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/typer.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    17301 2024-03-11 15:10:43.000000 seml-0.4.4/src/seml/utils.py
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.725006 seml-0.4.4/src/seml.egg-info/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6930 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/PKG-INFO
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      859 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/SOURCES.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)        1 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/dependency_links.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)       44 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/entry_points.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      279 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/requires.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)        5 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/top_level.txt
```

### Comparing `seml-0.4.3/LICENSE` & `seml-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/PKG-INFO` & `seml-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seml
-Version: 0.4.3
+Version: 0.4.4
 Summary: Slurm Experiment Management Library
 Author: DAML Group @ TUM
 Author-email: Daniel Zügner <zuegnerd@in.tum.de>, Johannes Gsteiger <johannes.gasteiger@tum.de>, Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 Maintainer-email: Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Johannes Klicpera, Daniel Zügner, Nicholas Gao
@@ -39,36 +39,38 @@
 Requires-Dist: numpy>=1.15
 Requires-Dist: pymongo>=3.11
 Requires-Dist: pandas
 Requires-Dist: sacred>=0.8.4
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: jsonpickle>=2.2
 Requires-Dist: munch>=2.0.4
-Requires-Dist: tqdm>=4.36
 Requires-Dist: debugpy>=1.2.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: typer<1.0,>=0.9
 Requires-Dist: rich<14.0,>=13.0
 Requires-Dist: omegaconf<3.0,>=2.3.0
 Requires-Dist: gitignore_parser>=0.1.11
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: ssh-forward
+Requires-Dist: sshtunnel>=0.4.0; extra == "ssh-forward"
+Requires-Dist: filelock>=3.13.3; extra == "ssh-forward"
 
 ![Github Actions](https://github.com/TUM-DAML/seml/workflows/Test/badge.svg)
 
 # `SEML`: Slurm Experiment Management Library
 **`SEML`** is the missing link between the open-source workload scheduling system `Slurm`, the experiment management tool `sacred`, and a `MongoDB` experiment database. It is lightweight, hackable, written in pure Python, and scales to thousands of experiments.
 
 Keeping track of computational experiments can be annoying and failure to do so can lead to lost results, duplicate running of the same experiments, and lots of headaches.
 While workload scheduling systems such as [`Slurm`](https://slurm.schedmd.com/overview.html) make it easy to run many experiments in parallel on a cluster, it can be hard to keep track of which parameter configurations are running, failed, or completed.
 [`sacred`](https://github.com/IDSIA/sacred) is a great tool to collect and manage experiments and their results, especially when used with a [`MongoDB`](https://www.mongodb.com/). However, it is lacking integration with workload schedulers.
 
-**`SEML`** enables you to 
+**`SEML`** enables you to
 * very easily define hyperparameter search spaces using YAML files,
 * run these hyperparameter configurations on a compute cluster using `Slurm`,
 * and to track the experimental results using `sacred` and `MongoDB`.
 
 
 In addition, **`SEML`** offers many more features to make your life easier, such as
 * automatically saving and loading your source code for reproducibility,
@@ -84,32 +86,43 @@
 ```
 or `conda` (the conda version may be outdated, we highly recommend the pypi version!):
 ```bash
 conda install -c conda-forge seml
 ```
 Then configure your MongoDB via:
 ```bash
-seml configure  --mongodb # provide your MongoDB credentials
+seml configure
 ```
 For convenience, you may create your first **`SEML`** project via:
 ```bash
 # initialize the default template in the 'new_project' folder.
 seml project init -t default new_project
 ```
 in an empty directoy. **`SEML`** will automatically create a python package for you.
 
+
+### SSH Port Forwarding
+If your MongoDB is only accessible via an SSH port forward, **`SEML`** allows you to directly configure this as well if you install the `ssh_forward` dependencies via:
+```bash
+pip install seml[ssh_forward]
+```
+It remains to configure the SSH settings:
+```bash
+seml configure --ssh_forward
+```
+
 ### Development
 If you want to develop `seml` please clone the repository and install it via
 ```bash
 pip install -e .[dev]
 ```
 and install pre-commit hooks via
 ```bash
 pre-commit install
-``` 
+```
 
 ## Documentation
 Documentation is available in our [docs.md](docs.md) or via the CLI:
 ```python
 seml --help
 ```
```

### Comparing `seml-0.4.3/README.md` & `seml-0.4.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # `SEML`: Slurm Experiment Management Library
 **`SEML`** is the missing link between the open-source workload scheduling system `Slurm`, the experiment management tool `sacred`, and a `MongoDB` experiment database. It is lightweight, hackable, written in pure Python, and scales to thousands of experiments.
 
 Keeping track of computational experiments can be annoying and failure to do so can lead to lost results, duplicate running of the same experiments, and lots of headaches.
 While workload scheduling systems such as [`Slurm`](https://slurm.schedmd.com/overview.html) make it easy to run many experiments in parallel on a cluster, it can be hard to keep track of which parameter configurations are running, failed, or completed.
 [`sacred`](https://github.com/IDSIA/sacred) is a great tool to collect and manage experiments and their results, especially when used with a [`MongoDB`](https://www.mongodb.com/). However, it is lacking integration with workload schedulers.
 
-**`SEML`** enables you to 
+**`SEML`** enables you to
 * very easily define hyperparameter search spaces using YAML files,
 * run these hyperparameter configurations on a compute cluster using `Slurm`,
 * and to track the experimental results using `sacred` and `MongoDB`.
 
 
 In addition, **`SEML`** offers many more features to make your life easier, such as
 * automatically saving and loading your source code for reproducibility,
@@ -27,32 +27,43 @@
 ```
 or `conda` (the conda version may be outdated, we highly recommend the pypi version!):
 ```bash
 conda install -c conda-forge seml
 ```
 Then configure your MongoDB via:
 ```bash
-seml configure  --mongodb # provide your MongoDB credentials
+seml configure
 ```
 For convenience, you may create your first **`SEML`** project via:
 ```bash
 # initialize the default template in the 'new_project' folder.
 seml project init -t default new_project
 ```
 in an empty directoy. **`SEML`** will automatically create a python package for you.
 
+
+### SSH Port Forwarding
+If your MongoDB is only accessible via an SSH port forward, **`SEML`** allows you to directly configure this as well if you install the `ssh_forward` dependencies via:
+```bash
+pip install seml[ssh_forward]
+```
+It remains to configure the SSH settings:
+```bash
+seml configure --ssh_forward
+```
+
 ### Development
 If you want to develop `seml` please clone the repository and install it via
 ```bash
 pip install -e .[dev]
 ```
 and install pre-commit hooks via
 ```bash
 pre-commit install
-``` 
+```
 
 ## Documentation
 Documentation is available in our [docs.md](docs.md) or via the CLI:
 ```python
 seml --help
 ```
```

### Comparing `seml-0.4.3/pyproject.toml` & `seml-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "seml"
-version = "0.4.3"
+version = "0.4.4"
 description = "Slurm Experiment Management Library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Daniel Zügner", email = "zuegnerd@in.tum.de" },
     { name = "Johannes Gsteiger", email = "johannes.gasteiger@tum.de" },
@@ -22,25 +22,25 @@
     "numpy>=1.15",
     "pymongo>=3.11",
     "pandas",
     "sacred>=0.8.4",
     "pyyaml>=5.1",
     "jsonpickle>=2.2",
     "munch>=2.0.4",
-    "tqdm>=4.36",
     "debugpy>=1.2.1",
     "requests>=2.28.1",
     "typer>=0.9, <1.0",
     "rich>=13.0, <14.0",
     "omegaconf>=2.3.0, <3.0",
     "gitignore_parser>=0.1.11",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "ruff", "pre-commit"]
+ssh_forward = ["sshtunnel>=0.4.0", "filelock>=3.13.3"]
 
 [tool.ruff.format]
 quote-style = "single"
 line-ending = "lf"
 
 [project.urls]
 Homepage = "https://github.com/TUM-DAML/seml"
```

### Comparing `seml-0.4.3/src/seml/__main__.py` & `seml-0.4.4/src/seml/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,35 +352,28 @@
     clean_unreferenced_artifacts(ctx.obj['collection'], yes=yes)
 
 
 @app.command('configure')
 @restrict_collection(False)
 def configure_command(
     ctx: typer.Context,
-    all: Annotated[
+    ssh_forward: Annotated[
         bool,
         typer.Option(
-            '-a',
-            '--all',
-            help='Configure all SEML settings',
+            '-sf',
+            '--ssh-forward',
+            help='Configure SSH forwarding settings for MongoDB.',
             is_flag=True,
         ),
     ] = False,
-    mongodb: Annotated[
-        bool,
-        typer.Option(
-            help='Configure MongoDB settings',
-            is_flag=True,
-        ),
-    ] = True,
 ):
     """
     Configure SEML (database, argument completion, ...).
     """
-    configure(all=all, mongodb=mongodb)
+    configure(all=False, mongodb=True, setup_ssh_forward=ssh_forward)
 
 
 @app.command('start-jupyter')
 @restrict_collection(False)
 def start_jupyter_command(
     ctx: typer.Context,
     lab: Annotated[
@@ -1169,16 +1162,23 @@
 
 def main():
     # We have to split the arguments manually to get proper chaining.
     # If we were to use typer built-in chaining, lists would end the chain.
     for args in split_args(sys.argv[1:], command_tree(app))[0]:
         # The app will typically exit after running once.
         # We want to run it multiple times, so we catch the SystemExit exception.
+        from seml.console import console
+
         try:
-            app(args)
+            if len(args) >= 2:
+                cmd = args[1]
+            else:
+                cmd = None
+            with console.status(f'Running command: {cmd}'):
+                app(args)
         except SystemExit as e:
             if e.code == 0:
                 continue
             else:
                 raise e
```

### Comparing `seml-0.4.3/src/seml/add.py` & `seml-0.4.4/src/seml/add.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/config.py` & `seml-0.4.4/src/seml/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,15 @@
         create_scaffolding,
         gather_ingredients_topological,
         distribute_config_updates,
         get_configuration,
         get_scaffolding_and_config_name,
         distribute_presets,
     )
-    from rich.progress import track
+    from seml.console import track
 
     configs_resolved = []
     if named_configs is None:
         named_configs = [()] * len(configs)
     for config, named_config in track(
         list(zip(configs, named_configs)),
         description='Resolving configurations',
@@ -558,15 +558,15 @@
         raise ExecutableError(
             f"Found more than 1 Sacred experiment in '{executable}'. "
             f"Can't resolve configs."
         )
     exp = exps[0]
     if not isinstance(exp, Experiment):
         logging.warn(
-            'The use of sacred.Experiemnt is deprecated. Please use seml.experiment.Experiment instead.\n'
+            'The use of sacred.Experiment is deprecated. Please use seml.experiment.Experiment instead.\n'
             'seml.experiment.Experiment already includes typical MongoDB observer and logging setups.\n'
             'Please familiar yourself with the new API and adjust your code accordingly.\n'
             'See https://github.com/TUM-DAML/seml/blob/master/examples/example_experiment.py'
         )
     with working_directory(working_dir):
         return _sacred_create_configs(exp, configs, named_configs)
 
@@ -612,21 +612,19 @@
 
     captured_args = {
         sacred.utils.join_paths(cf.prefix, n)
         for cf in exp.captured_functions
         for n in cf.signature.arguments
     }
 
-    config_keys_empty_run = flatten(empty_run.config).keys()
+    config_keys_empty_run = set(flatten(empty_run.config).keys())
 
     for config in configs:
         config_flat = flatten(config)
-        config_keys_added = {
-            k for k in config_flat.keys() if k not in config_keys_empty_run
-        }
+        config_keys_added = set(config_flat.keys()).difference(config_keys_empty_run)
 
         # Check for unused arguments
         for conf in sorted(config_keys_added):
             if not (set(sacred.utils.iter_prefixes(conf)) & captured_args):
                 raise sacred.utils.ConfigAddedError(
                     conf,
                     config={
```

### Comparing `seml-0.4.3/src/seml/database.py` & `seml-0.4.4/src/seml/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
+import random
+import time
 from typing import List
 
+import yaml
+
 from seml.errors import MongoDBError
 from seml.settings import SETTINGS
-from seml.typer import prompt
 from seml.utils import s_if
 
 States = SETTINGS.STATES
 
 
 def get_collection(collection_name, mongodb_config=None, suffix=None):
     if mongodb_config is None:
@@ -15,15 +18,77 @@
     db = get_database(**mongodb_config)
     if suffix is not None and not collection_name.endswith(suffix):
         collection_name = f'{collection_name}{suffix}'
 
     return db[collection_name]
 
 
-def get_mongo_client(db_name, host, port, username, password, **kwargs):
+def retried_and_locked_ssh_port_forward(
+    retries_max=SETTINGS.SSH_FORWARD.RETRIES_MAX,
+    retries_delay=SETTINGS.SSH_FORWARD.RETRIES_DELAY,
+    lock_file=SETTINGS.SSH_FORWARD.LOCK_FILE,
+    lock_timeout=SETTINGS.SSH_FORWARD.LOCK_TIMEOUT,
+    **ssh_config,
+):
+    try:
+        from sshtunnel import (
+            BaseSSHTunnelForwarderError,
+            SSHTunnelForwarder,
+            create_logger,
+        )
+    except ImportError:
+        logging.error(
+            'Opening ssh tunnel requires `sshtunnel` (e.g. `pip install sshtunnel`)'
+        )
+        exit(1)
+    try:
+        from filelock import FileLock, Timeout
+    except ImportError:
+        logging.error(
+            'Opening ssh tunnel requires `filelock` (e.g. `pip install filelock`)'
+        )
+        exit(1)
+
+    delay = retries_delay
+    error = None
+    for _ in range(retries_max):
+        try:
+            lock = FileLock(lock_file, timeout=lock_timeout)
+            with lock:
+                server = SSHTunnelForwarder(
+                    **ssh_config,
+                    logger=create_logger(logging.getLogger(), loglevel=logging.ERROR),
+                )
+                server.start()
+                return server
+        except Timeout as e:
+            error = e
+            logging.warn(f'Failed to aquire lock for ssh tunnel {lock_file}')
+        except BaseSSHTunnelForwarderError as e:
+            error = e
+            logging.warn(f'Retry establishing ssh tunnel in {delay} s')
+            # Jittered exponential retry
+            time.sleep(delay)
+            delay *= 2
+            delay += random.uniform(0, 1)
+
+    if error:
+        logging.error(f'Failed to establish ssh tunnel: {error}')
+        exit(1)
+
+
+def get_mongo_client(
+    db_name, host, port, username, password, ssh_config=None, **kwargs
+):
+    if ssh_config is not None:
+        server = retried_and_locked_ssh_port_forward(**ssh_config)
+
+        host = server.local_bind_host
+        port = server.local_bind_port
+
     import pymongo
 
     client = pymongo.MongoClient(
         host,
         int(port),
         username=username,
         password=password,
@@ -73,25 +138,35 @@
 
     Reads the file at the provided path or otherwise {SETTINGS.DATABASE.MONGODB_CONFIG_PATH} to get
         - database host
         - database port
         - database name
         - username
         - password
-        - directConnection
+        - directConnection (Optional)
+        - ssh_config (Optional)
 
     Default path is $HOME/.config/seml/mongodb.config.
 
     Config file should be in the format:
     username: <your_username>
     password: <your_password>
     port: <port>
     database: <database_name>
     host: <host>
     directConnection: <bool> (Optional)
+    ssh_config: <dict> (Optional)
+      ssh_address_or_host: <the url of the jump host>
+      ssh_pkey: <the ssh host key>
+      ssh_username: <username for jump host>
+      retries_max: <number of retries to establish shh tunnel, default 6> (Optional)
+      retries_delay: <initial wait time for exponential retry, default 1> (Optional)
+      lock_file: <lockfile to avoid establishing ssh tunnel parallely, default `~/seml_ssh.lock`> (Optional)
+      lock_timeout: <timeout for aquiring lock, default 30> (Optional)
+      ** further arguments passed to `SSHTunnelForwarder` (see https://github.com/pahaz/sshtunnel)
 
     Returns
     -------
     dict
         Contains the MongoDB config as detailed above.
 
     """
@@ -100,22 +175,16 @@
     config_str = '\nPlease run `seml configure` to provide your credentials.'
 
     if not path.exists():
         raise MongoDBError(
             f"MongoDB credentials could not be read at '{path}'.{config_str}"
         )
 
-    with open(path, 'r') as f:
-        for line in f.readlines():
-            # ignore lines that are empty
-            if len(line.strip()) > 0:
-                split = line.split(':')
-                key = split[0].strip()
-                value = split[1].strip()
-                access_dict[key] = value
+    with open(path, 'r') as conf:
+        access_dict = yaml.safe_load(conf)
 
     required_entries = ['username', 'password', 'port', 'host', 'database']
     for entry in required_entries:
         if entry not in access_dict:
             raise MongoDBError(f"No {entry} found in '{path}'.{config_str}")
 
     db_port = access_dict['port']
@@ -126,23 +195,32 @@
     # False is the default value for PyMongo > 4.0
     db_direct = (
         access_dict['directConnection'] == 'True'
         if 'directConnection' in access_dict
         else False
     )
 
-    return {
+    cfg = {
         'password': db_password,
         'username': db_username,
         'host': db_host,
         'db_name': db_name,
         'port': db_port,
         'directConnection': db_direct,
     }
 
+    if 'ssh_config' not in access_dict:
+        return cfg
+
+    cfg['ssh_config'] = access_dict['ssh_config']
+    cfg['ssh_config']['remote_bind_address'] = (db_host, db_port)
+    cfg['directConnection'] = True
+
+    return cfg
+
 
 def build_filter_dict(filter_states, batch_id, filter_dict, sacred_id=None):
     """
     Construct a dictionary to be used for filtering a MongoDB collection.
 
     Parameters
     ----------
@@ -252,15 +330,16 @@
     except IOError:
         logging.error(f'IOError: could not read {filename}')
     return None
 
 
 def delete_files(database, file_ids, progress=False):
     import gridfs
-    from rich.progress import track
+
+    from seml.console import track
 
     fs = gridfs.GridFS(database)
     it = track(file_ids, disable=not progress)
     for to_delete in it:
         fs.delete(to_delete)
 
 
@@ -275,15 +354,15 @@
         Database collection to be scanned. If None, all collections will be scanned.
     yes: bool
         Whether to automatically confirm the deletion dialog.
     Returns
     -------
     None
     """
-    from rich.progress import track
+    from seml.console import prompt, track
 
     all_collections = not bool(db_collection_name)
     if all_collections:
         config = get_mongodb_config()
         db = get_database(**config)
         collection_names = db.list_collection_names()
     else:
@@ -294,15 +373,14 @@
     collection_blacklist = {'fs.chunks', 'fs.files'}
     collection_names = collection_names - collection_blacklist
 
     referenced_files = set()
     tq = track(collection_names)
     logging.info('Scanning collections for orphaned artifacts...')
     for collection_name in tq:
-        tq.set_postfix(collection=collection_name)
         collection = db[collection_name]
         experiments = list(
             collection.find(
                 {}, {'artifacts': 1, 'experiment.sources': 1, 'source_files': 1}
             )
         )
         for exp in experiments:
```

### Comparing `seml-0.4.3/src/seml/description.py` & `seml-0.4.4/src/seml/description.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from typing import Dict, List, Optional
 
 from seml.database import build_filter_dict, get_collection
 from seml.errors import MongoDBError
 from seml.manage import detect_killed
 from seml.settings import SETTINGS
-from seml.typer import prompt
 from seml.utils import slice_to_str, to_slices
 
 States = SETTINGS.STATES
 
 
 def resolve_description(description: str, config: Dict) -> str:
     from omegaconf import OmegaConf
@@ -52,14 +51,15 @@
         Filter on the batch ID of experiments, by default None
     yes : bool, optional
         Whether to override confirmation prompts, by default False
     resolve : bool, optional
         Whether to use omegaconf to resolve descriptions
     """
     from pymongo import UpdateOne
+    from seml.console import prompt
 
     collection = get_collection(db_collection_name)
 
     filter_dict = build_filter_dict(
         filter_states, batch_id, filter_dict, sacred_id=sacred_id
     )
     exps = list(collection.find(filter_dict, {}))
@@ -125,14 +125,16 @@
     filter_dict : Optional[Dict], optional
         Additional filters, by default None
     batch_id : Optional[int], optional
         Filter on the batch ID of experiments, by default None
     yes : bool, optional
         Whether to override confirmation prompts, by default False
     """
+    from seml.console import prompt
+
     collection = get_collection(db_collection_name)
     update = {'$unset': {'seml.description': ''}}
     filter_dict = build_filter_dict(
         filter_states, batch_id, filter_dict, sacred_id=sacred_id
     )
     exps = [
         exp
```

### Comparing `seml-0.4.3/src/seml/errors.py` & `seml-0.4.4/src/seml/errors.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/evaluation.py` & `seml-0.4.4/src/seml/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     Returns
     -------
 
     """
     import functools
     import pandas as pd
-    from rich.progress import track
+    from seml.console import track
 
     if fields is None:
         fields = ['config', 'result']
 
     if states is None:
         states = States.COMPLETED
```

### Comparing `seml-0.4.3/src/seml/experiment.py` & `seml-0.4.4/src/seml/experiment.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/json.py` & `seml-0.4.4/src/seml/json.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/manage.py` & `seml-0.4.4/src/seml/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     get_collection,
     get_database,
     get_mongodb_config,
 )
 from seml.errors import MongoDBError
 from seml.settings import SETTINGS
 from seml.sources import delete_files, delete_orphaned_sources, upload_sources
-from seml.typer import prompt
 from seml.utils import (
     chunker,
     flatten,
     get_from_nested,
     make_hash,
     resolve_projection_path_conflicts,
     s_if,
@@ -162,14 +161,16 @@
     filter_dict : Optional[Dict], optional
         Additional filters on experiments, by default None
     yes : bool, optional
         Whether to override confirmation prompts, by default False
     wait : bool, optional
         Whether to wait for all experiments be cancelled (by checking the slurm queue), by default False
     """
+    from seml.console import prompt
+
     collection = get_collection(db_collection_name)
     # We check whether there are slurm jobs for which after this action no
     # RUNNING experiment remains. These slurm jobs can be killed altogether.
     # However, it is NOT possible right now to cancel a single experiment in a Slurm job with multiple
     # running experiments.
     try:
         if (
@@ -283,14 +284,16 @@
     batch_id : Optional[int], optional
         Filter on experiment batch ids, by default None
     filter_dict : Optional[Dict], optional
         Additional filters on experiments, by default None
     yes : bool, optional
         Whether to override confirmation prompts, by default False
     """
+    from seml.console import prompt
+
     collection = get_collection(db_collection_name)
     experiment_files_to_delete = []
 
     filter_dict = build_filter_dict(
         filter_states, batch_id, filter_dict, sacred_id=sacred_id
     )
     ndelete = collection.count_documents(filter_dict)
@@ -343,15 +346,15 @@
     pattern : str
         The regex collection names have to match against
     mongodb_config : dict or None
         A configuration for the mongodb. If None, the standard config is used.
     yes : bool
         Whether to override confirmation prompts
     """
-    from seml.console import list_items
+    from seml.console import list_items, prompt
 
     # Get the database
     if mongodb_config is None:
         mongodb_config = get_mongodb_config()
     db = get_database(**mongodb_config)
     expression = re.compile(pattern)
     collection_names = [
@@ -456,14 +459,15 @@
     batch_id : Optional[int], optional
         Filter on the batch ID of experiments, by default None
     filter_dict : Optional[Dict], optional
         Additional filters, by default None
     yes : bool, optional
         Whether to override confirmation prompts, by default False
     """
+    from seml.console import prompt
 
     collection = get_collection(db_collection_name)
     if len({*States.PENDING, *States.RUNNING, *States.KILLED} & set(filter_states)) > 0:
         detect_killed(db_collection_name, print_detected=False)
     filter_dict = build_filter_dict(
         filter_states, batch_id, filter_dict, sacred_id=sacred_id
     )
@@ -628,14 +632,15 @@
         Whether to override confirmation prompts, by default False
     resolve : bool, optional
         Whether to re-resolve the config values
     """
     import gridfs
     from pymongo import UpdateOne
     from importlib.metadata import version
+    from seml.console import prompt
 
     collection = get_collection(db_collection_name)
 
     if batch_ids is not None and len(batch_ids) > 0:
         filter_dict = {'batch_id': {'$in': list(batch_ids)}}
     else:
         filter_dict = {}
@@ -1045,15 +1050,15 @@
         Whether to update the status of experiments by checking log files. This may take a while.
     print_full_description : bool
         Whether to print full descriptions (wrap-arround) or truncate the descriptions otherwise.
     """
     import pandas as pd
     from rich.align import Align
     from rich.table import Column
-    from rich.progress import track
+    from seml.console import track
 
     from seml.console import console, Table
 
     # Get the database
     if mongodb_config is None:
         mongodb_config = get_mongodb_config()
     db = get_database(**mongodb_config)
```

### Comparing `seml-0.4.3/src/seml/mattermost_observer.py` & `seml-0.4.4/src/seml/mattermost_observer.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/module_hider.py` & `seml-0.4.4/src/seml/module_hider.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/network.py` & `seml-0.4.4/src/seml/network.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/observers.py` & `seml-0.4.4/src/seml/observers.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/parameters.py` & `seml-0.4.4/src/seml/parameters.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/prepare_experiment.py` & `seml-0.4.4/src/seml/prepare_experiment.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/project.py` & `seml-0.4.4/src/seml/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     git_commit : Optional[str]
         The commit to use.
     git_branch : Optional[str]
         The branch to use.
     yes : bool
         If True, no confirmation is asked before initializing the project.
     """
-    from click import prompt
+    from seml.console import prompt
     from gitignore_parser import parse_gitignore
 
     if directory is None:
         directory = Path()
     directory = Path(directory).absolute()
 
     # Ensure that the directory exists
```

### Comparing `seml-0.4.3/src/seml/settings.py` & `seml-0.4.4/src/seml/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         'VALID_SEML_CONFIG_VALUES': [
             'executable',
             'name',
             'output_dir',
             'conda_environment',
             'project_root_dir',
             'description',
+            'stash_all_py_files',
         ],
         'SEML_CONFIG_VALUE_VERSION': 'version',
         'VALID_SLURM_CONFIG_VALUES': [
             'experiments_per_job',
             'max_simultaneous_jobs',
             'sbatch_options_template',
             'sbatch_options',
@@ -140,14 +141,20 @@
             'CAPTURE_OUTPUT': False,  # whether to capture the output of the experiment in the database
             'TERMINAL_WIDTH': 80,  # width of the terminal for rich output
         },
         'CONFIG_RESOLUTION_PROGRESS_BAR_THRESHOLD': 25,
         'AUTOCOMPLETE_CACHE_ALIVE_TIME': 300,
         'SETUP_COMMAND': '',
         'END_COMMAND': '',
+        'SSH_FORWARD': {
+            'LOCK_FILE': '/tmp/seml_ssh_forward.lock',
+            'RETRIES_MAX': 6,
+            'RETRIES_DELAY': 1,
+            'LOCK_TIMEOUT': 30,
+        },
     },
 )
 
 # Load user settings
 if SETTINGS.USER_SETTINGS_PATH.exists():
     user_settings_source = run_path(str(SETTINGS.USER_SETTINGS_PATH))
     SETTINGS = munchify(merge_dicts(SETTINGS, user_settings_source['SETTINGS']))
```

### Comparing `seml-0.4.3/src/seml/sources.py` & `seml-0.4.4/src/seml/sources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import logging
 import os
 import sys
 from pathlib import Path
+from typing import Set
 
 from seml.database import delete_files, upload_file
 from seml.errors import ExecutableError, MongoDBError
 from seml.settings import SETTINGS
 from seml.utils import working_directory
 
 States = SETTINGS.STATES
@@ -73,40 +74,61 @@
     logging.root.handlers = orig_handlers
     logging.root.setLevel(orig_loglevel)
     del sys.path[0]
 
     return exe_module
 
 
-def get_imported_sources(executable, root_dir, conda_env, working_dir):
+def get_imported_sources(executable, root_dir, conda_env, working_dir, stash_all_py_files: bool) -> Set[str]:
+    """Get the sources imported by the given executable.
+
+    Args:
+        executable (_type_): The Python file containing the experiment.
+        root_dir (_type_): The root directory of the experiment.
+        conda_env (_type_): The experiment's Anaconda environment.
+        working_dir (_type_): The working directory of the experiment.
+        stash_all_py_files (_type_): Whether to stash all .py files in the working directory.
+
+    Returns:
+        List[str]: The sources imported by the given executable.
+    """
     import_exe(executable, conda_env, working_dir)
     root_path = str(Path(root_dir).expanduser().resolve())
 
     sources = set()
-    for name, mod in sys.modules.items():
-        if mod is None:
-            continue
-        if not getattr(mod, '__file__', False):
-            continue
-        filename = os.path.abspath(mod.__file__)
-        if filename not in sources and is_local_file(filename, root_path):
-            sources.add(filename)
+    source_added = True
+    while source_added:
+        source_added = False
+        for name, mod in list(sys.modules.items()):
+            if mod is None:
+                continue
+            if not getattr(mod, '__file__', False):
+                continue
+            filename = os.path.abspath(mod.__file__)
+            if filename not in sources and is_local_file(filename, root_path):
+                sources.add(filename)
+                source_added = True
+
+    if stash_all_py_files:
+        for file in Path(working_dir).glob('**/*.py'):
+            sources.add(str(file))
 
     return sources
 
 
 def upload_sources(seml_config, collection, batch_id):
     with working_directory(seml_config['working_dir']):
         root_dir = str(Path(seml_config['working_dir']).expanduser().resolve())
 
         sources = get_imported_sources(
             seml_config['executable'],
             root_dir=root_dir,
             conda_env=seml_config['conda_environment'],
             working_dir=seml_config['working_dir'],
+            stash_all_py_files=seml_config.get('stash_all_py_files', False),
         )
         executable_abs = str(Path(seml_config['executable']).expanduser().resolve())
 
         if executable_abs not in sources:
             raise ExecutableError(
                 f'Executable {executable_abs} was not found in the source code files to upload.'
             )
```

### Comparing `seml-0.4.3/src/seml/start.py` & `seml-0.4.4/src/seml/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import copy
+import json
 import logging
 import os
 import shlex
 import shutil
 import subprocess
 import sys
 import time
+import urllib
 import uuid
 from pathlib import Path
-from typing import Dict, Optional, List
+from typing import Dict, List, Optional
 
+from seml.config import generate_named_configs
+from seml.config import resolve_interpolations as resolve_config_interpolations
 from seml.database import build_filter_dict, get_collection
 from seml.errors import ArgumentError, ConfigError, MongoDBError
 from seml.json import PythonEncoder
 from seml.manage import cancel_experiment_by_id, reset_slurm_dict
 from seml.network import find_free_port
 from seml.settings import SETTINGS
 from seml.sources import load_sources_from_db
-from seml.utils import s_if, load_text_resource
-from seml.config import generate_named_configs
-from seml.config import resolve_interpolations as resolve_config_interpolations
+from seml.utils import load_text_resource, s_if
 
 States = SETTINGS.STATES
 SlurmStates = SETTINGS.SLURM_STATES
 
 
 def value_to_string(value, use_json=False):
     # We need the json encoding for vscode due to https://github.com/microsoft/vscode/issues/91578
@@ -43,14 +45,16 @@
     debug=False,
     debug_server=False,
     print_info=True,
     use_json=False,
     unresolved=False,
     resolve_interpolations: bool = True,
 ):
+    from seml.console import console
+
     if 'executable' not in exp['seml']:
         raise MongoDBError(
             f"No executable found for experiment {exp['_id']}. Aborting."
         )
     exe = exp['seml']['executable']
 
     if unresolved:
@@ -119,23 +123,41 @@
     if debug_server:
         ip_address, port = find_free_port()
         if print_info:
             logging.info(
                 f"Starting debug server with IP '{ip_address}' and port '{port}'. "
                 f'Experiment will wait for a debug client to attach.'
             )
+            attach_link = _generate_debug_attach_url(ip_address, port)
+
+            logging.info(
+                "If you are using VSCode, you can use the 'Debug Launcher' extension to attach:"
+            )
+            console.out(attach_link)
+
         interpreter = (
             f'python -m debugpy --listen {ip_address}:{port} --wait-for-client'
         )
     else:
         interpreter = 'python'
 
     return interpreter, exe, config_strings
 
 
+def _generate_debug_attach_url(ip_address, port):
+    launch_config = {
+        'type': 'debugpy',
+        'request': 'attach',
+        'connect': {'host': ip_address, 'port': port},
+        'pathMappings': [{'localRoot': '${workspaceFolder}', 'remoteRoot': '.'}],
+    }
+    launch_config = urllib.parse.quote(json.dumps(launch_config))
+    return f'vscode://fabiospampinato.vscode-debug-launcher/launch?args={launch_config}'
+
+
 def get_config_overrides(config):
     return ' '.join(map(shlex.quote, config))
 
 
 def get_shell_command(interpreter, exe, config, env: dict = None):
     config_overrides = get_config_overrides(config)
 
@@ -376,39 +398,41 @@
     seml_arguments: list
         A list that contains arguments for seml, e.g. ['--debug-server']
 
     Returns
     -------
     None
     """
+    from seml.console import pause_live_widget
 
-    # Construct srun options string
-    # srun will run 2 processes in parallel when ntasks is not specified. Probably because of hyperthreading.
-    if 'ntasks' not in srun_options:
-        srun_options['ntasks'] = 1
-    srun_options_str = create_slurm_options_string(srun_options, True)
+    with pause_live_widget():
+        # Construct srun options string
+        # srun will run 2 processes in parallel when ntasks is not specified. Probably because of hyperthreading.
+        if 'ntasks' not in srun_options:
+            srun_options['ntasks'] = 1
+        srun_options_str = create_slurm_options_string(srun_options, True)
 
-    if not unobserved:
-        collection.update_one(
-            {'_id': exp['_id']}, {'$set': {'slurm.sbatch_options': srun_options}}
-        )
+        if not unobserved:
+            collection.update_one(
+                {'_id': exp['_id']}, {'$set': {'slurm.sbatch_options': srun_options}}
+            )
 
-    # Set command args for job inside Slurm
-    cmd_args = f"--local --sacred-id {exp['_id']} "
-    cmd_args += ' '.join(seml_arguments)
+        # Set command args for job inside Slurm
+        cmd_args = f"--local --sacred-id {exp['_id']} "
+        cmd_args += ' '.join(seml_arguments)
 
-    cmd = f'srun{srun_options_str} seml {collection.name} start {cmd_args}'
-    try:
-        subprocess.run(cmd, shell=True, check=True)
-    except subprocess.CalledProcessError as e:
-        logging.error(
-            f"Could not start Slurm job via srun. Here's the sbatch error message:\n"
-            f"{e.stderr.decode('utf-8')}"
-        )
-        exit(1)
+        cmd = f'srun{srun_options_str} seml {collection.name} start {cmd_args}'
+        try:
+            subprocess.run(cmd, shell=True, check=True)
+        except subprocess.CalledProcessError as e:
+            logging.error(
+                f"Could not start Slurm job via srun. Here's the sbatch error message:\n"
+                f"{e.stderr.decode('utf-8')}"
+            )
+            exit(1)
 
 
 def start_local_job(
     collection,
     exp,
     unobserved=False,
     post_mortem=False,
@@ -436,14 +460,15 @@
         Run job with a debug server.
 
     Returns
     -------
     True if job was executed successfully; False if it failed; None if job was not started because the database entry
     was not in the PENDING state.
     """
+    from seml.console import pause_live_widget
 
     use_stored_sources = 'source_files' in exp['seml']
 
     interpreter, exe, config = get_command_from_exp(
         exp,
         collection.name,
         verbose=logging.root.level <= logging.VERBOSE,
@@ -505,22 +530,25 @@
                 },
             )
 
         logging.verbose(f'Running the following command:\n {cmd}')
 
         if output_dir_path:
             if output_to_console:
-                subprocess.run(cmd, shell=True, check=True)
+                # Let's pause the live widget so we can actually see the output.
+                with pause_live_widget():
+                    subprocess.run(cmd, shell=True, check=True)
             else:  # redirect output to logfile
                 with open(output_file, 'w') as log_file:
                     subprocess.run(
                         cmd, shell=True, stderr=log_file, stdout=log_file, check=True
                     )
         else:
-            subprocess.run(cmd, shell=True, check=True)
+            with pause_live_widget():
+                subprocess.run(cmd, shell=True, check=True)
 
     except subprocess.CalledProcessError:
         success = False
     except IOError:
         logging.error(f'Log file {output_file} could not be written.')
         # Since Sacred is never called in case of I/O error, we need to set the experiment state manually.
         if not unobserved:
@@ -809,14 +837,16 @@
 
     Returns
     -------
     None
     """
     from rich.progress import Progress
 
+    from seml.console import pause_live_widget
+
     check_compute_node()
 
     if 'SLURM_JOBID' in os.environ:
         node_str = subprocess.run(
             'squeue -j ${SLURM_JOBID} -O nodelist:1000',
             shell=True,
             check=True,
@@ -846,73 +876,77 @@
         exp_query['status'] = {'$in': States.PENDING}
     if not steal_slurm:
         exp_query['slurm.array_id'] = {'$exists': False}
         exp_query['slurm.id'] = {'$exists': False}
 
     exp_query.update(filter_dict)
 
-    with Progress(auto_refresh=False) as progress:
-        task = progress.add_task('Running experiments...', total=None)
-        while collection.count_documents(exp_query) > 0 and jobs_counter < num_exps:
-            if unobserved:
-                exp = collection.find_one(exp_query)
-            else:
-                exp = collection.find_one_and_update(
-                    exp_query, {'$set': {'status': States.RUNNING[0]}}
-                )
-            if exp is None:
-                continue
-            if 'array_id' in exp['slurm']:
-                # Clean up MongoDB entry
-                slurm_ids = {
-                    'array_id': exp['slurm']['array_id'],
-                    'task_id': exp['slurm']['task_id'],
-                }
-                reset_slurm_dict(exp)
-                collection.replace_one({'_id': exp['_id']}, exp, upsert=False)
-
-                # Cancel Slurm job; after cleaning up to prevent race conditions
-                cancel_experiment_by_id(
-                    collection, exp['_id'], set_interrupted=False, slurm_dict=slurm_ids
-                )
-
-            progress.console.print(
-                f"current id : {exp['_id']}, failed={num_exceptions}/{jobs_counter} experiments"
-            )
+    with pause_live_widget():
+        with Progress(auto_refresh=False) as progress:
+            task = progress.add_task('Running experiments...', total=None)
+            while collection.count_documents(exp_query) > 0 and jobs_counter < num_exps:
+                if unobserved:
+                    exp = collection.find_one(exp_query)
+                else:
+                    exp = collection.find_one_and_update(
+                        exp_query, {'$set': {'status': States.RUNNING[0]}}
+                    )
+                if exp is None:
+                    continue
+                if 'array_id' in exp['slurm']:
+                    # Clean up MongoDB entry
+                    slurm_ids = {
+                        'array_id': exp['slurm']['array_id'],
+                        'task_id': exp['slurm']['task_id'],
+                    }
+                    reset_slurm_dict(exp)
+                    collection.replace_one({'_id': exp['_id']}, exp, upsert=False)
 
-            # Add newline if we need to avoid tqdm's output
-            if (
-                debug_server
-                or output_to_console
-                or logging.root.level <= logging.VERBOSE
-            ):
-                print(file=sys.stderr)
+                    # Cancel Slurm job; after cleaning up to prevent race conditions
+                    cancel_experiment_by_id(
+                        collection,
+                        exp['_id'],
+                        set_interrupted=False,
+                        slurm_dict=slurm_ids,
+                    )
 
-            if output_to_file:
-                output_dir_path = get_output_dir_path(exp)
-            else:
-                output_dir_path = None
-            try:
-                success = start_local_job(
-                    collection=collection,
-                    exp=exp,
-                    unobserved=unobserved,
-                    post_mortem=post_mortem,
-                    output_dir_path=output_dir_path,
-                    output_to_console=output_to_console,
-                    debug_server=debug_server,
+                progress.console.print(
+                    f"current id : {exp['_id']}, failed={num_exceptions}/{jobs_counter} experiments"
                 )
-                if success is False:
-                    num_exceptions += 1
-            except KeyboardInterrupt:
-                logging.info('Caught KeyboardInterrupt signal. Aborting.')
-                exit(1)
-            jobs_counter += 1
-            progress.advance(task)
-            # tq.set_postfix(current_id=exp['_id'], failed=f"{num_exceptions}/{jobs_counter} experiments")
+
+                # Add newline if we need to avoid tqdm's output
+                if (
+                    debug_server
+                    or output_to_console
+                    or logging.root.level <= logging.VERBOSE
+                ):
+                    print(file=sys.stderr)
+
+                if output_to_file:
+                    output_dir_path = get_output_dir_path(exp)
+                else:
+                    output_dir_path = None
+                try:
+                    success = start_local_job(
+                        collection=collection,
+                        exp=exp,
+                        unobserved=unobserved,
+                        post_mortem=post_mortem,
+                        output_dir_path=output_dir_path,
+                        output_to_console=output_to_console,
+                        debug_server=debug_server,
+                    )
+                    if success is False:
+                        num_exceptions += 1
+                except KeyboardInterrupt:
+                    logging.info('Caught KeyboardInterrupt signal. Aborting.')
+                    exit(1)
+                jobs_counter += 1
+                progress.advance(task)
+                # tq.set_postfix(current_id=exp['_id'], failed=f"{num_exceptions}/{jobs_counter} experiments")
 
 
 def print_command(
     db_collection_name: str,
     sacred_id: Optional[int],
     batch_id: Optional[int],
     filter_states: List,
@@ -922,15 +956,15 @@
     worker_cpus: Optional[int] = None,
     worker_environment_vars: Dict = None,
     unresolved: bool = False,
     resolve_interpolations: bool = True,
 ):
     import rich
 
-    from seml.console import console, Heading
+    from seml.console import Heading, console
 
     collection = get_collection(db_collection_name)
 
     filter_dict = build_filter_dict(filter_states, batch_id, filter_dict, sacred_id)
 
     env_dict = get_environment_variables(
         worker_gpus, worker_cpus, worker_environment_vars
```

### Comparing `seml-0.4.3/src/seml/templates/slurm/jupyter_template.sh` & `seml-0.4.4/src/seml/templates/slurm/jupyter_template.sh`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/templates/slurm/slurm_template.sh` & `seml-0.4.4/src/seml/templates/slurm/slurm_template.sh`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml/utils.py` & `seml-0.4.4/src/seml/utils.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.3/src/seml.egg-info/PKG-INFO` & `seml-0.4.4/src/seml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seml
-Version: 0.4.3
+Version: 0.4.4
 Summary: Slurm Experiment Management Library
 Author: DAML Group @ TUM
 Author-email: Daniel Zügner <zuegnerd@in.tum.de>, Johannes Gsteiger <johannes.gasteiger@tum.de>, Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 Maintainer-email: Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Johannes Klicpera, Daniel Zügner, Nicholas Gao
@@ -39,36 +39,38 @@
 Requires-Dist: numpy>=1.15
 Requires-Dist: pymongo>=3.11
 Requires-Dist: pandas
 Requires-Dist: sacred>=0.8.4
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: jsonpickle>=2.2
 Requires-Dist: munch>=2.0.4
-Requires-Dist: tqdm>=4.36
 Requires-Dist: debugpy>=1.2.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: typer<1.0,>=0.9
 Requires-Dist: rich<14.0,>=13.0
 Requires-Dist: omegaconf<3.0,>=2.3.0
 Requires-Dist: gitignore_parser>=0.1.11
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: ssh-forward
+Requires-Dist: sshtunnel>=0.4.0; extra == "ssh-forward"
+Requires-Dist: filelock>=3.13.3; extra == "ssh-forward"
 
 ![Github Actions](https://github.com/TUM-DAML/seml/workflows/Test/badge.svg)
 
 # `SEML`: Slurm Experiment Management Library
 **`SEML`** is the missing link between the open-source workload scheduling system `Slurm`, the experiment management tool `sacred`, and a `MongoDB` experiment database. It is lightweight, hackable, written in pure Python, and scales to thousands of experiments.
 
 Keeping track of computational experiments can be annoying and failure to do so can lead to lost results, duplicate running of the same experiments, and lots of headaches.
 While workload scheduling systems such as [`Slurm`](https://slurm.schedmd.com/overview.html) make it easy to run many experiments in parallel on a cluster, it can be hard to keep track of which parameter configurations are running, failed, or completed.
 [`sacred`](https://github.com/IDSIA/sacred) is a great tool to collect and manage experiments and their results, especially when used with a [`MongoDB`](https://www.mongodb.com/). However, it is lacking integration with workload schedulers.
 
-**`SEML`** enables you to 
+**`SEML`** enables you to
 * very easily define hyperparameter search spaces using YAML files,
 * run these hyperparameter configurations on a compute cluster using `Slurm`,
 * and to track the experimental results using `sacred` and `MongoDB`.
 
 
 In addition, **`SEML`** offers many more features to make your life easier, such as
 * automatically saving and loading your source code for reproducibility,
@@ -84,32 +86,43 @@
 ```
 or `conda` (the conda version may be outdated, we highly recommend the pypi version!):
 ```bash
 conda install -c conda-forge seml
 ```
 Then configure your MongoDB via:
 ```bash
-seml configure  --mongodb # provide your MongoDB credentials
+seml configure
 ```
 For convenience, you may create your first **`SEML`** project via:
 ```bash
 # initialize the default template in the 'new_project' folder.
 seml project init -t default new_project
 ```
 in an empty directoy. **`SEML`** will automatically create a python package for you.
 
+
+### SSH Port Forwarding
+If your MongoDB is only accessible via an SSH port forward, **`SEML`** allows you to directly configure this as well if you install the `ssh_forward` dependencies via:
+```bash
+pip install seml[ssh_forward]
+```
+It remains to configure the SSH settings:
+```bash
+seml configure --ssh_forward
+```
+
 ### Development
 If you want to develop `seml` please clone the repository and install it via
 ```bash
 pip install -e .[dev]
 ```
 and install pre-commit hooks via
 ```bash
 pre-commit install
-``` 
+```
 
 ## Documentation
 Documentation is available in our [docs.md](docs.md) or via the CLI:
 ```python
 seml --help
 ```
```

### Comparing `seml-0.4.3/src/seml.egg-info/SOURCES.txt` & `seml-0.4.4/src/seml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

