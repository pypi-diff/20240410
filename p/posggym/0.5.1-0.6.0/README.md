# Comparing `tmp/posggym-0.5.1.tar.gz` & `tmp/posggym-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posggym-0.5.1.tar", last modified: Wed Nov 22 22:24:47 2023, max compression
+gzip compressed data, was "posggym-0.6.0.tar", last modified: Wed Apr 10 14:14:38 2024, max compression
```

## Comparing `posggym-0.5.1.tar` & `posggym-0.6.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.987355 posggym-0.5.1/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1067 2023-04-21 13:35:29.000000 posggym-0.5.1/LICENSE
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    11114 2023-11-22 22:24:47.987355 posggym-0.5.1/PKG-INFO
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8364 2023-10-26 03:12:14.000000 posggym-0.5.1/README.md
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.971355 posggym-0.5.1/posggym/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      844 2023-11-22 22:15:08.000000 posggym-0.5.1/posggym/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2669 2023-11-17 20:29:42.000000 posggym-0.5.1/posggym/agents/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/classic/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-06-16 19:26:10.000000 posggym-0.5.1/posggym/agents/classic/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/continuous/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/agents/continuous/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/continuous/driving_continuous/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2515 2023-06-19 12:22:32.000000 posggym-0.5.1/posggym/agents/continuous/driving_continuous/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/continuous/drone_team_capture/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      782 2023-08-09 21:53:31.000000 posggym-0.5.1/posggym/agents/continuous/drone_team_capture/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14002 2023-11-08 18:31:40.000000 posggym-0.5.1/posggym/agents/continuous/drone_team_capture/heuristic.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/continuous/predator_prey_continuous/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3472 2023-06-16 13:55:21.000000 posggym-0.5.1/posggym/agents/continuous/predator_prey_continuous/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10202 2023-11-08 18:34:29.000000 posggym-0.5.1/posggym/agents/continuous/predator_prey_continuous/heuristic.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/continuous/pursuit_evasion_continuous/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3271 2023-06-22 18:57:46.000000 posggym-0.5.1/posggym/agents/continuous/pursuit_evasion_continuous/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9860 2023-11-08 18:37:08.000000 posggym-0.5.1/posggym/agents/continuous/pursuit_evasion_continuous/shortest_path.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/evaluation/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-11-18 19:34:33.000000 posggym-0.5.1/posggym/agents/evaluation/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9411 2023-11-18 19:08:23.000000 posggym-0.5.1/posggym/agents/evaluation/diversity.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    18919 2023-11-18 19:03:30.000000 posggym-0.5.1/posggym/agents/evaluation/pairwise.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/agents/grid_world/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/cooperative_reaching/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      946 2023-11-18 18:03:02.000000 posggym-0.5.1/posggym/agents/grid_world/cooperative_reaching/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10237 2023-11-17 19:30:36.000000 posggym-0.5.1/posggym/agents/grid_world/cooperative_reaching/heuristic.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/driving/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2915 2023-11-18 18:03:21.000000 posggym-0.5.1/posggym/agents/grid_world/driving/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14094 2023-11-18 18:12:19.000000 posggym-0.5.1/posggym/agents/grid_world/driving/shortest_path.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/driving_gen/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1685 2023-11-17 20:34:47.000000 posggym-0.5.1/posggym/agents/grid_world/driving_gen/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2154 2023-11-08 16:20:52.000000 posggym-0.5.1/posggym/agents/grid_world/driving_gen/shortest_path.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/level_based_foraging/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3439 2023-11-17 20:12:49.000000 posggym-0.5.1/posggym/agents/grid_world/level_based_foraging/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10054 2023-11-17 19:56:25.000000 posggym-0.5.1/posggym/agents/grid_world/level_based_foraging/heuristic.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/predator_prey/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2143 2023-11-17 20:13:28.000000 posggym-0.5.1/posggym/agents/grid_world/predator_prey/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10576 2023-11-18 18:26:50.000000 posggym-0.5.1/posggym/agents/grid_world/predator_prey/heuristic.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/grid_world/pursuit_evasion/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6113 2023-11-17 20:21:31.000000 posggym-0.5.1/posggym/agents/grid_world/pursuit_evasion/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10025 2023-11-14 20:50:53.000000 posggym-0.5.1/posggym/agents/grid_world/pursuit_evasion/shortest_path.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9502 2023-11-08 14:53:30.000000 posggym-0.5.1/posggym/agents/policy.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4544 2023-11-08 18:17:26.000000 posggym-0.5.1/posggym/agents/random_policies.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    27346 2023-11-17 20:30:15.000000 posggym-0.5.1/posggym/agents/registration.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    23589 2023-11-17 19:46:28.000000 posggym-0.5.1/posggym/agents/torch_policy.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.975355 posggym-0.5.1/posggym/agents/utils/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-06-16 19:25:57.000000 posggym-0.5.1/posggym/agents/utils/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6628 2023-11-08 18:05:02.000000 posggym-0.5.1/posggym/agents/utils/action_distributions.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3035 2023-06-16 19:26:01.000000 posggym-0.5.1/posggym/agents/utils/download.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2928 2023-06-16 19:26:03.000000 posggym-0.5.1/posggym/agents/utils/processors.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/agents/wrappers/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       62 2023-11-18 12:46:28.000000 posggym-0.5.1/posggym/agents/wrappers/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4045 2023-11-07 16:16:52.000000 posggym-0.5.1/posggym/agents/wrappers/agent_env.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      468 2023-11-22 22:13:14.000000 posggym-0.5.1/posggym/config.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    25277 2023-08-11 15:13:08.000000 posggym-0.5.1/posggym/core.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/envs/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4524 2023-11-14 18:43:16.000000 posggym-0.5.1/posggym/envs/__init__.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/envs/classic/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/classic/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14697 2023-08-11 14:20:40.000000 posggym-0.5.1/posggym/envs/classic/mabc.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7745 2023-08-11 14:20:54.000000 posggym-0.5.1/posggym/envs/classic/rock_paper_scissors.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14694 2023-08-11 14:21:08.000000 posggym-0.5.1/posggym/envs/classic/tiger.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/envs/continuous/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/continuous/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37736 2023-08-11 14:20:13.000000 posggym-0.5.1/posggym/envs/continuous/core.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    36304 2023-08-11 14:19:54.000000 posggym-0.5.1/posggym/envs/continuous/driving_continuous.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    30637 2023-08-11 14:19:41.000000 posggym-0.5.1/posggym/envs/continuous/drone_team_capture.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    34510 2023-08-11 14:19:12.000000 posggym-0.5.1/posggym/envs/continuous/predator_prey_continuous.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37696 2023-08-11 14:19:26.000000 posggym-0.5.1/posggym/envs/continuous/pursuit_evasion_continuous.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/envs/grid_world/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    20001 2023-11-12 22:07:56.000000 posggym-0.5.1/posggym/envs/grid_world/cooperative_reaching.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    20053 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/core.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    39964 2023-11-10 15:33:23.000000 posggym-0.5.1/posggym/envs/grid_world/driving.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7204 2023-11-17 19:15:32.000000 posggym-0.5.1/posggym/envs/grid_world/driving_gen.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.979355 posggym-0.5.1/posggym/envs/grid_world/img/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8017 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/agent.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8853 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/agent_white.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    15966 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/apple.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10610 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/drone.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8020 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/house.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    13645 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/robber.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    35516 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/grid_world/img/robot.png
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37385 2023-11-14 16:24:15.000000 posggym-0.5.1/posggym/envs/grid_world/level_based_foraging.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    36380 2023-11-14 16:29:19.000000 posggym-0.5.1/posggym/envs/grid_world/predator_prey.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37012 2023-11-14 19:40:19.000000 posggym-0.5.1/posggym/envs/grid_world/pursuit_evasion.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14611 2023-10-25 00:50:39.000000 posggym-0.5.1/posggym/envs/grid_world/render.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    19420 2023-08-11 14:22:57.000000 posggym-0.5.1/posggym/envs/grid_world/two_paths.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    20171 2023-08-11 14:23:08.000000 posggym-0.5.1/posggym/envs/grid_world/uav.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    22033 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/envs/registration.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3968 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/error.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1735 2023-06-07 20:31:41.000000 posggym-0.5.1/posggym/logger.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    15420 2023-08-11 14:58:38.000000 posggym-0.5.1/posggym/model.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/py.typed
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/posggym/utils/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       74 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/utils/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9122 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/utils/env_checker.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5612 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/utils/history.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9191 2023-08-11 14:27:50.000000 posggym-0.5.1/posggym/utils/model_checker.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    31891 2023-08-11 14:27:28.000000 posggym-0.5.1/posggym/utils/passive_env_checker.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2647 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/utils/seeding.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/posggym/vector/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      125 2023-10-28 22:14:06.000000 posggym-0.5.1/posggym/vector/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    13837 2023-11-18 13:38:43.000000 posggym-0.5.1/posggym/vector/sync_vector_env.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/posggym/wrappers/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      645 2023-10-28 22:25:29.000000 posggym-0.5.1/posggym/wrappers/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4764 2023-08-11 17:12:53.000000 posggym-0.5.1/posggym/wrappers/discretize_actions.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2572 2023-08-11 17:12:59.000000 posggym-0.5.1/posggym/wrappers/env_checker.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      930 2023-08-11 17:13:15.000000 posggym-0.5.1/posggym/wrappers/flatten_observations.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/posggym/wrappers/monitoring/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.5.1/posggym/wrappers/monitoring/__init__.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7897 2023-11-22 22:21:20.000000 posggym-0.5.1/posggym/wrappers/monitoring/video_recorder.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1790 2023-08-11 17:13:47.000000 posggym-0.5.1/posggym/wrappers/order_enforcing.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3714 2023-08-11 18:15:39.000000 posggym-0.5.1/posggym/wrappers/petting_zoo.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5974 2023-11-18 13:58:54.000000 posggym-0.5.1/posggym/wrappers/record_episode_statistics.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7896 2023-11-22 22:21:20.000000 posggym-0.5.1/posggym/wrappers/record_video.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4218 2023-08-11 17:16:18.000000 posggym-0.5.1/posggym/wrappers/rescale_actions.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3646 2023-08-11 17:15:03.000000 posggym-0.5.1/posggym/wrappers/rescale_observations.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4708 2023-08-11 15:54:12.000000 posggym-0.5.1/posggym/wrappers/rllib_env.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6261 2023-11-18 13:38:51.000000 posggym-0.5.1/posggym/wrappers/stack.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2169 2023-08-11 17:15:56.000000 posggym-0.5.1/posggym/wrappers/time_limit.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/posggym.egg-info/
--rw-r--r--   0 jonathon  (1000) jonathon  (1000)    11114 2023-11-22 22:24:47.000000 posggym-0.5.1/posggym.egg-info/PKG-INFO
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3967 2023-11-22 22:24:47.000000 posggym-0.5.1/posggym.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        1 2023-11-22 22:24:47.000000 posggym-0.5.1/posggym.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      562 2023-11-22 22:24:47.000000 posggym-0.5.1/posggym.egg-info/requires.txt
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        8 2023-11-22 22:24:47.000000 posggym-0.5.1/posggym.egg-info/top_level.txt
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4317 2023-11-19 12:59:28.000000 posggym-0.5.1/pyproject.toml
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       38 2023-11-22 22:24:47.987355 posggym-0.5.1/setup.cfg
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3855 2023-11-22 22:12:51.000000 posggym-0.5.1/setup.py
-drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2023-11-22 22:24:47.983355 posggym-0.5.1/tests/
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5221 2023-08-11 14:07:21.000000 posggym-0.5.1/tests/test_core.py
--rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1748 2023-08-11 14:07:40.000000 posggym-0.5.1/tests/test_model.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.632297 posggym-0.6.0/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1067 2023-04-21 13:35:29.000000 posggym-0.6.0/LICENSE
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     9903 2024-04-10 14:14:38.632297 posggym-0.6.0/PKG-INFO
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7660 2024-04-10 13:41:06.000000 posggym-0.6.0/README.md
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.612296 posggym-0.6.0/posggym/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      845 2024-04-10 14:02:46.000000 posggym-0.6.0/posggym/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2669 2023-11-17 20:29:42.000000 posggym-0.6.0/posggym/agents/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/classic/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-06-16 19:26:10.000000 posggym-0.6.0/posggym/agents/classic/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/continuous/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/agents/continuous/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/continuous/driving_continuous/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2406 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/continuous/driving_continuous/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/continuous/drone_team_capture/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      782 2023-08-09 21:53:31.000000 posggym-0.6.0/posggym/agents/continuous/drone_team_capture/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14002 2023-11-08 18:31:40.000000 posggym-0.6.0/posggym/agents/continuous/drone_team_capture/heuristic.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/continuous/predator_prey_continuous/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3486 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/continuous/predator_prey_continuous/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10202 2023-11-08 18:34:29.000000 posggym-0.6.0/posggym/agents/continuous/predator_prey_continuous/heuristic.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/continuous/pursuit_evasion_continuous/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3131 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/continuous/pursuit_evasion_continuous/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9860 2023-11-08 18:37:08.000000 posggym-0.6.0/posggym/agents/continuous/pursuit_evasion_continuous/shortest_path.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/evaluation/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-11-18 19:34:33.000000 posggym-0.6.0/posggym/agents/evaluation/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9388 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/evaluation/diversity.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    18751 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/evaluation/pairwise.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/grid_world/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/agents/grid_world/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.616297 posggym-0.6.0/posggym/agents/grid_world/cooperative_reaching/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      946 2023-11-18 18:03:02.000000 posggym-0.6.0/posggym/agents/grid_world/cooperative_reaching/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10237 2023-11-17 19:30:36.000000 posggym-0.6.0/posggym/agents/grid_world/cooperative_reaching/heuristic.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/grid_world/driving/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2846 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/grid_world/driving/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    11773 2023-11-23 15:25:57.000000 posggym-0.6.0/posggym/agents/grid_world/driving/shortest_path.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/grid_world/driving_gen/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1685 2023-11-17 20:34:47.000000 posggym-0.6.0/posggym/agents/grid_world/driving_gen/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2379 2023-11-23 15:24:46.000000 posggym-0.6.0/posggym/agents/grid_world/driving_gen/shortest_path.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/grid_world/level_based_foraging/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3331 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/grid_world/level_based_foraging/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10054 2023-11-17 19:56:25.000000 posggym-0.6.0/posggym/agents/grid_world/level_based_foraging/heuristic.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/grid_world/predator_prey/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2074 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/grid_world/predator_prey/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10576 2023-11-18 18:26:50.000000 posggym-0.6.0/posggym/agents/grid_world/predator_prey/heuristic.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/grid_world/pursuit_evasion/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6051 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/agents/grid_world/pursuit_evasion/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10025 2023-11-14 20:50:53.000000 posggym-0.6.0/posggym/agents/grid_world/pursuit_evasion/shortest_path.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9508 2024-04-06 18:18:36.000000 posggym-0.6.0/posggym/agents/policy.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4544 2023-11-08 18:17:26.000000 posggym-0.6.0/posggym/agents/random_policies.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    27991 2024-04-06 19:11:35.000000 posggym-0.6.0/posggym/agents/registration.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    23982 2024-04-06 18:30:29.000000 posggym-0.6.0/posggym/agents/torch_policy.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/utils/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-06-16 19:25:57.000000 posggym-0.6.0/posggym/agents/utils/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6628 2023-11-08 18:05:02.000000 posggym-0.6.0/posggym/agents/utils/action_distributions.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2993 2024-04-06 18:31:32.000000 posggym-0.6.0/posggym/agents/utils/download.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2928 2023-06-16 19:26:03.000000 posggym-0.6.0/posggym/agents/utils/processors.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/agents/wrappers/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       62 2023-11-18 12:46:28.000000 posggym-0.6.0/posggym/agents/wrappers/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4327 2024-01-19 20:29:32.000000 posggym-0.6.0/posggym/agents/wrappers/agent_env.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      354 2024-04-10 00:41:00.000000 posggym-0.6.0/posggym/config.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    25362 2024-04-06 19:15:38.000000 posggym-0.6.0/posggym/core.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/envs/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4524 2023-11-14 18:43:16.000000 posggym-0.6.0/posggym/envs/__init__.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/envs/classic/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/classic/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14697 2023-08-11 14:20:40.000000 posggym-0.6.0/posggym/envs/classic/mabc.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7745 2023-08-11 14:20:54.000000 posggym-0.6.0/posggym/envs/classic/rock_paper_scissors.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14694 2023-08-11 14:21:08.000000 posggym-0.6.0/posggym/envs/classic/tiger.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.620297 posggym-0.6.0/posggym/envs/continuous/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/continuous/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    38207 2024-04-06 19:11:35.000000 posggym-0.6.0/posggym/envs/continuous/core.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    36309 2024-04-06 17:57:48.000000 posggym-0.6.0/posggym/envs/continuous/driving_continuous.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    30637 2023-08-11 14:19:41.000000 posggym-0.6.0/posggym/envs/continuous/drone_team_capture.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    34529 2024-04-06 17:59:24.000000 posggym-0.6.0/posggym/envs/continuous/predator_prey_continuous.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37696 2023-08-11 14:19:26.000000 posggym-0.6.0/posggym/envs/continuous/pursuit_evasion_continuous.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.624297 posggym-0.6.0/posggym/envs/grid_world/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    19998 2024-04-06 18:00:46.000000 posggym-0.6.0/posggym/envs/grid_world/cooperative_reaching.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    20315 2024-04-06 18:03:02.000000 posggym-0.6.0/posggym/envs/grid_world/core.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    39957 2024-04-06 18:03:50.000000 posggym-0.6.0/posggym/envs/grid_world/driving.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7204 2023-11-17 19:15:32.000000 posggym-0.6.0/posggym/envs/grid_world/driving_gen.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.624297 posggym-0.6.0/posggym/envs/grid_world/img/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8017 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/agent.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8853 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/agent_white.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    15966 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/apple.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    10610 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/drone.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     8020 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/house.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    13645 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/robber.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    35516 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/envs/grid_world/img/robot.png
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37329 2024-04-06 18:05:16.000000 posggym-0.6.0/posggym/envs/grid_world/level_based_foraging.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    36426 2024-04-06 18:05:37.000000 posggym-0.6.0/posggym/envs/grid_world/predator_prey.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    37017 2024-02-06 18:07:55.000000 posggym-0.6.0/posggym/envs/grid_world/pursuit_evasion.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    14637 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/envs/grid_world/render.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    19405 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/envs/grid_world/two_paths.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    20146 2024-01-19 17:55:55.000000 posggym-0.6.0/posggym/envs/grid_world/uav.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    22414 2024-04-06 18:26:33.000000 posggym-0.6.0/posggym/envs/registration.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3968 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/error.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1735 2023-06-07 20:31:41.000000 posggym-0.6.0/posggym/logger.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    15553 2024-04-06 17:51:28.000000 posggym-0.6.0/posggym/model.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/py.typed
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.624297 posggym-0.6.0/posggym/utils/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       74 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/utils/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9031 2024-04-06 17:41:35.000000 posggym-0.6.0/posggym/utils/env_checker.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5545 2024-01-02 20:05:13.000000 posggym-0.6.0/posggym/utils/history.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     9120 2024-04-06 17:42:59.000000 posggym-0.6.0/posggym/utils/model_checker.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    32128 2024-04-06 17:44:13.000000 posggym-0.6.0/posggym/utils/passive_env_checker.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2780 2024-04-06 17:45:31.000000 posggym-0.6.0/posggym/utils/seeding.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.624297 posggym-0.6.0/posggym/vector/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      125 2023-10-28 22:14:06.000000 posggym-0.6.0/posggym/vector/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)    13776 2024-04-06 17:39:59.000000 posggym-0.6.0/posggym/vector/sync_vector_env.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.628297 posggym-0.6.0/posggym/wrappers/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      645 2023-10-28 22:25:29.000000 posggym-0.6.0/posggym/wrappers/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4767 2024-04-06 17:29:48.000000 posggym-0.6.0/posggym/wrappers/discretize_actions.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2573 2024-04-06 17:29:37.000000 posggym-0.6.0/posggym/wrappers/env_checker.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      930 2023-08-11 17:13:15.000000 posggym-0.6.0/posggym/wrappers/flatten_observations.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.628297 posggym-0.6.0/posggym/wrappers/monitoring/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        0 2023-04-21 13:35:30.000000 posggym-0.6.0/posggym/wrappers/monitoring/__init__.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7647 2024-04-06 17:33:57.000000 posggym-0.6.0/posggym/wrappers/monitoring/video_recorder.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1790 2023-08-11 17:13:47.000000 posggym-0.6.0/posggym/wrappers/order_enforcing.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3714 2023-08-11 18:15:39.000000 posggym-0.6.0/posggym/wrappers/petting_zoo.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5974 2023-11-18 13:58:54.000000 posggym-0.6.0/posggym/wrappers/record_episode_statistics.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     7650 2024-04-06 17:30:26.000000 posggym-0.6.0/posggym/wrappers/record_video.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4218 2023-08-11 17:16:18.000000 posggym-0.6.0/posggym/wrappers/rescale_actions.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3646 2023-08-11 17:15:03.000000 posggym-0.6.0/posggym/wrappers/rescale_observations.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4957 2024-04-06 17:32:03.000000 posggym-0.6.0/posggym/wrappers/rllib_env.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     6261 2023-11-18 13:38:51.000000 posggym-0.6.0/posggym/wrappers/stack.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     2176 2024-04-06 17:32:23.000000 posggym-0.6.0/posggym/wrappers/time_limit.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.628297 posggym-0.6.0/posggym.egg-info/
+-rw-r--r--   0 jonathon  (1000) jonathon  (1000)     9903 2024-04-10 14:14:38.000000 posggym-0.6.0/posggym.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3967 2024-04-10 14:14:38.000000 posggym-0.6.0/posggym.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        1 2024-04-10 14:14:38.000000 posggym-0.6.0/posggym.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)      429 2024-04-10 14:14:38.000000 posggym-0.6.0/posggym.egg-info/requires.txt
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)        8 2024-04-10 14:14:38.000000 posggym-0.6.0/posggym.egg-info/top_level.txt
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     4034 2024-04-10 13:53:47.000000 posggym-0.6.0/pyproject.toml
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)       38 2024-04-10 14:14:38.632297 posggym-0.6.0/setup.cfg
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     3877 2024-04-10 13:53:47.000000 posggym-0.6.0/setup.py
+drwxrwxr-x   0 jonathon  (1000) jonathon  (1000)        0 2024-04-10 14:14:38.628297 posggym-0.6.0/tests/
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     5221 2023-08-11 14:07:21.000000 posggym-0.6.0/tests/test_core.py
+-rw-rw-r--   0 jonathon  (1000) jonathon  (1000)     1748 2023-08-11 14:07:40.000000 posggym-0.6.0/tests/test_model.py
```

### Comparing `posggym-0.5.1/LICENSE` & `posggym-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/PKG-INFO` & `posggym-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: posggym
-Version: 0.5.1
-Summary: A collection of diverse environments and reference agents for reinforcement learning and planning research in Partially Observable Stochastic Games (POSGs). .
+Version: 0.6.0
+Summary: A library for planning and reinforcement learning research in partially observable, multi-agent environments.
 Author-email: Jonathon Schwartz <jonathon.schwartz@anu.edu.au>
 License: MIT License
 Project-URL: Homepage, https://github.com/RDLLab/posggym
 Project-URL: Repository, https://github.com/RDLLab/posggym/
 Project-URL: Documentation, https://posggym.readthedocs.io/
 Project-URL: Bug Report, https://github.com/RDLLab/posggym/issues
 Keywords: multiagent-systems,reinforcement-learning,planning,gymnasium,POSG
@@ -21,86 +21,63 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium>=0.26
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: importlib-metadata>=4.8.0; python_version < "3.10"
-Provides-Extra: grid-world
-Requires-Dist: pygame>=2.0; extra == "grid-world"
-Provides-Extra: continuous
-Requires-Dist: pygame>=2.0; extra == "continuous"
-Requires-Dist: pymunk>=6.0.0; extra == "continuous"
-Provides-Extra: envs-all
-Requires-Dist: pygame>=2.0; extra == "envs-all"
-Requires-Dist: pymunk>=6.0.0; extra == "envs-all"
+Requires-Dist: pygame>=2.0
+Requires-Dist: pymunk>=6.0.0
 Provides-Extra: agents
-Requires-Dist: pygame>=2.0; extra == "agents"
-Requires-Dist: pymunk>=6.0.0; extra == "agents"
 Requires-Dist: types-requests>=2.28; extra == "agents"
 Requires-Dist: requests>=2.28; extra == "agents"
 Requires-Dist: clint>=0.5.1; extra == "agents"
 Requires-Dist: torch>=1.11.0; extra == "agents"
 Provides-Extra: other
 Requires-Dist: moviepy>=1.0.0; extra == "other"
 Requires-Dist: pandas>=1.0; extra == "other"
 Requires-Dist: seaborn>=0.13.0; extra == "other"
 Requires-Dist: matplotlib>=3.0.0; extra == "other"
 Provides-Extra: all
-Requires-Dist: pygame>=2.0; extra == "all"
-Requires-Dist: pymunk>=6.0.0; extra == "all"
 Requires-Dist: types-requests>=2.28; extra == "all"
 Requires-Dist: requests>=2.28; extra == "all"
 Requires-Dist: clint>=0.5.1; extra == "all"
-Requires-Dist: torch>=1.11.0; extra == "all"
+Requires-Dist: torch>=2.0; extra == "all"
 Requires-Dist: moviepy>=1.0.0; extra == "all"
 Requires-Dist: seaborn>=0.11.1; extra == "all"
 Requires-Dist: matplotlib>=3.3.4; extra == "all"
 Requires-Dist: pandas>=1.0; extra == "all"
 Provides-Extra: testing
 Requires-Dist: pytest>=7.2; extra == "testing"
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # POSGGym
 
-POSGGym is an open source Python library providing implementations of Partially Observable Stochastic Game (POSG) environments coupled with dynamic models of each environment, all under a unified API. While there are a number of amazing open-source implementations for POSG environments, very few have support for dynamic models that can be used for planning, especially for continuous domains. The aim of this library is to fill this gap.
+POSGGym is a Python library for planning and reinforcement learning research in partially observable, multi-agent environments. It provides a collection of discrete and continuous environments along with reference agents to allow for reproducible evaluations. The API aims to mimic that of [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) with the addition of a model API that can be used for planning.
 
-A key goal of POSGGym is to provide easy to use and understand open-source implementations for many of the environments commonly used in the partially observable multi-agent planning literature.
+The documentation for the project is available online at [posggym.readthedocs.io/](https://posggym.readthedocs.io/). For a guide to building the documentation locally see [docs/README.md](docs/README.md).
 
-POSGGym also provides a collection of reference agents for it's various environments and a unified Agents API for using these agents. These agents can be used to evaluate algorithms, and includes both hand-coded bots and agents trained using reinforcement learning.
-
-POSGGym is directly inspired by and adapted from the [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) libraries for reinforcement learning. The key additions in POSGGym are support for environment models which can be used for planning and reference agents. POSGGym's API aims to stay as close to the Gymnasium and PettingZoo Parallel APIs as possible while incorporating models and agents into the mix.
-
-Any POSGGym environment can be converted into a PettingZoo environment using a simple wrapper (`posggym.wrappers.petting_zoo.PettingZoo`). This allows for easy integration with the ecosystem of libraries that support PettingZoo.
-
-
-## Documentation
-
-The documentation for the project is available at [posggym.readthedocs.io/](https://posggym.readthedocs.io/).
-
-For a guide to building the documentation locally see [docs/README.md](docs/README.md).
+Some baseline implementations of planning and reinforcement learning algorithms for POSGGym are available in the [POSGGym-Baselines](https://github.com/RDLLab/posggym-baselines) library. Compatibility with other popular reinforcement learning libraries is possible using the [PettingZoo wrapper](#compatibility-with-pettingzoo).
 
 ## Installation
 
 POSGGym supports and tests for `Python>=3.8`. We recommend using a virtual environment to install POSGGym (e.g. [conda](https://docs.conda.io/projects/conda/en/latest/index.html), [venv](https://docs.python.org/3/library/venv.html)).
 
 ### Using pip
 
 The latest release version of POSGGym can be installed using `pip` by running:
 
 ```bash
 pip install posggym
 ```
 
-This will install the base dependencies for running the main environments and download the agent models (so may take a few minutes), but but in order to minimise the number of unused dependencies installed may not include all dependencies for all environments or for rendering some environments, and will not include dependencies for running many posggym agents.
-
-You can install all dependencies for a family of environments like `pip install posggym[grid-world]` and `pip install posggym[continuous]` or dependencies for all environments using `pip install posggym[envs-all]`.
+This will install the base dependencies for running all the environments and download the agent models (so may take a few minutes). In order to minimise the number of unused dependencies installed the default install does not include dependencies for running many posggym agents (specifically PyTorch).
 
 You can install dependencies for POSGGym agents using `pip install posggym[agents]` or to install dependencies for all environments and agents use `pip install posggym[all]`.
 
 ### Installing from source
 
 To install POSGGym from source, first clone the repository then run:
 
@@ -114,37 +91,36 @@
 ```bash
 pip install -e .[all]
 ```
 
 To run tests, install the test dependencies and then run the tests:
 
 ```bash
-pip install -e .[test]
+pip install -e .[testing]
 pytest
 ```
 
 Or alternatively you can run one of the examples from the `examples` directory:
 
 ```bash
-python examples/run_random_agents.py --env_id Driving-v0 --num_episodes 10 --render_mode human
+python examples/run_random_agents.py --env_id Driving-v1 --num_episodes 10 --render_mode human
 ```
 
-
 ## Environments
 
 POSGGym includes the following families of environments (for a full list of environments and their descriptsion see the [documentation](https://posggym.readthedocs.io/)).
 
 - [Classic](https://posggym.readthedocs.io/en/latest/environments/classic.html) - These are classic POSG problems from the literature.
 - [Grid-World](https://posggym.readthedocs.io/en/latest/environments/grid_world.html) - These environments are all based in a 2D Gridworld.
 - [Continuous](https://posggym.readthedocs.io/en/latest/environments/continuous.html) - 2D environments with continuous state, actions, and observations.
 
 
 ## Environment API
 
-POSGGym models each environment as a python `env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
+POSGGym models each environment as a python `Env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
 
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 observations, infos = env.reset(seed=42)
 
 for t in range(100):
@@ -156,19 +132,18 @@
         observations, infos = env.reset()
 
 env.close()
 ```
 
 ## Model API
 
-Every environment provides access to a model of the environment in the form of a python `model` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
+Every environment provides access to a model of the environment in the form of a `POSGModel` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
 
 The following is an example of accessing and using the environment model:
 
-
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 model = env.model
 model.seed(seed=42)
 
 state = model.sample_initial_state()
@@ -179,61 +154,73 @@
     state, observations, rewards, terminations, truncations, all_done, infos = model.step(state, actions)
 
     if all_done:
         state = model.sample_initial_state()
         observations = model.sample_initial_obs(state)
 ```
 
-The base model API is very similar to the environment API. The key difference that all methods are stateless so can be used repeatedly for planning. Indeed the `env` class for the built-in environments are mainly just a wrappers over the underlying `model` class that manage the state and add support for rendering.
+The base model API is very similar to the environment API. The key difference that all methods are stateless so can be repeatedly sampled for planning. Indeed the `Env` class implementations for the built-in environments are a wrapper over an underlying `POSGModel` class that manages the state and adds support for rendering.
 
-Note that unlike for the `env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
+Note that unlike for `Env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
 
 ```python
 timestep = model.step(state, actions)
 observations = timestep.observations
 infos = timestep.infos
 ```
 
-Both the `env` and `model` classes support a number of other methods, please see the documentation [posggym.readthedocs.io/](https://posggym.readthedocs.io/) for more details.
+Both the `Env` and `POSGModel` classes support a number of additional methods, refer to the [documentation](https://posggym.readthedocs.io/) for more details.
 
 ## Agents API
 
-POSGGym.Agents models each agent as a python `policy` class, which at it's simplest accepts an observation and returns the next action. Here's an example using one of the K-Level Reasoning policies in the `PursuitEvasion-v0` environment:
+The Agents API provides a way to easy load reference policies that come with POSGGym. Each policy is a `Policy` class, which at it's simplest accepts an observation and returns the next action. The basic Agents API is shown below:
 
 
 ```python
 import posggym
 import posggym.agents as pga
-env = posggym.make("PursuitEvasion-v0", grid="16x16")
+env = posggym.make("PursuitEvasion-v1", grid="16x16")
 
 policies = {
-    '0': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i0-v0", env.model, '0'),
-    '1': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i1-v0", env.model, '1')
+    '0': pga.make("PursuitEvasion-v1/grid=16x16/RL1_i0-v0", env.model, '0'),
+    '1': pga.make("PursuitEvasion-v1/grid=16x16/ShortestPath-v0", env.model, '1')
 }
 
-obs, info = env.reset(seed=42)
+obs, infos = env.reset(seed=42)
 for i, policy in policies.items():
     policy.reset(seed=7)
 
 for t in range(100):
     actions = {i: policies[i].step(obs[i]) for i in env.agents}
-    obs, rewards, termination, truncated, all_done, info = env.step(actions)
+    obs, rewards, terminations, truncations, all_done, infos = env.step(actions)
 
     if all_done:
-        obs, info = env.reset()
+        obs, infos = env.reset()
         for i, policy in policies.items():
             policy.reset()
 
 env.close()
 for policy in policies.values():
     policy.close()
 ```
 
 For a full explanation of the agent API please see the [POSGGym Agents Getting Started documentation](https://posggym.readthedocs.io/en/latest/agents/getting_started.html). A full list of implemented agents is also available in the documentation.
 
+## Compatibility with PettingZoo
+
+Any POSGGym environment can be converted into a PettingZoo `ParallelEnv` environment using the `posggym.wrappers.petting_zoo.PettingZoo` wrapper. This allows for easy integration with the ecosystem of libraries that support PettingZoo.
+
+```python
+import posggym
+from posggym.wrappers.petting_zoo import PettingZoo
+
+env = posggym.make("PredatorPrey-v0")
+env = PettingZoo(env)
+```
+
 ## Citation
 
 You can cite POSGGym as:
 
 ```bibtex
 @misc{schwartzPOSGGym2023,
     title = {POSGGym},
```

### Comparing `posggym-0.5.1/README.md` & `posggym-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,32 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # POSGGym
 
-POSGGym is an open source Python library providing implementations of Partially Observable Stochastic Game (POSG) environments coupled with dynamic models of each environment, all under a unified API. While there are a number of amazing open-source implementations for POSG environments, very few have support for dynamic models that can be used for planning, especially for continuous domains. The aim of this library is to fill this gap.
+POSGGym is a Python library for planning and reinforcement learning research in partially observable, multi-agent environments. It provides a collection of discrete and continuous environments along with reference agents to allow for reproducible evaluations. The API aims to mimic that of [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) with the addition of a model API that can be used for planning.
 
-A key goal of POSGGym is to provide easy to use and understand open-source implementations for many of the environments commonly used in the partially observable multi-agent planning literature.
+The documentation for the project is available online at [posggym.readthedocs.io/](https://posggym.readthedocs.io/). For a guide to building the documentation locally see [docs/README.md](docs/README.md).
 
-POSGGym also provides a collection of reference agents for it's various environments and a unified Agents API for using these agents. These agents can be used to evaluate algorithms, and includes both hand-coded bots and agents trained using reinforcement learning.
-
-POSGGym is directly inspired by and adapted from the [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) libraries for reinforcement learning. The key additions in POSGGym are support for environment models which can be used for planning and reference agents. POSGGym's API aims to stay as close to the Gymnasium and PettingZoo Parallel APIs as possible while incorporating models and agents into the mix.
-
-Any POSGGym environment can be converted into a PettingZoo environment using a simple wrapper (`posggym.wrappers.petting_zoo.PettingZoo`). This allows for easy integration with the ecosystem of libraries that support PettingZoo.
-
-
-## Documentation
-
-The documentation for the project is available at [posggym.readthedocs.io/](https://posggym.readthedocs.io/).
-
-For a guide to building the documentation locally see [docs/README.md](docs/README.md).
+Some baseline implementations of planning and reinforcement learning algorithms for POSGGym are available in the [POSGGym-Baselines](https://github.com/RDLLab/posggym-baselines) library. Compatibility with other popular reinforcement learning libraries is possible using the [PettingZoo wrapper](#compatibility-with-pettingzoo).
 
 ## Installation
 
 POSGGym supports and tests for `Python>=3.8`. We recommend using a virtual environment to install POSGGym (e.g. [conda](https://docs.conda.io/projects/conda/en/latest/index.html), [venv](https://docs.python.org/3/library/venv.html)).
 
 ### Using pip
 
 The latest release version of POSGGym can be installed using `pip` by running:
 
 ```bash
 pip install posggym
 ```
 
-This will install the base dependencies for running the main environments and download the agent models (so may take a few minutes), but but in order to minimise the number of unused dependencies installed may not include all dependencies for all environments or for rendering some environments, and will not include dependencies for running many posggym agents.
-
-You can install all dependencies for a family of environments like `pip install posggym[grid-world]` and `pip install posggym[continuous]` or dependencies for all environments using `pip install posggym[envs-all]`.
+This will install the base dependencies for running all the environments and download the agent models (so may take a few minutes). In order to minimise the number of unused dependencies installed the default install does not include dependencies for running many posggym agents (specifically PyTorch).
 
 You can install dependencies for POSGGym agents using `pip install posggym[agents]` or to install dependencies for all environments and agents use `pip install posggym[all]`.
 
 ### Installing from source
 
 To install POSGGym from source, first clone the repository then run:
 
@@ -53,37 +40,36 @@
 ```bash
 pip install -e .[all]
 ```
 
 To run tests, install the test dependencies and then run the tests:
 
 ```bash
-pip install -e .[test]
+pip install -e .[testing]
 pytest
 ```
 
 Or alternatively you can run one of the examples from the `examples` directory:
 
 ```bash
-python examples/run_random_agents.py --env_id Driving-v0 --num_episodes 10 --render_mode human
+python examples/run_random_agents.py --env_id Driving-v1 --num_episodes 10 --render_mode human
 ```
 
-
 ## Environments
 
 POSGGym includes the following families of environments (for a full list of environments and their descriptsion see the [documentation](https://posggym.readthedocs.io/)).
 
 - [Classic](https://posggym.readthedocs.io/en/latest/environments/classic.html) - These are classic POSG problems from the literature.
 - [Grid-World](https://posggym.readthedocs.io/en/latest/environments/grid_world.html) - These environments are all based in a 2D Gridworld.
 - [Continuous](https://posggym.readthedocs.io/en/latest/environments/continuous.html) - 2D environments with continuous state, actions, and observations.
 
 
 ## Environment API
 
-POSGGym models each environment as a python `env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
+POSGGym models each environment as a python `Env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
 
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 observations, infos = env.reset(seed=42)
 
 for t in range(100):
@@ -95,19 +81,18 @@
         observations, infos = env.reset()
 
 env.close()
 ```
 
 ## Model API
 
-Every environment provides access to a model of the environment in the form of a python `model` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
+Every environment provides access to a model of the environment in the form of a `POSGModel` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
 
 The following is an example of accessing and using the environment model:
 
-
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 model = env.model
 model.seed(seed=42)
 
 state = model.sample_initial_state()
@@ -118,61 +103,73 @@
     state, observations, rewards, terminations, truncations, all_done, infos = model.step(state, actions)
 
     if all_done:
         state = model.sample_initial_state()
         observations = model.sample_initial_obs(state)
 ```
 
-The base model API is very similar to the environment API. The key difference that all methods are stateless so can be used repeatedly for planning. Indeed the `env` class for the built-in environments are mainly just a wrappers over the underlying `model` class that manage the state and add support for rendering.
+The base model API is very similar to the environment API. The key difference that all methods are stateless so can be repeatedly sampled for planning. Indeed the `Env` class implementations for the built-in environments are a wrapper over an underlying `POSGModel` class that manages the state and adds support for rendering.
 
-Note that unlike for the `env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
+Note that unlike for `Env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
 
 ```python
 timestep = model.step(state, actions)
 observations = timestep.observations
 infos = timestep.infos
 ```
 
-Both the `env` and `model` classes support a number of other methods, please see the documentation [posggym.readthedocs.io/](https://posggym.readthedocs.io/) for more details.
+Both the `Env` and `POSGModel` classes support a number of additional methods, refer to the [documentation](https://posggym.readthedocs.io/) for more details.
 
 ## Agents API
 
-POSGGym.Agents models each agent as a python `policy` class, which at it's simplest accepts an observation and returns the next action. Here's an example using one of the K-Level Reasoning policies in the `PursuitEvasion-v0` environment:
+The Agents API provides a way to easy load reference policies that come with POSGGym. Each policy is a `Policy` class, which at it's simplest accepts an observation and returns the next action. The basic Agents API is shown below:
 
 
 ```python
 import posggym
 import posggym.agents as pga
-env = posggym.make("PursuitEvasion-v0", grid="16x16")
+env = posggym.make("PursuitEvasion-v1", grid="16x16")
 
 policies = {
-    '0': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i0-v0", env.model, '0'),
-    '1': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i1-v0", env.model, '1')
+    '0': pga.make("PursuitEvasion-v1/grid=16x16/RL1_i0-v0", env.model, '0'),
+    '1': pga.make("PursuitEvasion-v1/grid=16x16/ShortestPath-v0", env.model, '1')
 }
 
-obs, info = env.reset(seed=42)
+obs, infos = env.reset(seed=42)
 for i, policy in policies.items():
     policy.reset(seed=7)
 
 for t in range(100):
     actions = {i: policies[i].step(obs[i]) for i in env.agents}
-    obs, rewards, termination, truncated, all_done, info = env.step(actions)
+    obs, rewards, terminations, truncations, all_done, infos = env.step(actions)
 
     if all_done:
-        obs, info = env.reset()
+        obs, infos = env.reset()
         for i, policy in policies.items():
             policy.reset()
 
 env.close()
 for policy in policies.values():
     policy.close()
 ```
 
 For a full explanation of the agent API please see the [POSGGym Agents Getting Started documentation](https://posggym.readthedocs.io/en/latest/agents/getting_started.html). A full list of implemented agents is also available in the documentation.
 
+## Compatibility with PettingZoo
+
+Any POSGGym environment can be converted into a PettingZoo `ParallelEnv` environment using the `posggym.wrappers.petting_zoo.PettingZoo` wrapper. This allows for easy integration with the ecosystem of libraries that support PettingZoo.
+
+```python
+import posggym
+from posggym.wrappers.petting_zoo import PettingZoo
+
+env = posggym.make("PredatorPrey-v0")
+env = PettingZoo(env)
+```
+
 ## Citation
 
 You can cite POSGGym as:
 
 ```bibtex
 @misc{schwartzPOSGGym2023,
     title = {POSGGym},
```

### Comparing `posggym-0.5.1/posggym/__init__.py` & `posggym-0.6.0/posggym/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Root '__init__' of the posggym package."""
+
 # isort: skip_file
 # Need to import model and core before other modules
 from posggym.model import POSGFullModel, POSGModel
 from posggym.core import (
     ActionWrapper,
     Env,
     DefaultEnv,
@@ -34,8 +35,8 @@
     "envs",
     "utils",
     "vector",
     "wrappers",
     "error",
     "logger",
 ]
-__version__ = "0.5.1"
+__version__ = "0.6.0"
```

### Comparing `posggym-0.5.1/posggym/agents/__init__.py` & `posggym-0.6.0/posggym/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/continuous/driving_continuous/__init__.py` & `posggym-0.6.0/posggym/agents/continuous/driving_continuous/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Policies for the DrivingContinuous-v0 environment."""
-import os.path as osp
-
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
 ENV_ID = "DrivingContinuous-v0"
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "continuous", "driving_continuous")
+agent_model_dir = AGENT_MODEL_DIR / "continuous" / "driving_continuous"
 policy_specs = {}
 
 # 14x14RoundAbout, 2 agents
 for policy_file_name in [
     "sp_seed0.pkl",
     "sp_seed1.pkl",
     "sp_seed2.pkl",
@@ -21,19 +19,17 @@
         env_id=ENV_ID,
         env_args={
             "world": "14x14RoundAbout",
             "num_agents": 2,
             "obs_dist": 5.0,
             "n_sensors": 16,
         },
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=14x14RoundAbout-num_agents=2-obs_dist=5-n_sensors=16",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "world=14x14RoundAbout-num_agents=2-obs_dist=5-n_sensors=16"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather than always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.RescaleProcessor,
@@ -56,19 +52,17 @@
         env_id=ENV_ID,
         env_args={
             "world": "14x14RoundAbout",
             "num_agents": 4,
             "obs_dist": 5.0,
             "n_sensors": 16,
         },
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=14x14RoundAbout-num_agents=4-obs_dist=5-n_sensors=16",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "world=14x14RoundAbout-num_agents=4-obs_dist=5-n_sensors=16"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather than always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.RescaleProcessor,
```

### Comparing `posggym-0.5.1/posggym/agents/continuous/drone_team_capture/__init__.py` & `posggym-0.6.0/posggym/agents/continuous/drone_team_capture/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/continuous/drone_team_capture/heuristic.py` & `posggym-0.6.0/posggym/agents/continuous/drone_team_capture/heuristic.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/continuous/predator_prey_continuous/__init__.py` & `posggym-0.6.0/posggym/agents/continuous/predator_prey_continuous/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Policies for the PredatorPreyContinuous-v0 environment."""
-import os.path as osp
 
 from posggym.agents.registration import PolicySpec
 from posggym.agents.continuous.predator_prey_continuous import heuristic
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.config import AGENT_MODEL_DIR
 from posggym.agents.utils import processors
 
 
 ENV_ID = "PredatorPreyContinuous-v0"
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "continuous", "predator_prey_continuous")
+agent_model_dir = AGENT_MODEL_DIR / "continuous" / "predator_prey_continuous"
 policy_specs = {}
 
 
 for n, policy_class in enumerate(
     [
         heuristic.PPCHeuristic0Policy,
         heuristic.PPCHeuristic1Policy,
@@ -47,19 +46,20 @@
             "num_predators": 2,
             "num_prey": 3,
             "prey_strength": 2,
             "cooperative": True,
             "obs_dist": 4.0,
             "n_sensors": 16,
         },
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=10x10-num_predators=2-num_prey=3-prey_strength=2_cooperative=True-obs_dist=4-n_sensors=16",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / (
+            "world=10x10-num_predators=2-num_prey=3-prey_strength=2_cooperative=True-"
+            "obs_dist=4-n_sensors=16"
+        )
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather than always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.RescaleProcessor,
@@ -85,18 +85,21 @@
             "num_predators": 4,
             "num_prey": 3,
             "prey_strength": 3,
             "cooperative": True,
             "obs_dist": 4.0,
             "n_sensors": 16,
         },
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=10x10-num_predators=4-num_prey=3-prey_strength=3_cooperative=True-obs_dist=4-n_sensors=16",
-            policy_file_name,
+        policy_file_path=(
+            agent_model_dir
+            / (
+                "world=10x10-num_predators=4-num_prey=3-prey_strength=3_cooperative=True-"
+                "obs_dist=4-n_sensors=16"
+            )
+            / policy_file_name
         ),
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather than always taking most probable action
         deterministic=False,
```

### Comparing `posggym-0.5.1/posggym/agents/continuous/predator_prey_continuous/heuristic.py` & `posggym-0.6.0/posggym/agents/continuous/predator_prey_continuous/heuristic.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/continuous/pursuit_evasion_continuous/__init__.py` & `posggym-0.6.0/posggym/agents/continuous/pursuit_evasion_continuous/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Policies for the PursuitEvasionContinuous-v0 environment."""
 import math
-import os.path as osp
 
 from posggym.agents.continuous.pursuit_evasion_continuous import shortest_path
 from posggym.agents.registration import PolicySpec
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
 ENV_ID = "PursuitEvasionContinuous-v0"
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "continuous", "pursuit_evasion_continuous")
+agent_model_dir = AGENT_MODEL_DIR / "continuous" / "pursuit_evasion_continuous"
 policy_specs = {}
 
 _sp_spec = PolicySpec(
     policy_name="shortest_path",
     entry_point=shortest_path.PECShortestPathPolicy,
     version=0,
     env_id=ENV_ID,
@@ -33,19 +32,15 @@
     "sp_seed2_i1.pkl",
     "sp_seed3_i0.pkl",
     "sp_seed3_i1.pkl",
     "sp_seed4_i0.pkl",
     "sp_seed4_i1.pkl",
 ]:
     spec = PPOPolicy.get_spec_from_path(
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=8x8",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir / "world=8x8" / policy_file_name,
         env_id=ENV_ID,
         env_args={
             "world": "8x8",
             "fov": math.pi / 3,
             "max_obs_distance": 8.0 / 3,
             "n_sensors": 16,
         },
@@ -73,19 +68,15 @@
     "sp_seed2_i1.pkl",
     "sp_seed3_i0.pkl",
     "sp_seed3_i1.pkl",
     "sp_seed4_i0.pkl",
     "sp_seed4_i1.pkl",
 ]:
     spec = PPOPolicy.get_spec_from_path(
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "world=16x16",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir / "world=16x16" / policy_file_name,
         env_id=ENV_ID,
         env_args={
             "world": "16x16",
             "fov": math.pi / 3,
             "max_obs_distance": 16.0 / 3,
             "n_sensors": 16,
         },
```

### Comparing `posggym-0.5.1/posggym/agents/continuous/pursuit_evasion_continuous/shortest_path.py` & `posggym-0.6.0/posggym/agents/continuous/pursuit_evasion_continuous/shortest_path.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/evaluation/diversity.py` & `posggym-0.6.0/posggym/agents/evaluation/diversity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Functionality for measuring return based diversity of posggym.agents policies."""
 from __future__ import annotations
 
-import os
 from itertools import product
-from typing import Dict, List
+from typing import Dict, List, TYPE_CHECKING
 
+if TYPE_CHECKING:
+    from pathlib import Path
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 import posggym.agents as pga
 from posggym.agents.evaluation import pairwise
 
@@ -134,15 +135,15 @@
         "pairwise_return_ed": pw_ed,
         "policy_ed": policy_ed.reshape(-1, 1),
         "return_ed_clusters": clusters.reshape(-1, 1),
     }
 
 
 def run_return_diversity_analysis(
-    output_dir: str,
+    output_dir: Path,
     env_id: str | None,
     env_args_id: str | None = None,
     verbose: bool = False,
 ):
     """Run return diversity analysis from pairwise comparison results.
 
     Results of analysis will be output to the results directory for each env.
@@ -151,24 +152,22 @@
     if env_id is None:
         env_ids = list(all_envs)
         env_args_id = None
     else:
         env_ids = [env_id]
         env_args_id = env_args_id
 
-    for env_id in os.listdir(output_dir):
+    for env_results_dir in output_dir.glob("*"):
+        env_id = env_results_dir.name
         if env_id not in env_ids:
             continue
         print(f"Running return diversity analysis for {env_id=}")
-        env_results_dir = os.path.join(output_dir, env_id)
         print(f"  results saved to {env_results_dir=}")
 
-        env_result_files = [
-            fname for fname in os.listdir(env_results_dir) if fname.endswith(".csv")
-        ]
+        env_result_files = [x.name for x in env_results_dir.glob("*.csv")]
 
         env_args_map = pga.get_all_envs()[env_id]
         for args_id in env_args_map:
             if (env_args_id is not None and args_id != env_args_id) or (
                 env_args_id is None and str(args_id) + ".csv" not in env_result_files
             ):
                 continue
@@ -242,10 +241,10 @@
                         xticklabels=xticklabels,
                         yticklabels=policy_ids,
                         square=div_results[k].shape[1] != 1,
                         annot_kws={"fontsize": annot_fontsize},
                     )
                     axs[0][idx].set_title(f"agent `{i}`")
                 fig.savefig(
-                    os.path.join(env_results_dir, f"{args_id}_{k}.svg"),
+                    env_results_dir / f"{args_id}_{k}.svg",
                     bbox_inches="tight",
                 )
```

### Comparing `posggym-0.5.1/posggym/agents/evaluation/pairwise.py` & `posggym-0.6.0/posggym/agents/evaluation/pairwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Functions for pairwise evaluation of agents."""
 from __future__ import annotations
 
 import csv
 import multiprocessing as mp
-import os
 from datetime import datetime
 from itertools import product
-from typing import Dict, List, NamedTuple, Tuple
+from typing import Dict, List, NamedTuple, Tuple, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import torch
 
@@ -139,26 +141,26 @@
 
     if params.run_num % max(10, total_runs // 10) == 0:
         print(f"Run {params.run_num}/{total_runs} complete.")
 
 
 def get_pairwise_comparison_params(
     env_id: str,
-    output_dir: str,
+    output_dir: Path,
     env_args_id: str | None = None,
     num_episodes: int = 1000,
     seed: int | None = None,
     verbose: bool = False,
 ) -> List[PWCParams]:
     """Get parameters for pairwise comparisons of all of an environment's policies."""
     # attempt to make env to check if it is registered (displays nicer error msg)
     posggym.make(env_id)
 
-    env_output_dir = os.path.join(output_dir, env_id)
-    os.makedirs(env_output_dir, exist_ok=True)
+    env_output_dir = output_dir / env_id
+    env_output_dir.mkdir(exist_ok=True)
 
     # construct list of all possible policy pairings for the environment
     env_args_map = pga.get_all_envs()[env_id]
     all_pairwise_comparisons = []
     run_num = 1
     for args_id, env_args in env_args_map.items():
         if env_args_id is not None and args_id != env_args_id:
@@ -173,16 +175,16 @@
         all_agent_policies = pga.get_env_agent_policies(
             env_id, env_args, include_generic_policies=True
         )
         agent_ids = list(all_agent_policies.keys())
         if verbose:
             print(f"  - {len(agent_ids)} agents")
 
-        output_file = os.path.join(env_output_dir, f"{args_id}.csv")
-        if os.path.exists(output_file):
+        output_file = env_output_dir / f"{args_id}.csv"
+        if output_file.exists():
             logger.warn(f"{output_file} exists. Rewriting.")
 
         headers = [
             "env_id",
             "env_args_id",
             "symmetric",
             "seed",
@@ -276,15 +278,15 @@
     return all_pairwise_comparisons
 
 
 def run_pairwise_comparisons(
     env_id: str | None,
     env_args_id: str | None = None,
     num_episodes: int = 1000,
-    output_dir: str | None = None,
+    output_dir: Path | None = None,
     seed: int | None = None,
     n_procs: int | None = None,
     verbose: bool = False,
 ) -> str:
     """Run pairwise comparisons for all policies in an environment.
 
     Returns the directory where results are saved.
@@ -293,19 +295,19 @@
         env_ids = list(pga.get_all_envs())
         env_args_id = None
     else:
         env_ids = [env_id]
         env_args_id = env_args_id
 
     if output_dir is None:
-        output_dir = os.path.join(
-            BASE_RESULTS_DIR,
-            "pairwise_comparison" + datetime.now().strftime("%d-%m-%y_%H-%M-%S"),
+        output_dir = BASE_RESULTS_DIR / (
+            "pairwise_comparison" + datetime.now().strftime("%d-%m-%y_%H-%M-%S")
         )
-    os.makedirs(output_dir, exist_ok=True)
+
+    output_dir.mkdir(exist_ok=True)
 
     all_pairwise_comparisons = []
     for env_id in env_ids:
         all_pairwise_comparisons.extend(
             get_pairwise_comparison_params(
                 env_id=env_id,
                 env_args_id=env_args_id,
@@ -337,21 +339,21 @@
 
     print("All pairwise comparisons complete.")
     return output_dir
 
 
 def load_pairwise_comparison_results(
     env_id: str,
-    output_dir: str,
+    output_dir: Path,
     env_args_id: str | None = None,
 ) -> pd.DataFrame:
     """Load pairwise comparison results for an environment."""
-    env_output_dir = os.path.join(output_dir, env_id)
-    output_file = os.path.join(env_output_dir, f"{env_args_id}.csv")
-    if not os.path.exists(output_file):
+    env_output_dir = output_dir / env_id
+    output_file = env_output_dir / f"{env_args_id}.csv"
+    if not output_file.exists():
         raise ValueError(
             f"Results do not exist for {env_id=}, {env_args_id=} in {output_dir=}."
         )
     return pd.read_csv(output_file)
 
 
 def get_pairwise_returns_matrix(
@@ -426,15 +428,15 @@
                 1.96 * pw_returns_i[1, policy_idx, co_team_idx] / np.sqrt(num_episodes)
             )
     return pw_returns_per_agent
 
 
 def generate_pairwise_returns_plot(
     env_id: str,
-    output_dir: str,
+    output_dir: Path,
     env_args_id: str | None,
     pw_returns_per_agent: Dict[str, Tuple[np.ndarray, List[str], List[str]]],
     show: bool = True,
     save: bool = True,
     mean_only: bool = False,
 ) -> None:
     """Generate a plot of pairwise returns for an environment."""
@@ -478,29 +480,28 @@
                 square=True,
                 annot_kws={"fontsize": min(8, 24 / np.sqrt(max(values.shape)))},
             )
             axs[0][idx].set_title(f"Return {stat} - agent `{i}`")
 
         if save:
             if env_id in output_dir:
-                output_file = os.path.join(
-                    output_dir, f"{env_args_id}_pairwise_returns_{stat}.svg"
-                )
+                output_file = output_dir / f"{env_args_id}_pairwise_returns_{stat}.svg"
             else:
-                output_file = os.path.join(
-                    output_dir, f"{env_id}_{env_args_id}_pairwise_returns_{stat}.svg"
+                output_file = (
+                    output_dir / f"{env_id}_{env_args_id}_pairwise_returns_{stat}.svg"
                 )
+
             fig.savefig(output_file, bbox_inches="tight")
 
     if show:
         plt.show()
 
 
 def plot_pairwise_comparison_results(
-    output_dir: str,
+    output_dir: Path,
     env_id: str | None,
     env_args_id: str | None = None,
     show: bool = True,
     save: bool = True,
     mean_only: bool = False,
 ):
     """Run return diversity analysis from pairwise comparison results.
@@ -511,24 +512,23 @@
     if env_id is None:
         env_ids = list(all_envs)
         env_args_id = None
     else:
         env_ids = [env_id]
         env_args_id = env_args_id
 
-    for env_id in os.listdir(output_dir):
+    for env_results_dir in output_dir.glob("*"):
+        env_id = env_results_dir.name
         if env_id not in env_ids:
             continue
+
         print(f"Plotting pairwise comparison results for {env_id=}")
-        env_results_dir = os.path.join(output_dir, env_id)
         print(f"  results saved to {env_results_dir=}")
 
-        env_result_files = [
-            fname for fname in os.listdir(env_results_dir) if fname.endswith(".csv")
-        ]
+        env_result_files = [x.name for x in env_results_dir.glob("*.csv")]
 
         env_args_map = pga.get_all_envs()[env_id]
         for args_id in env_args_map:
             if (env_args_id is not None and args_id != env_args_id) or (
                 env_args_id is None and str(args_id) + ".csv" not in env_result_files
             ):
                 continue
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/cooperative_reaching/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/cooperative_reaching/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/grid_world/cooperative_reaching/heuristic.py` & `posggym-0.6.0/posggym/agents/grid_world/cooperative_reaching/heuristic.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/grid_world/driving/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/driving/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Policies for the Driving environments."""
-import os.path as osp
 
 from posggym.agents.grid_world.driving.shortest_path import DrivingShortestPathPolicy
 from posggym.agents.registration import PolicySpec
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
 
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "grid_world", "driving")
+agent_model_dir = AGENT_MODEL_DIR / "grid_world" / "driving"
 policy_specs = {}
 
 
 for a, description in [
     (
         0.0,
         (
@@ -75,19 +74,17 @@
         env_id="Driving-v1",
         env_args={
             "grid": "14x14RoundAbout",
             "num_agents": 2,
             "obs_dim": (3, 1, 1),
         },
         env_args_id="grid=14x14RoundAbout-num_agents=2",
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "grid=14x14RoundAbout-num_agents=2",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "grid=14x14RoundAbout-num_agents=2"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/driving_gen/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/driving_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/grid_world/driving_gen/shortest_path.py` & `posggym-0.6.0/posggym/agents/grid_world/driving_gen/shortest_path.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Shortest path policy for Driving Gen envs."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from posggym.agents.grid_world.driving.shortest_path import DrivingShortestPathPolicy
+from posggym.agents.grid_world.driving.shortest_path import (
+    DrivingShortestPathPolicy,
+    Pos,
+)
 
 
 if TYPE_CHECKING:
     from posggym.agents.policy import PolicyID
+    from posggym.envs.grid_world.core import Coord
     from posggym.model import POSGModel
 
 
 class DrivingGenShortestPathPolicy(DrivingShortestPathPolicy):
     """Shortest Path Policy for the Driving Gen environment.
 
     This policy sets the preferred action as the one which is on the shortest
@@ -45,14 +49,17 @@
         aggressiveness: float = 1.0,
     ):
         super().__init__(
             model,
             agent_id,
             policy_id,
             aggressiveness=aggressiveness,
-            precompute_shortest_paths=False,
         )
+        self.shortest_paths = {}
 
     def reset(self, *, seed: int | None = None):
         super().reset(seed=seed)
         self._grid = self.model.grid
         self.shortest_paths = {}
+
+    def get_dest_shortest_path_dist(self, dest_coord: Coord, pos: Pos) -> int:
+        return self.get_shortest_path(pos, dest_coord, self._grid, self.shortest_paths)
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/level_based_foraging/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/level_based_foraging/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Policies for the LevelBasedForaging-v2 environment."""
-import os.path as osp
 
 from posggym.agents.grid_world.level_based_foraging import heuristic
 from posggym.agents.registration import PolicySpec
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
 
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "grid_world", "level_based_foraging")
+agent_model_dir = AGENT_MODEL_DIR / "grid_world" / "level_based_foraging"
 
 policy_specs = {}
 for policy_class in [
     heuristic.LBFHeuristic1,
     heuristic.LBFHeuristic2,
     heuristic.LBFHeuristic3,
     heuristic.LBFHeuristic4,
@@ -48,19 +47,17 @@
             "max_food": 8,
             "sight": 2,
             "force_coop": False,
             "static_layout": False,
             "observation_mode": "tuple",
         },
         env_args_id="num_agents=2-size=10-static_layout=False",
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "num_agents=2-size=10-static_layout=False",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "num_agents=2-size=10-static_layout=False"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
@@ -90,19 +87,17 @@
             "max_food": 8,
             "sight": 2,
             "force_coop": False,
             "static_layout": True,
             "observation_mode": "tuple",
         },
         env_args_id="num_agents=2-size=10-static_layout=True",
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "num_agents=2-size=10-static_layout=True",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "num_agents=2-size=10-static_layout=True"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/level_based_foraging/heuristic.py` & `posggym-0.6.0/posggym/agents/grid_world/level_based_foraging/heuristic.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/grid_world/predator_prey/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/predator_prey/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Policies for the PredatorPrey-v0 environment."""
-import os.path as osp
 
 from posggym.agents.grid_world.predator_prey import heuristic
 from posggym.agents.registration import PolicySpec
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "grid_world", "predator_prey")
+agent_model_dir = AGENT_MODEL_DIR / "grid_world" / "predator_prey"
 policy_specs = {}
 
 for policy_class in [
     heuristic.PPHeuristic1,
     heuristic.PPHeuristic2,
     heuristic.PPHeuristic3,
 ]:
@@ -46,19 +45,17 @@
             "num_predators": 2,
             "num_prey": 3,
             "cooperative": True,
             "prey_strength": 2,
             "obs_dim": 2,
         },
         env_args_id="grid=10x10-num_predators=2-num_prey=3-cooperative=True",
-        policy_file_path=osp.join(
-            agent_model_dir,
-            "grid=10x10-num_predators=2-num_prey=3-cooperative=True",
-            policy_file_name,
-        ),
+        policy_file_path=agent_model_dir
+        / "grid=10x10-num_predators=2-num_prey=3-cooperative=True"
+        / policy_file_name,
         version=0,
         valid_agent_ids=None,
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/predator_prey/heuristic.py` & `posggym-0.6.0/posggym/agents/grid_world/predator_prey/heuristic.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/grid_world/pursuit_evasion/__init__.py` & `posggym-0.6.0/posggym/agents/grid_world/pursuit_evasion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Policies for the PursuitEvasion environment."""
-import os.path as osp
 
 from posggym.agents.grid_world.pursuit_evasion.shortest_path import PEShortestPathPolicy
 from posggym.agents.registration import PolicySpec
 from posggym.agents.torch_policy import PPOPolicy
 from posggym.agents.utils import processors
 from posggym.config import AGENT_MODEL_DIR
 
-agent_model_dir = osp.join(AGENT_MODEL_DIR, "grid_world", "pursuit_evasion")
+agent_model_dir = AGENT_MODEL_DIR / "grid_world" / "pursuit_evasion"
 policy_specs = {}
 
 spec = PolicySpec(
     policy_name="ShortestPath",
     entry_point=PEShortestPathPolicy,
     version=0,
     env_id="PursuitEvasion-v1",
@@ -67,15 +66,15 @@
         env_id="PursuitEvasion-v1",
         env_args={
             "grid": "16x16",
             "max_obs_distance": 12,
             "use_progress_reward": True,
         },
         env_args_id="grid=16x16",
-        policy_file_path=osp.join(agent_model_dir, "grid=16x16", policy_file_name),
+        policy_file_path=agent_model_dir / "grid=16x16" / policy_file_name,
         version=0,
         valid_agent_ids=["0"],
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
@@ -111,15 +110,15 @@
         env_id="PursuitEvasion-v1",
         env_args={
             "grid": "16x16",
             "max_obs_distance": 12,
             "use_progress_reward": True,
         },
         env_args_id="grid=16x16",
-        policy_file_path=osp.join(agent_model_dir, "grid=16x16", policy_file_name),
+        policy_file_path=agent_model_dir / "grid=16x16" / policy_file_name,
         version=0,
         valid_agent_ids=["1"],
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather than always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
@@ -151,15 +150,15 @@
         env_id="PursuitEvasion-v1",
         env_args={
             "grid": "8x8",
             "max_obs_distance": 12,
             "use_progress_reward": True,
         },
         env_args_id="grid=8x8",
-        policy_file_path=osp.join(agent_model_dir, "grid=8x8", policy_file_name),
+        policy_file_path=agent_model_dir / "grid=8x8" / policy_file_name,
         version=0,
         valid_agent_ids=["0"],
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
@@ -191,15 +190,15 @@
         env_id="PursuitEvasion-v1",
         env_args={
             "grid": "8x8",
             "max_obs_distance": 12,
             "use_progress_reward": True,
         },
         env_args_id="grid=8x8",
-        policy_file_path=osp.join(agent_model_dir, "grid=8x8", policy_file_name),
+        policy_file_path=agent_model_dir / "grid=8x8" / policy_file_name,
         version=0,
         valid_agent_ids=["1"],
         # policy is deterministic given random seed
         nondeterministic=False,
         # actions sampled, rather always taking most probable action
         deterministic=False,
         obs_processor_cls=processors.FlattenProcessor,
```

### Comparing `posggym-0.5.1/posggym/agents/grid_world/pursuit_evasion/shortest_path.py` & `posggym-0.6.0/posggym/agents/grid_world/pursuit_evasion/shortest_path.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/policy.py` & `posggym-0.6.0/posggym/agents/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The Policy class defining the core API for posggym.agents policies."""
+
 from __future__ import annotations
 
 import abc
 import copy
 from typing import TYPE_CHECKING, Any, Dict, Generic
 
 from posggym.model import ActType, ObsType
@@ -66,15 +67,14 @@
 
     The policy also maintains a reference to the last action it returned by the
     :meth:`step` method, which is stored in the :attr:`_last_action` attribute. This
     attribute is set to None when the policy is first created and whenever the
     :meth:`reset` method is called. It is used to update the policy's internal state
     each time the :meth:`step` method is called.
 
-
     """
 
     # PolicySpec used to initialize policy instance
     # This is set when policy is made using posggym.agents.make function
     spec: PolicySpec | None = None
 
     # Whether the policy expects the full state as it's observation or not
@@ -92,20 +92,20 @@
 
         This function updates the policy's current internal state given the most recent
         observation, and returns the next action for the policy.
 
         Arguments
         ---------
         obs : ObsType
-            the latest observation.
+            The latest observation.
 
         Returns
         -------
         action : ActType
-            the next action
+            The next action
 
         """
         self._state = self.get_next_state(self._last_action, obs, self._state)
         self._last_action = self.sample_action(self._state)
         return self._last_action
 
     def reset(self, *, seed: int | None = None):
@@ -118,15 +118,15 @@
         method and seed the RNG if a `seed` is provided. The expected behaviour is that
         this is that the seed provided once by the user, just after the policy is first
         created and before it interacts with an environment.
 
         Arguments
         ---------
         seed : int, optional
-            seed for random number generator.
+            Seed for random number generator.
 
         """
         self._state = self.get_initial_state()
         self._last_action = None
 
     def close(self):
         """Close policy and perform any necessary cleanup.
@@ -141,15 +141,15 @@
         Subclasses that utilize custom internal states (e.g. RNN policies) should
         override this method, but should first call `super.().get_initial_state()` to
         get the base policy state that can then be extended.
 
         Returns
         -------
         initial_state : PolicyState
-            the initial policy state
+            The initial policy state
 
         """
         return {}
 
     @abc.abstractmethod
     def get_next_state(
         self,
@@ -160,24 +160,24 @@
         """Get the next policy state.
 
         Subclasses must implement this method.
 
         Arguments
         ---------
         action : ActType, optional
-            the action performed. May be None if this is the first observation.
+            The action performed. May be None if this is the first observation.
         obs : ObsType
-            the observation received
+            The observation received
         state : PolicyState
-            the policy's state before action was performed and obs received
+            The policy's state before action was performed and obs received
 
         Returns
         -------
         next_state : PolicyState
-            the next policy state
+            The next policy state
 
         """
 
     @abc.abstractmethod
     def sample_action(self, state: PolicyState) -> ActType:
         """Sample an action given policy's current state.
 
@@ -186,20 +186,20 @@
         each time even if the state is the same.
 
         Subclasses must implement this method.
 
         Arguments
         ---------
         state : PolicyState
-            the policy's current state
+            The policy's current state.
 
         Returns
         -------
         action : ActType
-            the sampled action
+            The sampled action.
 
         """
 
     @abc.abstractmethod
     def get_pi(self, state: PolicyState) -> ActionDistribution:
         """Get policy's distribution over actions for given policy state.
 
@@ -207,97 +207,96 @@
         subclass of the
         :py:class:`posggym.agents.utils.action_distributions.ActionDistribution`
         class.
 
         Arguments
         ---------
         state : PolicyState
-            the policy's current state
+            The policy's current state.
 
         Returns
         -------
         pi : ActionDistribution
-            the policy's distribution over actions
+            The policy's distribution over actions.
 
         """
 
     @abc.abstractmethod
     def get_value(self, state: PolicyState) -> float:
         """Get a value estimate of a history.
 
         Subclasses must implement this method, but may set it to raise a
         NotImplementedError if the policy does not support value estimates.
 
         Arguments
         ---------
         state : PolicyState
-            the policy's current state
+            The policy's current state.
 
         Returns
         -------
         value : float
-            the value estimate
+            The value estimate.
 
         """
 
     def set_state(self, state: PolicyState, last_action: ActType | None = None):
         """Set the policy's internal state.
 
         Subclasses that utilize custom internal states (e.g. RNN policies) may wish to
         override this method, to set any attributes used for the by the class to store
         policy state.
 
         Arguments
         ---------
         state : PolicyState
-            the new policy state
+            The new policy state.
         last_action : ActType, optional
-            the last action taken by the policy. If not provided then the last action
+            The last action taken by the policy. If not provided then the last action
             will be set to None.
 
         Raises
         ------
-        AssertionError :
-            if new policy state is not valid.
+        AssertionError
+            If new policy state is not valid.
 
         """
         if self._state is not None and state is not None:
             assert all(k in state for k in self._state), f"Invalid policy state {state}"
         self._state = state
         self._last_action = last_action
 
     def get_state(self) -> PolicyState:
         """Get the policy's current state.
 
         Returns
         -------
         state : PolicyState
-            policy's current internal state.
+            Policy's current internal state.
 
         """
         return copy.deepcopy(self._state)
 
     def get_state_from_history(self, history: AgentHistory) -> PolicyState:
         """Get the policy's state given history.
 
         This function essentially unrolls the policy using the actions and observations
         contained in the agent history.
 
         Note, this function will return None for the action in the final output state,
         as this would correspond to the action that was selected by the policy to action
 
-
         Arguments
         ---------
         history : AgentHistory
-            the agent's action-observation history
+            The agent's action-observation history.
 
         Returns
         -------
         state : PolicyState
-            policy state given history
+            Policy state given history.
 
         """
         state = self.get_initial_state()
         for a, o in history:
             state = self.get_next_state(a, o, state)
         return state
```

### Comparing `posggym-0.5.1/posggym/agents/random_policies.py` & `posggym-0.6.0/posggym/agents/random_policies.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/registration.py` & `posggym-0.6.0/posggym/agents/registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions and classes for registering and loading implemented agents.
 
 Based on Farama Foundation Gymnasium,
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/envs/registration.py
 
 """
+
 from __future__ import annotations
 
 import copy
 import difflib
 import importlib
 import re
 from collections import defaultdict
@@ -41,20 +42,20 @@
 
 
 def load(name: str) -> PolicyEntryPoint:
     """Loads policy with name and returns a policy entry point.
 
     Arguments
     ---------
-    name
-        The policy name
+    name : str
+        The policy name.
 
     Returns
     -------
-    entry_point
+    entry_point : PolicyEntryPoint
         Policy creation function.
 
     """
     mod_name, attr_name = name.split(":")
     mod = importlib.import_module(mod_name)
     fn = getattr(mod, attr_name)
     return fn
@@ -65,32 +66,32 @@
 
     env_id is group 1, env_args_id is group 2. policy_id is group 2, version is group 3
 
     [env_id/][env_args_id/](policy_id)-v(version)
 
     Arguments
     ---------
-    policy_id
-        The policy id to parse
+    policy_id : str
+        The policy id to parse.
 
     Returns
     -------
-    env_id
-        The environment ID
-    env_args_id
-        ID string of environment arguments
-    pi_name
-        The policy name
-    version
-        The policy version
+    env_id : str | None
+        The environment ID.
+    env_args_id : str | None
+        ID string of environment arguments.
+    pi_name : str
+        The policy name.
+    version : int | None
+        The policy version.
 
     Raises
     ------
     Error
-        If the policy id does not a valid environment regex
+        If the policy id does not a valid environment regex.
 
     """
     match = POLICY_ID_RE.fullmatch(policy_id)
     if not match:
         raise error.Error(
             f"Malformed policy ID: {policy_id}. Currently all IDs must be of the "
             "form [env_id/][env_args_id/](policy_name)-v(version) (env_id and "
@@ -117,27 +118,27 @@
 ) -> str:
     """Get the full policy ID given a name and (optional) version and env-name.
 
     Inverse of :meth:`parse_policy_id`.
 
     Arguments
     ---------
-    env_id
-        The environment ID
-    env_args_id
-        ID string of environment arguments
-    policy_name
-        The policy name
-    version
-        The policy version
+    env_id : str | None
+        The environment ID.
+    env_args_id : str | None
+        ID string of environment arguments.
+    policy_name : str
+        The policy name.
+    version : int | None
+        The policy version.
 
     Returns
     -------
-    policy_id
-        The policy id
+    policy_id : str
+        The policy id.
 
     """
     if env_args_id is not None and env_id is None:
         raise error.Error(
             "Cannot create policy ID. Must include env_id if env_args_id is part of "
             "the policy ID."
         )
@@ -160,21 +161,21 @@
         k1=v1-k2=v2-k3=v3
 
     Note we assume keywords are valid python variable names and so do not contain
     any hyphen '-' characters.
 
     Arguments
     ---------
-    env_args
-        environment keyword arguments
+    env_args : Dict[str, Any]
+        Environment keyword arguments.
 
     Returns
     -------
-    env_args_id
-        string representation of the envrinment keyword arguments.
+    env_args_id : str
+        String representation of the envrinment keyword arguments.
 
     """
     return ("-".join(f"{k}={v}" for k, v in env_args.items())).replace(" ", "")
 
 
 @dataclass
 class PolicySpec:
@@ -182,22 +183,22 @@
 
     Used to register agent policies that can then be dynamically loaded using
     posggym_agents.make.
 
     Arguments
     ---------
     policy_name
-        The name of the policy
+        The name of the policy.
     entry_point
         The Python entrypoint for initializing an instance of the agent policy.
         Must be a Callable with signature matching `PolicyEntryPoint` or a string
         defining where the entry point function can be imported
         (e.g. module.name:Class).
     version
-        the policy version
+        The policy version.
     env_id
         Optional ID of the posggym environment that the policy is for.
     env_args
         Optional keywords arguments for the environment that the policy is for (if
         it is a environment specific policy). If None then assumes policy can be used
         for the environment with any arguments.
     env_args_id
@@ -347,22 +348,22 @@
     """Check if policy version exists for env ID. Print helpful error message if not.
 
     This is a complete test whether an policy ID is valid, and will provide the best
     available hints.
 
     Arguments
     ---------
-    env_id
-        The environment ID
-    env_args_ud
-        The ID of the environment keyword arguments
-    policy_name
-        The policy name
-    version
-        The policy version
+    env_id : str | None
+        The environment ID.
+    env_args_id : str | None
+        The ID of the environment keyword arguments.
+    policy_name : str
+        The policy name.
+    version : int | None
+        The policy version.
 
     Raises
     ------
     DeprecatedPolicy
         The policy doesn't exist but a default version does or the policy version is
         deprecated
     VersionNotFound
@@ -507,34 +508,34 @@
     """Register a policy with posggym.agents.
 
     The policy is registered in posggym so it can be used with
     :py:method:`posggym.agents.make`
 
     Arguments
     ---------
-    policy_name
+    policy_name : str
         The name of the policy
-    entry_point
+    entry_point : PolicyEntryPoint | str
         The entry point for creating the policy
-    env_id
-        Optional ID of the posggym environment that the policy is for.
-    version
+    version : int | None
         the policy version
-    env_args
+    env_id : str | None
+        Optional ID of the posggym environment that the policy is for.
+    env_args : Dict[str, Any] | None
         Optional keywords arguments for the environment that the policy is for (if
         it is a environment specific policy). If None then assumes policy can be used
         for the environment with any arguments.
-    valid_agent_ids
+    valid_agent_ids : List[str] | None
         Optional AgentIDs in environment that policy is compatible with. If
         None then assumes policy can be used for any agent in the environment.
-    nondeterministic
+    nondeterministic : bool
         Whether this policy is non-deterministic even after seeding.
-    description
+    description : str | none
         Optional description of the policy.
-    kwargs
+    **kwargs
         Additional kwargs, if any, to pass to the agent initializing
 
     """
     global registry
     new_spec = PolicySpec(
         policy_name=policy_name,
         entry_point=entry_point,
@@ -550,16 +551,16 @@
 
 
 def register_spec(spec: PolicySpec):
     """Register a policy spec with posggym-agents.
 
     Arguments
     ---------
-    spec
-        The policy spec
+    spec : PolicySpec
+        The policy spec.
 
     """
     global registry
     _check_spec_register(spec)
     if spec.id in registry:
         logger.warn(f"Overriding policy {spec.id} already in registry.")
     registry[spec.id] = spec
@@ -569,32 +570,32 @@
     """Create an policy according to the given ID.
 
     To find all available policies use `posggym_agents.agents.registry.keys()` for
     all valid ids.
 
     Arguments
     ---------
-    id
-      Unique identifier of the policy or a policy spec.
-    model
-      The model for the environment the policy will be interacting with.
-    agent_id
-      The ID of the agent the policy will be used for.
-    kwargs
-      Additional arguments to pass to the policy constructor.
+    id : str | PolicySpec
+        Unique identifier of the policy or a policy spec.
+    model : POSGModel
+        The model for the environment the policy will be interacting with.
+    agent_id : str
+        The ID of the agent the policy will be used for.
+    **kwargs
+        Additional arguments to pass to the policy constructor.
 
     Returns
     -------
-    policy
-      An instance of the policy.
+    Policy
+        An instance of the policy.
 
     Raises
     ------
     Error
-      If the ``id`` doesn't exist then an error is raised
+        If the ``id`` doesn't exist then an error is raised
 
     """
     if isinstance(id, PolicySpec):
         spec_: PolicySpec = id
     else:
         env_id, env_args_id, policy_name, version = parse_policy_id(id)
 
@@ -665,26 +666,26 @@
 
 
 def spec(id: str) -> PolicySpec:
     """Retrieve the spec for the given policy from the global registry.
 
     Arguments
     ---------
-    id
-        the policy id.
+    id : str
+        The policy id.
 
     Returns
     -------
-    spec
-        the policy spec from the global registry.
+    PolicySpec
+        The policy spec from the global registry.
 
     Raises
     ------
     Error
-        if policy with given ``id`` doesn't exist in global registry.
+        If policy with given ``id`` doesn't exist in global registry.
 
     """
     spec_ = registry.get(id)
     if spec_ is None:
         env_id, env_args_id, policy_name, version = parse_policy_id(id)
         _check_version_exists(env_id, env_args_id, policy_name, version)
 
@@ -697,41 +698,41 @@
         raise error.Error(f"No registered policy with id: {id}")
     else:
         assert isinstance(spec_, PolicySpec)
         return spec_
 
 
 def pprint_registry(
-    _registry: dict = registry,
+    _registry: Dict = registry,
     num_cols: int = 3,
     include_env_ids: List[str] | None = None,
     exclude_env_ids: List[str] | None = None,
     disable_print: bool = False,
 ) -> str | None:
     """Pretty print the policies in the registry.
 
     Arguments
     ---------
-    _registry
+    _registry : Dict
         Policy registry to be printed.
-    num_cols
+    num_cols : int
         Number of columns to arrange policies in, for display.
-    include_env_ids
+    include_env_ids : List[str] | None
         Print only policies for environments with these IDs. If None then all
         environments are included.
-    exclude_env_ids
+    exclude_env_ids : List[str] | None
         Exclude any policies for environments with thee IDs from being printed.
-    disable_print
+    disable_print : bool
         Whether to return a string of all the policy IDs instead of printing it to
         console.
 
     Returns
     -------
-    return_str
-        formatted str representation of registry, if ``disable_print=True``, otherwise
+    str | None
+        Formatted str representation of registry, if ``disable_print=True``, otherwise
         returns ``None``.
 
     """
     # Defaultdict to store policy names according to env_id.
     env_policies = defaultdict(lambda: defaultdict(lambda: []))
     max_justify = 0
     for spec in _registry.values():
@@ -777,29 +778,29 @@
     _registry: Dict = registry,
     include_generic_policies: bool = True,
 ) -> List[PolicySpec]:
     """Get all PolicySpecs that are associated with a given environment ID.
 
     Arguments
     ---------
-    env_id
-        The ID of the environment
-    env_args
+    env_id : str
+        The ID of the environment.
+    env_args : Dict[str, Any] | str | None
         Optional environment arguments or ID string of environment arguments. If
         None, will return all policies for given environment.
-    _registry
-        The policy registry
-    include_generic_policies
-        whether to also return policies that are valid for all environments (e.g. the
-        random-v0 policy)
+    _registry : Dict
+        The policy registry.
+    include_generic_policies : bool
+        Whether to also return policies that are valid for all environments (e.g. the
+        random-v0 policy).
 
     Returns
     -------
-    policy_specs
-        list of specs for policies associated with given environment.
+    List[PolicySpec]
+        List of specs for policies associated with given environment.
 
     """
     return [
         spec
         for spec in _registry.values()
         if (
             (include_generic_policies and spec.env_id is None)
@@ -822,29 +823,29 @@
     _registry: Dict = registry,
     include_generic_policies: bool = True,
 ) -> Dict[str, List[PolicySpec]]:
     """Get each agent's policy specs associated with given environment.
 
     Arguments
     ---------
-    env_id
-        The ID of the environment
-    env_args
+    env_id : str
+        The ID of the environment.
+    env_args : Dict[str, Any] | None
         Optional environment arguments. If None, will return all policies for
         given environment.
-    _registry
-        The policy registry
-    include_generic_policies
-        whether to also return policies that are valid for all environments (e.g. the
-        random-v0 policy) and environment args
+    _registry : Dict
+        The policy registry.
+    include_generic_policies : bool
+        Whether to also return policies that are valid for all environments (e.g. the
+        random-v0 policy) and environment args.
 
     Returns
     -------
-    policy_specs
-        list of specs for policies associated with given environment.
+    Dict[str, List[PolicySpec]]
+        List of specs for policies associated with given environment.
 
     """
     env = posggym.make(env_id) if env_args is None else posggym.make(env_id, **env_args)
 
     policies: Dict[str, List[PolicySpec]] = {i: [] for i in env.possible_agents}
     for spec in get_all_env_policies(
         env_id,
@@ -861,21 +862,21 @@
 def get_all_envs(
     _registry: Dict = registry,
 ) -> Dict[str, Dict[str | None, Dict[str, Any] | None]]:
     """Get all the environments that have at least one registered policy.
 
     Arguments
     ---------
-    _registry
-        The policy registry
+    _registry : Dict
+        The policy registry.
 
     Returns
     -------
-    envs
-        a dictionary with env IDs as keys as list of (env_args, env_args_id) tuples as
+    Dict[str, Dict[str | None, Dict[str, Any] | None]]
+        A dictionary with env IDs as keys as list of (env_args, env_args_id) tuples as
         the values.
 
     """
     envs: Dict[str, Dict[str | None, Dict[str, Any] | None]] = {}
     for spec in _registry.values():
         if spec.env_id is not None:
             envs.setdefault(spec.env_id, {})
```

### Comparing `posggym-0.5.1/posggym/agents/torch_policy.py` & `posggym-0.6.0/posggym/agents/torch_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """PyTorch Policies."""
+
 from __future__ import annotations
 
 import os
 import pickle
+from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     NamedTuple,
@@ -26,15 +28,14 @@
 from posggym import logger
 from posggym.agents.policy import ActType, ObsType, Policy, PolicyID, PolicyState
 from posggym.agents.registration import PolicySpec
 from posggym.agents.utils import action_distributions, processors
 from posggym.agents.utils.download import download_from_repo
 from posggym.utils import seeding
 
-
 if TYPE_CHECKING:
     import posggym.model as M
 
 
 class PPOTorchModelSaveFileFormat(NamedTuple):
     """Format for saving and loading POSGGym PPOLSTMModel."""
 
@@ -49,16 +50,16 @@
 
 
 class PPOLSTMModel(nn.Module):
     """A PPO LSTM Model.
 
     Follows architecture used by Rllib, namely:
 
-      Fully Connected Layers -> LSTM Layer -> policy head (Fully connected layer)
-                                           -> value head (Fully connected layer)
+        Fully Connected Layers -> LSTM Layer -> policy head (Fully connected layer)
+                                             -> value head (Fully connected layer)
 
     Note, this model is designed for the intended use of having it's weights loaded
     from a file, and not for training. Thus it makes no effort to do things like using
     good weight initialization, rather it just aims to match the architecture of the
     saved model's weights.
 
     Additionally, it's forward function is designed to take in a single step of
@@ -114,15 +115,15 @@
         activation_fn: Optional[Callable] = None
         if activation == "tanh":
             activation_fn = nn.Tanh
         elif activation == "relu":
             activation_fn = nn.ReLU
 
         # Fully connected trunk
-        prev_size = int(np.product(obs_space.shape))
+        prev_size = int(np.prod(obs_space.shape))
         trunk = []
         for size in trunk_sizes:
             trunk.append(nn.Linear(prev_size, size))
             if activation_fn:
                 trunk.append(activation_fn())
             prev_size = size
         self.trunk = nn.Sequential(*trunk)
@@ -153,14 +154,15 @@
         actor.append(nn.Linear(prev_size, self.action_dim))
         critic.append(nn.Linear(prev_size, 1))
         self.actor = nn.Sequential(*actor)
         self.critic = nn.Sequential(*critic)
 
         # Assume model is used for evaluation only
         self.eval()
+        self.requires_grad_(False)
 
     @property
     def device(self) -> torch.device:
         """The device this model is on."""
         return next(self.parameters()).device
 
     def get_next_state(
@@ -172,25 +174,30 @@
     ) -> Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         """Get next lstm output and state.
 
         If obs is not batched, adds batch dimension with batch size of 1.
 
         Arguments
         ---------
-        obs: the observation, shape=(batch_size, obs_size) | (obs_size, )
-        lstm_state: the lstm state, this is a tuple of two tensors, each with
+        obs
+            the observation, shape=(batch_size, obs_size) | (obs_size, )
+        lstm_state
+            the lstm state, this is a tuple of two tensors, each with
             shape=(num_layers, batch_size, cell_size)
-        prev_action: the previous actions, shape=(batch_size, action_size) |
-            (action_size, )
-        prev_reward: the previous reward, shape=(batch_size, 1) | (1, )
+        prev_action
+            the previous actions, shape=(batch_size, action_size) | (action_size, )
+        prev_reward
+            the previous reward, shape=(batch_size, 1) | (1, )
 
         Returns
         -------
-        lstm_output: the lstm output, shape=(batch_size, cell_size)
-        next_lstm_state: the next lstm state, this is a tuple of two tensors, each with
+        lstm_output
+            the lstm output, shape=(batch_size, cell_size)
+        next_lstm_state
+            the next lstm state, this is a tuple of two tensors, each with
             shape=(num_layers, batch_size, cell_size)
         """
         if isinstance(obs, np.ndarray):
             obs = torch.tensor(obs, dtype=torch.float32)
 
         if len(obs.shape) == 1:
             # Single observation
@@ -236,24 +243,28 @@
     ) -> torch.Tensor:
         """Get value function output.
 
         If input is not batched, then adds batch dimension with batch size of 1.
 
         Arguments
         ---------
-        obs: the observation, shape=(batch_size, obs_size) | (obs_size, )
-        lstm_state: the lstm state, this is a tuple of two tensors, each with
+        obs
+            the observation, shape=(batch_size, obs_size) | (obs_size, )
+        lstm_state
+            the lstm state, this is a tuple of two tensors, each with
             shape=(num_layers, batch_size, cell_size)
-        prev_action: the previous actions, shape=(batch_size, action_size) |
-            (action_size, )
-        prev_reward: the previous reward, shape=(batch_size, 1) | (1, )
+        prev_action
+            the previous actions, shape=(batch_size, action_size) | (action_size, )
+        prev_reward
+            the previous reward, shape=(batch_size, 1) | (1, )
 
         Returns
         -------
-        value: output of value function, shape=(batch_size, 1)
+        value
+            output of value function, shape=(batch_size, 1)
 
         """
         hidden_state, _ = self.get_next_state(obs, lstm_state, prev_action, prev_reward)
         return self.critic(hidden_state)
 
     def get_action_and_value(
         self,
@@ -267,31 +278,39 @@
     ]:
         """Get next action and value.
 
         If input is not batched, then adds batch dimension with batch size of 1.
 
         Arguments
         ---------
-        obs: the observation, shape=(batch_size, obs_size) | (obs_size, )
-        lstm_state: the lstm state, this is a tuple of two tensors, each
-            with shape=(num_layers, batch_size, cell_size)
-        prev_action: the previous actions, shape=(batch_size, action_size) |
-            (action_size, )
-        prev_reward: the previous reward, shape=(batch_size, 1) | (1, )
-        deterministic: whether to sample action from action distribution or
-            deterministicly select action with highest probability.
+        obs
+            the observation, shape=(batch_size, obs_size) | (obs_size, )
+        lstm_state
+            the lstm state, this is a tuple of two tensors, each with
+            shape=(num_layers, batch_size, cell_size)
+        prev_action
+            the previous actions, shape=(batch_size, action_size) | (action_size, )
+        prev_reward
+            the previous reward, shape=(batch_size, 1) | (1, )
+        deterministic
+            whether to sample action from action distribution or deterministicly select
+            action with highest probability.
 
         Returns
         -------
-        action: next action, shape=(batch_size, action_size)
-        next_lstm_state: state of LSTM layer after processing input, this is a tuple of
-            two tensors, each with shape=(num_layers, batch_size, cell_size)
-        value: output of value function, shape=(batch_size, 1)
-        action_dist: the policy action distribution, shape will differ depending on
-            the action space.
+        action
+            next action, shape=(batch_size, action_size)
+        next_lstm_state
+            state of LSTM layer after processing input, this is a tuple of two tensors,
+            each with shape=(num_layers, batch_size, cell_size)
+        value
+            output of value function, shape=(batch_size, 1)
+        action_dist
+            the policy action distribution, shape will differ depending on the action
+            space.
 
         """
         with torch.no_grad():
             hidden_state, next_lstm_state = self.get_next_state(
                 obs, lstm_state, prev_action, prev_reward
             )
             value = self.critic(hidden_state)
@@ -324,44 +343,52 @@
     def get_initial_state(
         self, batch_size: int = 1
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Get the initial LSTM state.
 
         Arguments
         ---------
-        batch_size: the batch size of the LSTM state
+        batch_size
+            the batch size of the LSTM state
 
         Returns
         -------
-        initial_state: the initial LSTM state, this is a tuple of two tensors, each
-            with shape=(num_layers, batch_size, cell_size)
+        initial_state
+            the initial LSTM state, this is a tuple of two tensors, each with
+            shape=(num_layers, batch_size, cell_size)
 
         """
         return (
             torch.zeros((self.lstm.num_layers, batch_size, self.lstm.hidden_size)),
             torch.zeros((self.lstm.num_layers, batch_size, self.lstm.hidden_size)),
         )
 
 
 class PPOPolicy(Policy[ActType, ObsType]):
     """A PyTorch PPO Policy.
 
     Arguments
     ---------
-    model: the model of the environment
-    agent_id: ID of the agent in the environment the policy is for
-    policy_id: ID of the policy
-    policy_model: the underlying PyTorch policy model
-    obs_processor: the observation processor to use for processing observations before
-        they are passed into the policy model. If None, then an identity processor is
-        used.
-    action_processor: the action processor to use for processing actions before they
-        are passed into the policy model, and for unprocessing actions sampled from the
-        policy model. If None, then an identity processor is used.
-    deterministic: whether to sample actions from the policy model stochastically or
+    model
+        the model of the environment
+    agent_id
+        ID of the agent in the environment the policy is for
+    policy_id
+        ID of the policy
+    policy_model
+        the underlying PyTorch policy model
+    obs_processor
+        the observation processor to use for processing observations before they are
+        passed into the policy model. If None, then an identity processor is used.
+    action_processor
+        the action processor to use for processing actions before they are passed into
+        the policy model, and for unprocessing actions sampled from the policy model.
+        If None, then an identity processor is used.
+    deterministic
+        whether to sample actions from the policy model stochastically or
         deterministically. If True, then actions are sampled deterministically.
 
     """
 
     def __init__(
         self,
         model: M.POSGModel,
@@ -459,15 +486,15 @@
 
         return {
             "obs": obs,
             "prev_action": action,
             "prev_reward": None,
             "lstm_state": lstm_state,
             "action_probs": action_probs.numpy().squeeze(),
-            "value": value[0],
+            "value": value[0].item(),
         }
 
     def sample_action(self, state: PolicyState) -> ActType:
         pi = self.get_pi(state)
         action = pi.sample()
         return self.action_processor.unprocess(action)
 
@@ -497,22 +524,22 @@
         )
 
     @staticmethod
     def load_from_path(
         model: M.POSGModel,
         agent_id: str,
         policy_id: str,
-        policy_file_path: str,
+        policy_file_path: Path,
         deterministic: bool = False,
         obs_processor_cls: Type[processors.Processor] | None = None,
         obs_processor_config: Dict[str, Any] | None = None,
         action_processor_cls: Type[processors.Processor] | None = None,
         action_processor_config: Dict[str, Any] | None = None,
     ) -> PPOPolicy:
-        if not os.path.exists(policy_file_path):
+        if not policy_file_path.exists():
             logger.info(
                 f"Local copy of policy file for policy `{policy_id}` not found, so "
                 "downloading it from posggym-agents repo and storing local copy for "
                 "future use."
             )
             download_from_repo(policy_file_path)
 
@@ -568,50 +595,61 @@
             obs_processor=obs_processor,
             action_processor=action_processor,
             deterministic=deterministic,
         )
 
     @staticmethod
     def get_spec_from_path(
-        policy_file_path: str,
+        policy_file_path: Path,
         env_id: str,
         env_args: Dict[str, Any] | None,
         env_args_id: str | None = None,
         version: int = 0,
         valid_agent_ids: List[str] | None = None,
         nondeterministic: bool = False,
         description: str | None = None,
         **kwargs,
     ) -> PolicySpec:
         """Load PPO policy spec from policy file.
 
         Arguments
         ---------
-        policy_file_path: path to the policy file.
-        env_id: ID of the posggym environment that the policy is for.
-        env_args: Optional keywords arguments for the environment that the policy is
+        policy_file_path
+            Path to the policy file.
+        env_id
+            ID of the posggym environment that the policy is for.
+        env_args
+            Optional keywords arguments for the environment that the policy is
             for (if it is a environment specific policy). If None then assumes policy
             can be used for the environment with any arguments.
-        env_args_id: Optional ID for the environment arguments. If None then an ID will
-            be generated automatically from the env_args.
-        version: the policy version
-        valid_agent_ids: Optional AgentIDs for agents in environment that policy is
-            compatible with. If None then assumes policy can be used for any agent in
-            the environment.
-        nondeterministic: Whether this policy is non-deterministic even after seeding.
-        kwargs: Additional kwargs, if any, to pass to the agent initializing function
-        description: Optional description of the policy.
+        env_args_id
+            Optional ID for the environment arguments. If None then an ID will be
+            generated automatically from the env_args.
+        version
+            The policy version.
+        valid_agent_ids
+            Optional AgentIDs for agents in environment that policy is compatible with.
+            If None then assumes policy can be used for any agent in the environment.
+        nondeterministic
+            Whether this policy is non-deterministic even after seeding.
+        description
+            Optional description of the policy.
+        **kwargs
+            Additional kwargs, if any, to pass to the agent initializing function.
+
 
         Returns
         -------
-        spec: Policy specs for PPO Policy loaded from policy file.
+        spec
+            Policy specs for PPO Policy loaded from policy file.
 
         """
         # remove file extension
-        policy_name = os.path.basename(policy_file_path).split(".")[0]
+        policy_name = Path(policy_file_path).stem
+
         kwargs = kwargs.copy()
         kwargs["policy_file_path"] = policy_file_path
         return PolicySpec(
             policy_name=policy_name,
             entry_point=PPOPolicy.load_from_path,  # type: ignore
             version=version,
             env_id=env_id,
```

### Comparing `posggym-0.5.1/posggym/agents/utils/action_distributions.py` & `posggym-0.6.0/posggym/agents/utils/action_distributions.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/utils/download.py` & `posggym-0.6.0/posggym/agents/utils/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """Utility functions for downloading agent files."""
+
 import os
-import os.path as osp
-import pathlib
+from pathlib import Path
 
 import requests
 from clint.textui import progress  # type: ignore
 
 from posggym import error, logger
 from posggym.config import AGENT_MODEL_REPO_URL
 
+
 # largest policy file is ~ 1.3-4 MB
 LARGEST_FILE_SIZE = int(1.5 * 1024 * 1024)
 
 
-def download_to_file(url: str, dest_file_path: str):
+def download_to_file(url: str, dest_file_path: Path):
     """Download file from URL and store at specified destination.
 
     Arguments
     ---------
-    url: full url to download file from
-    dest_file_path: file path to write downloaded file to.
+    url
+        Full url to download file from.
+    dest_file_path
+        File path to write downloaded file to.
 
     Raises
     ------
-    posggym.error.DownloadError: if error occurred while trying to download file.
+    posggym.error.DownloadError
+        If error occurred while trying to download file.
 
     """
-    dest_dir = osp.dirname(dest_file_path)
-    if not osp.exists(dest_dir):
-        # create dir if it does not exist
-        os.makedirs(dest_dir)
+    dest_dir = dest_file_path.parent
+    dest_dir.mkdir(exist_ok=True)
 
     r = requests.get(url, stream=True)
     if r.ok:
         with open(dest_file_path, "wb") as f:
             content_len = r.headers.get("content-length")
             if isinstance(content_len, str):
                 try:
@@ -58,41 +60,46 @@
         except requests.exceptions.HTTPError as e:
             # wrap exception in posggym-agents error
             raise error.DownloadError(
                 f"Error while downloading file, caused by: {type(e).__name__}: {str(e)}"
             ) from e
 
 
-def download_from_repo(file_path: str, rewrite_existing: bool = False):
+def download_from_repo(file_path: Path, rewrite_existing: bool = False):
     """Download file from the posggym-agent-models github repo.
 
     Arguments
     ---------
-    file_path: local path to posgym package file.
-    rewrite_existing: whether to re-download and rewrite an existing copy of the file.
+    file_path
+        Local path to posgym package file.
+    rewrite_existing
+        Whether to re-download and rewrite an existing copy of the file.
 
     Raises
     ------
-    posggym.error.InvalidFile: if file_path is not a valid posggym-agents package file.
-    posggym.error.DownloadError: if error occurred while trying to download file.
+    posggym.error.InvalidFile
+        If file_path is not a valid posggym-agents package file.
+    posggym.error.DownloadError
+        If error occurred while trying to download file.
 
     """
-    if osp.exists(file_path) and not rewrite_existing:
+    if file_path.exists() and not rewrite_existing:
         return
 
-    path = pathlib.Path(file_path)
-    if "agents" not in path.parts:
+    if "agents" not in file_path.parts:
         raise error.InvalidFile(
             f"Invalid posggym.agents file path '{file_path}'. Path must contain the "
             "`agents` directory."
         )
 
-    base_repo_dir_index = path.parts.index("agents")
+    base_repo_dir_index = file_path.parts.index("agents")
     file_repo_url = (
-        AGENT_MODEL_REPO_URL + "posggym/" + "/".join(path.parts[base_repo_dir_index:])
+        AGENT_MODEL_REPO_URL
+        + "posggym/"
+        + "/".join(file_path.parts[base_repo_dir_index:])
     )
 
     logger.info(
         f"Downloading file from posggym-agent-models repository: {file_repo_url}."
     )
 
     return download_to_file(file_repo_url, file_path)
```

### Comparing `posggym-0.5.1/posggym/agents/utils/processors.py` & `posggym-0.6.0/posggym/agents/utils/processors.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/agents/wrappers/agent_env.py` & `posggym-0.6.0/posggym/agents/wrappers/agent_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         agent_fn: Callable[[posggym.POSGModel], Dict[str, pga.Policy]],
     ):
         """Initializes the wrapper."""
         super().__init__(env)
         self.agent_fn = agent_fn
         self.policies = agent_fn(self.model)
         self.controlled_agents = list(self.policies)
+        self.last_actions = {}
         self.last_obs = {}
         self.last_terminateds = {}
 
     @property
     def possible_agents(self) -> Tuple[str, ...]:
         return tuple(
             i for i in super().possible_agents if i not in self.controlled_agents
@@ -78,27 +79,32 @@
         assert set(self.policies) == set(
             self.controlled_agents
         ), "Agent IDs must be consistent across resets."
 
         for policy in self.policies.values():
             policy.reset()
 
+        self.last_actions = {i: None for i in self.controlled_agents if i in obs}
         self.last_obs = {i: obs[i] for i in self.controlled_agents if i in obs}
         self.last_terminateds = {i: False for i in self.controlled_agents}
         return {i: o for i, o in obs.items() if i not in self.controlled_agents}, {
             i: info for i, info in infos.items() if i not in self.controlled_agents
         }
 
     def step(self, actions):
+        joint_action = {**actions}
         for i, policy in self.policies.items():
             assert i not in actions, f"Agent {i} is controlled by the environment."
             if not self.last_terminateds[i]:
-                actions[i] = policy.step(self.last_obs[i])
+                joint_action[i] = policy.step(self.last_obs[i])
 
-        obs, rewards, terminated, truncated, dones, infos = super().step(actions)
+        obs, rewards, terminated, truncated, dones, infos = super().step(joint_action)
+        self.last_actions = {
+            i: joint_action[i] for i in self.controlled_agents if i in joint_action
+        }
         self.last_obs = {i: obs[i] for i in self.controlled_agents if i in obs}
         self.last_terminateds = {
             i: terminated[i] for i in self.controlled_agents if i in terminated
         }
         return (
             {i: obs[i] for i in obs if i not in self.controlled_agents},
             {i: rewards[i] for i in rewards if i not in self.controlled_agents},
```

### Comparing `posggym-0.5.1/posggym/core.py` & `posggym-0.6.0/posggym/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The implementation is heavily inspired by Open AI Gym
 https://github.com/openai/gym
 
 And, the more recent, Farama Foundation Gymnasium
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/core.py
 
 """
+
 from __future__ import annotations
 
 import abc
 import copy
 from typing import TYPE_CHECKING, Any, Dict, Generic, List, Optional, Tuple, TypeVar
 
 from posggym.model import ActType, ObsType, POSGModel, StateType
@@ -96,41 +97,42 @@
 
         When the end of an episode is reached, the user is responsible for
         calling :meth:`reset()` to reset this environments state.
 
         Arguments
         ---------
         actions : Dict[str, ActType]
-          a joint action containing one action per active agent in the environment.
+            a joint action containing one action per active agent in the environment.
 
         Returns
         -------
         observations : Dict[str, ObsType]
-          the joint observation containing one observation per agent.
+            the joint observation containing one observation per agent.
         rewards : Dict[str, float]
-          the joint rewards containing one reward per agent.
+            the joint rewards containing one reward per agent.
         terminations : Dict[str, bool]
-          whether each agent has reached a terminal state in the environment.
-          Contains one value for each agent in the environment. It's possible,
-          depending on the environment, for only some of the agents to be in a
-          terminal during a given step.
+            whether each agent has reached a terminal state in the environment.
+            Contains one value for each agent in the environment. It's possible,
+            depending on the environment, for only some of the agents to be in a
+            terminal during a given step.
         truncations : Dict[str, bool]
-          whether the episode has been truncated for each agent in the
-          environment. Contains one value for each agent in the environment. Truncation
-          for an agent signifies that the episode was ended for that agent (e.g. due to
-          reaching the time limit) before the agent reached a terminal state.
+            whether the episode has been truncated for each agent in the
+            environment. Contains one value for each agent in the environment.
+            Truncation for an agent signifies that the episode was ended for that agent
+            (e.g. due to reaching the time limit) before the agent reached a terminal
+            state.
         all_done : bool
-          whether the episode is finished. Provided for convenience and to handle
-          the case where agents may be added and removed during an episode. For
-          environments where the active agents remains constant during each episode,
-          this is equivalent to checking if all agents are either in a terminated or
-          truncated state. If true, the user needs to call :py:func:`reset()`.
+            whether the episode is finished. Provided for convenience and to handle
+            the case where agents may be added and removed during an episode. For
+            environments where the active agents remains constant during each episode,
+            this is equivalent to checking if all agents are either in a terminated or
+            truncated state. If true, the user needs to call :py:func:`reset()`.
         infos : Dict[str, Dict[str, Any]]
-          contains auxiliary diagnostic information (helpful for debugging, learning,
-          and logging) for each agent.
+            contains auxiliary diagnostic information (helpful for debugging, learning,
+            and logging) for each agent.
 
         """
 
     def reset(
         self, *, seed: int | None = None, options: Dict[str, Any] | None = None
     ) -> Tuple[Dict[str, ObsType], Dict[str, Dict]]:
         """Resets the environment and returns an initial observations and info.
@@ -146,30 +148,31 @@
 
         For Custom environments, the first line of :meth:`reset` should be
         ``super().reset(seed=seed)`` which implements the seeding correctly.
 
         Arguments
         ---------
         seed : int,  optional
-          The seed that is used to initialize the environment's RNG. If the
-          ``seed=None`` is passed, the RNG will *not* be reset. If you pass an
-          integer, the RNG will be reset even if it already exists. Usually, you want
-          to pass an integer *right after the environment has been initialized and
-          then never again*.
+            The seed that is used to initialize the environment's RNG. If the
+            ``seed=None`` is passed, the RNG will *not* be reset. If you pass an
+            integer, the RNG will be reset even if it already exists. Usually, you want
+            to pass an integer *right after the environment has been initialized and
+            then never again*.
         options: dict, optional
-          Additional information to specify how the environment is reset (optional,
-          depending on the specific environment)
+            Additional information to specify how the environment is reset (optional,
+            depending on the specific environment)
 
         Returns
         -------
-        observations : Dict[str, ObsType], optional
-          The joint observation containing one observation per agent in the environment.
+        observations : Dict[str, ObsType]
+            The joint observation containing one observation per agent in the
+            environment.
         infos : Dict[str, Dict]
-          Auxiliary information for each agent. It should be analogous to the ``info``
-          returned by :meth:`step()` and can be empty.
+            Auxiliary information for each agent. It should be analogous to the ``info``
+            returned by :meth:`step()` and can be empty.
 
         """
         # initialize the RNG if the seed is manually passed
         if seed is not None:
             self.model.seed(seed)
         return {}, {}
 
@@ -306,15 +309,16 @@
         "asymmetric" environments there is no guarantee that the same "policy" will
         work for different agent IDs. Examples include Pursuit-Evasion games, any
         environments where action and/or observation space differs by agent ID.
 
         Returns
         -------
         bool
-          ``True`` if environment is symmetric, ``False`` if environment is asymmetric.
+            ``True`` if environment is symmetric, ``False`` if environment is
+            asymmetric.
 
         """
         return self.model.is_symmetric
 
     @property
     def unwrapped(self) -> "Env":
         """Completely unwrap this env.
```

### Comparing `posggym-0.5.1/posggym/envs/__init__.py` & `posggym-0.6.0/posggym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/classic/mabc.py` & `posggym-0.6.0/posggym/envs/classic/mabc.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/classic/rock_paper_scissors.py` & `posggym-0.6.0/posggym/envs/classic/rock_paper_scissors.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/classic/tiger.py` & `posggym-0.6.0/posggym/envs/classic/tiger.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/continuous/core.py` & `posggym-0.6.0/posggym/envs/continuous/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core functionality for continuous environments."""
+
 from __future__ import annotations
 
 import math
 import warnings
 from abc import ABC, abstractmethod
 from enum import Enum
 from itertools import product
@@ -10,14 +11,15 @@
 from typing import Dict, Iterable, List, NamedTuple, Set, Tuple, Union
 
 import numpy as np
 from gymnasium import spaces
 
 from posggym.error import DependencyNotInstalled
 
+
 try:
     import pymunk
     from pymunk import Vec2d
 except ImportError as e:
     raise DependencyNotInstalled(
         "pymunk is not installed, run `pip install posggym[continuous]`"
     ) from e
@@ -188,18 +190,21 @@
         recommended and improves efficiency.
 
         Also performing multiple steps `t` with a smaller `dt` creates a more stable
         and accurate simulation.
 
         Arguments
         ---------
-        dt: the step size
-        t: the number of steps
-        normalize_angles: whether to normalize angle of each entity to be in [0, 2*pi]
-            at the end of the simulation.
+        dt : float
+            the step size
+        t : int
+            the number of steps
+        normalize_angles : bool
+            whether to normalize angle of each entity to be in [0, 2*pi] at the end of
+            the simulation.
 
         Reference
         ---------
         https://www.pymunk.org/en/latest/pymunk.html#pymunk.Space.step
 
         """
         for _ in range(t):
@@ -219,22 +224,27 @@
         color: Tuple[int, int, int, int] | None,
         is_static: bool = False,
     ) -> Tuple[pymunk.Body, pymunk.Circle]:
         """Add moveable entity to the world.
 
         Arguments
         ---------
-        id: the unique ID of the entity
-        radius: the radius of the entity. If none uses `self.agent_radius`
-        color: optional color for the entity. This only impacts rendering of the world.
+        id : str
+            the unique ID of the entity
+        radius : float | None
+            the radius of the entity. If none uses `self.agent_radius`
+        color : Tuple[int, int, int, int] | None
+            optional color for the entity. This only impacts rendering of the world.
 
         Returns
         -------
-        body: underlying physics Body of the entity
-        shape: the shape of the entity
+        body : pymunk.Body
+            underlying physics Body of the entity
+        shape : pymunk.Circle
+            the shape of the entity
 
         """
         if radius is None:
             radius = self.agent_radius
         mass = 1.0
         inertia = pymunk.moment_for_circle(mass, 0.0, radius)
         body_type = pymunk.Body.STATIC if is_static else pymunk.Body.DYNAMIC
@@ -308,15 +318,14 @@
         vel: FloatCoord | List[float] | np.ndarray | Vec2d | None = None,
         vangle: float | None = None,
     ):
         """Update the state of an entity.
 
         Can be used to update specific parts of the entity state, while leaving the
         other components unchanged.
-
         """
         body, _ = self.entities[id]
         if coord is not None:
             body.position = Vec2d(coord[0], coord[1])
 
         if angle is not None:
             body.angle = angle
@@ -444,26 +453,30 @@
         lines_start_coords: np.ndarray,
         lines_end_coords: np.ndarray,
     ) -> np.ndarray:
         """Check if lines intersect circles.
 
         Arguments
         ---------
-        circle_coords: array containing the `(x, y)` of the center of each circle.
-            Should have shape `(n_circles, 2)`
-        circle_radii: array containing the radius of each circle. Should have shape
-            `(n_circles,)`
-        lines_start_coords: array containing the `(x, y)` coords of the start of each of
-            the lines. Should have shape `(n_lines, 2)`
-        lines_end_coords: array containing the `(x, y)` coords of the end of of each of
-            the lines. Should have shape `(n_lines, 2)`
+        circle_coords
+            array containing the `(x, y)` of the center of each circle. Should have
+            shape `(n_circles, 2)`
+        circle_radii
+            array containing the radius of each circle. Should have shape `(n_circles,)`
+        lines_start_coords
+            array containing the `(x, y)` coords of the start of each of the lines.
+            Should have shape `(n_lines, 2)`
+        lines_end_coords
+            array containing the `(x, y)` coords of the end of of each of the lines.
+            Should have shape `(n_lines, 2)`
 
         Returns
         -------
-        distances: An array containing the euclidean distance from each lines start to
+        distances
+            An array containing the euclidean distance from each lines start to
             the first point of intersection with the corresponding circle. If the line
             does not intersect the circle, its distance will be `np.nan`.
             Should have shape `(n_circles, n_lines)`
 
         """
         starts = lines_start_coords[None, :, :] - circle_coords[:, None, :]
         ends = lines_end_coords[None, :, :] - circle_coords[:, None, :]
@@ -497,31 +510,37 @@
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Check if lines intersect.
 
         Checks for each line in `l1` if it intersects with any line in `l2`.
 
         Arguments
         ---------
-        l1_start_coords: array with shape `(n_lines1, 2)` containing the (x, y) coord
-          for the start of each of the first set of lines.
-        l1_end_coords: array with shape `(n_lines1, 2)` containing the (x, y) coord
-          for the end of each of the first set of lines.
-        l2_start_coords: array with shape `(n_lines2, 2)` containing the (x, y) coord
-          for the start of each of the second set of lines.
-        l2_end_coords: array with shape `(n_lines2, 2)` containing the (x, y) coord
-          for the end of each of the second set of lines.
+        l1_start_coords
+            array with shape `(n_lines1, 2)` containing the (x, y) coord for the start
+            of each of the first set of lines.
+        l1_end_coords
+            array with shape `(n_lines1, 2)` containing the (x, y) coord for the end of
+            each of the first set of lines.
+        l2_start_coords
+            array with shape `(n_lines2, 2)` containing the (x, y) coord for the start
+            of each of the second set of lines.
+        l2_end_coords
+            array with shape `(n_lines2, 2)` containing the (x, y) coord for the end of
+            each of the second set of lines.
 
         Returns
         -------
-        intersection_coords: array with shape `(n_lines1, n_lines2, 2)` containing the
-           (x, y) coords for the point of intersection between each pair of line
-           segments from `l1` and `l2`. If a pair of lines does not intersect, the
-           x and y coordinate values will be `np.nan`.
-        distances: array with shape `(n_lines1, n_lines2)` containing the distances
-            between the intersection point (if exists) and the corresponding point in
+        intersection_coords
+            array with shape `(n_lines1, n_lines2, 2)` containing the (x, y) coords for
+            the point of intersection between each pair of line segments from `l1` and
+            `l2`. If a pair of lines does not intersect, the x and y coordinate values
+            will be `np.nan`.
+        distances
+            array with shape `(n_lines1, n_lines2)` containing the distances between
+            the intersection point (if exists) and the corresponding point in
             l1_start_cooords.  If a pair of lines does not intersect, the distance value
             will be `np.nan`.
 
         """
         # https://stackoverflow.com/questions/3252194/numpy-and-line-intersections?noredirect=1&lq=1
         # https://en.wikipedia.org/wiki/Line%E2%80%93line_intersection
         dl1 = l1_end_coords - l1_start_coords  # (n_lines1, 2)
@@ -587,30 +606,36 @@
         include_blocks: bool = True,
         check_walls: bool = True,
     ) -> Tuple[np.ndarray, np.ndarray]:
         """Check for collision along rays.
 
         Arguments
         ---------
-        ray_start_coords: start coords of rays. Should be 2D array with shape
-           `(n_rays, 2`),
-        ray_end_coords: end coords of rays. Should be 2D array with shape
-           `(n_rays, 2`),
-        max_ray_distance: maximum ray distance
-        other_agents: `(x, y)` coordinates of any other agents to check for collisions
-           with. Should be a 2D array with shape `(n_agents, 2)`.
-        include_blocks: whether to check for collisions with blocks in the world
-        check_walls: whether to check for collisions with the world border.
+        ray_start_coords
+            start coords of rays. Should be 2D array with shape `(n_rays, 2`),
+        ray_end_coords
+            end coords of rays. Should be 2D array with shape `(n_rays, 2`),
+        max_ray_distance
+            maximum ray distance
+        other_agents
+            `(x, y)` coordinates of any other agents to check for collisions with.
+            Should be a 2D array with shape `(n_agents, 2)`.
+        include_blocks
+            whether to check for collisions with blocks in the world
+        check_walls
+            whether to check for collisions with the world border.
 
         Returns
         -------
-        distances: the distance each ray extends sway from the origin, up to a max of
+        distances
+            the distance each ray extends sway from the origin, up to a max of
             `max_ray_distance`. Array will have shape `(n_rays,)`.
-        collision_types: the type of collision for each ray (see CollisionType), if any.
-            Will have shape `(n_rays,)`.
+        collision_types
+            the type of collision for each ray (see CollisionType), if any. Will have
+            shape `(n_rays,)`.
 
         """
         n_rays = len(ray_start_coords)
         closest_distances = np.full(n_rays, max_ray_distance, dtype=np.float32)
         collision_types = np.full(n_rays, CollisionType.NONE.value, dtype=np.uint8)
 
         if other_agents is not None and len(other_agents):
@@ -693,32 +718,40 @@
         """Check for collision along rays that radiate away from the origin.
 
         Rays are evenly spaced around the origin, with the number of rays controlled
         by the `n_rays` arguments.
 
         Arguments
         ---------
-        origin: the origin position
-        ray_distance: how far each ray extends from the origin in a straight line
-        n_rays: the number of rays
-        other_agents: `(x, y)` coordinates of any other agents to check for collisions
-           with. Should be a 2D array with shape `(n_agents, 2)`.
-        include_blocks: whether to check for collisions with blocks in the world
-        check_walls: whether to check for collisions with the world border.
-        use_relative_angle: whether ray angles should be relative to the origin
-            position's angle. Otherwise line angle is treated as absolute (i.e.
-            relative to angle of 0). This controls the ordering of the rays in the
-            output.
-        angle_bounds: The maximum and minimum of the FOV as a tuple. By default
-            the agent will have a full FOV as a circle around them. This will
-            be between 0 and 2π. This can be decreased as needed.
+        origin
+            the origin position
+        ray_distance
+            how far each ray extends from the origin in a straight line
+        n_rays
+            the number of rays
+        other_agents
+            `(x, y)` coordinates of any other agents to check for collisions with.
+            Should be a 2D array with shape `(n_agents, 2)`.
+        include_blocks
+            whether to check for collisions with blocks in the world
+        check_walls
+            whether to check for collisions with the world border.
+        use_relative_angle
+            whether ray angles should be relative to the origin position's angle.
+            Otherwise line angle is treated as absolute (i.e. relative to angle of 0).
+            This controls the ordering of the rays in the output.
+        angle_bounds
+            The maximum and minimum of the FOV as a tuple. By default the agent will
+            have a full FOV as a circle around them. This will be between 0 and 2π.
+            This can be decreased as needed.
 
         Returns
         -------
-        distances: the distance each ray extends sway from the origin, up to a max of
+        distances
+            the distance each ray extends sway from the origin, up to a max of
             `ray_distance`. Array will have shape `(n_rays,)`.
 
         """
         x, y, rel_angle = origin
         if not use_relative_angle:
             rel_angle = 0.0
```

### Comparing `posggym-0.5.1/posggym/envs/continuous/driving_continuous.py` & `posggym-0.6.0/posggym/envs/continuous/driving_continuous.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The Driving Continuous Environment."""
+
 import math
 from itertools import product
 from typing import Any, Dict, List, NamedTuple, Optional, Set, Tuple, Union, cast
 
 import numpy as np
 from gymnasium import spaces
 from pymunk import Vec2d
@@ -363,18 +364,18 @@
     Parameters
     ----------
     world : str, DrivingWorld
         the world environment for the model scenario
     num_agents : int
         the number of agents in the model scenario
     obs_dists : float
-        number of cells in front, behind, and to the side that each agent
-        can observe
-    n_sensors : the number of sensor lines eminating from the agent. The agent will
-        observe at `n_sensors` equidistance intervals over `[0, 2*pi]`
+        number of cells in front, behind, and to the side that each agent can observe
+    n_sensors : int
+        the number of sensor lines eminating from the agent. The agent will observe at
+        `n_sensors` equidistance intervals over `[0, 2*pi]`
 
     """
 
     R_STEP_COST = 0.00
     R_CRASH_VEHICLE = -1.0
     R_DESTINATION_REACHED = 1.0
     R_PROGRESS = 0.05
```

### Comparing `posggym-0.5.1/posggym/envs/continuous/drone_team_capture.py` & `posggym-0.6.0/posggym/envs/continuous/drone_team_capture.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/continuous/predator_prey_continuous.py` & `posggym-0.6.0/posggym/envs/continuous/predator_prey_continuous.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The Continuous Predator-Prey Environment."""
+
 import math
 from itertools import product
 from typing import Dict, List, NamedTuple, Optional, Set, Tuple, Union, cast
 
 import numpy as np
 from gymnasium import spaces
 
@@ -347,15 +348,15 @@
     num_predators : int
         the number of predator (and thus controlled agents)
     num_prey : int
         the number of prey
     cooperative : bool
         whether environment rewards are fully shared (True) or only awarded to
         capturing predators (i.e. mixed) (False)
-    prey_strenth : int
+    prey_strenth : int, optional
         the minimum number of predators needed to capture a prey
     obs_dists : float
         number of cells in each direction around the agent that the agent can
         observe
     n_sensors : int
         the number of sensor lines for each predator
 
@@ -878,17 +879,17 @@
             prey_coords.add(pos)
         else:
             assert char == "."
 
     return PPWorld(
         size,
         blocks=list(blocks),
-        predator_start_positions=None
-        if len(predator_coords) == 0
-        else list(predator_coords),
+        predator_start_positions=(
+            None if len(predator_coords) == 0 else list(predator_coords)
+        ),
         prey_start_positions=None if len(prey_coords) == 0 else list(prey_coords),
     )
 
 
 def get_default_world(size: int, include_blocks: bool) -> PPWorld:
     """Get function for generaing default world with given size.
```

### Comparing `posggym-0.5.1/posggym/envs/continuous/pursuit_evasion_continuous.py` & `posggym-0.6.0/posggym/envs/continuous/pursuit_evasion_continuous.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/cooperative_reaching.py` & `posggym-0.6.0/posggym/envs/grid_world/cooperative_reaching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """The Cooperative Reaching Grid World Environment."""
+
 from itertools import product
-from os import path
+from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
 from posggym.core import DefaultEnv
 from posggym.envs.grid_world.core import Coord, Direction, Grid
 from posggym.utils import seeding
 
-
 # State = (coord_0, coord_1)
 CRState = Tuple[Coord, Coord]
 
 # The actions
 CRAction = int
 DO_NOTHING = 0
 UP = 1
@@ -215,15 +215,15 @@
                 self.render_mode,
                 model.grid,
                 render_fps=self.metadata["render_fps"],
                 env_name="CooperativeReaching",
             )
 
         if self._agent_imgs is None:
-            img_path = path.join(path.dirname(__file__), "img", "robot.png")
+            img_path = Path(__file__).parent / "img" / "robot.png"
             agent_img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self._agent_imgs = {
                 i: render_lib.GWImage((0, 0), self.renderer.cell_size, agent_img)
                 for i in self.possible_agents
             }
 
         observed_coords = []
@@ -281,15 +281,15 @@
         the size (width and height) of grid.
     num_goals : int
         the number of goals in the grid.
     mode : str
         the mode of the environment, which determines the layout of goals in the
         grid as well as their values. The available modes are: ["square", "line",
         "original"]
-    obs_distance : int or None
+    obs_distance : int, optional
         the number of cells in each direction that each agent can observe. This
         determines how close agents need to be to each other to be able to observe each
         other's location. Setting this to be `2*size` will make the environment fully
         observable. If `None` then will be set to `2*size`.
 
     """
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/core.py` & `posggym-0.6.0/posggym/envs/grid_world/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """General grid world problem utility functions and classes."""
+
 import enum
 import itertools
 import random
 from queue import PriorityQueue, Queue
 from typing import Dict, Iterable, List, Optional, Set, Tuple
 
 # (x, y) coord = (col, row) coord
@@ -241,29 +242,35 @@
         """Map a coord relative origin to coord on the grid.
 
         This is useful for mapping from coords in agent observations to coords in the
         actual grid.
 
         Arguments
         ---------
-        rel_coord: the relative coordinate. This is the coordinate relative to the
-            origin coordinate.
-        origin: the origin coordinate. This is the coordinate in the actual grid that
+        rel_coord
+            the relative coordinate. This is the coordinate relative to the origin
+            coordinate.
+        origin
+            the origin coordinate. This is the coordinate in the actual grid that
             the relative coordinate is based on.
-        facing_dir: the direction the relative grid is oriented.
-        forward_dim: the distance from the origin in the facing dir that the relative
-            grid reaches. Defines where the zeroth row of the relative grid is relative
+        facing_dir
+            the direction the relative grid is oriented.
+        forward_dim
+            the distance from the origin in the facing dir that the relative grid
+            reaches. Defines where the zeroth row of the relative grid is relative
             to the origin.
-        side_dim: the distance from the origin perpendicular to the facing dir that the
+        side_dim
+            the distance from the origin perpendicular to the facing dir that the
             relative grid reaches. Defines where the zeroth column of the grid is
             relative to the origin.
 
         Returns
         -------
-        The relative coord mapped to the actual grid.
+        Coord
+            The relative coord mapped to the actual grid.
 
         """
         grid_col, grid_row = origin
 
         if facing_dir == Direction.NORTH:
             grid_row += rel_coord[1] - forward_dim
             grid_col += rel_coord[0] - side_dim
@@ -281,25 +288,29 @@
     def get_rectangular_bounds(
         self, origin: Coord, facing_dir: Direction, rect_size: Tuple[int, int, int, int]
     ) -> Tuple[int, int, int, int]:
         """Get rectangular bounds for a rectangle with given origin and size.
 
         Arguments
         ---------
-        origin: the origin coordinate for the rectangle
-        facing_dir: which direction the rectangle is oriented
-        rect_size: the size of the rectangle relative to the origin. Specifically,
-            rect_size[0] = number of cells in front
-            rect_size[1] = number of cells behind
-            rect_size[2] = number of cells left
-            rect_size[3] = number of cells right
+        origin
+            the origin coordinate for the rectangle
+        facing_dir
+            which direction the rectangle is oriented
+        rect_size
+            the size of the rectangle relative to the origin. Specifically,
+                rect_size[0] = number of cells in front
+                rect_size[1] = number of cells behind
+                rect_size[2] = number of cells left
+                rect_size[3] = number of cells right
 
         Returns
         -------
-        min_col, max_col, min_row, max_row of rectangle that is within the grid's
+        Tuple[int, int, int, int]
+            min_col, max_col, min_row, max_row of rectangle that is within the grid's
             bounds. Note that this may be smaller than the rectangle as specified by the
             rect_size.
 
         """
         assert 0 <= origin[0] < self.width and 0 <= origin[1] < self.height
         assert all(d >= 0 for d in rect_size)
         col, row = origin
@@ -326,25 +337,29 @@
         """Get padding for a rectangle with given origin and size.
 
         The padding quantities are the number of cells the rectangle is out-of-bounds
         on each dimension.
 
         Arguments
         ---------
-        origin: the origin coordinate for the rectangle
-        facing_dir: which direction the rectangle is oriented
-        rect_size: the size of the rectangle relative to the origin. Specifically,
-            rect_size[0] = number of cells in front
-            rect_size[1] = number of cells behind
-            rect_size[2] = number of cells left
-            rect_size[3] = number of cells right
+        origin
+            the origin coordinate for the rectangle
+        facing_dir
+            which direction the rectangle is oriented
+        rect_size
+            the size of the rectangle relative to the origin. Specifically,
+                rect_size[0] = number of cells in front
+                rect_size[1] = number of cells behind
+                rect_size[2] = number of cells left
+                rect_size[3] = number of cells right
 
         Returns
         -------
-        (before_col, after_col), (before_row, after_row padding)
+        Tuple[Tuple[int, int], Tuple[int, int]]
+            (before_col, after_col), (before_row, after_row padding)
 
         """
         assert 0 <= origin[0] < self.width and 0 <= origin[1] < self.height
         assert all(d >= 0 for d in rect_size)
         col, row = origin
 
         # rotate rectangle sizes based on direction so they are treated as if
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/driving.py` & `posggym-0.6.0/posggym/envs/grid_world/driving.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The Driving Grid World Environment."""
+
 import enum
 from itertools import product
 from typing import Any, Dict, List, NamedTuple, Optional, Sequence, Set, Tuple, Union
 
 from gymnasium import spaces
 
 import posggym.model as M
@@ -367,16 +368,15 @@
     Parameters
     ----------
     grid : DrivingGrid
         the grid environment for the model scenario
     num_agents : int
         the number of agents in the model scenario
     obs_dims : (int, int, int)
-        number of cells in front, behind, and to the side that each agent
-        can observe
+        number of cells in front, behind, and to the side that each agent can observe
     """
 
     R_CRASH_VEHICLE = -1.0
     R_DESTINATION_REACHED = 0.5
     R_PROGRESS_TOTAL = 0.5
 
     def __init__(
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/driving_gen.py` & `posggym-0.6.0/posggym/envs/grid_world/driving_gen.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/agent.png` & `posggym-0.6.0/posggym/envs/grid_world/img/agent.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/agent_white.png` & `posggym-0.6.0/posggym/envs/grid_world/img/agent_white.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/apple.png` & `posggym-0.6.0/posggym/envs/grid_world/img/apple.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/drone.png` & `posggym-0.6.0/posggym/envs/grid_world/img/drone.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/house.png` & `posggym-0.6.0/posggym/envs/grid_world/img/house.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/robber.png` & `posggym-0.6.0/posggym/envs/grid_world/img/robber.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/img/robot.png` & `posggym-0.6.0/posggym/envs/grid_world/img/robot.png`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/envs/grid_world/level_based_foraging.py` & `posggym-0.6.0/posggym/envs/grid_world/level_based_foraging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The Level-Based Foraging Environment."""
+
 import enum
 import math
 from collections import defaultdict
 from itertools import product
-from os import path
+from pathlib import Path
 from typing import Dict, List, NamedTuple, Optional, Tuple, Union
 
 import numpy as np
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
@@ -288,29 +289,29 @@
                 self.render_mode,
                 model.grid,
                 render_fps=self.metadata["render_fps"],
                 env_name="LevelBasedForaging",
             )
 
         if self.agent_imgs is None:
-            img_path = path.join(path.dirname(__file__), "img", "robot.png")
+            img_path = Path(__file__).parent / "img" / "robot.png"
             agent_img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             font = render_lib.load_font(
                 "Comic Sans MC",
                 render_lib.get_default_font_size(self.renderer.cell_size),
             )
             self.agent_imgs = {
                 i: render_lib.GWImageAndText(
                     (0, 0), self.renderer.cell_size, agent_img, str(1), font
                 )
                 for i in self.possible_agents
             }
 
         if self.food_imgs is None:
-            img_path = path.join(path.dirname(__file__), "img", "apple.png")
+            img_path = Path(__file__).parent / "img" / "apple.png"
             food_img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             font = render_lib.load_font(
                 "Comic Sans MC",
                 render_lib.get_default_font_size(self.renderer.cell_size),
             )
             self.food_imgs = [
                 render_lib.GWImageAndText(
@@ -367,15 +368,15 @@
         width and height of the playing field
     max_food : int
         the max number of food that can be spawned
     sight : int
         observation size of each agent
     force_coop : bool
         whether to force cooperation or not
-    observation_mode : str, optional
+    observation_mode : str
         The observation mode for agent (default='tuple')
           - 'grid' - observations are multiple 2D grids (3D np.ndarray)
           - 'vector' - observations are vector (1D np.ndarray)
           - 'tuple' - observations are a tuple with same format as 'vector'
                       observations but as a hashable Python tuple object
                       containing integers instead of floats
     """
@@ -845,16 +846,15 @@
         self, obs: LBFObs
     ) -> Tuple[List[Tuple[int, int, int]], List[Tuple[int, int, int]]]:
         """Parse observation into (x, y, level) agent and food triplets.
 
         Agent obs are ordered so the observing agent is first, then the
         remaining observations are by agent order.
 
-        On triplet of [-1, -1, 0] means no observation for the given agent or
-        food.
+        On triplet of [-1, -1, 0] means no observation for the given agent or food.
         """
         if self.observation_mode == "tuple":
             assert isinstance(obs, tuple)
             return self.parse_tuple_obs(obs)
 
         assert isinstance(obs, np.ndarray)
         if self.observation_mode == "grid":
@@ -866,29 +866,27 @@
         self, obs: np.ndarray
     ) -> Tuple[List[Tuple[int, int, int]], List[Tuple[int, int, int]]]:
         """Parse grid observation int (x, y, level) agent and food triplets.
 
         Agent obs are ordered so the observing agent is first, then the
         remaining observations are by agent order.
 
-        On triplet of [-1, -1, 0] means no observation for the given agent or
-        food.
+        On triplet of [-1, -1, 0] means no observation for the given agent or food.
         """
         raise NotImplementedError
 
     def parse_vector_obs(
         self, obs: np.ndarray
     ) -> Tuple[List[Tuple[int, int, int]], List[Tuple[int, int, int]]]:
         """Parse vector obs into (x, y, level) agent and food triplets.
 
         Agent obs are ordered so the observing agent is first, then the
         remaining observations are by agent order.
 
-        On triplet of [-1, -1, 0] means no observation for the given agent or
-        food.
+        On triplet of [-1, -1, 0] means no observation for the given agent or food.
         """
         assert obs.shape[0] == 3 * (len(self.possible_agents) + self.max_food)
         agent_obs = []
         food_obs = []
         for i in range(0, obs.shape[0], 3):
             triplet = (int(obs[i]), int(obs[i + 1]), int(obs[i + 2]))
             if i < len(self.possible_agents) * 3:
@@ -901,16 +899,15 @@
         self, obs: Tuple[int, ...]
     ) -> Tuple[List[Tuple[int, int, int]], List[Tuple[int, int, int]]]:
         """Parse tuple obs into (x, y, level) agent and food triplets.
 
         Agent obs are ordered so the observing agent is first, then the
         remaining observations are by agent order.
 
-        On triplet of [-1, -1, 0] means no observation for the given agent or
-        food.
+        On triplet of [-1, -1, 0] means no observation for the given agent or food.
         """
         assert len(obs) == 3 * (len(self.possible_agents) + self.max_food)
         agent_obs = []
         food_obs = []
         for i in range(0, len(obs), 3):
             triplet = (int(obs[i]), int(obs[i + 1]), int(obs[i + 2]))
             if i < len(self.possible_agents) * 3:
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/predator_prey.py` & `posggym-0.6.0/posggym/envs/grid_world/predator_prey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The Predator-Prey Grid World Environment."""
+
 import math
 from itertools import product
-from os import path
+from pathlib import Path
 from typing import Dict, List, NamedTuple, Optional, Sequence, Set, Tuple, Union
 
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
 from posggym.core import DefaultEnv
@@ -265,15 +266,15 @@
                 self.render_mode,
                 model.grid,
                 render_fps=self.metadata["render_fps"],
                 env_name="PredatorPrey",
             )
 
         if self._predator_imgs is None:
-            img_path = path.join(path.dirname(__file__), "img", "robot.png")
+            img_path = Path(__file__).parent / "img" / "robot.png"
             agent_img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self._predator_imgs = {
                 i: render_lib.GWImage((0, 0), self.renderer.cell_size, agent_img)
                 for i in self.possible_agents
             }
 
         observed_coords = []
@@ -327,15 +328,15 @@
     num_predators : int
         the number of predator (and thus controlled agents)
     num_prey : int
         the number of prey
     cooperative : bool
         whether environment rewards are fully shared (True) or only awarded to
         capturing predators (i.e. mixed) (False)
-    prey_strenth : int
+    prey_strenth : int, optional
         how many predators are required to capture each prey, minimum is `1` and maximum
         is `min(4, num_predators)`. If `None` this is set to `min(4, num_predators)`
     obs_dims : int
         number of cells in each direction around the agent that the agent can
         observe
 
     """
@@ -573,17 +574,19 @@
 
         raise AssertionError("Something has gone wrong, please investigate.")
 
     def _move_away_from_preys(
         self, prey_coord: Coord, state: PPState, occupied_coords: Set[Coord]
     ) -> Optional[Coord]:
         prey_dists = [
-            self.grid.manhattan_dist(prey_coord, c)
-            if (c != prey_coord and not state.prey_caught[i])
-            else float("inf")
+            (
+                self.grid.manhattan_dist(prey_coord, c)
+                if (c != prey_coord and not state.prey_caught[i])
+                else float("inf")
+            )
             for i, c in enumerate(state.prey_coords)
         ]
         min_prey_dist = min(prey_dists)
         all_closest_prey_coords = [
             state.prey_coords[i]
             for i in range(self.num_prey)
             if prey_dists[i] == min_prey_dist
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/pursuit_evasion.py` & `posggym-0.6.0/posggym/envs/grid_world/pursuit_evasion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """The Pursuit-Evasion Grid World Environment."""
+
 from collections import deque
 from typing import Any, Deque, Dict, List, NamedTuple, Optional, Set, Tuple, Union, cast
 
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
 from posggym.core import DefaultEnv
 from posggym.envs.grid_world.core import Coord, Direction, Grid
 from posggym.utils import seeding
 
-
 # State = (e_coord, e_dir, p_coord, p_dir, e_0_coord, p_0_coord, e_goal_coord)
 INITIAL_DIR = Direction.NORTH
 
 
 class PEState(NamedTuple):
     """Environment state in Pursuit Evastion problem."""
 
@@ -441,15 +441,15 @@
     def get_agents(self, state: PEState) -> List[str]:
         return list(self.possible_agents)
 
     def sample_initial_state(self) -> PEState:
         return self._sample_initial_state(None, None, None)
 
     def sample_agent_initial_state(self, agent_id: str, obs: PEObs) -> PEState:
-        if agent_id == self.EVADER_IDX:
+        if agent_id == str(self.EVADER_IDX):
             return self._sample_initial_state(
                 evader_coord=obs[1], pursuer_coord=obs[2], goal_coord=obs[3]
             )
         return self._sample_initial_state(
             evader_coord=obs[1], pursuer_coord=obs[2], goal_coord=None
         )
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/render.py` & `posggym-0.6.0/posggym/envs/grid_world/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions and classes for rendering grid world environments."""
 import abc
 from typing import Dict, List, Optional, Tuple, Union
 
+from pathlib import Path
 import numpy as np
 
 from posggym.envs.grid_world.core import Coord, Direction, Grid
 from posggym.error import DependencyNotInstalled
 
 ColorTuple = Union[Tuple[int, int, int], Tuple[int, int, int, int]]
 
@@ -36,15 +37,15 @@
 
 
 def get_color(color_name: str) -> ColorTuple:
     """Get color from name."""
     return pygame.colordict.THECOLORS[color_name]
 
 
-def load_img_file(img_path: str, cell_size: Tuple[int, int]):
+def load_img_file(img_path: Path, cell_size: Tuple[int, int]):
     """Load an image from file and scale it to cell size."""
     return pygame.transform.scale(pygame.image.load(img_path), cell_size)
 
 
 def get_default_font_size(cell_size: Tuple[int, int]) -> int:
     """Get the default font size based on cell size."""
     return cell_size[1] // 2
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/two_paths.py` & `posggym-0.6.0/posggym/envs/grid_world/two_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The Two-Paths Grid World Environment."""
 import itertools
-from os import path
+from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple, Union
 
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
 from posggym.core import DefaultEnv
@@ -184,20 +184,20 @@
                     coord, self.renderer.cell_size, render_lib.get_color("green")
                 )
                 for coord in grid.goal_coords
             ]
             self.renderer.static_objects.extend(goal_imgs)
 
         if self.runner_img is None:
-            img_path = path.join(path.dirname(__file__), "img", "robot.png")
+            img_path = Path(__file__).parent / "img" / "robot.png"
             img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self.runner_img = render_lib.GWImage((0, 0), self.renderer.cell_size, img)
 
         if self.chaser_img is None:
-            img_path = path.join(path.dirname(__file__), "img", "robot.png")
+            img_path = Path(__file__).parent / "img" / "robot.png"
             img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self.chaser_img = render_lib.GWImage((0, 0), self.renderer.cell_size, img)
 
         self.runner_img.coord = self._state[0]
         self.chaser_img.coord = self._state[1]
         render_objects = [self.runner_img, self.chaser_img]
```

### Comparing `posggym-0.5.1/posggym/envs/grid_world/uav.py` & `posggym-0.6.0/posggym/envs/grid_world/uav.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The Unmanned Aerial Vehicle Grid World Environment."""
 import random
-from os import path
+from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple, Union
 
 from gymnasium import spaces
 
 import posggym.model as M
 from posggym import logger
 from posggym.core import DefaultEnv
@@ -178,28 +178,28 @@
                 render_fps=self.metadata["render_fps"],
                 env_name="UAV",
                 bg_color=(255, 255, 255),
                 grid_line_color=(0, 0, 0),
             )
 
             # add house to static objects list
-            img_path = path.join(path.dirname(__file__), "img", "house.png")
+            img_path = Path(__file__).parent / "img" / "house.png"
             img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             house_img = render_lib.GWImage(
                 grid.safe_house_coord, self.renderer.cell_size, img
             )
             self.renderer.static_objects.append(house_img)
 
         if self.uav_img is None:
-            img_path = path.join(path.dirname(__file__), "img", "drone.png")
+            img_path = Path(__file__).parent / "img" / "drone.png"
             img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self.uav_img = render_lib.GWImage((0, 0), self.renderer.cell_size, img)
 
         if self.fug_img is None:
-            img_path = path.join(path.dirname(__file__), "img", "robber.png")
+            img_path = Path(__file__).parent / "img" / "robber.png"
             img = render_lib.load_img_file(img_path, self.renderer.cell_size)
             self.fug_img = render_lib.GWImage((0, 0), self.renderer.cell_size, img)
 
         self.uav_img.coord = self._state[0]
         self.fug_img.coord = self._state[1]
 
         return self.renderer.render([self.uav_img, self.fug_img])
```

### Comparing `posggym-0.5.1/posggym/envs/registration.py` & `posggym-0.6.0/posggym/envs/registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Functions and classes for registering and loading implemented environments.
 
 Based on Farama Foundation Gymnasium, copied and adapted here to avoid issues with
 gymnasiums global registry and difference in naming format.
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/envs/registration.py
 
 """
+
 from __future__ import annotations
 
 import contextlib
 import copy
 import difflib
 import importlib
 import re
 import sys
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Any, Callable, Dict, Iterable, List, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Tuple
 
 from posggym import error, logger
 from posggym.wrappers import OrderEnforcing, PassiveEnvChecker, TimeLimit
 
-
 if sys.version_info < (3, 10):
     import importlib_metadata as metadata  # type: ignore
-else:
-    import importlib.metadata as metadata
 
 
 if TYPE_CHECKING:
     from posggym.core import Env
 
 
 # [namespace/](env-name)-v(version)
@@ -38,19 +36,21 @@
 
 
 def load(name: str) -> Callable:
     """Loads environment with name and returns an environment creation function.
 
     Arguments
     ---------
-    name: The environment name
+    name : str
+        The environment name
 
     Returns
     -------
-    entry_point: Environment creation function.
+    entry_point : Callable
+        Environment creation function.
 
     """
     mod_name, attr_name = name.split(":")
     mod = importlib.import_module(mod_name)
     fn = getattr(mod, attr_name)
     return fn
 
@@ -58,25 +58,30 @@
 def parse_env_id(env_id: str) -> Tuple[str | None, str, int | None]:
     """Parse environment ID string format.
 
     [namespace/](env-name)-v(version)    env-name is group 1, version is group 2
 
     Arguments
     ---------
-    env_id: The environment id to parse
+    env_id : str
+        The environment id to parse
 
     Returns
     -------
-    ns: The environment namespace
-    name: The environment name
-    version: The environment version
+    ns : str | None
+        The environment namespace
+    name : str
+        The environment name
+    version : int | None
+        The environment version
 
     Raises
     ------
-    Error: If the environment id does not a valid environment regex
+    Error
+        If the environment id does not a valid environment regex
 
     """
     match = ENV_ID_RE.fullmatch(env_id)
     if not match:
         raise error.Error(
             f"Malformed environment ID: {env_id}. (Currently all IDs must be of the "
             "form [namespace/](env-name)-v(version) (namespace is optional))."
@@ -91,21 +96,25 @@
 def get_env_id(ns: str | None, name: str, version: int | None) -> str:
     """Get the full env ID given a name and (optional) version and namespace.
 
     Inverse of :meth:`parse_env_id`.
 
     Arguments
     ---------
-    ns: The environment namespace
-    name: The environment name
-    version: The environment version
+    ns : str | None
+        The environment namespace.
+    name : str
+        The environment name.
+    version : int | None
+        The environment version.
 
     Returns
     -------
-    env_id: The environment id
+    str
+        The environment id.
 
     """
     full_name = name
     if version is not None:
         full_name += f"-v{version}"
     if ns is not None:
         full_name = ns + "/" + full_name
@@ -114,25 +123,32 @@
 
 @dataclass
 class EnvSpec:
     """A specification for creating environments with posggym.make.
 
     Attributes
     ----------
-    id: The official environment ID.
-    entry_point: Python entrypoint of the environment class (e.g. module.name:Class).
-    reward_threshold: The reward threshold before the task is considered solved.
-    nondeterministic: Whether this environment is non-deterministic even after seeding.
-    max_episode_steps: The maximum number of steps that an episode can take before.
-        truncation.
-    order_enforce: Whether to wrap the environment in an orderEnforcing wrapper, that
-        enforces the order of of `reset` before `step` and `render` functions.
-    disable_env_checker: Whether to disable the environment checker wrapper in
-        `posggym.make`, by default False (runs the environment checker)
-    kwargs: Additional kwargs to pass to the environment class
+    id
+        The official environment ID.
+    entry_point
+        Python entrypoint of the environment class (e.g. module.name:Class).
+    reward_threshold
+        The reward threshold before the task is considered solved.
+    nondeterministic
+        Whether this environment is non-deterministic even after seeding.
+    max_episode_steps
+        The maximum number of steps that an episode can take before truncation.
+    order_enforce
+        Whether to wrap the environment in an orderEnforcing wrapper, that enforces the
+        order of of `reset` before `step` and `render` functions.
+    disable_env_checker
+        Whether to disable the environment checker wrapper in `posggym.make`, by default
+        False (runs the environment checker).
+    kwargs
+        Additional kwargs to pass to the environment class.
 
     """
 
     id: str
     entry_point: Callable | str
 
     # Environment attributes
@@ -213,23 +229,28 @@
     """Check if env version exists in namespace. Print helpful error message if not.
 
     This is a complete test whether an environment identifier is valid, and will
     provide the best available hints.
 
     Arguments
     ---------
-    ns: The environment namespace
-    name: The environment space
-    version: The environment version
+    ns : str | None
+        The environment namespace.
+    name : str
+        The environment space.
+    version : int | None
+        The environment version.
 
     Raises
     ------
-    DeprecatedEnv: The environment doesn't exist but a default version does or the
-        environment version is deprecated
-    VersionNotFound: The ``version`` used doesn't exist
+    DeprecatedEnv
+        The environment doesn't exist but a default version does or the environment
+        version is deprecated.
+    VersionNotFound
+        The ``version`` used doesn't exist.
 
     """
     if get_env_id(ns, name, version) in registry:
         return
 
     _check_name_exists(ns, name)
     if version is None:
@@ -386,27 +407,34 @@
 
         `(namespace)/(env_name)-v(version)` where `namespace` is optional.
 
     It takes arbitrary keyword arguments, which are passed to the `EnvSpec` constructor.
 
     Arguments
     ---------
-    id: The environment id
-    entry_point: The entry point for creating the environment
-    reward_threshold: The reward threshold considered to have learnt an environment
-    nondeterministic: If the environment is nondeterministic (even with knowledge of
-        the initial seed and all actions)
-    max_episode_steps: The maximum number of episodes steps before truncation. Used
-        by the Time Limit wrapper.
-    order_enforce: If to enable the order enforcer wrapper to ensure users run
-        functions in the correct order
-    disable_env_checker: Whether to disable the environment checker for the environment.
-        Recommended to False.
-    **kwargs: arbitrary keyword arguments which are passed to the environment
-        constructor
+    id : str
+        The environment id.
+    entry_point : Callable | str
+        The entry point for creating the environment.
+    reward_threshold : float | None
+        The reward threshold considered to have learnt an environment.
+    nondeterministic : bool
+        If the environment is nondeterministic (even with knowledge of the initial seed
+        and all actions).
+    max_episode_steps : int | None
+        The maximum number of episodes steps before truncation. Used by the Time Limit
+        wrapper.
+    order_enforce : bool
+        If to enable the order enforcer wrapper to ensure users run functions in the
+        correct order.
+    disable_env_checker : bool
+        Whether to disable the environment checker for the environment. Recommended to
+        False.
+    **kwargs
+        Arbitrary keyword arguments which are passed to the environment constructor.
 
     """
     global registry, current_namespace
     ns, name, version = parse_env_id(id)
 
     ns_id = ns
     if current_namespace is not None:
@@ -449,30 +477,36 @@
     """Create an environment according to the given ID.
 
     To find all available environments use `posggym.envs.registry.keys()` for all valid
     ids.
 
     Arguments
     ---------
-    id: Name of the environment. Optionally, a module to import can be included,
-        eg. 'module:Env-v0'
-    max_episode_steps: Maximum length of an episode (TimeLimit wrapper).
-    disable_env_checker: Whether to run the env checker, None will default to the
-            environment specification `disable_env_checker` (which is by default False,
-            running the environment checker), otherwise will run according to this
-            parameter (`True` = not run, `False` = run)
-    kwargs: Additional arguments to pass to the environment constructor.
+    id : str | EnvSpec
+        Name of the environment. Optionally, a module to import can be included,
+        eg. 'module:Env-v0'.
+    max_episode_steps : int | None
+        Maximum length of an episode (TimeLimit wrapper).
+    disable_env_checker : bool | None
+        Whether to run the env checker, None will default to the environment
+        specification `disable_env_checker` (which is by default False, running the
+        environment checker), otherwise will run according to this parameter
+        (`True` = not run, `False` = run).
+    **kwargs
+        Additional arguments to pass to the environment constructor.
 
     Returns
     -------
-    env: An instance of the environment.
+    Env
+        An instance of the environment.
 
     Raises
     ------
-    Error: If the ``id`` doesn't exist then an error is raised
+    Error
+        If the ``id`` doesn't exist then an error is raised
 
     """
     if isinstance(id, EnvSpec):
         spec_ = id
     else:
         module, id = (None, id) if ":" not in id else id.split(":")  # type: ignore
         if module is not None:
@@ -525,17 +559,14 @@
 
     render_modes = None
     if hasattr(env_creator, "metadata"):
         _check_metadata(env_creator.metadata)
         render_modes = env_creator.metadata.get("render_modes")
     mode = _kwargs.get("render_mode")
 
-    # TODO Johnny
-    # Add support for attempting to apply applying HumanRendering/RenderCollection
-    # wrappers (see gymnasium.envs.registration:make function)
     if mode is not None and render_modes is not None and mode not in render_modes:
         raise error.UnsupportedMode(
             f"The environment is being initialised with render_mode={mode} "
             f"that is not in the possible render_modes ({render_modes})."
         )
 
     try:
@@ -570,55 +601,63 @@
 
 
 def spec(env_id: str) -> EnvSpec:
     """Retrieve the spec for the given environment from the global registry.
 
     Arguments
     ---------
-    env_id: the environment id.
+    env_id : str
+        The environment id.
 
     Returns
     -------
-    spec: the environment spec from the global registry.
+    EnvSpec
+        The environment spec from the global registry.
 
     Raises
     ------
-    Error: if environment with given ``env_id`` doesn't exist in global registry.
+    Error
+        If environment with given ``env_id`` doesn't exist in global registry.
 
     """
     spec_ = registry.get(env_id)
     if spec_ is None:
         ns, name, version = parse_env_id(env_id)
         _check_version_exists(ns, name, version)
         raise error.Error(f"No registered env with id: {env_id}")
     else:
         assert isinstance(spec_, EnvSpec)
         return spec_
 
 
 def pprint_registry(
-    _registry: dict = registry,
+    _registry: Dict = registry,
     num_cols: int = 3,
     exclude_namespaces: List[str] | None = None,
     disable_print: bool = False,
 ) -> str | None:
     """Pretty print the environments in the registry.
 
     Arguments
     ---------
-    _registry: Environment registry to be printed.
-    num_cols: Number of columns to arrange environments in, for display.
-    exclude_namespaces: Exclude any namespaces from being printed.
-    disable_print: Whether to return a string of all the namespaces and environment IDs
-        instead of printing it to console.
+    _registry : Dict
+        Environment registry to be printed.
+    num_cols : int
+        Number of columns to arrange environments in, for display.
+    exclude_namespaces : List[str] | None
+        Exclude any namespaces from being printed.
+    disable_print : bool
+        Whether to return a string of all the namespaces and environment IDs instead of
+        printing it to console.
 
     Returns
     -------
-    return_str: formatted str representation of registry, if ``disable_print=True``,
-        otherwise returns ``None``.
+    str | None
+        Formatted str representation of registry, if ``disable_print=True``, otherwise
+        returns ``None``.
 
     """
     # Defaultdict to store environment names according to namespace.
     namespace_envs = defaultdict(lambda: [])
     max_justify = float("-inf")
     for env in _registry.values():
         namespace, _, _ = parse_env_id(env.id)
```

### Comparing `posggym-0.5.1/posggym/error.py` & `posggym-0.6.0/posggym/error.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/logger.py` & `posggym-0.6.0/posggym/logger.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/model.py` & `posggym-0.6.0/posggym/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """The model data structure."""
+
 from __future__ import annotations
 
 import abc
 import dataclasses
 import enum
 import random
 from typing import TYPE_CHECKING, Dict, Generic, List, Tuple, TypeVar
 
 import numpy as np
 
 from posggym import error
 from posggym.utils import seeding
 
-
 if TYPE_CHECKING:
     from gymnasium import spaces
 
     from posggym.envs.registration import EnvSpec
 
 
 StateType = TypeVar("StateType")
@@ -127,45 +127,50 @@
         """Get list of IDs for all agents that are active in given state.
 
         The list of active agents may change depending on state.
 
         For any environment where the number of agents remains constant during AND
         across episodes. This will be :attr:`possible_agents`, independent of state.
 
+        Arguments
+        ---------
+        state : StateType
+            The environment state
+
         Returns
         -------
         List[str]
-          List of IDs for all agents that active in given state,
+            List of IDs for all agents that active in given state,
 
         """
 
     @abc.abstractmethod
     def sample_initial_state(self) -> StateType:
         """Sample an initial state.
 
         Returns
         -------
         StateType
-          An initial state.
+            An initial state.
 
         """
 
     @abc.abstractmethod
     def sample_initial_obs(self, state: StateType) -> Dict[str, ObsType]:
         """Sample initial agent observations given an initial state.
 
         Arguments
         ---------
         state : StateType
-          The initial state.
+            The initial state.
 
         Returns
         -------
         Dict[str, ObsType]
-          A mapping from agent ID to their initial observation.
+            A mapping from agent ID to their initial observation.
 
         """
 
     @abc.abstractmethod
     def step(
         self, state: StateType, actions: Dict[str, ActType]
     ) -> JointTimestep[StateType, ObsType]:
@@ -182,39 +187,39 @@
         encouraged to include this information in the `info` property of the returned
         value. We suggest using the "outcome" key with an instance of the ``Outcome``
         class for values.
 
         Arguments
         ---------
         state : StateType
-          The state.
+            The state.
         actions : Dict[str, ActType]
-          a joint action containing one action per active agent in the environment.
+            a joint action containing one action per active agent in the environment.
 
         Returns
         -------
-        JointTimestep :
-          joint timestep result of performing actions in given state, including next
-          state, observations, rewards, terminations, truncations, all done, infos.
+        JointTimestep
+            joint timestep result of performing actions in given state, including next
+            state, observations, rewards, terminations, truncations, all done, infos.
 
         """
 
     def seed(self, seed: int | None = None):
         """Set the seed for the model random number generator.
 
         Also handles seeding for the action, observation, and (if it exists) state
         spaces.
 
         Arguments
         ---------
         seed : int, optional
-          The seed that is used to initialize the models's RNG. If the
-          ``seed=None`` is passed, the RNG will *not* be reset. If you pass an
-          integer, the RNG will be reset even if it already exists. Usually, you want
-          to pass a seed when you first initialize the model.
+            The seed that is used to initialize the models's RNG. If the
+            ``seed=None`` is passed, the RNG will *not* be reset. If you pass an
+            integer, the RNG will be reset even if it already exists. Usually, you want
+            to pass a seed when you first initialize the model.
 
         """
         if isinstance(self.rng, random.Random):
             self._rng, seed = seeding.std_random(seed)
         elif isinstance(self.rng, np.random.Generator):
             self._rng, seed = seeding.np_random(seed)
         else:
@@ -243,27 +248,27 @@
         It is optional to implement this method but can be helpful in environments that
         are used for planning and where there are a huge number of possible initial
         states.
 
         Arguments
         ---------
         agent_id : Union[int, str]
-          The ID of the agent to get initial state for.
+            The ID of the agent to get initial state for.
         obs : ObsType
-          The initial observation of the agent.
+            The initial observation of the agent.
 
         Returns
         -------
         StateType
-          An initial state for the agent conditioned on their initial observation.
+            An initial state for the agent conditioned on their initial observation.
 
         Raises
         ------
         NotImplementedError
-          If this method is not implemented.
+            If this method is not implemented.
 
         """
         raise NotImplementedError
 
     @property
     def reward_ranges(self) -> Dict[str, Tuple[float, float]]:
         r"""A mapping from Agent ID to min and max possible rewards for that agent.
@@ -327,17 +332,17 @@
 
         The initial belief distribution :math:`b_{0}` maps initial states to
         probabilities.
 
         Returns
         -------
         Dict[StateType, float]
-           :math:`Pr(s_{0}=s)` the initial probability of each state. If a state is not
-           included in the initial distribution object, it should be assumed to have
-           probability 0.
+            :math:`Pr(s_{0}=s)` the initial probability of each state. If a state is not
+            included in the initial distribution object, it should be assumed to have
+            probability 0.
 
         """
 
     @abc.abstractmethod
     def transition_fn(
         self, state: StateType, actions: Dict[str, ActType], next_state: StateType
     ) -> float:
@@ -346,25 +351,25 @@
         The transition function :math:`T(s, a, s') \rightarrow [0, 1]` defines
         :math:`Pr(s'|s, a)`, the probability of getting next state `s'` given the
         environment was in state `s` and joint action `a` was performed.
 
         Arguments
         ---------
         state : StateType
-          the state the environment was in
+            the state the environment was in
         actions : Dict[str, ActType]
-          the joint action performed
+            the joint action performed
         next_state : StateType
-          the state of the environment after actions were performed
+            the state of the environment after actions were performed
 
         Returns
         -------
         float
-          :math:`Pr(s'|s, a)`, the probability of getting next state `s'` given the
-          environment was in state `s` and joint action `a` was performed.
+            :math:`Pr(s'|s, a)`, the probability of getting next state `s'` given the
+            environment was in state `s` and joint action `a` was performed.
 
         """
 
     @abc.abstractmethod
     def observation_fn(
         self,
         obs: Dict[str, ObsType],
@@ -376,25 +381,25 @@
         The observation function :math:`Z(o, s', a) \rightarrow [0, 1]` defines
         :math:`Pr(o|s', a)`, the probability of joint observation `o` given the joint
         action `a` was performed and the environment ended up in state `s'`
 
         Arguments
         ---------
         obs : Dict[str, ObsType]
-          the observation received
+            the observation received
         actions : Dict[str, ActType]
-          the joint action performed
+            the joint action performed
         next_state : StateType
-          the state of the environment after actions were performed
+            the state of the environment after actions were performed
 
         Returns
         -------
         float
-          :math:`Pr(o|s', a)`, the probability of joint observation `o` given the joint
-          action `a` was performed and the environment ended up in state `s'`.
+            :math:`Pr(o|s', a)`, the probability of joint observation `o` given the
+            joint action `a` was performed and the environment ended up in state `s'`.
 
         """
 
     @abc.abstractmethod
     def reward_fn(
         self, state: StateType, actions: Dict[str, ActType]
     ) -> Dict[str, float]:
@@ -403,23 +408,23 @@
         The reward function :math:`R(s, a) \rightarrow \mathbf{R}^n` where `n` is the
         number of agents, defines the reward each agent receives given joint action
         `a` was performed in state `s`.
 
         Arguments
         ---------
         state : StateType
-          the state the environment was in
+            the state the environment was in
         actions : Dict[str, ActType]
-          the joint action performed
+            the joint action performed
 
         Returns
         -------
         Dict[str, float]
-          The reward each agent receives given joint action `a` was performed in state
-          `s`.
+            The reward each agent receives given joint action `a` was performed in
+            state `s`.
 
         """
 
 
 class Outcome(enum.Enum):
     """An enum for final episode Outcome of an agent.
 
@@ -439,8 +444,7 @@
     LOSS = -1
     DRAW = 0
     WIN = 1
     NA = None
 
     def __str__(self):
         return self.name
-        return self.name
```

### Comparing `posggym-0.5.1/posggym/utils/env_checker.py` & `posggym-0.6.0/posggym/utils/env_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,43 +9,46 @@
   (https://github.com/DLR-RM/stable-baselines3/). Original Author: Antonin Raffin.
 - warnings/assertions from the PettingZoo repository hosted on GitHub
   (https://github.com/PettingZoo-Team/PettingZoo). Original Author: J K Terry/.
 
 These projects are covered by the MIT License.
 
 """
+
 import inspect
 from copy import deepcopy
 
 import posggym
 from posggym import error, logger
 from posggym.utils.passive_env_checker import (
-    check_rng_equality,
-    data_equivalence,
     check_agent_action_spaces,
     check_agent_observation_spaces,
     check_agent_space_limits,
     check_reset_obs,
+    check_rng_equality,
+    data_equivalence,
     env_render_passive_checker,
     env_reset_passive_checker,
     env_step_passive_checker,
 )
 
 
 def check_reset_seed(env: posggym.Env):
     """Check that the environment can be reset with a seed.
 
     Arguments
     ---------
-    env: The environment to check
+    env
+        The environment to check
 
     Raises
     ------
-    AssertionError: The environment cannot be reset with a random seed,
-        even though `seed` or `kwargs` appear in the signature.
+    AssertionError
+        The environment cannot be reset with a random seed, even though `seed` or
+        `kwargs` appear in the signature.
 
     """
     signature = inspect.signature(env.reset)
     if "seed" in signature.parameters or (
         "kwargs" in signature.parameters
         and signature.parameters["kwargs"].kind is inspect.Parameter.VAR_KEYWORD
     ):
@@ -123,20 +126,22 @@
 
 
 def check_reset_options(env: posggym.Env):
     """Check that the environment can be reset with options.
 
     Arguments
     ---------
-    env: The environment to check
+    env
+        The environment to check
 
     Raises
     ------
-    AssertionError: The environment cannot be reset with options, even though
-        `options` or `kwargs` appear in the signature.
+    AssertionError
+        The environment cannot be reset with options, even though `options` or `kwargs`
+        appear in the signature.
 
     """
     signature = inspect.signature(env.reset)
     if "options" in signature.parameters or (
         "kwargs" in signature.parameters
         and signature.parameters["kwargs"].kind is inspect.Parameter.VAR_KEYWORD
     ):
@@ -156,19 +161,21 @@
 
 
 def check_reset_return_type(env: posggym.Env):
     """Checks that :meth:`reset` correctly returns a tuple of the form `(obs , info)`.
 
     Arguments
     ---------
-    env: The environment to check
+    env
+        The environment to check
 
     Raises
     ------
-    AssertionError depending on spec violation
+    AssertionError
+        depending on spec violation
 
     """
     result = env.reset()
     assert isinstance(result, tuple), (
         "The result returned by `env.reset()` was not a tuple of the form "
         "`(obs, info)`, where `obs` is a observation and `info` is a dictionary "
         f"containing additional information. Actual type: `{type(result)}`"
@@ -188,24 +195,21 @@
 def check_env(env: posggym.Env, skip_render_check: bool = False):
     """Check that an environment follows posggym API.
 
     This is an invasive function that calls the environment's reset and step.
 
     This is particularly useful when using a custom environment.
 
-    TODO Update links
-
-    Please take a look at https://gymnasium.farama.org/content/environment_creation/
-    for more information about the API.
-
     Arguments
     ---------
-    env: The posggym environment that will be checked
-    skip_render_check: Whether to skip the checks for the render method.
-        True by default (useful for the CI)
+    env
+        The posggym environment that will be checked
+    skip_render_check
+        Whether to skip the checks for the render method. True by default (useful for
+        the CI)
 
     """
     more_info_msg = "See COMING SOON for more info."
 
     assert isinstance(
         env, posggym.Env
     ), f"The environment must inherit from the posggym.Env class. {more_info_msg}"
```

### Comparing `posggym-0.5.1/posggym/utils/history.py` & `posggym-0.6.0/posggym/utils/history.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Utilities for storing and managing agent action-observation histories."""
-from typing import Generic, List, Optional, Tuple
+from typing import Dict, Generic, List, Optional, Tuple
 
 import posggym.model as M
 
 
 class AgentHistory(Generic[M.ActType, M.ObsType]):
     """An Action-Observation history for a single agent in a POSG environment.
 
     A History is an ordered Tuple of (Action, Observation) tuples with one
-    entry for each time step in the environment
+    entry for each time step in the environment.
     """
 
     def __init__(
         self, history: Tuple[Tuple[Optional[M.ActType], Optional[M.ObsType]], ...]
     ):
         self.history = history
         self.t = len(history) - 1
@@ -94,77 +94,73 @@
             return self.history[self._idx - 1]
         raise StopIteration
 
 
 class JointHistory:
     """A joint history for all agents in the environment."""
 
-    def __init__(self, agent_histories: Tuple[AgentHistory, ...]):
+    def __init__(self, agent_histories: Dict[str, AgentHistory]):
         self.agent_histories = agent_histories
+        self.agent_ids = sorted(agent_histories.keys())
         self.num_agents = len(self.agent_histories)
 
     @classmethod
     def get_init_history(
-        cls, num_agents: int, obs: Optional[Tuple[Optional[M.ObsType], ...]] = None
+        cls, agent_ids: List[str], obs: Optional[Dict[str, M.ObsType]] = None
     ) -> "JointHistory":
         """Get Initial joint history."""
         if obs is None:
-            return cls(
-                tuple(AgentHistory.get_init_history() for _ in range(num_agents))
-            )
-        return cls(
-            tuple(AgentHistory.get_init_history(obs[i]) for i in range(num_agents))
-        )
+            return cls({i: AgentHistory.get_init_history() for i in agent_ids})
+        return cls({i: AgentHistory.get_init_history(obs[i]) for i in agent_ids})
 
-    def get_agent_history(self, agent_id: int) -> AgentHistory:
+    def get_agent_history(self, agent_id: str) -> AgentHistory:
         """Get the history of given agent."""
         return self.agent_histories[agent_id]
 
     def extend(
-        self, action: Tuple[M.ActType, ...], obs: Tuple[M.ObsType, ...]
+        self, action: Dict[str, M.ActType], obs: Dict[str, M.ObsType]
     ) -> "JointHistory":
         """Extend the current history with given action, observation pair."""
-        new_agent_histories = []
-        for i in range(self.num_agents):
-            new_agent_histories.append(
-                self.agent_histories[i].extend(action[i], obs[i])
-            )
-        return JointHistory(tuple(new_agent_histories))
+        new_agent_histories = {
+            i: self.agent_histories[i].extend(action[i], obs[i]) for i in self.agent_ids
+        }
+        return JointHistory(new_agent_histories)
 
     def get_sub_history(self, horizon: int) -> "JointHistory":
         """Get a subset of history up to given horizon."""
-        sub_agent_histories = []
-        for i in range(self.num_agents):
-            sub_agent_histories.append(self.agent_histories[i].get_sub_history(horizon))
-        return JointHistory(tuple(sub_agent_histories))
+        sub_agent_histories = {
+            i: self.agent_histories[i].get_sub_history(horizon) for i in self.agent_ids
+        }
+        return JointHistory(sub_agent_histories)
 
     def get_history_tm1(self) -> "JointHistory":
         """Get history at time t-1."""
-        sub_agent_histories: List[AgentHistory] = []
-        for i in range(self.num_agents):
-            sub_agent_histories.append(AgentHistory(self.agent_histories[i][:-1]))
-        return JointHistory(tuple(sub_agent_histories))
+        sub_agent_histories = {
+            i: AgentHistory(self.agent_histories[i][:-1]) for i in self.agent_ids
+        }
+        return JointHistory(sub_agent_histories)
 
     def __len__(self) -> int:
-        return len(self.agent_histories[0])
+        return len(self.agent_histories[self.agent_ids[0]])
 
     def __hash__(self):
-        return hash(self.agent_histories)
+        return hash(tuple(self.agent_histories[i] for i in self.agent_ids))
 
     def __eq__(self, other):
         if not isinstance(other, JointHistory):
             return False
         return self.agent_histories == other.agent_histories
 
     def __getitem__(self, key):
-        actions = tuple(h[key][0] for h in self.agent_histories)
-        obs = tuple(h[key][1] for h in self.agent_histories)
+        # get actions and observations at time step key
+        actions = {i: h[key][0] for i, h in self.agent_histories.items()}
+        obs = {i: h[key][1] for i, h in self.agent_histories.items()}
         return actions, obs
 
     def __str__(self):
-        h_str = [f"{i} {h}" for i, h in enumerate(self.agent_histories)]
+        h_str = [f"{i} {h}" for i, h in self.agent_histories.items()]
         h_str.insert(0, "<JointHistory:")
         h_str.append(">")
         return "\n".join(h_str)
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `posggym-0.5.1/posggym/utils/model_checker.py` & `posggym-0.6.0/posggym/utils/model_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   (https://github.com/DLR-RM/stable-baselines3/). Original Author: Antonin Raffin.
 - warnings/assertions from the PettingZoo repository hosted on GitHub
   (https://github.com/PettingZoo-Team/PettingZoo). Original Author: J K Terry/.
 
 These projects are covered by the MIT License.
 
 """
+
 import inspect
 from copy import deepcopy
 from typing import Optional
 
 import posggym.model as M
 from posggym import logger
 from posggym.utils.passive_env_checker import (
@@ -28,49 +29,55 @@
     check_state,
     check_state_space,
     data_equivalence,
     model_step_passive_checker,
 )
 
 
-def check_initial_state_type(model: M.POSGModel):
+def check_initial_state_type(model: M.POSGModel) -> M.StateType:
     """Checks that :meth:`sample_initial_state` correctly returns a valid state.
 
     Arguments
     ---------
-    model: The model to check
+    model
+        The model to check
 
     Returns
     -------
-    state: sampled initial state
+    state
+        sampled initial state
 
     Raises
     ------
-    AssertionError depending on spec violation
+    AssertionError
+        depending on spec violation
 
     """
     state = model.sample_initial_state()
     check_state(state, model)
     return state
 
 
 def check_initial_obs_type(model: M.POSGModel, state: Optional[M.StateType] = None):
     """Checks that :meth:`sample_initial_obs` works correctly.
 
     Assumes ``model.sample_initial_state()`` works as expected.
 
     Arguments
     ---------
-    model: the model to check
-    state: the state to use for check, default is None in which case a new state is
-           sampled from the model.
+    model
+        the model to check
+    state
+        the state to use for check, default is None in which case a new state is
+        sampled from the model.
 
     Raises
     ------
-    AssertionError depending on spec violation
+    AssertionError
+        depending on spec violation
 
     """
     if state is None:
         state = model.sample_initial_state()
 
     try:
         obs = model.sample_initial_obs(state)
@@ -82,19 +89,21 @@
 
 
 def check_initial_sampling_seed(model: M.POSGModel):
     """Check that model seeding works correctly for initial conditions.
 
     Arguments
     ---------
-    model: The environment model to check
+    model
+        The environment model to check
 
     Raises
     ------
-    AssertionError: The model random seeding doesn't work as expected.
+    AssertionError
+        The model random seeding doesn't work as expected.
 
     """
     signature = inspect.signature(model.seed)
     assert "seed" in signature.parameters or (
         "kwargs" in signature.parameters
         and signature.parameters["kwargs"].kind is inspect.Parameter.VAR_KEYWORD
     ), "The `seed` method does not provide a `seed` or `**kwargs` keyword argument."
@@ -180,22 +189,18 @@
 def check_model(model: M.POSGModel):
     """Check that an environment model follows posggym API.
 
     This is an invasive function that calls the models step.
 
     This is particularly useful when using a custom environment.
 
-    TODO Update links
-
-    Please take a look at https://gymnasium.farama.org/content/environment_creation/
-    for more information about the API.
-
     Arguments
     ---------
-    model: The posggym environment model that will be checked
+    model
+        The posggym environment model that will be checked
 
     """
     more_info_msg = (
         "For more info see: "
         "https://posggym.readthedocs.io/en/latest/tutorials/environment_creation.html."
     )
     assert isinstance(
```

### Comparing `posggym-0.5.1/posggym/utils/passive_env_checker.py` & `posggym-0.6.0/posggym/utils/passive_env_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """A set of functions for passively checking environment implementations.
 
 This module is heavily based on the passive_env_checker from gymnasium. It's copied and
 adapted here to ensure compatibility across different gymnasium versions:
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/utils/passive_env_checker.py
 
 """
+
 import inspect
 import random
 from functools import partial
 from typing import Callable, Dict, Optional, Sequence
 
 import numpy as np
 from gymnasium import Space, spaces
@@ -20,20 +21,23 @@
 
 
 def data_equivalence(data_1, data_2) -> bool:
     """Assert equality between data 1 and 2, i.e observations, actions, info.
 
     Arguments
     ---------
-    data_1: data structure 1
-    data_2: data structure 2
+    data_1
+        data structure 1
+    data_2
+        data structure 2
 
     Returns
     -------
-    bool: If observation 1 and 2 are equivalent
+    bool
+        If observation 1 and 2 are equivalent
 
     """
     if type(data_1) == type(data_2):
         if isinstance(data_1, dict):
             return data_1.keys() == data_2.keys() and all(
                 data_equivalence(data_1[k], data_2[k]) for k in data_1
             )
@@ -306,30 +310,35 @@
 
 
 def check_state(state: M.StateType, model: M.POSGModel):
     """Check state is valid.
 
     Arguments
     ---------
-    state: the state to check
-    model: the environment model
+    state
+        the state to check
+    model
+        the environment model
 
     """
     if model.state_space is not None:
         assert model.state_space.contains(state)
 
 
 def check_obs(obs, observation_space: spaces.Space, method_name: str):
     """Check the observation returned by the environment correspond to the declared one.
 
     Arguments
     ---------
-    obs: The observation to check
-    observation_space: The observation space of the observation
-    method_name: The method name that generated the observation
+    obs
+        The observation to check
+    observation_space
+        The observation space of the observation
+    method_name
+        The method name that generated the observation
 
     """
     pre = f"The obs returned by the `{method_name}()` method"
     if isinstance(observation_space, spaces.Discrete):
         if not isinstance(obs, (np.int64, int)):
             logger.warn(f"{pre} should be an int or np.int64, actual type: {type(obs)}")
     elif isinstance(observation_space, spaces.Box):
@@ -377,33 +386,38 @@
     observation_spaces: Dict[str, Space],
     method_name: str,
 ):
     """Check that each agent's observation returned by the environment is valid.
 
     Arguments
     ---------
-    obs: The observation for each agent to check
-    observation_spaces: The observation spaces for each agent's observation
-    method_name: The method name that generated the observation
+    obs
+        The observation for each agent to check
+    observation_spaces
+        The observation spaces for each agent's observation
+    method_name
+        The method name that generated the observation
 
     """
     for i, obs_i in obs.items():
         try:
             check_obs(obs_i, observation_spaces[i], method_name)
         except AssertionError as e:
             raise AssertionError("Invalid observation for agent `{i}`.") from e
 
 
 def check_reset_obs(obs: Dict[str, M.ObsType], model: M.POSGModel):
     """Check agent observations returned by the environment `reset()` method are valid.
 
     Arguments
     ---------
-    obs: The observation for each agent to check
-    model: The environment model
+    obs
+        The observation for each agent to check
+    model
+        The environment model
 
     """
     assert isinstance(obs, dict), (
         "Expected observation from `env.reset()` to be a dictionary, mapping agent IDs "
         " to agent obs."
     )
     for i, o_i in obs.items():
@@ -465,27 +479,29 @@
             f"actual type: {type(info)}"
         )
     return result
 
 
 def _check_agent_dict(
     agent_dict,
-    possible_agents: Sequence[str],
+    possible_agents: Optional[Sequence[str]],
     dict_type: str,
     expected_agents: Optional[Sequence[str]] = None,
 ):
     assert isinstance(agent_dict, dict), (
         f"Agent {dict_type} dictionary  must be a dictionary mapping agentID to values."
         f"Actual type: {type(agent_dict)}."
     )
-    for i in agent_dict:
-        assert i in possible_agents, (
-            f"Agent {dict_type} dictionary must only contain valid agent IDs: "
-            f"invalid ID `{i}`."
-        )
+    if possible_agents is not None:
+        for i in agent_dict:
+            assert i in possible_agents, (
+                f"Agent {dict_type} dictionary must only contain valid agent IDs: "
+                f"invalid ID `{i}`."
+            )
+
     if expected_agents is not None:
         for i in expected_agents:
             assert (
                 i in agent_dict
             ), f"Expected agent ID `{i}` missing from {dict_type} dictionary."
 
 
@@ -514,15 +530,16 @@
 
     _check_agent_dict(obs, model.possible_agents, "observation", step_agents)
     _check_agent_dict(reward, model.possible_agents, "reward", step_agents)
     _check_agent_dict(terminated, model.possible_agents, "terminated", step_agents)
     _check_agent_dict(truncated, model.possible_agents, "truncated", step_agents)
     # Less strict on checking there are entries for all agents in info values
     # as these are not functionally critical and are more for record keeping
-    _check_agent_dict(info, model.possible_agents, "info")
+    # Also less strict on possible agents and allow extra information in the dictionary.
+    _check_agent_dict(info, None, "info", None)
 
     check_state(next_state, model)
     check_agent_obs(obs, model.observation_spaces, "step")
 
     if not all(isinstance(t_i, (bool, np.bool_)) for t_i in terminated.values()):
         logger.warn(
             "Expects `terminated` signal to be a boolean for every agent, "
```

### Comparing `posggym-0.5.1/posggym/utils/seeding.py` & `posggym-0.6.0/posggym/utils/seeding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Random number generator functions.
 
 Ref:
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/utils/seeding.py
 
 """
+
 import random
 from typing import Optional, Tuple, Union
 
 import numpy as np
 
 from posggym import error
 
@@ -16,24 +17,28 @@
 
 
 def np_random(seed: Optional[int] = None) -> Tuple[np.random.Generator, int]:
     """Create a numpy random number generator.
 
     Arguments
     ---------
-    seed : the seed used to create the generator.
+    seed : int, optional
+        the seed used to create the generator.
 
     Returns
     -------
-    rng : the random number generator
-    seed : the seed used for the rng (will equal argument seed if one is provided.)
+    rng : np.random.Generator
+        the random number generator
+    seed : int
+        the seed used for the rng (will equal argument seed if one is provided.)
 
     Raises
     ------
-    Error: if seed is not None or a non-negative integer.
+    Error
+        if seed is not None or a non-negative integer.
 
     """
     if seed is not None and not (isinstance(seed, int) and seed >= 0):
         if isinstance(seed, int) is False:
             raise error.Error(
                 f"Seed must be a python integer, actual type: {type(seed)}"
             )
@@ -51,24 +56,28 @@
 
 
 def std_random(seed: Optional[int] = None) -> Tuple[random.Random, int]:
     """Create random number generator using python built-in `random.Random`.
 
     Arguments
     ---------
-    seed : the seed used to create the generator.
+    seed : int, optional
+        the seed used to create the generator.
 
     Returns
     -------
-    rng : the random number generator
-    seed : the seed used for the rng (will equal argument seed if one is provided.)
+    rng : random.Random
+        the random number generator
+    seed : int
+        the seed used for the rng (will equal argument seed if one is provided.)
 
     Raises
     ------
-    Error: if seed is not None or a non-negative integer.
+    Error
+        if seed is not None or a non-negative integer.
 
     """
     if seed is not None and not (isinstance(seed, int) and seed >= 0):
         if isinstance(seed, int) is False:
             raise error.Error(
                 f"Seed must be a python integer, actual type: {type(seed)}"
             )
```

### Comparing `posggym-0.5.1/posggym/vector/sync_vector_env.py` & `posggym-0.6.0/posggym/vector/sync_vector_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Synchronized vectorized environment class.
 
 Based on Gymnasium Vectorized Environments:
 https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/vector/vector_env.py
 https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/vector/sync_vector_env.py
 
 """
+
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any, Callable, Dict, Iterable, List, Tuple
 
 import numpy as np
 from gymnasium.vector.utils import concatenate, create_empty_array
@@ -58,17 +59,17 @@
         env_fns: Iterable[Callable[[], posggym.Env]],
         copy: bool = True,
     ):
         """Initialize the vectorized environment.
 
         Arguments
         ---------
-        env_fns:
+        env_fns
             iterable of callable functions that create the environments.
-        copy:
+        copy
             If ``True``, then the :meth:`reset` and :meth:`step` methods return a
             copy of the observations.
 
         """
         self.env_fns = env_fns
         self.envs = [fn() for fn in env_fns]
         self.copy = copy
@@ -156,40 +157,40 @@
         If any environment is done, then it is reset before taking the next step. The
         final observation and info of the previous environment is stored in the info
         dictionary under the keys ``final_observation`` and ``final_info``.
 
 
         Arguments
         ---------
-        actions:
+        actions
             dict mapping agent ID to batch of actions for that agent, with one action
             for each environment. So should be a dict of arrays or lists, with each
             array/list having length equal to the number of environments.
 
         Returns
         -------
-        observations:
+        observations
             dict mapping agent ID to batch of observations for that agent, with one
             observation for each environment. Each array having shape
             ``(num_envs,) + observation_space.shape``.
-        rewards:
+        rewards
             dict mapping agent ID to batch of rewards for that agent, with one reward
             for each environment. Each entry is an array with  shape ``(num_envs,)``.
-        terminateds:
+        terminateds
             dict mapping agent ID to batch of termination signals for that agent, with
             one termination signal for each environment. Each entry is an array with
             shape ``(num_envs,)``.
-        truncateds:
+        truncateds
             dict mapping agent ID to batch of truncation signals for that agent, with
             one truncation signal for each environment. Each entry is an array with
             shape ``(num_envs,)``.
-        all_dones:
+        all_dones
             array of booleans, with one entry for each environment, indicating whether
             the environment is done. Shape is ``(num_envs,)``.
-        infos:
+        infos
             dict mapping agent ID to batch of info objects for that agent, with one
             info object for each environment. Each entry is a dict with one entry for
 
 
         The batched environment step results.
 
         """
@@ -280,24 +281,24 @@
         Given the `info` of a single environment add it to the `infos` dictionary
         which represents all the infos of the vectorized environment.
         Every `key` of `info` is paired with a boolean mask `_key` representing
         whether or not the i-indexed environment has this `info`.
 
         Arguments:
         ----------
-        infos: dict
+        infos
             the infos of the vectorized environment
-        info: dict
+        info
             the info coming from the single environment
-        env_num: int
+        env_num
             the index of the single environment
 
         Returns
         -------
-        infos: dict
+        infos
             the (updated) infos of the vectorized environment
 
         """
         for k in info:
             if k not in infos:
                 info_array, array_mask = self._init_info_arrays(type(info[k]))
             else:
@@ -313,22 +314,22 @@
         Initialize the info array. If the dtype is numeric the info array will have the
         same dtype, otherwise will be an array of `None`. Also, a boolean array of the
         same length is returned. It will be used for assessing which environment has
         info data.
 
         Arguments
         ---------
-        dtype: type
+        dtype
             data type of the info coming from the env.
 
         Returns
         -------
-        array: np.ndarray
+        array
             the initialized info array.
-        array_mask: np.ndarray
+        array_mask
             the initialized boolean array.
 
         """
         if dtype in [int, float, bool] or issubclass(dtype, np.number):
             array = np.zeros(self.num_envs, dtype=dtype)
         else:
             array = np.zeros(self.num_envs, dtype=object)
```

### Comparing `posggym-0.5.1/posggym/wrappers/__init__.py` & `posggym-0.6.0/posggym/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/discretize_actions.py` & `posggym-0.6.0/posggym/wrappers/discretize_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper to discretize continuous actions."""
+
 from typing import Dict, Sequence, Union, cast
 
 import numpy as np
 from gymnasium import spaces
 
 from posggym import ActionWrapper, Env
 
@@ -19,16 +20,16 @@
     ---------
     env : posggym.Env
         The environment to apply the wrapper
     num_actions : int
         The number of actions to discretize space into. For multi-dimensional
         continuous spaces each dimension will be discretized into this many actions.
     flatten : bool
-       Whether to flatten action space into one-dimensional discrete space, or keep
-       number of dimensions of the original action space.
+        Whether to flatten action space into one-dimensional discrete space, or keep
+        number of dimensions of the original action space.
 
     """
 
     def __init__(self, env: Env, num_actions: int, flatten: bool = False):
         super().__init__(env)
         assert all(
             isinstance(act_space, spaces.Box)
```

### Comparing `posggym-0.5.1/posggym/wrappers/env_checker.py` & `posggym-0.6.0/posggym/wrappers/env_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A passive environment checker wrapper for an environment."""
+
 from typing import Dict
 
 import posggym
 import posggym.model as M
 from posggym.utils.passive_env_checker import (
     check_agent_action_spaces,
     check_agent_observation_spaces,
```

### Comparing `posggym-0.5.1/posggym/wrappers/flatten_observations.py` & `posggym-0.6.0/posggym/wrappers/flatten_observations.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/monitoring/video_recorder.py` & `posggym-0.6.0/posggym/wrappers/monitoring/video_recorder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Classes for recording videos of episodes.
 
 Ref:
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/wrappers/monitoring/video_recorder.py
 
 """
+
 import json
-import os
-import os.path
 import tempfile
+from pathlib import Path
 from typing import Dict, List, Optional
 
 from posggym import Env, error, logger
 
 
 class VideoRecorder:
     """VideoRecorder renders a nice movie of a rollout, frame by frame.
@@ -31,49 +31,50 @@
     """
 
     combatible_render_modes = ["rgb_array", "rgb_array_dict"]
 
     def __init__(
         self,
         env: Env,
-        path: Optional[str] = None,
+        path: Optional[Path] = None,
         metadata: Optional[Dict] = None,
         enabled: bool = True,
-        base_path: Optional[str] = None,
+        base_path: Optional[Path] = None,
         disable_logger: bool = False,
-        resize: Optional[int] = None,
     ):
         """Video recorder renders a nice movie of a rollout, frame by frame.
 
         Arguments
         ---------
-        env: Environment to take video of.
-        path: Path to the video file; will be randomly chosen if omitted.
-        metadata: Contents to save to the metadata file.
-        enabled: Whether to actually record video, or just no-op (for convenience)
-        base_path: Alternatively, path to the video file without extension, which will
+        env : posggym.Env
+            Environment to take video of.
+        path : Path, optional
+            Path to the video file; will be randomly chosen if omitted.
+        metadata : Dict, optional
+            Contents to save to the metadata file.
+        enabled : bool
+            Whether to actually record video, or just no-op (for convenience)
+        base_path : Path, optional
+            Alternatively, path to the video file without extension, which will
             be added.
-        disable_logger: Whether to disable moviepy logger or not.
-        resize: If not None, resize the video to the given dimensions (will resize
-            the width to given number of pixels with the height computed automatically
-            to conserve the width/height dimension).
+        disable_logger : bool
+            Whether to disable moviepy logger or not.
 
         """
         try:
             # check that moviepy is now installed
             import moviepy  # noqa
         except ImportError as e:
             raise error.DependencyNotInstalled(
                 "MoviePy is not installed, run `pip install moviepy`"
             ) from e
 
         self._async = env.metadata.get("semantics.async")
         self.enabled = enabled
         self.disable_logger = disable_logger
-        self.resize = resize
         self._closed = False
 
         self.render_history: List = []
         self.env = env
 
         self.render_mode = env.render_mode
 
@@ -96,22 +97,24 @@
         self.last_frame = None
         self.env = env
 
         required_ext = ".mp4"
         if path is None:
             if base_path is not None:
                 # Base path given, append ext
-                path = base_path + required_ext
+                path = base_path.with_suffix(required_ext)
             else:
                 # Otherwise, just generate a unique filename
                 with tempfile.NamedTemporaryFile(suffix=required_ext) as f:
-                    path = f.name
+                    path = Path(f.name)
+
         self.path = path
 
-        path_base, actual_ext = os.path.splitext(self.path)
+        path_base = self.path.with_suffix("")
+        actual_ext = self.path.suffix
 
         if actual_ext != required_ext:
             raise error.Error(
                 f"Invalid path given: {self.path} -- must have file extension "
                 f"{required_ext}."
             )
 
@@ -184,27 +187,23 @@
         if not self.enabled or self._closed:
             # mark as closed in case it is broken to save future warnings
             self._closed = True
             return
 
         if len(self.recorded_frames) > 0:
             try:
-                from moviepy.video.fx.resize import resize
                 from moviepy.video.io.ImageSequenceClip import ImageSequenceClip
             except ImportError as e:
                 raise error.DependencyNotInstalled(
                     "MoviePy is not installed, run `pip install moviepy`"
                 ) from e
 
             clip = ImageSequenceClip(self.recorded_frames, fps=self.frames_per_sec)
             moviepy_logger = None if self.disable_logger else "bar"
-            if self.resize is not None:
-                clip = resize(clip, width=self.resize)
-
-            clip.write_videofile(self.path, logger=moviepy_logger)
+            clip.write_videofile(str(self.path), logger=moviepy_logger)
         else:
             # No frames captured. Set metadata.
             if self.metadata is None:
                 self.metadata = {}
             self.metadata["empty"] = True
 
         self.write_metadata()
```

### Comparing `posggym-0.5.1/posggym/wrappers/order_enforcing.py` & `posggym-0.6.0/posggym/wrappers/order_enforcing.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/petting_zoo.py` & `posggym-0.6.0/posggym/wrappers/petting_zoo.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/record_episode_statistics.py` & `posggym-0.6.0/posggym/wrappers/record_episode_statistics.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/record_video.py` & `posggym-0.6.0/posggym/wrappers/record_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Wrapper for recording videos of an environment.
 
 Ref
 https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/wrappers/record_video.py
 
 """
-import os
-from typing import Callable, Optional
+
+from pathlib import Path
+from typing import Callable, Optional, Union
 
 from posggym import logger
 from posggym.core import Env, Wrapper
 from posggym.wrappers.monitoring.video_recorder import VideoRecorder
 
 
 def capped_cubic_video_schedule(episode_id: int) -> bool:
@@ -18,20 +19,20 @@
     Triggers recording of episodes numbers that are perfect cubes :math:`k^3` up to
     the 1000th episode, then every 1000 episodes after that:
     0, 1, 8, 27, 64, 125, 216, 343, 512, 729, 1000, 2000, 3000, ...
 
     Arguments
     ---------
     episode_id: int
-      The episode number
+        The episode number
 
     Returns
     -------
     bool
-      Whether to record episode or not.
+        Whether to record episode or not.
 
     """
     if episode_id < 1000:
         return int(round(episode_id ** (1.0 / 3))) ** 3 == episode_id
     else:
         return episode_id % 1000 == 0
 
@@ -54,61 +55,58 @@
     video_length: int
         The length of recorded episodes. If 0, entire episodes are recorded. Otherwise,
         snippets of the specified length are captured
     name_prefix: str, optional
         Will be prepended to the filename of the recordings
     disable_logger: bool
         Whether to disable moviepy logger or not.
-    resize: Optional[int]
-        If not None, resize the video to the given dimensions (will resize the width to
-        given number of pixels with the height computed automatically to conserve the
-        width/height dimension).
 
     Note
     ----
     This implementation is based on the gymnasium.wrappers.RecordVideo (version
     gymnasium 0.27) wrapper, adapted here to work with posggym's multiagent environment:
     https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/wrappers/record_video.py
 
     """
 
     def __init__(
         self,
         env: Env,
-        video_folder: str,
+        video_folder: Union[Path, str],
         episode_trigger: Optional[Callable[[int], bool]] = None,
         step_trigger: Optional[Callable[[int], bool]] = None,
         video_length: int = 0,
         name_prefix: str = "posggym-video",
         disable_logger: bool = False,
-        resize: Optional[int] = None,
     ):
         super().__init__(env)
 
         if episode_trigger is None and step_trigger is None:
             episode_trigger = capped_cubic_video_schedule
 
         trigger_count = sum(x is not None for x in [episode_trigger, step_trigger])
         assert trigger_count == 1, "Must specify exactly one trigger"
 
         self.episode_trigger = episode_trigger
         self.step_trigger = step_trigger
         self.video_recorder: Optional[VideoRecorder] = None
         self.disable_logger = disable_logger
-        self.resize = resize
 
-        self.video_folder = os.path.abspath(video_folder)
+        if isinstance(video_folder, str):
+            video_folder = Path(video_folder)
+
+        self.video_folder = video_folder
         # Create output folder if needed
-        if os.path.isdir(self.video_folder):
+        if self.video_folder.is_dir():
             logger.warn(
                 f"Overwriting existing videos at {self.video_folder} folder (try "
                 "specifying a different `video_folder` for the `RecordVideo` wrapper "
                 "if this is not desired)"
             )
-        os.makedirs(self.video_folder, exist_ok=True)
+        self.video_folder.mkdir(exist_ok=True)
 
         self.name_prefix = name_prefix
         self.video_length = video_length
         self.step_id = 0
         self.episode_id = 0
 
         self.recording = False
@@ -188,21 +186,20 @@
         """Starts video recorder."""
         self.close_video_recorder()
 
         video_name = f"{self.name_prefix}-step-{self.step_id}"
         if self.episode_trigger:
             video_name = f"{self.name_prefix}-episode-{self.episode_id}"
 
-        base_path = os.path.join(self.video_folder, video_name)
+        base_path = self.video_folder / video_name
         self.video_recorder = VideoRecorder(
             env=self.env,
             base_path=base_path,
             metadata={"step_id": self.step_id, "episode_id": self.episode_id},
             disable_logger=self.disable_logger,
-            resize=self.resize,
         )
 
         self.video_recorder.capture_frame()
         self.recorded_frames = 1
         self.recording = True
 
     def close_video_recorder(self):
```

### Comparing `posggym-0.5.1/posggym/wrappers/rescale_actions.py` & `posggym-0.6.0/posggym/wrappers/rescale_actions.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/rescale_observations.py` & `posggym-0.6.0/posggym/wrappers/rescale_observations.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/rllib_env.py` & `posggym-0.6.0/posggym/wrappers/rllib_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper for converting a posggym environment into rllib multi-agent environment."""
+
 import warnings
 from typing import Optional, Set, Tuple
 
 from gymnasium import spaces
 
 import posggym
 
@@ -82,23 +83,33 @@
         MultiAgentDict, MultiAgentDict, MultiAgentDict, MultiAgentDict, MultiAgentDict
     ]:
         """Returns observations from ready agents.
 
         The returns are dicts mapping from agent_id strings to values. The
         number of agents in the env can vary over time.
 
+        Arguments
+        ---------
+        action_dict : MultiAgentDict
+            action for each agent
+
         Returns
         -------
-        observations: new observations for each ready agent
-        rewards: reward values for each ready agent. If the episode is just started, the
+        observations : MultiAgentDict
+            new observations for each ready agent
+        rewards : MultiAgentDict
+            reward values for each ready agent. If the episode is just started, the
             value will be None.
-        terminateds: terminated values for each ready agent. The special key "__all__"
+        terminateds : MultiAgentDict
+            terminated values for each ready agent. The special key "__all__"
             (required) is used to indicate env termination.
-        truncateds: truncated values for each ready agent.
-        infos: info values for each agent id (may be empty dicts).
+        truncateds : MultiAgentDict
+            truncated values for each ready agent.
+        infos : MultiAgentDict
+            info values for each agent id (may be empty dicts).
 
         """
         obs, rewards, terminated, truncated, all_done, info = self.env.step(action_dict)
 
         # remove obs for already done agents, since pettingzoo expects no output for
         # agents that were terminated or truncated in a previous step
         for d in (obs, rewards, terminated, truncated, info):
```

### Comparing `posggym-0.5.1/posggym/wrappers/stack.py` & `posggym-0.6.0/posggym/wrappers/stack.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/posggym/wrappers/time_limit.py` & `posggym-0.6.0/posggym/wrappers/time_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper for limiting the time steps of an environment."""
+
 from typing import Optional, Set
 
 import posggym
 
 
 class TimeLimit(posggym.Wrapper):
     """Wraps environment to enforce environment time limit.
@@ -11,18 +12,18 @@
     agents that have not already reached a terminal state by the time a maximum number
     of timesteps is exceeded. It will also signal that the episode is `done` for all
     agents.
 
     Arguments
     ---------
     env : posggym.Env
-      The environment to apply the wrapper
+        The environment to apply the wrapper
     max_episode_steps : int, optional
-      The maximum length of episode before it is truncated. If None then will not
-      truncate episodes.
+        The maximum length of episode before it is truncated. If None then will not
+        truncate episodes.
 
     Note
     ----
     This implementation is based on the similar Gymnasium wrapper:
     https://github.com/Farama-Foundation/Gymnasium/blob/v0.27.0/gymnasium/wrappers/time_limit.py
 
     """
```

### Comparing `posggym-0.5.1/posggym.egg-info/PKG-INFO` & `posggym-0.6.0/posggym.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: posggym
-Version: 0.5.1
-Summary: A collection of diverse environments and reference agents for reinforcement learning and planning research in Partially Observable Stochastic Games (POSGs). .
+Version: 0.6.0
+Summary: A library for planning and reinforcement learning research in partially observable, multi-agent environments.
 Author-email: Jonathon Schwartz <jonathon.schwartz@anu.edu.au>
 License: MIT License
 Project-URL: Homepage, https://github.com/RDLLab/posggym
 Project-URL: Repository, https://github.com/RDLLab/posggym/
 Project-URL: Documentation, https://posggym.readthedocs.io/
 Project-URL: Bug Report, https://github.com/RDLLab/posggym/issues
 Keywords: multiagent-systems,reinforcement-learning,planning,gymnasium,POSG
@@ -21,86 +21,63 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gymnasium>=0.26
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: importlib-metadata>=4.8.0; python_version < "3.10"
-Provides-Extra: grid-world
-Requires-Dist: pygame>=2.0; extra == "grid-world"
-Provides-Extra: continuous
-Requires-Dist: pygame>=2.0; extra == "continuous"
-Requires-Dist: pymunk>=6.0.0; extra == "continuous"
-Provides-Extra: envs-all
-Requires-Dist: pygame>=2.0; extra == "envs-all"
-Requires-Dist: pymunk>=6.0.0; extra == "envs-all"
+Requires-Dist: pygame>=2.0
+Requires-Dist: pymunk>=6.0.0
 Provides-Extra: agents
-Requires-Dist: pygame>=2.0; extra == "agents"
-Requires-Dist: pymunk>=6.0.0; extra == "agents"
 Requires-Dist: types-requests>=2.28; extra == "agents"
 Requires-Dist: requests>=2.28; extra == "agents"
 Requires-Dist: clint>=0.5.1; extra == "agents"
 Requires-Dist: torch>=1.11.0; extra == "agents"
 Provides-Extra: other
 Requires-Dist: moviepy>=1.0.0; extra == "other"
 Requires-Dist: pandas>=1.0; extra == "other"
 Requires-Dist: seaborn>=0.13.0; extra == "other"
 Requires-Dist: matplotlib>=3.0.0; extra == "other"
 Provides-Extra: all
-Requires-Dist: pygame>=2.0; extra == "all"
-Requires-Dist: pymunk>=6.0.0; extra == "all"
 Requires-Dist: types-requests>=2.28; extra == "all"
 Requires-Dist: requests>=2.28; extra == "all"
 Requires-Dist: clint>=0.5.1; extra == "all"
-Requires-Dist: torch>=1.11.0; extra == "all"
+Requires-Dist: torch>=2.0; extra == "all"
 Requires-Dist: moviepy>=1.0.0; extra == "all"
 Requires-Dist: seaborn>=0.11.1; extra == "all"
 Requires-Dist: matplotlib>=3.3.4; extra == "all"
 Requires-Dist: pandas>=1.0; extra == "all"
 Provides-Extra: testing
 Requires-Dist: pytest>=7.2; extra == "testing"
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 # POSGGym
 
-POSGGym is an open source Python library providing implementations of Partially Observable Stochastic Game (POSG) environments coupled with dynamic models of each environment, all under a unified API. While there are a number of amazing open-source implementations for POSG environments, very few have support for dynamic models that can be used for planning, especially for continuous domains. The aim of this library is to fill this gap.
+POSGGym is a Python library for planning and reinforcement learning research in partially observable, multi-agent environments. It provides a collection of discrete and continuous environments along with reference agents to allow for reproducible evaluations. The API aims to mimic that of [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) with the addition of a model API that can be used for planning.
 
-A key goal of POSGGym is to provide easy to use and understand open-source implementations for many of the environments commonly used in the partially observable multi-agent planning literature.
+The documentation for the project is available online at [posggym.readthedocs.io/](https://posggym.readthedocs.io/). For a guide to building the documentation locally see [docs/README.md](docs/README.md).
 
-POSGGym also provides a collection of reference agents for it's various environments and a unified Agents API for using these agents. These agents can be used to evaluate algorithms, and includes both hand-coded bots and agents trained using reinforcement learning.
-
-POSGGym is directly inspired by and adapted from the [Gymnasium](https://gymnasium.farama.org/) and [PettingZoo](https://pettingzoo.farama.org/) libraries for reinforcement learning. The key additions in POSGGym are support for environment models which can be used for planning and reference agents. POSGGym's API aims to stay as close to the Gymnasium and PettingZoo Parallel APIs as possible while incorporating models and agents into the mix.
-
-Any POSGGym environment can be converted into a PettingZoo environment using a simple wrapper (`posggym.wrappers.petting_zoo.PettingZoo`). This allows for easy integration with the ecosystem of libraries that support PettingZoo.
-
-
-## Documentation
-
-The documentation for the project is available at [posggym.readthedocs.io/](https://posggym.readthedocs.io/).
-
-For a guide to building the documentation locally see [docs/README.md](docs/README.md).
+Some baseline implementations of planning and reinforcement learning algorithms for POSGGym are available in the [POSGGym-Baselines](https://github.com/RDLLab/posggym-baselines) library. Compatibility with other popular reinforcement learning libraries is possible using the [PettingZoo wrapper](#compatibility-with-pettingzoo).
 
 ## Installation
 
 POSGGym supports and tests for `Python>=3.8`. We recommend using a virtual environment to install POSGGym (e.g. [conda](https://docs.conda.io/projects/conda/en/latest/index.html), [venv](https://docs.python.org/3/library/venv.html)).
 
 ### Using pip
 
 The latest release version of POSGGym can be installed using `pip` by running:
 
 ```bash
 pip install posggym
 ```
 
-This will install the base dependencies for running the main environments and download the agent models (so may take a few minutes), but but in order to minimise the number of unused dependencies installed may not include all dependencies for all environments or for rendering some environments, and will not include dependencies for running many posggym agents.
-
-You can install all dependencies for a family of environments like `pip install posggym[grid-world]` and `pip install posggym[continuous]` or dependencies for all environments using `pip install posggym[envs-all]`.
+This will install the base dependencies for running all the environments and download the agent models (so may take a few minutes). In order to minimise the number of unused dependencies installed the default install does not include dependencies for running many posggym agents (specifically PyTorch).
 
 You can install dependencies for POSGGym agents using `pip install posggym[agents]` or to install dependencies for all environments and agents use `pip install posggym[all]`.
 
 ### Installing from source
 
 To install POSGGym from source, first clone the repository then run:
 
@@ -114,37 +91,36 @@
 ```bash
 pip install -e .[all]
 ```
 
 To run tests, install the test dependencies and then run the tests:
 
 ```bash
-pip install -e .[test]
+pip install -e .[testing]
 pytest
 ```
 
 Or alternatively you can run one of the examples from the `examples` directory:
 
 ```bash
-python examples/run_random_agents.py --env_id Driving-v0 --num_episodes 10 --render_mode human
+python examples/run_random_agents.py --env_id Driving-v1 --num_episodes 10 --render_mode human
 ```
 
-
 ## Environments
 
 POSGGym includes the following families of environments (for a full list of environments and their descriptsion see the [documentation](https://posggym.readthedocs.io/)).
 
 - [Classic](https://posggym.readthedocs.io/en/latest/environments/classic.html) - These are classic POSG problems from the literature.
 - [Grid-World](https://posggym.readthedocs.io/en/latest/environments/grid_world.html) - These environments are all based in a 2D Gridworld.
 - [Continuous](https://posggym.readthedocs.io/en/latest/environments/continuous.html) - 2D environments with continuous state, actions, and observations.
 
 
 ## Environment API
 
-POSGGym models each environment as a python `env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
+POSGGym models each environment as a python `Env` class. Creating environment instances and interacting with them is very simple, and flows almost identically to the Gymnasium user flow. Here's an example using the `PredatorPrey-v0` environment:
 
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 observations, infos = env.reset(seed=42)
 
 for t in range(100):
@@ -156,19 +132,18 @@
         observations, infos = env.reset()
 
 env.close()
 ```
 
 ## Model API
 
-Every environment provides access to a model of the environment in the form of a python `model` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
+Every environment provides access to a model of the environment in the form of a `POSGModel` class. Each model implements a generative model, which can be used for planning, along with functions for sampling initial states. Some environments also implement a full POSG model including the transition, joint observation and joint reward functions.
 
 The following is an example of accessing and using the environment model:
 
-
 ```python
 import posggym
 env = posggym.make("PredatorPrey-v0")
 model = env.model
 model.seed(seed=42)
 
 state = model.sample_initial_state()
@@ -179,61 +154,73 @@
     state, observations, rewards, terminations, truncations, all_done, infos = model.step(state, actions)
 
     if all_done:
         state = model.sample_initial_state()
         observations = model.sample_initial_obs(state)
 ```
 
-The base model API is very similar to the environment API. The key difference that all methods are stateless so can be used repeatedly for planning. Indeed the `env` class for the built-in environments are mainly just a wrappers over the underlying `model` class that manage the state and add support for rendering.
+The base model API is very similar to the environment API. The key difference that all methods are stateless so can be repeatedly sampled for planning. Indeed the `Env` class implementations for the built-in environments are a wrapper over an underlying `POSGModel` class that manages the state and adds support for rendering.
 
-Note that unlike for the `env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
+Note that unlike for `Env` class, for convenience the output of the `model.step()` method is a `dataclass` instance and so it's components can be accessed as attributes. For example:
 
 ```python
 timestep = model.step(state, actions)
 observations = timestep.observations
 infos = timestep.infos
 ```
 
-Both the `env` and `model` classes support a number of other methods, please see the documentation [posggym.readthedocs.io/](https://posggym.readthedocs.io/) for more details.
+Both the `Env` and `POSGModel` classes support a number of additional methods, refer to the [documentation](https://posggym.readthedocs.io/) for more details.
 
 ## Agents API
 
-POSGGym.Agents models each agent as a python `policy` class, which at it's simplest accepts an observation and returns the next action. Here's an example using one of the K-Level Reasoning policies in the `PursuitEvasion-v0` environment:
+The Agents API provides a way to easy load reference policies that come with POSGGym. Each policy is a `Policy` class, which at it's simplest accepts an observation and returns the next action. The basic Agents API is shown below:
 
 
 ```python
 import posggym
 import posggym.agents as pga
-env = posggym.make("PursuitEvasion-v0", grid="16x16")
+env = posggym.make("PursuitEvasion-v1", grid="16x16")
 
 policies = {
-    '0': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i0-v0", env.model, '0'),
-    '1': pga.make("PursuitEvasion-v0/grid=16x16/klr_k1_seed0_i1-v0", env.model, '1')
+    '0': pga.make("PursuitEvasion-v1/grid=16x16/RL1_i0-v0", env.model, '0'),
+    '1': pga.make("PursuitEvasion-v1/grid=16x16/ShortestPath-v0", env.model, '1')
 }
 
-obs, info = env.reset(seed=42)
+obs, infos = env.reset(seed=42)
 for i, policy in policies.items():
     policy.reset(seed=7)
 
 for t in range(100):
     actions = {i: policies[i].step(obs[i]) for i in env.agents}
-    obs, rewards, termination, truncated, all_done, info = env.step(actions)
+    obs, rewards, terminations, truncations, all_done, infos = env.step(actions)
 
     if all_done:
-        obs, info = env.reset()
+        obs, infos = env.reset()
         for i, policy in policies.items():
             policy.reset()
 
 env.close()
 for policy in policies.values():
     policy.close()
 ```
 
 For a full explanation of the agent API please see the [POSGGym Agents Getting Started documentation](https://posggym.readthedocs.io/en/latest/agents/getting_started.html). A full list of implemented agents is also available in the documentation.
 
+## Compatibility with PettingZoo
+
+Any POSGGym environment can be converted into a PettingZoo `ParallelEnv` environment using the `posggym.wrappers.petting_zoo.PettingZoo` wrapper. This allows for easy integration with the ecosystem of libraries that support PettingZoo.
+
+```python
+import posggym
+from posggym.wrappers.petting_zoo import PettingZoo
+
+env = posggym.make("PredatorPrey-v0")
+env = PettingZoo(env)
+```
+
 ## Citation
 
 You can cite POSGGym as:
 
 ```bibtex
 @misc{schwartzPOSGGym2023,
     title = {POSGGym},
```

### Comparing `posggym-0.5.1/posggym.egg-info/SOURCES.txt` & `posggym-0.6.0/posggym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/pyproject.toml` & `posggym-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "posggym"
-description = "A collection of diverse environments and reference agents for reinforcement learning and planning research in Partially Observable Stochastic Games (POSGs). ."
+description = "A library for planning and reinforcement learning research in partially observable, multi-agent environments."
 readme = "README.md"
 requires-python = ">= 3.8"
 authors = [
 	{ name = "Jonathon Schwartz", email = "jonathon.schwartz@anu.edu.au" },
 ]
 license = { text = "MIT License" }
 keywords = [
@@ -33,51 +33,41 @@
 	'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
 dependencies = [
 	"gymnasium >=0.26",
 	"numpy >=1.21.0",
 	"typing-extensions >=4.3.0",
 	"importlib-metadata >=4.8.0; python_version < '3.10'",
+	"pygame >=2.0",
+	"pymunk >=6.0.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # Update dependencies in `all` if any are added or removed
-grid-world = ["pygame >=2.0"]
-continuous = ["pygame >=2.0", "pymunk >=6.0.0"]
-envs-all = [
-	# Dependencies for all environment types above
-	"pygame >=2.0",
-	"pymunk >=6.0.0",
-]
 agents = [
-	"pygame >=2.0",
-	"pymunk >=6.0.0",
 	"types-requests >=2.28",
 	"requests >= 2.28",
 	"clint >= 0.5.1",
 	"torch >=1.11.0",
 ]
 other = [
 	# Dependencies used in wrappers, notebooks, and scripts
 	"moviepy >=1.0.0",
 	"pandas >=1.0",
 	"seaborn >=0.13.0",
 	"matplotlib >=3.0.0",
 ]
 all = [
 	# Dependencieis for all envs and agents
-	# envs
-	"pygame >=2.0",
-	"pymunk>=6.0.0",
 	# agents
 	"types-requests >=2.28",
 	"requests >= 2.28",
 	"clint >= 0.5.1",
-	"torch >=1.11.0",
+	"torch >= 2.0",
 	# other
 	"moviepy >=1.0.0",
 	"seaborn >=0.11.1",
 	"matplotlib >=3.3.4",
 	"pandas >=1.0",
 ]
 testing = ["pytest >=7.2"]
@@ -117,15 +107,14 @@
 max-complexity = 10
 
 [tool.ruff.isort]
 lines-after-imports = 2
 extra-standard-library = ["typing_extensions"]
 
 [tool.black]
-safe = true
 line-length = 88
 
 [tool.pyright]
 include = ["posggym/**"]
 exclude = ["**/node_modules", "**/__pycache__"]
 strict = []
```

### Comparing `posggym-0.5.1/setup.py` & `posggym-0.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Setup for the posggym package."""
-import os
-import pathlib
+
 import shutil
 import tarfile
 import urllib.request
+from pathlib import Path
 
 from setuptools import setup
 from setuptools.command import build_py
 
-CWD = pathlib.Path(__file__).absolute().parent
+CWD = Path(__file__).absolute().parent
 
 ASSETS_URL = (
-    "https://github.com/RDLLab/posggym-agent-models/archive/refs/tags/v0.5.1.tar.gz"
+    "https://github.com/RDLLab/posggym-agent-models/archive/refs/tags/v0.6.0.tar.gz"
 )
 
 
 def get_version():
     """Gets the posggym version."""
     path = CWD / "posggym" / "__init__.py"
     content = path.read_text()
@@ -44,33 +44,32 @@
         if not self.editable_mode:
             super().run()
             self.build_assets()
 
     def download_and_extract_assets(self):
         """Downloads and extracts the assets."""
         print("Downloading and extracting assets...", flush=True)
-        tar_file_path = os.path.join(self.get_package_dir("assets"), "assets.tar.gz")
-        if os.path.exists(tar_file_path):
+        tar_file_path = self.get_package_dir("assets") / "assets.tar.gz"
+        if tar_file_path.exists():
             print(f"Found cached assets {tar_file_path}", flush=True)
         else:
-            os.makedirs(os.path.dirname(tar_file_path), exist_ok=True)
+            tar_file_path.parent.mkdir(exist_ok=True)
             print("Downloading assets...", flush=True)
             urllib.request.urlretrieve(
                 ASSETS_URL, filename=tar_file_path, reporthook=show_progress
             )
             print(f"Downloaded assets to {tar_file_path}", flush=True)
 
-        root_dir = os.path.join(self.get_package_dir(""), "posggym")
-        asset_dir = os.path.join(root_dir, "assets")
-        os.makedirs(root_dir, exist_ok=True)
-        if os.path.exists(asset_dir):
+        root_dir = self.get_package_dir("") / "posggym"
+        asset_dir = root_dir / "assets"
+        root_dir.mkdir(exist_ok=True)
+        if asset_dir.exists():
             shutil.rmtree(asset_dir)
             print("Deleted existing assets", flush=True)
-
-        os.makedirs(asset_dir, exist_ok=True)
+        asset_dir.mkdir(exist_ok=True)
         print("Extracting assets...", flush=True)
 
         def members(tarball):
             # strip the top-level directory from the tarball
             # ref:
             # https://stackoverflow.com/questions/8008829/extract-only-a-single-directory-from-tar-in-python
             top_level_dirs = "/".join(tarball.getmembers()[-1].name.split("/")[:2])
@@ -79,26 +78,30 @@
                     member.path = member.path[len(top_level_dirs) + 1 :]
                     yield member
 
         with tarfile.open(tar_file_path, mode="r") as tarball:
             tarball.extractall(asset_dir, members=members(tarball))
         print(f"Extracted assets from {tar_file_path} to {asset_dir}", flush=True)
 
+    def get_package_dir(self, package: str) -> Path:
+        """Gets the package directory."""
+        return Path(super().get_package_dir(package))
+
     def build_assets(self):
         """Copies assets from package to build directory."""
         print("Building assets...", flush=True)
-        package_root = os.path.join(self.get_package_dir(""), "posggym")
-        os.makedirs(package_root, exist_ok=True)
-        build_root = os.path.join(self.build_lib, "posggym")
+        package_root = self.get_package_dir("") / "posggym"
+        package_root.mkdir(exist_ok=True)
+        build_root = Path(self.build_lib) / "posggym"
 
-        if os.path.exists(f"{build_root}/assets"):
-            shutil.rmtree(f"{build_root}/assets")
+        if (build_root / "assets").exists():
+            shutil.rmtree(build_root / "assets")
             print("deleted existing assets", flush=True)
 
-        shutil.copytree(f"{package_root}/assets", f"{build_root}/assets")
+        shutil.copytree(package_root / "assets", build_root / "assets")
         print(
             f"copied assets from {package_root}/assets to {build_root}/assets",
             flush=True,
         )
 
 
 setup(name="posggym", version=get_version(), cmdclass={"build_py": BuildPy})
```

### Comparing `posggym-0.5.1/tests/test_core.py` & `posggym-0.6.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `posggym-0.5.1/tests/test_model.py` & `posggym-0.6.0/tests/test_model.py`

 * *Files identical despite different names*

