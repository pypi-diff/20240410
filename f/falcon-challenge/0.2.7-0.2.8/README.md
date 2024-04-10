# Comparing `tmp/falcon_challenge-0.2.7.tar.gz` & `tmp/falcon_challenge-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.7.tar", last modified: Fri Apr  5 20:40:38 2024, max compression
+gzip compressed data, was "falcon_challenge-0.2.8.tar", last modified: Wed Apr 10 11:08:30 2024, max compression
```

## Comparing `falcon_challenge-0.2.7.tar` & `falcon_challenge-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.753359 falcon_challenge-0.2.7/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 20:40:38.000000 falcon_challenge-0.2.7/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:40:38.757359 falcon_challenge-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 20:40:34.000000 falcon_challenge-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17333 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 11:08:30.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/setup.py
```

### Comparing `falcon_challenge-0.2.7/LICENSE` & `falcon_challenge-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/PKG-INFO` & `falcon_challenge-0.2.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
@@ -58,33 +58,34 @@
 - The `falcon_challenge` folder contains the logic for the evaluator. Submitted solutions must conform to the interface specified in `falcon_challenge.interface`.
 - In `data_demos`, we provide notebooks that survey each dataset released as part of this challenge.
 - In `decoder_demos`, we provide sample decoders and baselines that are formatted to be ready for submission to the challenge. To use them, see the comments in the header of each file ending in `_sample.py`. Your solutions should look similar once implemented!
 
 For example, you can prepare and evaluate a linear decoder by running:
 ```bash
 python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib/ --calibration_dir data/h1/held_out_calib/ --mode all --task h1
-python sklearn_sample.py --evaluation local --phase minival --split h1
+python decoder_demos/sklearn_sample.py --evaluation local --phase minival --split h1
 ```
 
 ### Docker Submission
 To interface with our challenge, your code will need to be packaged in a Docker container that is submitted to EvalAI. Try this process by building and running the provided `sklearn_sample.Dockerfile`, to confirm your setup works. Do this with the following commands (once Docker is installed)
 ```bash
 # Build
-sudo docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
-sudo docker run -v PATH_TO_YOUR_DATA_DIR:/dataset/evaluation_data -it sk_smoke
-## If your solution needs GPUs, append a --gpus all flag to `docker run`
+docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
+bash test_docker_local.sh --docker-name sk_smoke
 ```
 
 ## EvalAI Submission
-Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands, or run `test_docker_local.sh --docker-name mysubmission`. This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
+Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands with your own Dockerfile (in place of sk_smoke). This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
 
-To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). It should look something like:
+To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). This will instruct you to first install EvalAI, then add your token, and finally push the submission. It should look something like:
 `
 evalai push mysubmission:latest --phase <phase-name> (dev or test)
 `
+(Note that you will not see these instruction unless you have first created a team to submit. The phase should contain a specific challenge identifier. You may need to refresh the page before instructions will appear.)
+
 
 ### Troubleshooting
 Docker:
 - If this is your first time with docker, note that `sudo` access is needed, or your user needs to be in the `docker` group. `docker info` should run without error.
 - While `sudo` is sufficient for local development, the EvalAI submission step will ultimately require your user to be able to run `docker` commands without `sudo`.
 - To do this, [add yourself to the `docker` group](https://docs.docker.com/engine/install/linux-postinstall/). Note you may [need vigr](https://askubuntu.com/questions/964040/usermod-says-account-doesnt-exist-but-adduser-says-it-does) to add your own user.
```

### Comparing `falcon_challenge-0.2.7/README.md` & `falcon_challenge-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,33 +39,34 @@
 - The `falcon_challenge` folder contains the logic for the evaluator. Submitted solutions must conform to the interface specified in `falcon_challenge.interface`.
 - In `data_demos`, we provide notebooks that survey each dataset released as part of this challenge.
 - In `decoder_demos`, we provide sample decoders and baselines that are formatted to be ready for submission to the challenge. To use them, see the comments in the header of each file ending in `_sample.py`. Your solutions should look similar once implemented!
 
 For example, you can prepare and evaluate a linear decoder by running:
 ```bash
 python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib/ --calibration_dir data/h1/held_out_calib/ --mode all --task h1
-python sklearn_sample.py --evaluation local --phase minival --split h1
+python decoder_demos/sklearn_sample.py --evaluation local --phase minival --split h1
 ```
 
 ### Docker Submission
 To interface with our challenge, your code will need to be packaged in a Docker container that is submitted to EvalAI. Try this process by building and running the provided `sklearn_sample.Dockerfile`, to confirm your setup works. Do this with the following commands (once Docker is installed)
 ```bash
 # Build
-sudo docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
-sudo docker run -v PATH_TO_YOUR_DATA_DIR:/dataset/evaluation_data -it sk_smoke
-## If your solution needs GPUs, append a --gpus all flag to `docker run`
+docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
+bash test_docker_local.sh --docker-name sk_smoke
 ```
 
 ## EvalAI Submission
-Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands, or run `test_docker_local.sh --docker-name mysubmission`. This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
+Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands with your own Dockerfile (in place of sk_smoke). This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
 
-To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). It should look something like:
+To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). This will instruct you to first install EvalAI, then add your token, and finally push the submission. It should look something like:
 `
 evalai push mysubmission:latest --phase <phase-name> (dev or test)
 `
+(Note that you will not see these instruction unless you have first created a team to submit. The phase should contain a specific challenge identifier. You may need to refresh the page before instructions will appear.)
+
 
 ### Troubleshooting
 Docker:
 - If this is your first time with docker, note that `sudo` access is needed, or your user needs to be in the `docker` group. `docker info` should run without error.
 - While `sudo` is sufficient for local development, the EvalAI submission step will ultimately require your user to be able to run `docker` commands without `sudo`.
 - To do this, [add yourself to the `docker` group](https://docs.docker.com/engine/install/linux-postinstall/). Note you may [need vigr](https://askubuntu.com/questions/964040/usermod-says-account-doesnt-exist-but-adduser-says-it-does) to add your own user.
```

### Comparing `falcon_challenge-0.2.7/decoder_demos/decoding_utils.py` & `falcon_challenge-0.2.8/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/decoder_demos/filtering.py` & `falcon_challenge-0.2.8/preproc/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,29 +27,28 @@
     kernel = np.exp(-t / tau)
     kernel /= np.sum(kernel)
     # Apply the filter
     filtered_signal = np.array([signal.convolve(x[:, ch], kernel, mode='full')[:len(x)] for ch in range(x.shape[1])]).T
     return filtered_signal
 
 
-
 def gaussian_kernel(size, sigma):
     """
     Create a 1D Gaussian kernel.
     """
     size = int(size)
     x = np.linspace(-size // 2, size // 2, size)
     kernel = np.exp(-0.5 * (x / sigma) ** 2)
     kernel /= kernel.sum()
     return kernel
 
 def smooth(position, kernel_size: int, sigma: float):
     """
     Apply Gaussian smoothing on the position data (dim 0)
-    kernel_size: size of the kernel (in input bins)
+    kernel_size: size of the kernel
     sigma: standard deviation of the Gaussian kernel
     """
     kernel = gaussian_kernel(kernel_size, sigma)
     pad_total = kernel_size - 1
     pad_left = pad_total // 2
     pad_right = pad_total - pad_left
```

### Comparing `falcon_challenge-0.2.7/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.2.8/decoder_demos/ndt2_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.2.8/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/decoder_demos/random_decoder.py` & `falcon_challenge-0.2.8/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.2.8/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.2.8/decoder_demos/sklearn_decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -99,24 +99,31 @@
             if dataset_tag not in self.x_mean:
                 raise ValueError(f"Dataset tag {dataset_tag} not found in calibration set {self.x_mean.keys()} - did you calibrate on this dataset?")
             self.local_x_mean = self.x_mean[dataset_tag]
             self.local_x_std = self.x_std[dataset_tag]
         else:
             self.local_x_mean = self.x_mean
             self.local_x_std = self.x_std
+        if isinstance(self.clf, dict):
+            dataset_tag =  self._task_config.hash_dataset(dataset.stem)
+            if dataset_tag not in self.clf:
+                raise ValueError(f"Dataset tag {dataset_tag} not found decoder set {self.clf.keys()}")
+            self.local_clf = self.clf[dataset_tag]
+        else:
+            self.local_clf = self.clf
         self.raw_history_buffer = np.zeros_like(self.raw_history_buffer)
         self.observation_buffer = np.zeros_like(self.observation_buffer)
 
     def predict(self, neural_observations: np.ndarray):
         r"""
             neural_observations: array of shape (n_channels), binned spike counts
         """
         self.observe(neural_observations)
         decoder_in = self.observation_buffer[::-1].copy().flatten().reshape(1, -1) # Reverse since this happens to be how the lagged matrix is formatted
-        out = self.clf.predict(decoder_in)[0]
+        out = self.local_clf.predict(decoder_in)[0]
         return out
 
     def observe(self, neural_observations: np.ndarray):
         r"""
             neural_observations: array of shape (n_channels), binned spike counts
             - for timestamps where we don't want predictions but neural data may be informative (start of trial)
         """
@@ -209,20 +216,76 @@
         fit_datafiles,
         calibration_datafiles,
         task_config,
         save_path,
         history = history
     )
 
+def fit_many_decoders(
+    datafiles: List[Path],
+    calibration_datafiles: List[Path],
+    task_config: FalconConfig,
+    save_path: Path,
+    history = 0,
+):
+    all_datafiles = [*calibration_datafiles, *datafiles]
+    day_unique = set([f.stem.split('_')[0] for f in all_datafiles])
+    all_decoders = {}
+    x_means = {}
+    x_stds = {}
+    for day in sorted(day_unique):
+        print(f"Training on day {day}")
+        fit_datafiles = [d for d in all_datafiles if day == d.stem.split('_')[0]]
+        (
+            neural_data,
+            covariates,
+            trial_change,
+            eval_mask
+        ) = zip(*[load_nwb(fn, task_config.task) for fn in fit_datafiles])
+        neural_data = np.concatenate(neural_data)
+        covariates = np.concatenate(covariates)
+        trial_change = np.concatenate(trial_change)
+        eval_mask = np.concatenate(eval_mask)
+        (
+            train_x,
+            train_y,
+            test_x,
+            test_y,
+            x_mean,
+            x_std,
+            y_mean,
+            y_std
+        ) = prepare_train_test(neural_data, covariates, ~eval_mask, history=history)
+        score, decoder = fit_and_eval_decoder(train_x, train_y, test_x, test_y)
+        for f in fit_datafiles:
+            fn = task_config.hash_dataset(f.stem)
+            all_decoders[fn] = decoder
+            x_means[fn], x_stds[fn] = np.mean(neural_data, axis=0), np.std(neural_data, axis=0)
+            if np.any(x_stds[fn] == 0):
+                x_stds[fn][x_stds[fn] == 0] = 1
+        print(f"CV Fit score: {score:.2f}")
+    decoder_obj = {
+        'decoder': all_decoders,
+        'task': task_config.task,
+        'history': history,
+        'x_mean': x_means,
+        'x_std': x_stds,
+    }
+    with open(save_path, 'wb') as f:
+        pickle.dump(decoder_obj, f)
+    return decoder_obj
+
 def main(task, training_dir, calibration_dir, history, mode):
     # Your main function logic here
     if mode == 'all':
         fit_fn = fit_sklearn_decoder
     elif mode == 'last':
         fit_fn = fit_last_session
+    elif mode == 'per-day':
+        fit_fn = fit_many_decoders # saves down a dict
     else:
         raise ValueError(f"Unknown mode: {mode}")
     training_dir = Path(training_dir)
     calibration_dir = Path(calibration_dir)
     task_config = FalconConfig(
         task=FalconTask.__dict__[task],
     )
@@ -234,13 +297,13 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='Train sklearn decoder')
 
     parser.add_argument('--task', type=str, choices=['h1', 'm1', 'm2'], help='Task for training')
     parser.add_argument('--training_dir', '-t', type=str, help='Root directory for training files')
     parser.add_argument('--calibration_dir', '-c', type=str, help='Root directory for calibration files')
-    parser.add_argument('--mode', '-m', type=str, choices=['all', 'last'], help='Mode for training')
+    parser.add_argument('--mode', '-m', type=str, choices=['all', 'last', 'per-day'], help='Mode for training')
     parser.add_argument('--history', type=int, default=0, help='History for decoder')
 
     args = parser.parse_args()
 
     main(args.task, args.training_dir, args.calibration_dir, args.history, args.mode)
```

### Comparing `falcon_challenge-0.2.7/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.2.8/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/falcon_challenge/config.py` & `falcon_challenge-0.2.8/falcon_challenge/config.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/falcon_challenge/dataloaders.py` & `falcon_challenge-0.2.8/falcon_challenge/dataloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
         - trial_change: boolean of shape (time,) true if the trial has changed
         - eval_mask: boolean array indicating whether to evaluate each time step, True if should
     """
     if not dataset in [FalconTask.h1, FalconTask.h2, FalconTask.m1, FalconTask.m2]:
         raise ValueError(f"Unknown dataset {dataset}")
     with NWBHDF5IO(str(fn), 'r') as io:
         nwbfile = io.read()
-        units = nwbfile.units.to_dataframe()
         if dataset == FalconTask.h1:
+            units = nwbfile.units.to_dataframe()
             kin = nwbfile.acquisition['OpenLoopKinematicsVelocity'].data[:]
             timestamps = nwbfile.acquisition['OpenLoopKinematics'].offset + np.arange(kin.shape[0]) * nwbfile.acquisition['OpenLoopKinematics'].rate
             eval_mask = nwbfile.acquisition['eval_mask'].data[:].astype(bool)
             binned_units = bin_units(units, bin_size_s=0.02, bin_timestamps=timestamps)
             return binned_units, kin, np.zeros(kin.shape[0]), eval_mask
         elif dataset == FalconTask.h2: 
             binned_spikes = nwbfile.acquisition['binned_spikes'].data[()]
@@ -102,14 +102,15 @@
             eval_mask = nwbfile.acquisition['eval_mask'].data[()].astype(bool)
             trial_info = (
                 nwbfile.trials.to_dataframe()
                 .reset_index()
             )
             return binned_spikes, trial_info.cue.values, np.concatenate([[False], np.diff(time) > 0.02]), eval_mask
         elif dataset == FalconTask.m1:
+            units = nwbfile.units.to_dataframe()
             raw_emg = nwbfile.acquisition['preprocessed_emg']
             muscles = [ts for ts in raw_emg.time_series]
             emg_data = []
             emg_timestamps = []
             for m in muscles:
                 mdata = raw_emg.get_timeseries(m)
                 data = mdata.data[:]
@@ -129,14 +130,15 @@
             )
             switch_inds = np.searchsorted(emg_timestamps, trial_info.start_time)
             trial_change = np.zeros(emg_timestamps.shape[0], dtype=bool)
             trial_change[switch_inds] = True
 
             return binned_units, emg_data, trial_change, eval_mask
         elif dataset == FalconTask.m2:
+            units = nwbfile.units.to_dataframe()
             vel_container = nwbfile.acquisition['finger_vel']
             labels = [ts for ts in vel_container.time_series]
             vel_data = []
             vel_timestamps = None
             for ts in labels:
                 ts_data = vel_container.get_timeseries(ts)
                 vel_data.append(ts_data.data[:])
```

### Comparing `falcon_challenge-0.2.7/falcon_challenge/evaluator.py` & `falcon_challenge-0.2.8/falcon_challenge/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,30 +232,36 @@
         return all_preds, all_targets, all_eval_mask
 
     def evaluate_files(self, decoder: BCIDecoder, eval_files: List):
         all_preds, all_targets, all_eval_mask = self.predict_files(decoder, eval_files)
         metrics = self.compute_metrics(all_preds, all_targets, all_eval_mask)
         return metrics
 
-    def evaluate(self, decoder: BCIDecoder, phase: str, held_out_only: bool = False, specific_keys: List = []):
+    def evaluate(
+            self, 
+            decoder: BCIDecoder, 
+            phase: str, 
+            held_out_only: bool = False, 
+            specific_keys: List = []
+        ):
         r"""
             Note: Locally, this can produce metrics, but locally and remotely it should also write a submission file 
             that the actual evaluator on remote uses. The evaluation is done separately on remote.
 
             held_out_only: Only run predictions on held out
             specific_keys: Overrides held_out_only. Only run predictions on datafiles with specific keys.
         """
         assert phase in ['minival', 'test'], "Phase must be minival or test."
         if phase == 'minival' and (held_out_only or specific_keys):
             logger.warning("Ignoring held_out_only and specific_keys for minival phase.")
             held_out_only = False
         
         np.random.seed(0)
         # ! TODO ideally seed other libraries as well...? Is that our responsibility?
-
+        
         eval_files = self.get_eval_files(phase=phase)
         metrics = {}
         prediction_env_var = "PREDICTION_PATH" if self.eval_remote else "PREDICTION_PATH_LOCAL"
         prediction_path = os.environ.get(prediction_env_var, './local_prediction.pkl')
         if not prediction_path:
             raise ValueError("PREDICTION_PATH not set in remote env which expects it. Cannot forward to separate evaluate runscript.")
         gt_path = os.environ.get("GT_PATH", './local_gt.pkl')
@@ -308,19 +314,19 @@
 
             if self.eval_remote:
                 print("Sleeping before exiting for remote eval - feel free to interrupt for local eval.", flush=True)
                 # Gunjan, EvalAI contact says that current static code eval has an issue where the submission dump is only polled by the EvalAI worker comparison script every 5 minutes
                 # Sleep so it's definitely available
                 time.sleep(300) 
             else:
-                print(evaluate(
+                return evaluate(
                     test_annotation_file=gt_path,
                     user_submission_file=prediction_path,
                     phase_codename=phase
-                ), flush=True)
+                )
         else:
             for k, v in metrics.items():
                 logger.info("{}: {}".format(k, v))
         
     @staticmethod
     def compute_metrics_regression(preds, targets, eval_mask):
         # assumes targets are already masked
```

### Comparing `falcon_challenge-0.2.7/falcon_challenge/interface.py` & `falcon_challenge-0.2.8/falcon_challenge/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import abc
 from pathlib import Path
 import numpy as np
 
 class BCIDecoder:
+
+    batch_size: int = 1
+
     @abc.abstractmethod
     def reset(self, dataset_tag: str = ""):
         pass
 
     # @staticmethod
     # def get_file_tag(filepath: Path, is_dandi=False):
     #     if filepath.name.endswith('behavior+ecephys') # clearly dandi
@@ -33,8 +36,11 @@
             - for timestamps where we don't want predictions but neural data may be informative (start of trial)
         """
         self.predict(neural_observations)
 
     @abc.abstractmethod
     def on_trial_end(self):
         # Optional hook available in H2 (handwriting) to allow periodic test-time adaptation
-        pass
+        pass
+
+    def set_batch_size(self, batch_size: int):
+        self.batch_size = batch_size
```

### Comparing `falcon_challenge-0.2.7/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.2.8/falcon_challenge.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
@@ -58,33 +58,34 @@
 - The `falcon_challenge` folder contains the logic for the evaluator. Submitted solutions must conform to the interface specified in `falcon_challenge.interface`.
 - In `data_demos`, we provide notebooks that survey each dataset released as part of this challenge.
 - In `decoder_demos`, we provide sample decoders and baselines that are formatted to be ready for submission to the challenge. To use them, see the comments in the header of each file ending in `_sample.py`. Your solutions should look similar once implemented!
 
 For example, you can prepare and evaluate a linear decoder by running:
 ```bash
 python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib/ --calibration_dir data/h1/held_out_calib/ --mode all --task h1
-python sklearn_sample.py --evaluation local --phase minival --split h1
+python decoder_demos/sklearn_sample.py --evaluation local --phase minival --split h1
 ```
 
 ### Docker Submission
 To interface with our challenge, your code will need to be packaged in a Docker container that is submitted to EvalAI. Try this process by building and running the provided `sklearn_sample.Dockerfile`, to confirm your setup works. Do this with the following commands (once Docker is installed)
 ```bash
 # Build
-sudo docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
-sudo docker run -v PATH_TO_YOUR_DATA_DIR:/dataset/evaluation_data -it sk_smoke
-## If your solution needs GPUs, append a --gpus all flag to `docker run`
+docker build -t sk_smoke -f ./decoder_demos/sklearn_sample.Dockerfile .
+bash test_docker_local.sh --docker-name sk_smoke
 ```
 
 ## EvalAI Submission
-Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands, or run `test_docker_local.sh --docker-name mysubmission`. This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
+Please ensure that your submission runs locally before running remote evaluation. You can run the previously listed commands with your own Dockerfile (in place of sk_smoke). This should produce a log of nontrivial metrics (evaluation is run on locally available minival).
 
-To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). It should look something like:
+To submit to the FALCON benchmark once your decoder Docker container is ready, follow the instructions on the [EvalAI submission tab](https://eval.ai/web/challenges/challenge-page/2264/submission). This will instruct you to first install EvalAI, then add your token, and finally push the submission. It should look something like:
 `
 evalai push mysubmission:latest --phase <phase-name> (dev or test)
 `
+(Note that you will not see these instruction unless you have first created a team to submit. The phase should contain a specific challenge identifier. You may need to refresh the page before instructions will appear.)
+
 
 ### Troubleshooting
 Docker:
 - If this is your first time with docker, note that `sudo` access is needed, or your user needs to be in the `docker` group. `docker info` should run without error.
 - While `sudo` is sufficient for local development, the EvalAI submission step will ultimately require your user to be able to run `docker` commands without `sudo`.
 - To do this, [add yourself to the `docker` group](https://docs.docker.com/engine/install/linux-postinstall/). Note you may [need vigr](https://askubuntu.com/questions/964040/usermod-says-account-doesnt-exist-but-adduser-says-it-does) to add your own user.
```

### Comparing `falcon_challenge-0.2.7/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.2.8/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/assemble_data.py` & `falcon_challenge-0.2.8/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/filtering.py` & `falcon_challenge-0.2.8/decoder_demos/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch.nn.functional as F
 
 r"""
     H1 filtering
 """
 NEURAL_TAU_MS = 240. # exponential filter from H1 Lab
 def apply_exponential_filter(
-        x, tau=NEURAL_TAU_MS, bin_size=10, extent: int=1
+        x, tau=NEURAL_TAU_MS, bin_size=20, extent: int=1
     ):
     """
     Apply a **causal** exponential filter to the neural signal.
 
     :param x: NumPy array of shape (time, channels)
     :param tau: Decay rate (time constant) of the exponential filter
     :param bin_size: Bin size in ms (default is 10ms)
@@ -27,28 +27,29 @@
     kernel = np.exp(-t / tau)
     kernel /= np.sum(kernel)
     # Apply the filter
     filtered_signal = np.array([signal.convolve(x[:, ch], kernel, mode='full')[:len(x)] for ch in range(x.shape[1])]).T
     return filtered_signal
 
 
+
 def gaussian_kernel(size, sigma):
     """
     Create a 1D Gaussian kernel.
     """
     size = int(size)
     x = np.linspace(-size // 2, size // 2, size)
     kernel = np.exp(-0.5 * (x / sigma) ** 2)
     kernel /= kernel.sum()
     return kernel
 
 def smooth(position, kernel_size: int, sigma: float):
     """
     Apply Gaussian smoothing on the position data (dim 0)
-    kernel_size: size of the kernel
+    kernel_size: size of the kernel (in input bins)
     sigma: standard deviation of the Gaussian kernel
     """
     kernel = gaussian_kernel(kernel_size, sigma)
     pad_total = kernel_size - 1
     pad_left = pad_total // 2
     pad_right = pad_total - pad_left
```

### Comparing `falcon_challenge-0.2.7/preproc/h2_preproc.py` & `falcon_challenge-0.2.8/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.2.8/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.2.8/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.2.8/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/m2_preproc.py` & `falcon_challenge-0.2.8/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/merge_answers.py` & `falcon_challenge-0.2.8/preproc/merge_answers.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         for d in dataset_files:
             print(d.stem)
             neural_data, decoding_targets, trial_change, eval_mask = load_nwb(d, dataset=task)
             annotations[dataset][config.hash_dataset(d.stem)] = {
                 'data': decoding_targets[eval_mask],
                 'mask': eval_mask
             }
+        print(annotations[dataset].keys())
     return annotations
 
 minival_annotations = assemble_phase_answer_key('minival')
 eval_annotations = assemble_phase_answer_key('eval')
 # save these as pickles
 
 with open('./data/answer_key/minival.pkl', 'wb') as f:
```

### Comparing `falcon_challenge-0.2.7/preproc/nwb_create_utils.py` & `falcon_challenge-0.2.8/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/preproc/zip_data.py` & `falcon_challenge-0.2.8/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.7/setup.py` & `falcon_challenge-0.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.7',
+    version='0.2.8',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

