# Comparing `tmp/jj_wingman-0.7.1.tar.gz` & `tmp/jj_wingman-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.7.1.tar", last modified: Sun Mar 17 12:03:13 2024, max compression
+gzip compressed data, was "jj_wingman-0.8.0.tar", last modified: Wed Apr 10 14:36:54 2024, max compression
```

## Comparing `jj_wingman-0.7.1.tar` & `jj_wingman-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/jj_wingman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-17 12:03:12.000000 jj_wingman-0.7.1/jj_wingman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/test/test_replay_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 12:03:12.997935 jj_wingman-0.7.1/wingman/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/cli_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/neural_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/replay_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15647 2024-03-17 12:03:04.000000 jj_wingman-0.7.1/wingman/wingman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/jj_wingman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 14:36:54.000000 jj_wingman-0.8.0/jj_wingman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/test/test_replay_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:36:54.287834 jj_wingman-0.8.0/wingman/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/cli_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/neural_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/replay_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-04-10 14:36:42.000000 jj_wingman-0.8.0/wingman/wingman.py
```

### Comparing `jj_wingman-0.7.1/LICENSE.txt` & `jj_wingman-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/PKG-INFO` & `jj_wingman-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.7.1
+Version: 0.8.0
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -74,17 +74,17 @@
 This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
-weights_directory: 'weights'
-version_number: null
-mark_number: 0
+save_directory: 'weights'
+model_id: null
+ckpt_number: 0
 log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
@@ -94,19 +94,19 @@
 wandb_id: ''
 wandb_entity: 'jjshoots'
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
-- `weights_directory`: Where should Wingman point to for model weight saving
-- `version_number`: Wingman versions different models using this number, if this is left as null, Wingman automatically chooses a number.
-- `mark_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `save_directory`: Where should Wingman point to for model weight saving
+- `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
+- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
-- `increment`: Whether to increment mark number, if this is set to false, Wingman won't save multiple variations of the same model.
+- `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
 - `wandb_notes`: Some helpful notes that you can leave for your runs that will be recorded in WandB.
 - `wandb_id`: A Unique ID for this run. If left blank, one is automatically assigned.
@@ -131,17 +131,17 @@
     cfg = wm.cfg
 
     # load the model and optimizer, `cfg.device` is automatically generated
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
-    # this checking is done using the `version_number` param, if `latest=True` is set,
+    # this checking is done using the `model_id` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
-    # otherwise, Wingman uses the checkpoint specified by `mark_number`
+    # otherwise, Wingman uses the checkpoint specified by `ckpt_number`
     have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
@@ -167,15 +167,15 @@
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
 #### Weights Directory Compression
 
 If you train a lot of models, the weights directory can start to use a lot of disk space.
-Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant checkpoint numbers and delete all empty directories.
 
 
 <br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
@@ -303,18 +303,18 @@
     # rollover the observation
     obs = next_obs
 
     # get an action from the policy
     act = policy(obs)
 
     # sample a new transition
-    next_obs, rew, dne, next_lbl = env.step(act)
+    next_obs, rew, done, next_lbl = env.step(act)
 
     # store stuff in the replay buffer
-    memory.push((obs, act, rew, next_obs, dne))
+    memory.push((obs, act, rew, next_obs, done))
 
 # perform training using the buffer
 dataloader = torch.utils.data.DataLoader(
     memory, batch_size=32, shuffle=True, drop_last=False
 )
 
 # easily treat the replay buffer as an iterable that we can iterate through
```

### Comparing `jj_wingman-0.7.1/README.md` & `jj_wingman-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
-weights_directory: 'weights'
-version_number: null
-mark_number: 0
+save_directory: 'weights'
+model_id: null
+ckpt_number: 0
 log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
@@ -57,19 +57,19 @@
 wandb_id: ''
 wandb_entity: 'jjshoots'
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
-- `weights_directory`: Where should Wingman point to for model weight saving
-- `version_number`: Wingman versions different models using this number, if this is left as null, Wingman automatically chooses a number.
-- `mark_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `save_directory`: Where should Wingman point to for model weight saving
+- `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
+- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
-- `increment`: Whether to increment mark number, if this is set to false, Wingman won't save multiple variations of the same model.
+- `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
 - `wandb_notes`: Some helpful notes that you can leave for your runs that will be recorded in WandB.
 - `wandb_id`: A Unique ID for this run. If left blank, one is automatically assigned.
@@ -94,17 +94,17 @@
     cfg = wm.cfg
 
     # load the model and optimizer, `cfg.device` is automatically generated
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
-    # this checking is done using the `version_number` param, if `latest=True` is set,
+    # this checking is done using the `model_id` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
-    # otherwise, Wingman uses the checkpoint specified by `mark_number`
+    # otherwise, Wingman uses the checkpoint specified by `ckpt_number`
     have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
@@ -130,15 +130,15 @@
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
 #### Weights Directory Compression
 
 If you train a lot of models, the weights directory can start to use a lot of disk space.
-Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant checkpoint numbers and delete all empty directories.
 
 
 <br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
@@ -266,18 +266,18 @@
     # rollover the observation
     obs = next_obs
 
     # get an action from the policy
     act = policy(obs)
 
     # sample a new transition
-    next_obs, rew, dne, next_lbl = env.step(act)
+    next_obs, rew, done, next_lbl = env.step(act)
 
     # store stuff in the replay buffer
-    memory.push((obs, act, rew, next_obs, dne))
+    memory.push((obs, act, rew, next_obs, done))
 
 # perform training using the buffer
 dataloader = torch.utils.data.DataLoader(
     memory, batch_size=32, shuffle=True, drop_last=False
 )
 
 # easily treat the replay buffer as an iterable that we can iterate through
```

### Comparing `jj_wingman-0.7.1/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.8.0/jj_wingman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.7.1
+Version: 0.8.0
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -74,17 +74,17 @@
 This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
-weights_directory: 'weights'
-version_number: null
-mark_number: 0
+save_directory: 'weights'
+model_id: null
+ckpt_number: 0
 log_status: false
 
 increment: true
 logging_interval: 10
 max_skips: 5
 greater_than: 0.0
 
@@ -94,19 +94,19 @@
 wandb_id: ''
 wandb_entity: 'jjshoots'
 wandb_project: 'my_new_project'
 ```
 
 The parameters described are as follows:
 - `debug`: Whether to set the model to debug mode
-- `weights_directory`: Where should Wingman point to for model weight saving
-- `version_number`: Wingman versions different models using this number, if this is left as null, Wingman automatically chooses a number.
-- `mark_number`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
+- `save_directory`: Where should Wingman point to for model weight saving
+- `model_id`: Wingman records the model under this ID, if this is left as null, Wingman automatically chooses a number.
+- `model_num`: Wingman checkpoints models using this number if left at 0, automatic checkpoint numbering occurs if the `increment` parameter is set to true.
 - `log_status`: Whether to save a `.txt` log file of Wingman's outputs.
-- `increment`: Whether to increment mark number, if this is set to false, Wingman won't save multiple variations of the same model.
+- `increment`: Whether to increment checkpoint number, if this is set to false, Wingman won't save multiple variations of the same model.
 - `logging_interval`: During training, pass the training step to wingman, and after `logging_interval` steps has passed, Wingman will record the training. If Wingman has found a new lowest point, the model weights will be saved to a new file.
 - `max_skips`: How many logging steps skipped without finding a new lowest point (specified using the `logging_interval` argument) before Wingman will save an intermediary checkpoint of the model.
 - `greater_than`: You can tell Wingman to only checkpoint the model when the previous checkpointed loss is more than the current loss by this value.
 - `wandb`: Whether to log things to WandB.
 - `wandb_name`: The name of the run to be displayed in WandB. If left blank, Wingman automatically assigns one depending on the model version number.
 - `wandb_notes`: Some helpful notes that you can leave for your runs that will be recorded in WandB.
 - `wandb_id`: A Unique ID for this run. If left blank, one is automatically assigned.
@@ -131,17 +131,17 @@
     cfg = wm.cfg
 
     # load the model and optimizer, `cfg.device` is automatically generated
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
-    # this checking is done using the `version_number` param, if `latest=True` is set,
+    # this checking is done using the `model_id` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
-    # otherwise, Wingman uses the checkpoint specified by `mark_number`
+    # otherwise, Wingman uses the checkpoint specified by `ckpt_number`
     have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
@@ -167,15 +167,15 @@
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
 #### Weights Directory Compression
 
 If you train a lot of models, the weights directory can start to use a lot of disk space.
-Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant checkpoint numbers and delete all empty directories.
 
 
 <br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
@@ -303,18 +303,18 @@
     # rollover the observation
     obs = next_obs
 
     # get an action from the policy
     act = policy(obs)
 
     # sample a new transition
-    next_obs, rew, dne, next_lbl = env.step(act)
+    next_obs, rew, done, next_lbl = env.step(act)
 
     # store stuff in the replay buffer
-    memory.push((obs, act, rew, next_obs, dne))
+    memory.push((obs, act, rew, next_obs, done))
 
 # perform training using the buffer
 dataloader = torch.utils.data.DataLoader(
     memory, batch_size=32, shuffle=True, drop_last=False
 )
 
 # easily treat the replay buffer as an iterable that we can iterate through
```

### Comparing `jj_wingman-0.7.1/pyproject.toml` & `jj_wingman-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.7.1"
+version = "0.8.0"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.7.1/test/test_replay_buffer.py` & `jj_wingman-0.8.0/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/cli_scripts.py` & `jj_wingman-0.8.0/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/neural_blocks.py` & `jj_wingman-0.8.0/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/print_utils.py` & `jj_wingman-0.8.0/wingman/print_utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/replay_buffer.py` & `jj_wingman-0.8.0/wingman/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/utils.py` & `jj_wingman-0.8.0/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.7.1/wingman/wingman.py` & `jj_wingman-0.8.0/wingman/wingman.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,50 +78,48 @@
         self.cumulative_loss = 0
         self.lowest_loss = math.inf
         self.next_log_step = self.cfg.logging_interval
         self.previous_checkpoint_step = 0
         self.skips = 0
 
         # weight file variables
-        self.version_number = self.cfg.version_number
-        self.mark_number = self.cfg.mark_number
-        self.previous_mark_number = -1
+        self.model_id = self.cfg.model_id
+        self.ckpt_number = self.cfg.ckpt_number
+        self.previous_checkpoint_number = -1
 
         # directory itself
-        self.version_directory = (
-            Path(self.cfg.weights_directory) / f"Version{self.version_number}"
-        )
+        self.model_directory = Path(self.cfg.save_directory) / str(self.model_id)
 
         # file paths
-        self.model_file = self.version_directory / f"weights{self.mark_number}.path"
-        self.optim_file = self.version_directory / "optimizer_path"
-        self.status_file = self.version_directory / "lowest_loss.npy"
-        self.intermediary_file = self.version_directory / "weights-1.npy"
+        self.model_file = self.model_directory / f"weights{self.ckpt_number}.path"
+        self.optim_file = self.model_directory / "optimizer_path"
+        self.status_file = self.model_directory / "lowest_loss.npy"
+        self.intermediary_file = self.model_directory / "weights-1.npy"
         if self.log_file:
-            self.log_file = self.version_directory / "log.txt"
+            self.log_file = self.model_directory / "log.txt"
 
         wm_print("--------------𓆩𓆪--------------")
         wm_print(f"Using device {cstr(self.device, 'HEADER')}")
-        wm_print(f"Saving weights to {cstr(self.version_directory, 'HEADER')}...")
+        wm_print(f"Saving weights to {cstr(self.model_directory, 'HEADER')}...")
 
         # check to record that we're in a new training session and save the config file
         self.fresh_directory = False
-        if not self.version_directory.is_dir():
+        if not self.model_directory.is_dir():
             self.fresh_directory = True
             wm_print(
                 cstr(
                     "New training instance detected, generating weights directory in 3 seconds...",
                     "WARNING",
                 ),
             )
             time.sleep(3)
-            self.version_directory.mkdir(parents=True, exist_ok=True)
+            self.model_directory.mkdir(parents=True, exist_ok=True)
             shutil.copyfile(
                 self.config_yaml,
-                self.version_directory / "config_copy.yaml",
+                self.model_directory / "config_copy.yaml",
             )
 
     def __get_device(self):
         """__get_device."""
         from warnings import warn
 
         try:
@@ -147,39 +145,39 @@
         parser = argparse.ArgumentParser(description=self.experiment_description)
 
         with open(self.config_yaml) as f:
             # read in the file
             config = yaml.load(f, Loader=yaml.FullLoader)
 
             # checks that we have the default params in the file
-            assertation_list = [
+            assertion_list = [
                 "debug",
-                "weights_directory",
-                "version_number",
-                "mark_number",
+                "save_directory",
+                "model_id",
+                "ckpt_number",
                 "log_status",
                 "increment",
                 "logging_interval",
                 "max_skips",
                 "greater_than",
                 "wandb",
                 "wandb_name",
                 "wandb_notes",
                 "wandb_id",
                 "wandb_entity",
                 "wandb_project",
             ]
-            for item in assertation_list:
+            for item in assertion_list:
                 assert item in config, cstr(
                     f"Missing parameter {item} in config file.", "FAIL"
                 )
 
-            # override version number if needed
-            if config["version_number"] is None:
-                config["version_number"] = np.random.randint(999999)
+            # override model_id if needed
+            if config["model_id"] is None:
+                config["model_id"] = np.random.randint(999999)
 
             # make a logging file if required
             self.log_file = config["log_status"]
 
             # add all to argparse
             for item in config:
                 parser.add_argument(
@@ -193,29 +191,27 @@
 
         # dict of all arguments, by default will be overridden by commandline args
         config = {**vars(parser.parse_args())}
 
         # add the gpu
         config["device"] = self.__get_device()
 
-        # change the version if debugging
-        config["version_number"] = (
-            "Debug" if config["debug"] else str(config["version_number"])
-        )
+        # change the model_id if debugging
+        config["model_id"] = "Debug" if config["debug"] else str(config["model_id"])
 
         # cfg depending on whether wandb is enabled
         cfg = None
         if config["wandb"]:
             wandb.init(
                 project=config["wandb_project"],
                 entity=config["wandb_entity"],
                 config=config,
-                name=config["wandb_name"] + ", v=" + config["version_number"]
+                name=config["wandb_name"] + ", v=" + config["model_id"]
                 if config["wandb_name"] != ""
-                else config["version_number"],
+                else config["model_id"],
                 notes=config["wandb_notes"],
                 id=config["wandb_id"] if config["wandb_id"] != "" else None,
             )
 
             # also save the code if wandb
             # wandb.run.log_code(".", exclude_fn=lambda path: "venv" in path)  # type: ignore
 
@@ -232,16 +228,16 @@
     ) -> Tuple[bool, Path, Path]:
         """checkpoint.
 
         Records training every logging_interval steps.
 
         Returns three things:
         - indicator on whether we should save weights
-        - directory of where the weight files should be saved
-        - directory of where the optim files should be saved
+        - path of where the weight files should be saved
+        - path of where the optim files should be saved
 
         Args:
             loss (float): learning loss of the model as a detached float
             step (int | None): step number, automatically incremented if None
 
         Returns:
             Tuple[bool, Path, Path]: to_update, weights_file, optim_file
@@ -303,33 +299,33 @@
                 return True, self.intermediary_file, self.optim_file
 
         """NEW LOSS IS BETTER"""
         # redefine the new lowest loss and reset the skips
         self.lowest_loss = avg_loss
         self.skips = 0
 
-        # increment means return the files with incremented mark number
+        # increment means return the files with incremented checkpoint number
         if self.cfg.increment:
-            # check if we are safe to increment mark numbers and regenerate weights file
-            if self.previous_mark_number == -1 or self.model_file.exists():
-                self.previous_mark_number = self.mark_number
+            # check if we are safe to increment checkpoint numbers and regenerate weights file
+            if self.previous_checkpoint_number == -1 or self.model_file.exists():
+                self.previous_checkpoint_number = self.ckpt_number
                 self.model_file = (
-                    self.version_directory / f"weights{self.mark_number}.pth"
+                    self.model_directory / f"weights{self.ckpt_number}.pth"
                 )
-                self.mark_number += 1
+                self.ckpt_number += 1
 
             else:
                 wm_print(
                     cstr(
-                        "Didn't save weights file for the previous mark number (self.mark_number), not incrementing mark number.",
+                        "Didn't save weights file for the previous checkpoint number (self.ckpt_number), not incrementing checkpoint number.",
                         "WARNING",
                     ),
                     self.log_file,
                 )
-                self.mark_number = self.previous_mark_number
+                self.ckpt_number = self.previous_checkpoint_number
 
         # record the lowest running loss in the status file
         np.save(self.status_file, self.lowest_loss)
 
         wm_print(
             f"New lowest point, saving weights to: {cstr(self.model_file, 'OKGREEN')}",
             self.log_file,
@@ -365,60 +361,60 @@
             variable_name (str): variable_name
             precision (str): precision
 
         Returns:
             None:
         """
         assert len(data.shape) == 1, "Data must be only 1 dimensional ndarray"
-        filename = self.version_directory / f"{variable_name}.csv"
+        filename = self.model_directory / f"{variable_name}.csv"
         with open(filename, "ab") as f:
             np.savetxt(f, [data], delimiter=",", fmt=precision)
 
     def get_weight_files(self, latest: bool = True) -> Tuple[bool, Path, Path]:
         """get_weight_files.
 
         Returns three things:
         - indicator on whether we have weight files
         - directory of where the weight files are
         - directory of where the optim files are
 
         Args:
-            latest (bool): whether we want the latest file or the one determined by `mark_number`
+            latest (bool): whether we want the latest file or the one determined by `ckpt_number`
 
         Returns:
             Tuple[bool, Path, Path]: have_file, weights_file, optim_file
         """
         # if we don't need the latest file, get the one specified
         if not latest:
             if os.path.isfile(self.model_file):
                 self.model_file = (
-                    self.version_directory / f"weights{self.mark_number}.pth"
+                    self.model_directory / f"weights{self.ckpt_number}.pth"
                 )
                 wm_print(
-                    f"Using weights file: {cstr(f'{self.version_directory}/weights{self.mark_number}.pth', 'OKGREEN')}",
+                    f"Using weights file: {cstr(f'{self.model_directory}/weights{self.ckpt_number}.pth', 'OKGREEN')}",
                     self.log_file,
                 )
                 return True, self.model_file, self.optim_file
             else:
                 raise ValueError(
                     cstr(
-                        f"Mark number {self.mark_number} was requested, but it doesn't exist.",
+                        f"Checkpoint number {self.ckpt_number} was requested, but it doesn't exist.",
                         "FAIL",
                     )
                 )
 
-        # while the file exists, try to look for a file one version later
-        self.mark_number = 0
+        # while the file exists, try to look for a file one checkpoint later
+        self.ckpt_number = 0
         while self.model_file.is_file():
-            self.mark_number += 1
-            self.model_file = self.version_directory / f"weights{self.mark_number}.pth"
+            self.ckpt_number += 1
+            self.model_file = self.model_directory / f"weights{self.ckpt_number}.pth"
 
-        # once the file version doesn't exist, decrement by one and use that file
-        self.mark_number = max(self.mark_number - 1, 0)
-        self.model_file = self.version_directory / f"weights{self.mark_number}.pth"
+        # once the checkpoint doesn't exist, decrement by one and use that file
+        self.ckpt_number = max(self.ckpt_number - 1, 0)
+        self.model_file = self.model_directory / f"weights{self.ckpt_number}.pth"
 
         # if the file doesn't exist, notify and ignore
         if not self.model_file.is_file():
             if not self.fresh_directory:
                 wm_print(
                     cstr(
                         "No weights file found, generating new one during training.",
@@ -430,15 +426,15 @@
 
             return False, self.model_file, self.optim_file
         else:
             # hitch a ride to update the lowest running loss
             self.lowest_loss = np.load(self.status_file).item()
 
             wm_print(
-                f"Using weights file: {cstr(f'{self.version_directory}/weights{self.mark_number}.pth', 'OKGREEN')}",
+                f"Using weights file: {cstr(f'{self.model_directory}/weights{self.ckpt_number}.pth', 'OKGREEN')}",
                 self.log_file,
             )
             wm_print(
                 f"Lowest Running Loss for Net: {cstr(self.lowest_loss, 'OKCYAN')}",
                 self.log_file,
             )
```

