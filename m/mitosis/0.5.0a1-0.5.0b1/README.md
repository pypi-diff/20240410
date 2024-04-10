# Comparing `tmp/mitosis-0.5.0a1.tar.gz` & `tmp/mitosis-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosis-0.5.0a1.tar", last modified: Tue Apr  9 10:18:22 2024, max compression
+gzip compressed data, was "mitosis-0.5.0b1.tar", last modified: Wed Apr 10 11:59:36 2024, max compression
```

## Comparing `mitosis-0.5.0a1.tar` & `mitosis-0.5.0b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.549101 mitosis-0.5.0a1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis/
--rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/bad_return_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/mock_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/pyproject_malformed.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/pyproject_missing.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/mitosis/tests/test_pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:18:22.553101 mitosis-0.5.0a1/mitosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 10:18:22.000000 mitosis-0.5.0a1/mitosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-09 10:18:11.000000 mitosis-0.5.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 10:18:22.557101 mitosis-0.5.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.903243 mitosis-0.5.0b1/mitosis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.903243 mitosis-0.5.0b1/mitosis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/bad_return_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/pyproject_malformed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/pyproject_missing.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/mitosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/setup.cfg
```

### Comparing `mitosis-0.5.0a1/.github/workflows/main.yaml` & `mitosis-0.5.0b1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/.github/workflows/release.yaml` & `mitosis-0.5.0b1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/.gitignore` & `mitosis-0.5.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/.pre-commit-config.yaml` & `mitosis-0.5.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/LICENSE` & `mitosis-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/PKG-INFO` & `mitosis-0.5.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,7 @@
-Metadata-Version: 2.1
-Name: mitosis
-Version: 0.5.0a1
-Summary: Reproduce Machine Learning experiments easily
-Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
-Keywords: Machine Learning,Science,Mathematics,Experiments
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: SQL
-Classifier: Topic :: Documentation
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dill
-Requires-Dist: GitPython
-Requires-Dist: importlib_metadata
-Requires-Dist: ipykernel
-Requires-Dist: matplotlib
-Requires-Dist: nbconvert
-Requires-Dist: nbclient
-Requires-Dist: nbformat
-Requires-Dist: pandas
-Requires-Dist: sqlalchemy
-Requires-Dist: toml
-Requires-Dist: types-toml
-Provides-Extra: dev
-Requires-Dist: pytest<8.0.0,>=6.0.0; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flake8-comprehensions>=3.1.0; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pandas-stubs; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-lazy-fixture; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: codecov; extra == "dev"
-
 [![Documentation Status](https://readthedocs.org/projects/mitosis/badge/?version=latest)](https://mitosis.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/mitosis.svg)](https://badge.fury.io/py/mitosis)
 [![Downloads](https://pepy.tech/badge/mitosis)](https://pepy.tech/project/mitosis)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
@@ -64,32 +9,34 @@
 _Reproduce Machine Learning experiments easily_
 
 A package designed to manage and visualize experiments, tracking changes across
 different commits, parameterizations, and random seed.
 
 ## Trivial Example
 
-*sine_experiment.py*
+Hypothesis: the maximum value of a sine wave is equal to its amplitude.
+
+*sine_experiment/\_\_init\_\_.py*
 
 
     import numpy as np
 
     name = "sine-exp"
     lookup_dict = {"frequency": {"fast": 10, "slow": 1}}
 
-    def run(seed, amplitude, frequency):
+    def run(amplitude, frequency):
         """Deterimne if the maximum value of the sine function equals ``amplitude``"""
         x = np.arange(0, 10, .05)
         y = amplitude * np.sin(frequency * x)
         err = np.abs(max(y) - amplitude)
         return {"main": err}
 
 Commit these changes to a repository.  After installing sine_experiment as a python package, in CLI, run:
 
-    mitosis sine_experiment --param frequency=slow --eval-param amplitude=4
+    mitosis -m sine_experiment --param frequency=slow --eval-param amplitude=4
 
 Mitosis will run `sin_experiment.run()`, saving
 all output as an html file in the current directory.  It will also
 track the parameters and results.
 If you later change the variant named "slow" to set frequency=2, mitosis will
 raise a `RuntimeError`, preventing you from running a trial.  If you want to run
 `sine_experiment` with a different parameter value, you need to name that variant
@@ -108,79 +55,98 @@
 5. Create and run a jupyter notebook in memory, saving the result as an HTML file
 6. Updating the database of all trials with the results of the experiment.
 7. Save experiment config of parameters actually created by jupyter notebook (in metadata folder)
 8. Save a freezefile of python packages installed (in metadata folder)
 9. Save the experiments results (in metadata folder)
 
 In step 3, `mitosis` attempts to create a unique and reproduceable string from each
-parameter value.  This is tricky, since most python objects are mutable and/or have
-their `id()` stored in their string representation.  So lists must be sorted, dicts must
-be ordered, and function and method arguments must be wrapped in a class with and a
-custom `__str__()` attribute.  This is imperfectly done, see the **Reproduceability **
+parameter value.
+This is essential, since it strikes at the heart of what reproducibility means when talking about experiments.
+It's also hard, since most python objects are mutable and/or have
+their `id()` stored in their string representation.
+So lists must be sorted, dicts must
+be ordered, and function and method arguments must have their `__str__()` attribute replaced.
+This is imperfectly done, see the **Reproduceability **
 section for comments on the edge cases where `mitosis` will either treat the same
 parameter as a new variant, or treat two different parameters as having the same value.
 
 In step 5, `mitosis` needs to start the jupyter notebook with the appropriate variables.
 Instead of sending the variables to the notebook, the notebook re-evaluates eval
 parameters and re-looks up lookup parameters.  Previously, parameters were sent
 to the notebook via pickle; that proved fragile.
 
 The next time `mitosis.run()` is given the same experiment, it will
 1. Determine whether parameter names and values match parameters in a previously established
-variant.  If they do not, it will either:
-   1. Reject the trial if the passed variant names match existing variants
+variant.  It will either:
+   * Reject the trial if the passed variant names match existing variants
    but with different values.
-   2. Create a new variant for the parameter.
-1. do steps 4 to 9 above.
+   * Create a new variant for the parameter.
+2. Proceeds through steps 4 to 9 above.
 
 
 ## Abstractions
 
 **Experiment:** the definition of a procedure that will test a hypothesis.
-As a python object, an experiment must have a `Callable` attribute named "run"
+As a python object, an experiment is a series of steps, each of which is
+a tuple of a `name`, a lookup dictionary, and a `Callable`
 that takes any number of arguments and returns a dict with at least a key named
-"main".  It also requires a `name` and `lookup_dict` attribute.
+"main".  All but the last also need a key "data" to pass to the next step.  All
+but the first step need to accept an argument named data.
 
-In its current form, `mitosis` does not require a hypothesis, but it does
-require experiments to define the "main" metric worth evaluating (though a
+In its current form, `mitosis` does not require a hypothesis, but consider
+the "main" metric to stand in for a more formal hypothesis (though a
 user can always define an experiment that sets the main metric to a constant).
 
+When running in module mode (`-m` on command line), the lookup dictionary, name, and
+callable are all loaded from the module's `lookup_dict`, `__qualname__`, and `run`
+variables.  Otherwise, they're configured in pyproject.toml.
+
 **Parameter**: An argument to an experiment.  These are the axes by which an experiment
-may vary, e.g. `sim_params`, `data_params`, `solver_params`... etc.  When this argument
+step may vary, e.g. `sim_params`, `data_params`, `solver_params`... etc.  When this argument
 is a `Collection`, sometimes the singular (parameter) and plural (parameters) are used
-interchangeably.  Parameters can either be lookup parameters (which require the
-experiment to have an attribute `lookup_dict`) or eval parameters (which are typically
+interchangeably.  Parameters can either be lookup parameters (which use the
+step's' `lookup_dict`) or eval parameters (which are typically
 simple evaluations, e.g. setting the random seed to a given integer).  Eval parameters
 which are strings need quotes.
 
+When running in module mode (`-m` on command line), experiments only have a single step,
+so mitosis associates all arguments with that step.  In normal mode, the arguments for a
+step must be prefixed with that step name, e.g. `step1.noise_level`
+
 **Variant**: An experimental parameter assigned to specific values and given a name.
 
 **Trial**: a single run of an experiment with all variants specified.  Within `mitosis`,
 the name of a trial is the experiment name, concatenated with variant names for each
 argument, and suffixed by the number of times that particular trial has been run.  E.g.
 If an experiment has three arguments, the first trial run could be called
 "trial_sine-arg1a-arg2test-arg3foo-1"  If a bugfix is committed to the experiment and
 the trial re-run with the same parameters, the new trial would be named
 "trial_sine-arg1a-arg2test-arg3foo-2".
 
 Within `mitosis`, the trial is used to name the resulting html file and is stored in
 the "variant" and "iteration" columns in the experiment's sqlite database.
+the pseudorandom key that is attached to filename serves as an effective primary key
+over all variants and trials.
+
+# API
+
+Mitosis is primarily intended as a command line program, so `mitosis --help` has the syntax documentation.   There is only one intentionally publi part of the api: `mitosis.load_trial_data()`.
+
+Here's a [pre-0.5.0 example](https://github.com/Jacob-Stevens-Haas/gen-experiments/blob/57877df35a9775db15719e16396fe8b06df5e3fa/run_exps.sh), when the `-m` flag was assumed.  For 0.5.0 usage, see the section on "More advanced usage"
 
-# CLI
 
-See [an example](https://github.com/Jacob-Stevens-Haas/gen-experiments/blob/57877df35a9775db15719e16396fe8b06df5e3fa/run_exps.sh).
 
 ## Untracked parameters
 
 If there are certain parameters that are not worth tracking, e.g. plotting flags
 that do not change the mathematical results, prepend the argument name with "+".
 An example:
 
 ```
-mitosis project_pkg.exp1 -e +plot=True -p +plot_axes=dense
+mitosis -m project_pkg.exp1 -e +plot=True -p +plot_axes=dense
 ```
 
 ## Fast iterations: Debug
 
 Debug is straightforwards: `mitosis project_pkg.exp1 -d ...` runs in debug mode.
 This arg allows you to run experiments in a dirty git repository (or no repository)
 and will neither save results in the experimental database, nor increment the trials
@@ -193,64 +159,83 @@
 somewhat intentional, but you can free up names by deleting or renaming the
 experiment database or deleting records in the `variant_param_name` table.
 
 Mitosis also sets the log level of the experiment module to INFO and gives it
 a FileHandler to the metadata directory.  In Debug mode, mitosis sets the log
 level of the experiment to DEBUG.
 
-## Sharing code between experiments: Group
-
-If your experimental code is intended to be used for multiple dissimilar
-experiments and want to track results separately, assign a group at the command
-line.  The string is passed as an argument "group" to the experiment's run()
-function.  It is treated as a special eval parameter, so if passed, there must
-be no other params named group
-
-Group is more complex, but a simple example will help:
-```
-mitosis project_pkg.pdes -g heat -p initial_condition=origin-bump
-mitosis project_pkg.pdes -g heat2d -p initial_condition=origin-bump2d
-mitosis project_pkg.gridsearch -g pdes-heat -p initial_condition=origin-bump
-```
+# More advanced usage.
 
-# Some more advanced usage.
+## Module-style experiments
 
-It should be noted that mitosis only works on installed packages - modules that you can run using `python -m pkgname`.
+It should be noted that mitosis only works on installed packages - modules that you can run using `python -m pkgname.modname`.
 
- When you want two modules share the same, long lookup_dict, I have found creating a
+When you want two modules share the same, long lookup_dict, I have found creating a
 module with multiple dictionaries works well, e.g.
 
     project_pkg/
         |-- __init__.py     # Should look like
         |                   param_1 = {"var1": 1, "var2": 2}
         |                   param_2 = {"foo": "hello", "bar": "world"}
         |
         |                   # Each experiment gets same lookup dict
         |-- exp1.py         lookup_dict = vars(project_pkg)
         |-- exp2.py         lookup_dict = vars(project_pkg)
 
 This way, the same variants can be used for different experiemnts:
 
 ```
-mitosis project_pkg.exp1 -e seed=2 -p param_1=var_1 -p param_2=foo
-mitosis project_pkg.exp2 -e seed=2 -p param_1=var_1 -p param_2=foo
+mitosis -m project_pkg.exp1 -e seed=2 -p param_1=var_1 -p param_2=foo
+mitosis -m project_pkg.exp2 -e seed=2 -p param_1=var_1 -p param_2=foo
 ```
 It is also common to have one experiment wrap another, e.g. if exp2 is a gridsearch
 around exp1.
 
-I typically run experiments on servers, so `nohup ... &> exp.log &` frees up the
-terminal and lets me disconnect ssh, returning later and reading exp.log to see
-that the experiment worked or what errors occurred
-(if error occurs inside the experiment and not inside `mitosis`, they will also
-be visible in the generated html notebook).
-If I have a variety of experiments that I want to run, I can copy and paste a
-lot of experiments all at once into the terminal, and they will all execute in
-parallel.
+## Recommended: multi-step experiments
+
+Sometimes it's useful to combine steps from different packages, or share steps across projects,
+or distribute your experiment without the clutter of a lookup dictionary holding every variant
+you tried out.
+In these cases, the _project_ is responsible for naming and connecting the callable <-> lookup-dictionary association.
+These experiment steps are specified in pyproject.toml, in the `[tools.mitosis.steps]` table using
+object reference notation (à la plugins).
+
+Let's say your project folder is called `my_paper` and contains an eponymous python package.  You have an experiment defined in the package `first_exp`, broken down into functions `make_data()` and `linear_pipeline`, but you want to be able to swap out the first step for real data in another module `geospatial.datasets`, you could have the following table in your project's pyproject.toml (likely within the `my_paper` repo):
+
+    [tool.mitosis.steps]
+    real_data = ["geospatial.datasets:load_data", "my_paper:data_config"]
+    sim_data = ["first_exp:make_data", "my_paper:data_config"]
+    fit_eval = ["first_exp:linear_pipeline", "my_paper:meth_config"]
+
+This also says that the lookup dicts for each step are all imported from `my_paper`.  You would invoke experiments like:
+
+```
+mitosis sim_data fit_eval --p sim_data.noise=low -e linear_pipeline.alpha=.5
+mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e linear_pipeline.alpha=.5
+```
+
+Needless to say, all of the callables need to pass data compatibly, e.g.
+`first_exp.linear_pipeline(first_exp.make_data(...)["data"], ...)` must make sense, as must
+`first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
+
+You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
+
+I'm often on a server and want to disconnect while the experiment is running, so I wrap my experiments in `nohup ... &> exp1.log &`.
+
+
+## Using persistent data
+
+There are two obviously useful things to do after an experiment:
+* view the html file.  `python -m http.server` is helpful to browse results
+* load the data with `load_trial_data()`
+
+Beyond this, the metadata mitosis keeps to disk is useful for troubleshooting or reproducing experiments, but no facility yet exists to browse or compare experiments.
+
 
-# Reproduceability Thoughts
+<!-- # Reproduceability Thoughts
 
 The goal of the package, experimental reproduceability, poses a few fun challenges.
 Here are my thoughts on reproduceable desiderata.
 
 ## Raison d'être
 I designed `mitosis` for the primary purpose of stopping my confusion when I tried to
 reproduce plots for my advisor after a small code change.  Without an automatic
@@ -278,8 +263,8 @@
 3. Using the same versions of binary libraries
 4. Using the same versions of python packages and python executable
 5. Same git commit of all experimental code
 6. Only run experiments with hashable parameters
 7. Ability to freeze/reproduce mutable arguments
 8. Ability to recreate arguments from either their `__repr__` string or their serialization
 9. Don't run experiments without specifying a hypothesis first
-10. For experiments that require randomness, only use a single, reproduceable generator.
+10. For experiments that require randomness, only use a single, reproduceable generator. -->
```

### Comparing `mitosis-0.5.0a1/docs/source/conf.py` & `mitosis-0.5.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/mitosis/__init__.py` & `mitosis-0.5.0b1/mitosis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,16 +580,17 @@
     req_str += "\n".join(f"{pkg}=='{version(pkg)}'" for pkg in installed)
     with open(folder / "requirements.txt", "w") as f:
         f.write(req_str)
 
 
 def _prettyprint_config(folder: Path, params: Collection[Parameter]):
     pretty = pprint.pformat(params)
-    with open(folder / "config.txt", "w") as f:
+    with open(folder / "config.txt", "a") as f:
         f.write(pretty)
+        f.write("\n")
 
 
 def unpack(obj_ref: str) -> Any:
     modname, _, qualname = obj_ref.partition(":")
     obj = import_module(modname)
     for attr in qualname.split("."):
         obj = getattr(obj, attr)
```

### Comparing `mitosis-0.5.0a1/mitosis/__main__.py` & `mitosis-0.5.0b1/mitosis/__main__.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/mitosis/_disk.py` & `mitosis-0.5.0b1/mitosis/_disk.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/mitosis/_typing.py` & `mitosis-0.5.0b1/mitosis/_typing.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/mitosis/tests/test_all.py` & `mitosis-0.5.0b1/mitosis/tests/test_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,39 +138,49 @@
         debug=True,
         trials_folder=tmp_path,
     )
     data = mitosis.load_trial_data(exp_key, trials_folder=tmp_path)
     assert len(data[1]["data"]) == 5
 
 
-def test_mod_logging_debug(mock_steps, tmp_path):
+def test_mod_metadata_debug(mock_steps, tmp_path):
     hexstr = mitosis.run(
         mock_steps,
         debug=True,
         trials_folder=tmp_path,
     )
     trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
     with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" in log_str
+    with open(trial_folder / "config.txt") as f:
+        config_lines = f.readlines()
+    config_params = [eval(line) for line in config_lines]
+    passed_params = [{p.arg_name: p.vals for p in step.args} for step in mock_steps]
+    assert config_params == passed_params
 
 
 @pytest.mark.clean
-def test_mod_logging(mock_steps, tmp_path):
+def test_mod_metadata(mock_steps, tmp_path):
     hexstr = mitosis.run(
         mock_steps,
         debug=False,
         trials_folder=tmp_path,
     )
     trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
     with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" not in log_str
+    with open(trial_folder / "config.txt") as f:
+        config_lines = f.readlines()
+    config_params = [eval(line) for line in config_lines]
+    passed_params = [{p.arg_name: p.vals for p in step.args} for step in mock_steps]
+    assert config_params == passed_params
 
 
 def test_malfored_return_experiment(mock_steps, tmp_path):
     bad_steps = [
         mock_steps[0],
         ExpStep(
             mock_steps[1].name,
```

### Comparing `mitosis-0.5.0a1/mitosis/tests/test_cli.py` & `mitosis-0.5.0b1/mitosis/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/mitosis.egg-info/PKG-INFO` & `mitosis-0.5.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.0a1
+Version: 0.5.0b1
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -64,32 +64,34 @@
 _Reproduce Machine Learning experiments easily_
 
 A package designed to manage and visualize experiments, tracking changes across
 different commits, parameterizations, and random seed.
 
 ## Trivial Example
 
-*sine_experiment.py*
+Hypothesis: the maximum value of a sine wave is equal to its amplitude.
+
+*sine_experiment/\_\_init\_\_.py*
 
 
     import numpy as np
 
     name = "sine-exp"
     lookup_dict = {"frequency": {"fast": 10, "slow": 1}}
 
-    def run(seed, amplitude, frequency):
+    def run(amplitude, frequency):
         """Deterimne if the maximum value of the sine function equals ``amplitude``"""
         x = np.arange(0, 10, .05)
         y = amplitude * np.sin(frequency * x)
         err = np.abs(max(y) - amplitude)
         return {"main": err}
 
 Commit these changes to a repository.  After installing sine_experiment as a python package, in CLI, run:
 
-    mitosis sine_experiment --param frequency=slow --eval-param amplitude=4
+    mitosis -m sine_experiment --param frequency=slow --eval-param amplitude=4
 
 Mitosis will run `sin_experiment.run()`, saving
 all output as an html file in the current directory.  It will also
 track the parameters and results.
 If you later change the variant named "slow" to set frequency=2, mitosis will
 raise a `RuntimeError`, preventing you from running a trial.  If you want to run
 `sine_experiment` with a different parameter value, you need to name that variant
@@ -108,79 +110,98 @@
 5. Create and run a jupyter notebook in memory, saving the result as an HTML file
 6. Updating the database of all trials with the results of the experiment.
 7. Save experiment config of parameters actually created by jupyter notebook (in metadata folder)
 8. Save a freezefile of python packages installed (in metadata folder)
 9. Save the experiments results (in metadata folder)
 
 In step 3, `mitosis` attempts to create a unique and reproduceable string from each
-parameter value.  This is tricky, since most python objects are mutable and/or have
-their `id()` stored in their string representation.  So lists must be sorted, dicts must
-be ordered, and function and method arguments must be wrapped in a class with and a
-custom `__str__()` attribute.  This is imperfectly done, see the **Reproduceability **
+parameter value.
+This is essential, since it strikes at the heart of what reproducibility means when talking about experiments.
+It's also hard, since most python objects are mutable and/or have
+their `id()` stored in their string representation.
+So lists must be sorted, dicts must
+be ordered, and function and method arguments must have their `__str__()` attribute replaced.
+This is imperfectly done, see the **Reproduceability **
 section for comments on the edge cases where `mitosis` will either treat the same
 parameter as a new variant, or treat two different parameters as having the same value.
 
 In step 5, `mitosis` needs to start the jupyter notebook with the appropriate variables.
 Instead of sending the variables to the notebook, the notebook re-evaluates eval
 parameters and re-looks up lookup parameters.  Previously, parameters were sent
 to the notebook via pickle; that proved fragile.
 
 The next time `mitosis.run()` is given the same experiment, it will
 1. Determine whether parameter names and values match parameters in a previously established
-variant.  If they do not, it will either:
-   1. Reject the trial if the passed variant names match existing variants
+variant.  It will either:
+   * Reject the trial if the passed variant names match existing variants
    but with different values.
-   2. Create a new variant for the parameter.
-1. do steps 4 to 9 above.
+   * Create a new variant for the parameter.
+2. Proceeds through steps 4 to 9 above.
 
 
 ## Abstractions
 
 **Experiment:** the definition of a procedure that will test a hypothesis.
-As a python object, an experiment must have a `Callable` attribute named "run"
+As a python object, an experiment is a series of steps, each of which is
+a tuple of a `name`, a lookup dictionary, and a `Callable`
 that takes any number of arguments and returns a dict with at least a key named
-"main".  It also requires a `name` and `lookup_dict` attribute.
+"main".  All but the last also need a key "data" to pass to the next step.  All
+but the first step need to accept an argument named data.
 
-In its current form, `mitosis` does not require a hypothesis, but it does
-require experiments to define the "main" metric worth evaluating (though a
+In its current form, `mitosis` does not require a hypothesis, but consider
+the "main" metric to stand in for a more formal hypothesis (though a
 user can always define an experiment that sets the main metric to a constant).
 
+When running in module mode (`-m` on command line), the lookup dictionary, name, and
+callable are all loaded from the module's `lookup_dict`, `__qualname__`, and `run`
+variables.  Otherwise, they're configured in pyproject.toml.
+
 **Parameter**: An argument to an experiment.  These are the axes by which an experiment
-may vary, e.g. `sim_params`, `data_params`, `solver_params`... etc.  When this argument
+step may vary, e.g. `sim_params`, `data_params`, `solver_params`... etc.  When this argument
 is a `Collection`, sometimes the singular (parameter) and plural (parameters) are used
-interchangeably.  Parameters can either be lookup parameters (which require the
-experiment to have an attribute `lookup_dict`) or eval parameters (which are typically
+interchangeably.  Parameters can either be lookup parameters (which use the
+step's' `lookup_dict`) or eval parameters (which are typically
 simple evaluations, e.g. setting the random seed to a given integer).  Eval parameters
 which are strings need quotes.
 
+When running in module mode (`-m` on command line), experiments only have a single step,
+so mitosis associates all arguments with that step.  In normal mode, the arguments for a
+step must be prefixed with that step name, e.g. `step1.noise_level`
+
 **Variant**: An experimental parameter assigned to specific values and given a name.
 
 **Trial**: a single run of an experiment with all variants specified.  Within `mitosis`,
 the name of a trial is the experiment name, concatenated with variant names for each
 argument, and suffixed by the number of times that particular trial has been run.  E.g.
 If an experiment has three arguments, the first trial run could be called
 "trial_sine-arg1a-arg2test-arg3foo-1"  If a bugfix is committed to the experiment and
 the trial re-run with the same parameters, the new trial would be named
 "trial_sine-arg1a-arg2test-arg3foo-2".
 
 Within `mitosis`, the trial is used to name the resulting html file and is stored in
 the "variant" and "iteration" columns in the experiment's sqlite database.
+the pseudorandom key that is attached to filename serves as an effective primary key
+over all variants and trials.
+
+# API
+
+Mitosis is primarily intended as a command line program, so `mitosis --help` has the syntax documentation.   There is only one intentionally publi part of the api: `mitosis.load_trial_data()`.
+
+Here's a [pre-0.5.0 example](https://github.com/Jacob-Stevens-Haas/gen-experiments/blob/57877df35a9775db15719e16396fe8b06df5e3fa/run_exps.sh), when the `-m` flag was assumed.  For 0.5.0 usage, see the section on "More advanced usage"
 
-# CLI
 
-See [an example](https://github.com/Jacob-Stevens-Haas/gen-experiments/blob/57877df35a9775db15719e16396fe8b06df5e3fa/run_exps.sh).
 
 ## Untracked parameters
 
 If there are certain parameters that are not worth tracking, e.g. plotting flags
 that do not change the mathematical results, prepend the argument name with "+".
 An example:
 
 ```
-mitosis project_pkg.exp1 -e +plot=True -p +plot_axes=dense
+mitosis -m project_pkg.exp1 -e +plot=True -p +plot_axes=dense
 ```
 
 ## Fast iterations: Debug
 
 Debug is straightforwards: `mitosis project_pkg.exp1 -d ...` runs in debug mode.
 This arg allows you to run experiments in a dirty git repository (or no repository)
 and will neither save results in the experimental database, nor increment the trials
@@ -193,64 +214,83 @@
 somewhat intentional, but you can free up names by deleting or renaming the
 experiment database or deleting records in the `variant_param_name` table.
 
 Mitosis also sets the log level of the experiment module to INFO and gives it
 a FileHandler to the metadata directory.  In Debug mode, mitosis sets the log
 level of the experiment to DEBUG.
 
-## Sharing code between experiments: Group
+# More advanced usage.
 
-If your experimental code is intended to be used for multiple dissimilar
-experiments and want to track results separately, assign a group at the command
-line.  The string is passed as an argument "group" to the experiment's run()
-function.  It is treated as a special eval parameter, so if passed, there must
-be no other params named group
+## Module-style experiments
 
-Group is more complex, but a simple example will help:
-```
-mitosis project_pkg.pdes -g heat -p initial_condition=origin-bump
-mitosis project_pkg.pdes -g heat2d -p initial_condition=origin-bump2d
-mitosis project_pkg.gridsearch -g pdes-heat -p initial_condition=origin-bump
-```
-
-# Some more advanced usage.
+It should be noted that mitosis only works on installed packages - modules that you can run using `python -m pkgname.modname`.
 
-It should be noted that mitosis only works on installed packages - modules that you can run using `python -m pkgname`.
-
- When you want two modules share the same, long lookup_dict, I have found creating a
+When you want two modules share the same, long lookup_dict, I have found creating a
 module with multiple dictionaries works well, e.g.
 
     project_pkg/
         |-- __init__.py     # Should look like
         |                   param_1 = {"var1": 1, "var2": 2}
         |                   param_2 = {"foo": "hello", "bar": "world"}
         |
         |                   # Each experiment gets same lookup dict
         |-- exp1.py         lookup_dict = vars(project_pkg)
         |-- exp2.py         lookup_dict = vars(project_pkg)
 
 This way, the same variants can be used for different experiemnts:
 
 ```
-mitosis project_pkg.exp1 -e seed=2 -p param_1=var_1 -p param_2=foo
-mitosis project_pkg.exp2 -e seed=2 -p param_1=var_1 -p param_2=foo
+mitosis -m project_pkg.exp1 -e seed=2 -p param_1=var_1 -p param_2=foo
+mitosis -m project_pkg.exp2 -e seed=2 -p param_1=var_1 -p param_2=foo
 ```
 It is also common to have one experiment wrap another, e.g. if exp2 is a gridsearch
 around exp1.
 
-I typically run experiments on servers, so `nohup ... &> exp.log &` frees up the
-terminal and lets me disconnect ssh, returning later and reading exp.log to see
-that the experiment worked or what errors occurred
-(if error occurs inside the experiment and not inside `mitosis`, they will also
-be visible in the generated html notebook).
-If I have a variety of experiments that I want to run, I can copy and paste a
-lot of experiments all at once into the terminal, and they will all execute in
-parallel.
+## Recommended: multi-step experiments
+
+Sometimes it's useful to combine steps from different packages, or share steps across projects,
+or distribute your experiment without the clutter of a lookup dictionary holding every variant
+you tried out.
+In these cases, the _project_ is responsible for naming and connecting the callable <-> lookup-dictionary association.
+These experiment steps are specified in pyproject.toml, in the `[tools.mitosis.steps]` table using
+object reference notation (à la plugins).
+
+Let's say your project folder is called `my_paper` and contains an eponymous python package.  You have an experiment defined in the package `first_exp`, broken down into functions `make_data()` and `linear_pipeline`, but you want to be able to swap out the first step for real data in another module `geospatial.datasets`, you could have the following table in your project's pyproject.toml (likely within the `my_paper` repo):
+
+    [tool.mitosis.steps]
+    real_data = ["geospatial.datasets:load_data", "my_paper:data_config"]
+    sim_data = ["first_exp:make_data", "my_paper:data_config"]
+    fit_eval = ["first_exp:linear_pipeline", "my_paper:meth_config"]
+
+This also says that the lookup dicts for each step are all imported from `my_paper`.  You would invoke experiments like:
+
+```
+mitosis sim_data fit_eval --p sim_data.noise=low -e linear_pipeline.alpha=.5
+mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e linear_pipeline.alpha=.5
+```
+
+Needless to say, all of the callables need to pass data compatibly, e.g.
+`first_exp.linear_pipeline(first_exp.make_data(...)["data"], ...)` must make sense, as must
+`first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
+
+You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
+
+I'm often on a server and want to disconnect while the experiment is running, so I wrap my experiments in `nohup ... &> exp1.log &`.
+
+
+## Using persistent data
+
+There are two obviously useful things to do after an experiment:
+* view the html file.  `python -m http.server` is helpful to browse results
+* load the data with `load_trial_data()`
+
+Beyond this, the metadata mitosis keeps to disk is useful for troubleshooting or reproducing experiments, but no facility yet exists to browse or compare experiments.
+
 
-# Reproduceability Thoughts
+<!-- # Reproduceability Thoughts
 
 The goal of the package, experimental reproduceability, poses a few fun challenges.
 Here are my thoughts on reproduceable desiderata.
 
 ## Raison d'être
 I designed `mitosis` for the primary purpose of stopping my confusion when I tried to
 reproduce plots for my advisor after a small code change.  Without an automatic
@@ -278,8 +318,8 @@
 3. Using the same versions of binary libraries
 4. Using the same versions of python packages and python executable
 5. Same git commit of all experimental code
 6. Only run experiments with hashable parameters
 7. Ability to freeze/reproduce mutable arguments
 8. Ability to recreate arguments from either their `__repr__` string or their serialization
 9. Don't run experiments without specifying a hypothesis first
-10. For experiments that require randomness, only use a single, reproduceable generator.
+10. For experiments that require randomness, only use a single, reproduceable generator. -->
```

### Comparing `mitosis-0.5.0a1/mitosis.egg-info/SOURCES.txt` & `mitosis-0.5.0b1/mitosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0a1/pyproject.toml` & `mitosis-0.5.0b1/pyproject.toml`

 * *Files identical despite different names*

