# Comparing `tmp/pyTooling-6.0.1.tar.gz` & `tmp/pyTooling-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTooling-6.0.1.tar", last modified: Tue Jan 16 23:13:11 2024, max compression
+gzip compressed data, was "pyTooling-6.1.0.tar", last modified: Tue Apr  9 22:31:52 2024, max compression
```

## Comparing `pyTooling-6.0.1.tar` & `pyTooling-6.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.661147 pyTooling-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-01-16 23:12:56.000000 pyTooling-6.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-01-16 23:13:11.661147 pyTooling-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-01-16 23:12:56.000000 pyTooling-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.645147 pyTooling-6.0.1/pyTooling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.645147 pyTooling-6.0.1/pyTooling/Attributes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.649147 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/ArgParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.649147 pyTooling-6.0.1/pyTooling/CLIAbstraction/
--rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/Argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/BooleanFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/Command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/Flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/KeyValueFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/OptionalValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedFlagList.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedTupleFlag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CLIAbstraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.649147 pyTooling-6.0.1/pyTooling/CallByRef/
--rw-r--r--   0 runner    (1001) docker     (127)    20766 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/CallByRef/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.649147 pyTooling-6.0.1/pyTooling/Common/
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Configuration/JSON.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Configuration/YAML.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/GenericPath/
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/GenericPath/URL.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/GenericPath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Graph/
--rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Graph/GraphML.py
--rw-r--r--   0 runner    (1001) docker     (127)    90663 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Licensing/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Licensing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/MetaClasses/
--rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/MetaClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Packaging/
--rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Packaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Platform/
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/StateMachine/
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/StateMachine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/TerminalUI/
--rw-r--r--   0 runner    (1001) docker     (127)    35984 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/TerminalUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Timer/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Timer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Tree/
--rw-r--r--   0 runner    (1001) docker     (127)    34203 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling/Versioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/Versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyTooling/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 23:13:11.653148 pyTooling-6.0.1/pyTooling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-01-16 23:13:11.000000 pyTooling-6.0.1/pyTooling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-01-16 23:13:11.000000 pyTooling-6.0.1/pyTooling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 23:13:11.000000 pyTooling-6.0.1/pyTooling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-16 23:13:11.000000 pyTooling-6.0.1/pyTooling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-16 23:13:11.000000 pyTooling-6.0.1/pyTooling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-01-16 23:12:56.000000 pyTooling-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 23:13:11.661147 pyTooling-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-01-16 23:12:56.000000 pyTooling-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.887079 pyTooling-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-09 22:31:49.000000 pyTooling-6.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-04-09 22:31:52.887079 pyTooling-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17878 2024-04-09 22:31:49.000000 pyTooling-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.871079 pyTooling-6.1.0/pyTooling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.875079 pyTooling-6.1.0/pyTooling/Attributes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.875079 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/ArgParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/CLIAbstraction/
+-rw-r--r--   0 runner    (1001) docker     (127)    23614 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/BooleanFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/Flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/KeyValueFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlagList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CLIAbstraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/CallByRef/
+-rw-r--r--   0 runner    (1001) docker     (127)    20766 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/CallByRef/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Common/
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/JSON.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/YAML.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/GenericPath/
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/GenericPath/URL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/GenericPath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    20618 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Graph/GraphML.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90663 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Licensing/
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Licensing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/MetaClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)    36132 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/MetaClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)    18857 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Packaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/Platform/
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/StateMachine/
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/StateMachine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.879078 pyTooling-6.1.0/pyTooling/TerminalUI/
+-rw-r--r--   0 runner    (1001) docker     (127)    35984 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/TerminalUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Timer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Timer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Tree/
+-rw-r--r--   0 runner    (1001) docker     (127)    34203 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling/Versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/Versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyTooling/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:31:52.883078 pyTooling-6.1.0/pyTooling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 22:31:52.000000 pyTooling-6.1.0/pyTooling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-09 22:31:49.000000 pyTooling-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:31:52.887079 pyTooling-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-09 22:31:49.000000 pyTooling-6.1.0/setup.py
```

### Comparing `pyTooling-6.0.1/LICENSE.md` & `pyTooling-6.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/PKG-INFO` & `pyTooling-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.0.1
+Version: 6.1.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,66 +21,66 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
+Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
+Requires-Dist: setuptools>=69.0.0; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: typing_extensions>=4.9.0; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: Coverage>=7.4; extra == "test"
-Requires-Dist: ruamel.yaml>=0.18; extra == "test"
 Requires-Dist: colorama>=0.4.6; extra == "test"
 Requires-Dist: lxml>=5.0; extra == "test"
+Requires-Dist: pytest>=7.4.0; extra == "test"
 Requires-Dist: mypy>=1.8.0; extra == "test"
+Requires-Dist: ruamel.yaml>=0.18; extra == "test"
+Requires-Dist: Coverage>=7.4; extra == "test"
+Requires-Dist: typing_extensions>=4.9.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
-Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: Coverage>=7.4; extra == "all"
-Requires-Dist: mypy>=1.8.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
 Requires-Dist: pytest>=7.4.0; extra == "all"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
+Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
+Requires-Dist: pyTooling~=6.0; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
-Requires-Dist: typing_extensions>=4.9.0; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: lxml>=5.0; extra == "all"
+Requires-Dist: Coverage>=7.4; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18; extra == "all"
+Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
+Requires-Dist: mypy>=1.8.0; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: lxml>=5.0; extra == "all"
+Requires-Dist: typing_extensions>=4.9.0; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pyTooling-6.0.1/README.md` & `pyTooling-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/Argument.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Argument.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/BooleanFlag.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/Flag.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/Flag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/KeyValueFlag.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/KeyValueFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/ValuedFlag.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/ArgParse/__init__.py` & `pyTooling-6.1.0/pyTooling/Attributes/ArgParse/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Attributes/__init__.py` & `pyTooling-6.1.0/pyTooling/Attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/Argument.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/Argument.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/BooleanFlag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/BooleanFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/Command.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/Command.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/Flag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/Flag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/KeyValueFlag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/KeyValueFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/OptionalValuedFlag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/OptionalValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedFlag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedFlagList.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedFlagList.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/ValuedTupleFlag.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/ValuedTupleFlag.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CLIAbstraction/__init__.py` & `pyTooling-6.1.0/pyTooling/CLIAbstraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/CallByRef/__init__.py` & `pyTooling-6.1.0/pyTooling/CallByRef/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Common/__init__.py` & `pyTooling-6.1.0/pyTooling/Common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 .. hint:: See :ref:`high-level help <COMMON>` for explanations and usage examples.
 """
 __author__ =        "Patrick Lehmann"
 __email__ =         "Paebbels@gmail.com"
 __copyright__ =     "2017-2024, Patrick Lehmann"
 __license__ =       "Apache License, Version 2.0"
-__version__ =       "6.0.1"
+__version__ =       "6.1.0"
 __keywords__ =      ["abstract", "argparse", "attributes", "bfs", "cli", "console", "data structure", "decorators",
 					  "dfs", "exceptions", "generators", "generic library", "generic path", "graph", "installation",
 					  "iterators", "licensing", "message logging", "meta-classes", "overloading", "override", "packaging",
 					  "path", "platform", "setuptools", "shell", "singleton", "slots","terminal", "text user interface",
 					  "timer", "tree", "TUI", "url", "versioning", "wheel"]
 __issue_tracker__ = "https://GitHub.com/pyTooling/pyTooling/issues"
```

### Comparing `pyTooling-6.0.1/pyTooling/Configuration/JSON.py` & `pyTooling-6.1.0/pyTooling/Configuration/JSON.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Configuration/YAML.py` & `pyTooling-6.1.0/pyTooling/Configuration/YAML.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Configuration/__init__.py` & `pyTooling-6.1.0/pyTooling/Configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Decorators/__init__.py` & `pyTooling-6.1.0/pyTooling/Decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Exceptions/__init__.py` & `pyTooling-6.1.0/pyTooling/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/GenericPath/URL.py` & `pyTooling-6.1.0/pyTooling/GenericPath/URL.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/GenericPath/__init__.py` & `pyTooling-6.1.0/pyTooling/GenericPath/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Graph/GraphML.py` & `pyTooling-6.1.0/pyTooling/Graph/GraphML.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Graph/__init__.py` & `pyTooling-6.1.0/pyTooling/Graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Licensing/__init__.py` & `pyTooling-6.1.0/pyTooling/Licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/MetaClasses/__init__.py` & `pyTooling-6.1.0/pyTooling/MetaClasses/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #
 """
 The MetaClasses package implements Python meta-classes (classes to construct other classes in Python).
 
 .. hint:: See :ref:`high-level help <META>` for explanations and usage examples.
 """
 from functools  import wraps
-from inspect    import signature, Parameter
+# from inspect    import signature, Parameter
 from threading  import Condition
-from types      import MethodType, FunctionType
+from types      import FunctionType  #, MethodType
 from typing     import Any, Tuple, List, Dict, Callable, Generator, Set, Iterator, Iterable, Union
 from typing     import Type, TypeVar, Generic, _GenericAlias, ClassVar, Optional as Nullable
 
 try:
 	from pyTooling.Exceptions import ToolingException
 	from pyTooling.Decorators import export
 	from pyTooling.Attributes import ATTRIBUTES_MEMBER_NAME, AttributeScope
@@ -287,91 +287,91 @@
 	   * :func:`~pyTooling.Metaclasses.abstractmethod`
 	   * :func:`~pyTooling.Metaclasses.notimplemented`
 	"""
 	method.__mustOverride__ = True
 	return method
 
 
-@export
-def overloadable(method: M) -> M:
-	method.__overloadable__ = True
-	return method
+# @export
+# def overloadable(method: M) -> M:
+# 	method.__overloadable__ = True
+# 	return method
 
 
-@export
-class DispatchableMethod:
-	"""Represents a single multimethod."""
+# @export
+# class DispatchableMethod:
+# 	"""Represents a single multimethod."""
+#
+# 	_methods: Dict[Tuple, Callable]
+# 	__name__: str
+# 	__slots__ = ("_methods", "__name__")
+#
+# 	def __init__(self, name: str) -> None:
+# 		self.__name__ = name
+# 		self._methods = {}
+#
+# 	def __call__(self, *args: Any):
+# 		"""Call a method based on type signature of the arguments."""
+# 		types = tuple(type(arg) for arg in args[1:])
+# 		meth = self._methods.get(types, None)
+# 		if meth:
+# 			return meth(*args)
+# 		else:
+# 			raise TypeError(f"No matching method for types {types}.")
+#
+# 	def __get__(self, instance, cls):  # Starting with Python 3.11+, use typing.Self as return type
+# 		"""Descriptor method needed to make calls work in a class."""
+# 		if instance is not None:
+# 			return MethodType(self, instance)
+# 		else:
+# 			return self
+#
+# 	def register(self, method: Callable) -> None:
+# 		"""Register a new method as a dispatchable."""
+#
+# 		# Build a signature from the method's type annotations
+# 		sig = signature(method)
+# 		types: List[Type] = []
+#
+# 		for name, parameter in sig.parameters.items():
+# 			if name == "self":
+# 				continue
+#
+# 			if parameter.annotation is Parameter.empty:
+# 				raise TypeError(f"Parameter '{name}' in method '{method.__name__}' must be annotated with a type.")
+#
+# 			if not isinstance(parameter.annotation, type):
+# 				raise TypeError(f"Parameter '{name}' in method '{method.__name__}' annotation must be a type.")
+#
+# 			if parameter.default is not Parameter.empty:
+# 				self._methods[tuple(types)] = method
+#
+# 			types.append(parameter.annotation)
+#
+# 		self._methods[tuple(types)] = method
 
-	_methods: Dict[Tuple, Callable]
-	__name__: str
-	__slots__ = ("_methods", "__name__")
-
-	def __init__(self, name: str) -> None:
-		self.__name__ = name
-		self._methods = {}
-
-	def __call__(self, *args: Any):
-		"""Call a method based on type signature of the arguments."""
-		types = tuple(type(arg) for arg in args[1:])
-		meth = self._methods.get(types, None)
-		if meth:
-			return meth(*args)
-		else:
-			raise TypeError(f"No matching method for types {types}.")
-
-	def __get__(self, instance, cls):  # Starting with Python 3.11+, use typing.Self as return type
-		"""Descriptor method needed to make calls work in a class."""
-		if instance is not None:
-			return MethodType(self, instance)
-		else:
-			return self
-
-	def register(self, method: Callable) -> None:
-		"""Register a new method as a dispatchable."""
-
-		# Build a signature from the method's type annotations
-		sig = signature(method)
-		types: List[Type] = []
-
-		for name, parameter in sig.parameters.items():
-			if name == "self":
-				continue
-
-			if parameter.annotation is Parameter.empty:
-				raise TypeError(f"Parameter '{name}' in method '{method.__name__}' must be annotated with a type.")
-
-			if not isinstance(parameter.annotation, type):
-				raise TypeError(f"Parameter '{name}' in method '{method.__name__}' annotation must be a type.")
-
-			if parameter.default is not Parameter.empty:
-				self._methods[tuple(types)] = method
-
-			types.append(parameter.annotation)
-
-		self._methods[tuple(types)] = method
-
-
-@export
-class DispatchDictionary(dict):
-	"""Special dictionary to build dispatchable methods in a metaclass."""
-
-	def __setitem__(self, key: str, value: Any):
-		if callable(value) and key in self:
-			# If key already exists, it must be a dispatchable method or callable
-			currentValue = self[key]
-			if isinstance(currentValue, DispatchableMethod):
-				currentValue.register(value)
-			else:
-				dispatchable = DispatchableMethod(key)
-				dispatchable.register(currentValue)
-				dispatchable.register(value)
-
-				super().__setitem__(key, dispatchable)
-		else:
-			super().__setitem__(key, value)
+
+# @export
+# class DispatchDictionary(dict):
+# 	"""Special dictionary to build dispatchable methods in a metaclass."""
+#
+# 	def __setitem__(self, key: str, value: Any):
+# 		if callable(value) and key in self:
+# 			# If key already exists, it must be a dispatchable method or callable
+# 			currentValue = self[key]
+# 			if isinstance(currentValue, DispatchableMethod):
+# 				currentValue.register(value)
+# 			else:
+# 				dispatchable = DispatchableMethod(key)
+# 				dispatchable.register(currentValue)
+# 				dispatchable.register(value)
+#
+# 				super().__setitem__(key, dispatchable)
+# 		else:
+# 			super().__setitem__(key, value)
 
 
 @export
 class ExtendedType(type):
 	"""
 	An updates meta-class to construct new classes with an extended feature set.
 
@@ -384,20 +384,20 @@
 	* Allow only a single instance to be created (:term:`singleton`).
 	* Define methods as :term:`abstract <abstract method>` or :term:`must-override <mustoverride method>` and prohibit
 	  instantiation of :term:`abstract classes <abstract class>`.
 
 	.. #* Allow method overloading and dispatch overloads based on argument signatures.
 	"""
 
-	@classmethod
-	def __prepare__(cls, className, baseClasses, slots: bool = False, mixin: bool = False, singleton: bool = False):
-		return DispatchDictionary()
+	# @classmethod
+	# def __prepare__(cls, className, baseClasses, slots: bool = False, mixin: bool = False, singleton: bool = False):
+	# 	return DispatchDictionary()
 
 	def __new__(self, className: str, baseClasses: Tuple[type], members: Dict[str, Any],
-							slots: bool = False, mixin: bool = False, singleton: bool = False) -> type:
+							slots: bool = False, mixin: bool = False, singleton: bool = False) -> "ExtendedType":
 		"""
 		Construct a new class using this :term:`meta-class`.
 
 		:param className:       The name of the class to construct.
 		:param baseClasses:     The tuple of :term:`base-classes <base-class>` the class is derived from.
 		:param members:         The dictionary of members for the constructed class.
 		:param slots:           If true, store object attributes in :term:`__slots__ <slots>` instead of ``__dict__``.
@@ -441,15 +441,15 @@
 				pyAttr = getattr(base, ATTRIBUTES_MEMBER_NAME)
 				for att in pyAttr:
 					if AttributeScope.Class in att.Scope:
 						attributes.append(att)
 						att.__class__._classes.append(newClass)
 
 		# Check methods for attributes
-		methods, methodsWithAttributes = self._findMethods(newClass, members)
+		methods, methodsWithAttributes = self._findMethods(newClass, baseClasses, members)
 
 		# Add new fields for found methods
 		newClass.__methods__ = tuple(methods)
 		newClass.__methodsWithAttributes__ = tuple(methodsWithAttributes)
 
 		# Additional methods on a class
 		def HasClassAttributes(self) -> bool:
@@ -521,15 +521,15 @@
 		# GetClassAtrributes -> list[attributes] / generator
 		# MethodHasAttributes(predicate) -> bool
 		# GetAttribute
 
 		return newClass
 
 	@classmethod
-	def _findMethods(self, newClass: type, members: Dict[str, Any]):
+	def _findMethods(self, newClass: "ExtendedType", baseClasses: Tuple[type], members: Dict[str, Any]):
 		try:
 			from ..Attributes import Attribute
 		except (ImportError, ModuleNotFoundError):  # pragma: no cover
 			try:
 				from Attributes import Attribute
 			except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 				raise ex
@@ -543,14 +543,19 @@
 			setattr(instance, methodName, boundMethod)
 
 			return boundMethod
 
 		methods = []
 		methodsWithAttributes = []
 		attributeIndex = {}
+
+		for base in baseClasses:
+			if hasattr(base, "__methodsWithAttributes__"):
+				methodsWithAttributes.extend(base.__methodsWithAttributes__)
+
 		for memberName, member in members.items():
 			if isinstance(member, FunctionType):
 				method = newClass.__dict__[memberName]
 				if hasattr(method, "__classobj__") and getattr(method, "__classobj__") is not newClass:
 					raise TypeError(f"Method '{memberName}' is used by multiple classes: {method.__classobj__} and {newClass}.")
 				else:
 					setattr(method, "__classobj__", newClass)
```

### Comparing `pyTooling-6.0.1/pyTooling/Packaging/__init__.py` & `pyTooling-6.1.0/pyTooling/Packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Platform/__init__.py` & `pyTooling-6.1.0/pyTooling/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/StateMachine/__init__.py` & `pyTooling-6.1.0/pyTooling/StateMachine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/TerminalUI/__init__.py` & `pyTooling-6.1.0/pyTooling/TerminalUI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Timer/__init__.py` & `pyTooling-6.1.0/pyTooling/Timer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Tree/__init__.py` & `pyTooling-6.1.0/pyTooling/Tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyTooling/Versioning/__init__.py` & `pyTooling-6.1.0/pyTooling/Versioning/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,49 +92,52 @@
 	_pre     : int = 0                #: Pre-release version number part.
 	_post    : int = 0                #: Post-release version number part.
 	_prefix  : str = ""               #: Prefix string
 	_postfix : str = ""               #: Postfix string
 # QUESTION: was this how many commits a version is ahead of the last tagged version?
 #	ahead   : int = 0
 
-	def __init__(self, versionString : str) -> None:
+	def __init__(self, major: int, minor: int, patch: int = 0, build: int = 0, flags: Flags = Flags.Clean) -> None:
+		self._major = major
+		self._minor = minor
+		self._patch = patch
+		self._build = build
+		self._parts = Parts.Minor | Parts.Minor | Parts.Patch | Parts.Build
+		self._flags = flags
+
+	@classmethod
+	def Parse(cls, versionString : str) -> "SemanticVersion":
 		if versionString == "":
 			raise ValueError("Parameter 'versionString' is empty.")
 		elif versionString is None:
 			raise ValueError("Parameter 'versionString' is None.")
 		elif versionString.startswith(("V", "v", "I", "i", "R", "r")):
 			versionString = versionString[1:]
 		elif versionString.startswith(("rev", "REV")):
 			versionString = versionString[3:]
 
 		split = versionString.split(".")
 		length = len(split)
-		self._major = int(split[0])
-		self._minor = 0
-		self._patch = 0
-		self._build = 0
-		self._parts = Parts.Major
+		major = int(split[0])
+		minor = 0
+		patch = 0
+		build = 0
+		parts = Parts.Major
 		if length >= 2:
-			self._minor = int(split[1])
-			self._parts |= Parts.Minor
+			minor = int(split[1])
+			parts |= Parts.Minor
 		if length >= 3:
-			self._patch = int(split[2])
-			self._parts |= Parts.Patch
+			patch = int(split[2])
+			parts |= Parts.Patch
 		if length >= 4:
-			self._build = int(split[3])
-			self._parts |= Parts.Build
-		self._flags = Flags.Clean
+			build = int(split[3])
+			parts |= Parts.Build
+		flags = Flags.Clean
 
-	def __init__(self, major: int, minor: int, patch: int = 0, build: int = 0) -> None:  # type: ignore[no-redef]
-		self._major = major
-		self._minor = minor
-		self._patch = patch
-		self._build = build
-		self._parts = Parts.Minor | Parts.Minor | Parts.Patch | Parts.Build
-		self._flags = Flags.Clean
+		return cls(major, minor, patch, build, flags)
 
 	@readonly
 	def Major(self) -> int:
 		return self._major
 
 	@readonly
 	def Minor(self) -> int:
```

### Comparing `pyTooling-6.0.1/pyTooling.egg-info/PKG-INFO` & `pyTooling-6.1.0/pyTooling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 6.0.1
+Version: 6.1.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -21,66 +21,66 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: doc
-Requires-Dist: setuptools>=69.0.0; extra == "doc"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: pyTooling~=6.0; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinx<8.0,>=7.2; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinx_reports>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "doc"
+Requires-Dist: ruamel.yaml>=0.18.5; extra == "doc"
+Requires-Dist: setuptools>=69.0.0; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Provides-Extra: test
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
-Requires-Dist: typing_extensions>=4.9.0; extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: Coverage>=7.4; extra == "test"
-Requires-Dist: ruamel.yaml>=0.18; extra == "test"
 Requires-Dist: colorama>=0.4.6; extra == "test"
 Requires-Dist: lxml>=5.0; extra == "test"
+Requires-Dist: pytest>=7.4.0; extra == "test"
 Requires-Dist: mypy>=1.8.0; extra == "test"
+Requires-Dist: ruamel.yaml>=0.18; extra == "test"
+Requires-Dist: Coverage>=7.4; extra == "test"
+Requires-Dist: typing_extensions>=4.9.0; extra == "test"
 Provides-Extra: packaging
 Requires-Dist: setuptools>=69.0.0; extra == "packaging"
 Provides-Extra: terminal
 Requires-Dist: colorama>=0.4.6; extra == "terminal"
 Provides-Extra: yaml
 Requires-Dist: ruamel.yaml>=0.18; extra == "yaml"
 Provides-Extra: all
-Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: pytest-cov>=4.1.0; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: Coverage>=7.4; extra == "all"
-Requires-Dist: mypy>=1.8.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: pyTooling~=6.0; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
 Requires-Dist: pytest>=7.4.0; extra == "all"
-Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
+Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints>=1.25.2; extra == "all"
-Requires-Dist: sphinx<8.0,>=7.2; extra == "all"
+Requires-Dist: pyTooling~=6.0; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
 Requires-Dist: docutils<0.19.0,>=0.18.0; extra == "all"
-Requires-Dist: typing_extensions>=4.9.0; extra == "all"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: ruamel.yaml>=0.18; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: lxml>=5.0; extra == "all"
+Requires-Dist: Coverage>=7.4; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18; extra == "all"
+Requires-Dist: sphinx_reports>=0.5.0; extra == "all"
+Requires-Dist: mypy>=1.8.0; extra == "all"
+Requires-Dist: ruamel.yaml>=0.18.5; extra == "all"
 Requires-Dist: setuptools>=69.0.0; extra == "all"
 Requires-Dist: ruamel.yaml>=0.18; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: lxml>=5.0; extra == "all"
+Requires-Dist: typing_extensions>=4.9.0; extra == "all"
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyTooling-pyTooling-63bf7f.svg?longCache=true&style=flat-square&longCache=true&logo=GitHub)](https://GitHub.com/pyTooling/pyTooling)
 [![Sourcecode License](https://img.shields.io/pypi/l/pyTooling?longCache=true&style=flat-square&logo=Apache&label=code)](LICENSE.md)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=pyTooling.github.io%2FpyTooling&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2FpyTooling.github.io%2FpyTooling%2Findex.html)](https://pyTooling.github.io/pyTooling/)
 [![Documentation License](https://img.shields.io/badge/doc-CC--BY%204.0-green?longCache=true&style=flat-square&logo=CreativeCommons&logoColor=fff)](LICENSE.md)  
 [![PyPI](https://img.shields.io/pypi/v/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)](https://pypi.org/project/pyTooling/)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyTooling?longCache=true&style=flat-square&logo=PyPI&logoColor=FBE072)
```

### Comparing `pyTooling-6.0.1/pyTooling.egg-info/SOURCES.txt` & `pyTooling-6.1.0/pyTooling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/pyproject.toml` & `pyTooling-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyTooling-6.0.1/setup.py` & `pyTooling-6.1.0/setup.py`

 * *Files identical despite different names*

