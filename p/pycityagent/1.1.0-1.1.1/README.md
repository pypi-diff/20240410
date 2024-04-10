# Comparing `tmp/pycityagent-1.1.0.tar.gz` & `tmp/pycityagent-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.0.tar", last modified: Mon Apr  8 09:08:15 2024, max compression
+gzip compressed data, was "pycityagent-1.1.1.tar", last modified: Wed Apr 10 07:29:13 2024, max compression
```

## Comparing `pycityagent-1.1.0.tar` & `pycityagent-1.1.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 09:08:11.000000 pycityagent-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-08 09:08:15.525119 pycityagent-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-08 09:08:11.000000 pycityagent-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.517119 pycityagent-1.1.0/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.517119 pycityagent-1.1.0/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27610 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:08:15.525119 pycityagent-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 07:29:05.000000 pycityagent-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-10 07:29:13.967618 pycityagent-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-10 07:29:05.000000 pycityagent-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.959618 pycityagent-1.1.1/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.963618 pycityagent-1.1.1/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.963618 pycityagent-1.1.1/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/ac/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.963618 pycityagent-1.1.1/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.963618 pycityagent-1.1.1/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.963618 pycityagent-1.1.1/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:29:13.967618 pycityagent-1.1.1/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-10 07:29:13.000000 pycityagent-1.1.1/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 07:29:13.000000 pycityagent-1.1.1/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:29:13.000000 pycityagent-1.1.1/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 07:29:13.000000 pycityagent-1.1.1/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 07:29:13.000000 pycityagent-1.1.1/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 07:29:05.000000 pycityagent-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:29:13.967618 pycityagent-1.1.1/setup.cfg
```

### Comparing `pycityagent-1.1.0/LICENSE` & `pycityagent-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/PKG-INFO` & `pycityagent-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.0
+Version: 1.1.1
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 <!-- TOC -->
 
 ## Introduction
 ### Framework of CityAgent
 - ![framwork](./static/framework.png)
 
 ### Workflow of CityAgent
-- ![workflow](./static/workflow.png)
+- ![workflow](./static/workflow_1.png)
 
 ## Hands On - By An Easy Demo
 ### Apply for your App
 - You first need to register your account in the [Opencity website](https://opencity.fiblab.net/)
 - Login to the console, create your own app.
 - Get your app_id and app_secret
     - ![app](./static/app.png)
```

### Comparing `pycityagent-1.1.0/README.md` & `pycityagent-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 <!-- TOC -->
 
 ## Introduction
 ### Framework of CityAgent
 - ![framwork](./static/framework.png)
 
 ### Workflow of CityAgent
-- ![workflow](./static/workflow.png)
+- ![workflow](./static/workflow_1.png)
 
 ## Hands On - By An Easy Demo
 ### Apply for your App
 - You first need to register your account in the [Opencity website](https://opencity.fiblab.net/)
 - Login to the console, create your own app.
 - Get your app_id and app_secret
     - ![app](./static/app.png)
```

### Comparing `pycityagent-1.1.0/pycityagent/ac/ac.py` & `pycityagent-1.1.1/pycityagent/ac/ac.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/action.py` & `pycityagent-1.1.1/pycityagent/ac/action.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/action_stream.py` & `pycityagent-1.1.1/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.1/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.1/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.1/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.1/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.1/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/controled.py` & `pycityagent-1.1.1/pycityagent/ac/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/converse.py` & `pycityagent-1.1.1/pycityagent/ac/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.1/pycityagent/ac/hub_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/shop.py` & `pycityagent-1.1.1/pycityagent/ac/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.1/pycityagent/ac/sim_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/ac/trip.py` & `pycityagent-1.1.1/pycityagent/ac/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/agent.py` & `pycityagent-1.1.1/pycityagent/agent.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/agent_citizen.py` & `pycityagent-1.1.1/pycityagent/agent_citizen.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/agent_func.py` & `pycityagent-1.1.1/pycityagent/agent_func.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/brain.py` & `pycityagent-1.1.1/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/memory.py` & `pycityagent-1.1.1/pycityagent/brain/memory.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.1/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.1/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/reason/social.py` & `pycityagent-1.1.1/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.1/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/reason/user.py` & `pycityagent-1.1.1/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/scheduler.py` & `pycityagent-1.1.1/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/brain/sence.py` & `pycityagent-1.1.1/pycityagent/brain/sence.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,15 +293,16 @@
         Args:
         - radius (int): 感知半径; Perceive radius
 
         Returns:
         - List[dict]: 可达位置列表
             - lane_id (int)
             - s (float)
-            - longlat (Tuple[float, float]): [longitude, latitude]
+            - xy (Tuple[float, float]): (x, y)
+            - longlat (Tuple[float, float]): (longitude, latitude)
             - type (str): 'driving' / 'walking' / 'unspecified'
         '''
         radius_ = self._sence_radius
         if radius != None:
             radius_ = radius
         positions = []
         if 'aoi_position' in self._agent.motion['position'].keys():
@@ -314,22 +315,24 @@
             walking_positions = aoi['walking_positions']
             walking_gates = aoi['walking_gates']
             for i in range(len(driving_positions)):
                 longlat = self._agent._simulator.map.xy2lnglat(x=driving_gates[i]['x'], y=driving_gates[i]['y'])
                 positions.append({
                     'lane_id': driving_positions[i]['lane_id'], 
                     's': driving_positions[i]['s'],
+                    'xy': (driving_gates[i]['x'], driving_gates[i]['y']),
                     'longlat': longlat,
                     'type': 'driving'
                 })
             for i in range(len(walking_positions)):
                 longlat = self._agent._simulator.map.xy2lnglat(x=walking_gates[i]['x'], y=walking_gates[i]['y'])
                 positions.append({
                     'lane_id': walking_positions[i]['lane_id'], 
                     's': walking_positions[i]['s'],
+                    'xy': (walking_gates[i]['x'], walking_gates[i]['y']),
                     'longlat': longlat,
                     'type': 'walking'
                 })
         else:
             # agent in lane
             lane_id = self._agent.motion['position']['lane_position']['lane_id']  # 所在lane_id
             lane = copy.deepcopy(self._agnet._simualtor.map.get_lane(lane_id))  # 获取lane信息
@@ -339,65 +342,89 @@
                 # 处于当前道路的首部端点位置
                 # 1. 当前道路
                 tmp_s = radius_
                 tmp_s = tmp_s if tmp_s <= lane['length'] else lane['length']
                 x, y = get_xy_in_lane(nodes, tmp_s)
                 longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = copy.deepcopy(self._lane_type_mapping.get(lane['type'], 'unspecified'))
-                positions += [{'lane_id': lane_id, 's': tmp_s, 'longlat': longlat, 'type': type}]
+                positions += [{'lane_id': lane_id, 
+                               's': tmp_s, 
+                               'xy': (x, y),
+                               'longlat': longlat, 
+                               'type': type}]
 
                 # 2. 前驱道路
                 pre_lanes = lane['predecessors']
                 for pre_lane in pre_lanes:
                     pre_lane_id = pre_lane['id']
                     pre_lane_ = copy.deepcopy(self._agent._simulator.map.get_lane(pre_lane_id))
                     pre_lane_nodes = pre_lane_['center_line']['nodes']
                     tmp_s = pre_lane_['length'] - radius_
                     tmp_s = tmp_s if tmp_s >= 0 else 0
                     x, y = get_xy_in_lane(pre_lane_nodes, tmp_s, 'back')
                     longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                     type = self._lane_type_mapping.get(pre_lane_['type'], 'unspecified')
-                    positions += [{'lane_id': pre_lane_id, 's': tmp_s, 'longlat': longlat, 'type': type}]
+                    positions += [{'lane_id': pre_lane_id, 
+                                   's': tmp_s, 
+                                   'xy': (x, y),
+                                   'longlat': longlat, 
+                                   'type': type}]
             elif agent_s == lane['length']:
                 # 处于当前道路的尾部端点位置
                 # 1. 当前道路
                 tmp_s = agent_s - radius_
                 tmp_s = tmp_s if tmp_s >= 0 else 0
                 x, y = get_xy_in_lane(nodes, tmp_s, 'back')
                 longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                positions += [{'lane_id': lane_id, 's': tmp_s, 'longlat': longlat, 'type': type}]
+                positions += [{'lane_id': lane_id, 
+                               's': tmp_s, 
+                               'xy': (x, y),
+                               'longlat': longlat, 
+                               'type': type}]
 
                 # 2. 后继道路
                 suc_lanes = lane['successors']
                 for suc_lane in suc_lanes:
                     suc_lane_id = suc_lane['id']
                     suc_lane_ = copy.deepcopy(self._agent._simulator.map.get_lane(suc_lane_id))
                     suc_lane_nodes = suc_lane_['center_line']['nodes']
                     tmp_s = radius_
                     tmp_s = tmp_s if tmp_s <= suc_lane_['length'] else suc_lane_['length']
                     x, y = get_xy_in_lane(suc_lane_nodes, tmp_s)
                     longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
                     type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                    positions += [{'lane_id': suc_lane_id, 's': tmp_s, 'longlat': longlat, 'type': type}]
+                    positions += [{'lane_id': suc_lane_id, 
+                                   's': tmp_s, 
+                                   'xy': (x, y),
+                                   'longlat': longlat, 
+                                   'type': type}]
             else:
                 # 非端点位置
                 neg_s = agent_s - radius_
                 neg_s = neg_s if neg_s >= 0 else 0
                 x, y = get_xy_in_lane(nodes, neg_s, 'back')
                 longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                positions += [{'lans_id': lane_id, 's': neg_s, 'longlat': longlat, 'type': type}]
+                positions += [{'lans_id': lane_id, 
+                               's': neg_s, 
+                               'xy': (x, y),
+                               'longlat': longlat, 
+                               'type': type}]
 
                 pos_s = agent_s + radius_
                 pos_s = pos_s if pos_s <= lane['length'] else lane['length']
                 x, y = get_xy_in_lane(nodes, pos_s)
                 longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
-                positions += [{'lans_id': lane_id, 's': neg_s, 'longlat': longlat, 'type': type}]
+                positions += [{'lans_id': lane_id, 
+                               's': neg_s, 
+                               'xy': (x, y),
+                               'longlat': longlat, 
+                               'type': type}]
         return positions
 
     async def PerceivePoi(self, radius:int=None, category:str=None):
         """
         POI感知
         Sence POI
```

### Comparing `pycityagent-1.1.0/pycityagent/brain/static.py` & `pycityagent-1.1.1/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/cc/cc.py` & `pycityagent-1.1.1/pycityagent/cc/cc.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.1/pycityagent/hubconnector/hubconnector.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/image/image.py` & `pycityagent-1.1.1/pycityagent/image/image.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/simulator.py` & `pycityagent-1.1.1/pycityagent/simulator.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/st/st.py` & `pycityagent-1.1.1/pycityagent/st/st.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.1/pycityagent/urbanllm/urbanllm.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         - prompt: 理解提示词 - 例如理解方向. The understanding prompts
 
         Returns:
         - (str): the understanding content
         """
         ppt = "如何理解这幅图像？"
         if prompt != None:
-            ppt += prompt
+            ppt = prompt
         dialog = [{
             'role': 'user',
             'content': [
                 {'image': 'file://' + img_path},
                 {'text': ppt}
             ]
         }]
@@ -97,15 +97,15 @@
                 )
         if response.status_code == HTTPStatus.OK:
             return response.output.choices[0]['message']['content']
         else:
             print(response.code)  # The error code.
             return "Error"
 
-    def img_generate(self, prompt, size:str='512*512', quantity:int = 1):
+    def img_generate(self, prompt:str, size:str='512*512', quantity:int = 1):
         """
         图像生成
         Image generation
 
         Args:
         - prompt (str): 图像生成提示词. The image generation prompts
         - size (str): 生成图像尺寸, 默认为'512*512'. The image size, default: '512*512'
```

### Comparing `pycityagent-1.1.0/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.1/pycityagent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.0
+Version: 1.1.1
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 <!-- TOC -->
 
 ## Introduction
 ### Framework of CityAgent
 - ![framwork](./static/framework.png)
 
 ### Workflow of CityAgent
-- ![workflow](./static/workflow.png)
+- ![workflow](./static/workflow_1.png)
 
 ## Hands On - By An Easy Demo
 ### Apply for your App
 - You first need to register your account in the [Opencity website](https://opencity.fiblab.net/)
 - Login to the console, create your own app.
 - Get your app_id and app_secret
     - ![app](./static/app.png)
```

### Comparing `pycityagent-1.1.0/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.1/pycityagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.0/pyproject.toml` & `pycityagent-1.1.1/pyproject.toml`

 * *Files identical despite different names*

