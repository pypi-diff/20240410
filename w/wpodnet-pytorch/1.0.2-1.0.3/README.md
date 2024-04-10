# Comparing `tmp/wpodnet-pytorch-1.0.2.tar.gz` & `tmp/wpodnet-pytorch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpodnet-pytorch-1.0.2.tar", last modified: Mon Jan 29 09:38:22 2024, max compression
+gzip compressed data, was "wpodnet-pytorch-1.0.3.tar", last modified: Wed Apr 10 09:38:13 2024, max compression
```

## Comparing `wpodnet-pytorch-1.0.2.tar` & `wpodnet-pytorch-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:38:22.487939 wpodnet-pytorch-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-01-29 09:38:22.487939 wpodnet-pytorch-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 09:38:22.487939 wpodnet-pytorch-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:38:22.483939 wpodnet-pytorch-1.0.2/wpodnet/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/wpodnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/wpodnet/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/wpodnet/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-29 09:38:12.000000 wpodnet-pytorch-1.0.2/wpodnet/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:38:22.483939 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-01-29 09:38:22.000000 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-29 09:38:22.000000 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 09:38:22.000000 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-29 09:38:22.000000 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-29 09:38:22.000000 wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:13.476731 wpodnet-pytorch-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-10 09:38:13.476731 wpodnet-pytorch-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:38:13.476731 wpodnet-pytorch-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:13.472731 wpodnet-pytorch-1.0.3/wpodnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/wpodnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/wpodnet/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/wpodnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 09:38:09.000000 wpodnet-pytorch-1.0.3/wpodnet/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:13.472731 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-10 09:38:13.000000 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-10 09:38:13.000000 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:38:13.000000 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 09:38:13.000000 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 09:38:13.000000 wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/top_level.txt
```

### Comparing `wpodnet-pytorch-1.0.2/PKG-INFO` & `wpodnet-pytorch-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpodnet-pytorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: The implementation of ECCV 2018 paper "License Plate Detection and Recognition in Unconstrained Scenarios" in PyTorch
 Author: Pandede
 Maintainer: Pandede
 Project-URL: Source, https://github.com/Pandede/WPODNet-Pytorch
 Keywords: python,ai,computer-vision,deep-learning,torch,object-detection,license-plate-recognition,wpod,wpod-net
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -73,15 +73,15 @@
     git clone https://github.com/Pandede/WPODNet-Pytorch.git
     ```
 2. Install [PyTorch](https://pytorch.org) depends on your environment.
 3. Install packages in `requirements.txt`
     ```bash
     pip3 install -r requirements.txt
     ```
-4. Download the pretrained weight `wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link)
+4. Download the pretrained weight `wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/download/1.0.0/wpodnet.pth)
 5. Predict with an image
     ```bash
     python3 predict.py  docs/sample/original/03009.jpg          # The path to the an image
                         # docs/sample/original                  # OR the path to the directory with bulk of images
                         -w weights/wpodnet.pth                  # The path to the weight
                         --save-annotated docs/sample/annotated  # The directory to save the annotated images
                         --save-warped docs/sample/warped        # The directory to save the warped images
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wpodnet-pytorch Version: 1.0.2 Summary: The
+Metadata-Version: 2.1 Name: wpodnet-pytorch Version: 1.0.3 Summary: The
 implementation of ECCV 2018 paper "License Plate Detection and Recognition in
 Unconstrained Scenarios" in PyTorch Author: Pandede Maintainer: Pandede
 Project-URL: Source, https://github.com/Pandede/WPODNet-Pytorch Keywords:
 python,ai,computer-vision,deep-learning,torch,object-detection,license-plate-
 recognition,wpod,wpod-net Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier:
@@ -32,21 +32,21 @@
 Warp perspective [./docs/sample/      [./docs/sample/      [./docs/sample/
                  warped/03009.jpg]    warped/03016.jpg]    warped/03025.jpg]
 Confidence       0.9841               0.9945               0.9979
 ## Quick Run 1. Clone this repository ```bash git clone https://github.com/
 Pandede/WPODNet-Pytorch.git ``` 2. Install [PyTorch](https://pytorch.org)
 depends on your environment. 3. Install packages in `requirements.txt` ```bash
 pip3 install -r requirements.txt ``` 4. Download the pretrained weight
-`wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/
-1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link) 5. Predict with an image
-```bash python3 predict.py docs/sample/original/03009.jpg # The path to the an
-image # docs/sample/original # OR the path to the directory with bulk of images
--w weights/wpodnet.pth # The path to the weight --save-annotated docs/sample/
-annotated # The directory to save the annotated images --save-warped docs/
-sample/warped # The directory to save the warped images ``` ## Future works -
-[x] Inference with GPU - [x] Inference with bulk of images - [ ] Inference with
-video - [ ] Introduce training procedure - [x] The matrix multiplication seems
-weird in function `postprocess`, may improve the computation. ## Citation
-```bibtex @inproceedings{silva2018license, title={License plate detection and
-recognition in unconstrained scenarios}, author={Silva, Sergio Montazzolli and
-Jung, Cl{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
+`wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/
+download/1.0.0/wpodnet.pth) 5. Predict with an image ```bash python3 predict.py
+docs/sample/original/03009.jpg # The path to the an image # docs/sample/
+original # OR the path to the directory with bulk of images -w weights/
+wpodnet.pth # The path to the weight --save-annotated docs/sample/annotated #
+The directory to save the annotated images --save-warped docs/sample/warped #
+The directory to save the warped images ``` ## Future works - [x] Inference
+with GPU - [x] Inference with bulk of images - [ ] Inference with video - [ ]
+Introduce training procedure - [x] The matrix multiplication seems weird in
+function `postprocess`, may improve the computation. ## Citation ```bibtex
+@inproceedings{silva2018license, title={License plate detection and recognition
+in unconstrained scenarios}, author={Silva, Sergio Montazzolli and Jung, Cl
+{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
 computer vision (ECCV)}, pages={580--596}, year={2018} } ```
```

### Comparing `wpodnet-pytorch-1.0.2/README.md` & `wpodnet-pytorch-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     git clone https://github.com/Pandede/WPODNet-Pytorch.git
     ```
 2. Install [PyTorch](https://pytorch.org) depends on your environment.
 3. Install packages in `requirements.txt`
     ```bash
     pip3 install -r requirements.txt
     ```
-4. Download the pretrained weight `wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link)
+4. Download the pretrained weight `wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/download/1.0.0/wpodnet.pth)
 5. Predict with an image
     ```bash
     python3 predict.py  docs/sample/original/03009.jpg          # The path to the an image
                         # docs/sample/original                  # OR the path to the directory with bulk of images
                         -w weights/wpodnet.pth                  # The path to the weight
                         --save-annotated docs/sample/annotated  # The directory to save the annotated images
                         --save-warped docs/sample/warped        # The directory to save the warped images
```

#### html2text {}

```diff
@@ -12,21 +12,21 @@
 Warp perspective [./docs/sample/      [./docs/sample/      [./docs/sample/
                  warped/03009.jpg]    warped/03016.jpg]    warped/03025.jpg]
 Confidence       0.9841               0.9945               0.9979
 ## Quick Run 1. Clone this repository ```bash git clone https://github.com/
 Pandede/WPODNet-Pytorch.git ``` 2. Install [PyTorch](https://pytorch.org)
 depends on your environment. 3. Install packages in `requirements.txt` ```bash
 pip3 install -r requirements.txt ``` 4. Download the pretrained weight
-`wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/
-1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link) 5. Predict with an image
-```bash python3 predict.py docs/sample/original/03009.jpg # The path to the an
-image # docs/sample/original # OR the path to the directory with bulk of images
--w weights/wpodnet.pth # The path to the weight --save-annotated docs/sample/
-annotated # The directory to save the annotated images --save-warped docs/
-sample/warped # The directory to save the warped images ``` ## Future works -
-[x] Inference with GPU - [x] Inference with bulk of images - [ ] Inference with
-video - [ ] Introduce training procedure - [x] The matrix multiplication seems
-weird in function `postprocess`, may improve the computation. ## Citation
-```bibtex @inproceedings{silva2018license, title={License plate detection and
-recognition in unconstrained scenarios}, author={Silva, Sergio Montazzolli and
-Jung, Cl{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
+`wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/
+download/1.0.0/wpodnet.pth) 5. Predict with an image ```bash python3 predict.py
+docs/sample/original/03009.jpg # The path to the an image # docs/sample/
+original # OR the path to the directory with bulk of images -w weights/
+wpodnet.pth # The path to the weight --save-annotated docs/sample/annotated #
+The directory to save the annotated images --save-warped docs/sample/warped #
+The directory to save the warped images ``` ## Future works - [x] Inference
+with GPU - [x] Inference with bulk of images - [ ] Inference with video - [ ]
+Introduce training procedure - [x] The matrix multiplication seems weird in
+function `postprocess`, may improve the computation. ## Citation ```bibtex
+@inproceedings{silva2018license, title={License plate detection and recognition
+in unconstrained scenarios}, author={Silva, Sergio Montazzolli and Jung, Cl
+{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
 computer vision (ECCV)}, pages={580--596}, year={2018} } ```
```

### Comparing `wpodnet-pytorch-1.0.2/pyproject.toml` & `wpodnet-pytorch-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wpodnet-pytorch-1.0.2/wpodnet/backend.py` & `wpodnet-pytorch-1.0.3/wpodnet/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,20 +54,25 @@
     def _resize_to_fixed_ratio(self, image: Image.Image, dim_min: int, dim_max: int) -> Image.Image:
         h, w = image.height, image.width
 
         wh_ratio = max(h, w) / min(h, w)
         side = int(wh_ratio * dim_min)
         bound_dim = min(side + side % self._stride, dim_max)
 
-        factor = bound_dim / min(h, w)
+        factor = bound_dim / max(h, w)
         reg_w, reg_h = int(w * factor), int(h * factor)
 
         # Ensure the both width and height are the multiply of `self._stride`
-        reg_w += self._stride - reg_w % self._stride
-        reg_h += self._stride - reg_h % self._stride
+        reg_w_mod = reg_w % self._stride
+        if reg_w_mod > 0:
+            reg_w += self._stride - reg_w_mod
+
+        reg_h_mod = reg_h % self._stride
+        if reg_h_mod > 0:
+            reg_h += self._stride - reg_h % self._stride
 
         return image.resize((reg_w, reg_h))
 
     def _to_torch_image(self, image: Image.Image) -> torch.Tensor:
         tensor = to_tensor(image)
         return tensor.unsqueeze_(0)
```

### Comparing `wpodnet-pytorch-1.0.2/wpodnet/model.py` & `wpodnet-pytorch-1.0.3/wpodnet/model.py`

 * *Files identical despite different names*

### Comparing `wpodnet-pytorch-1.0.2/wpodnet/stream.py` & `wpodnet-pytorch-1.0.3/wpodnet/stream.py`

 * *Files identical despite different names*

### Comparing `wpodnet-pytorch-1.0.2/wpodnet_pytorch.egg-info/PKG-INFO` & `wpodnet-pytorch-1.0.3/wpodnet_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpodnet-pytorch
-Version: 1.0.2
+Version: 1.0.3
 Summary: The implementation of ECCV 2018 paper "License Plate Detection and Recognition in Unconstrained Scenarios" in PyTorch
 Author: Pandede
 Maintainer: Pandede
 Project-URL: Source, https://github.com/Pandede/WPODNet-Pytorch
 Keywords: python,ai,computer-vision,deep-learning,torch,object-detection,license-plate-recognition,wpod,wpod-net
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -73,15 +73,15 @@
     git clone https://github.com/Pandede/WPODNet-Pytorch.git
     ```
 2. Install [PyTorch](https://pytorch.org) depends on your environment.
 3. Install packages in `requirements.txt`
     ```bash
     pip3 install -r requirements.txt
     ```
-4. Download the pretrained weight `wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link)
+4. Download the pretrained weight `wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/download/1.0.0/wpodnet.pth)
 5. Predict with an image
     ```bash
     python3 predict.py  docs/sample/original/03009.jpg          # The path to the an image
                         # docs/sample/original                  # OR the path to the directory with bulk of images
                         -w weights/wpodnet.pth                  # The path to the weight
                         --save-annotated docs/sample/annotated  # The directory to save the annotated images
                         --save-warped docs/sample/warped        # The directory to save the warped images
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wpodnet-pytorch Version: 1.0.2 Summary: The
+Metadata-Version: 2.1 Name: wpodnet-pytorch Version: 1.0.3 Summary: The
 implementation of ECCV 2018 paper "License Plate Detection and Recognition in
 Unconstrained Scenarios" in PyTorch Author: Pandede Maintainer: Pandede
 Project-URL: Source, https://github.com/Pandede/WPODNet-Pytorch Keywords:
 python,ai,computer-vision,deep-learning,torch,object-detection,license-plate-
 recognition,wpod,wpod-net Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier:
@@ -32,21 +32,21 @@
 Warp perspective [./docs/sample/      [./docs/sample/      [./docs/sample/
                  warped/03009.jpg]    warped/03016.jpg]    warped/03025.jpg]
 Confidence       0.9841               0.9945               0.9979
 ## Quick Run 1. Clone this repository ```bash git clone https://github.com/
 Pandede/WPODNet-Pytorch.git ``` 2. Install [PyTorch](https://pytorch.org)
 depends on your environment. 3. Install packages in `requirements.txt` ```bash
 pip3 install -r requirements.txt ``` 4. Download the pretrained weight
-`wpodnet.pth` from [Google Drive](https://drive.google.com/file/d/
-1SPfJIgEBX6j0fQbQryQxRp_sHkEnJnKa/view?usp=share_link) 5. Predict with an image
-```bash python3 predict.py docs/sample/original/03009.jpg # The path to the an
-image # docs/sample/original # OR the path to the directory with bulk of images
--w weights/wpodnet.pth # The path to the weight --save-annotated docs/sample/
-annotated # The directory to save the annotated images --save-warped docs/
-sample/warped # The directory to save the warped images ``` ## Future works -
-[x] Inference with GPU - [x] Inference with bulk of images - [ ] Inference with
-video - [ ] Introduce training procedure - [x] The matrix multiplication seems
-weird in function `postprocess`, may improve the computation. ## Citation
-```bibtex @inproceedings{silva2018license, title={License plate detection and
-recognition in unconstrained scenarios}, author={Silva, Sergio Montazzolli and
-Jung, Cl{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
+`wpodnet.pth` from [here](https://github.com/Pandede/WPODNet-Pytorch/releases/
+download/1.0.0/wpodnet.pth) 5. Predict with an image ```bash python3 predict.py
+docs/sample/original/03009.jpg # The path to the an image # docs/sample/
+original # OR the path to the directory with bulk of images -w weights/
+wpodnet.pth # The path to the weight --save-annotated docs/sample/annotated #
+The directory to save the annotated images --save-warped docs/sample/warped #
+The directory to save the warped images ``` ## Future works - [x] Inference
+with GPU - [x] Inference with bulk of images - [ ] Inference with video - [ ]
+Introduce training procedure - [x] The matrix multiplication seems weird in
+function `postprocess`, may improve the computation. ## Citation ```bibtex
+@inproceedings{silva2018license, title={License plate detection and recognition
+in unconstrained scenarios}, author={Silva, Sergio Montazzolli and Jung, Cl
+{\'a}udio Rosito}, booktitle={Proceedings of the European conference on
 computer vision (ECCV)}, pages={580--596}, year={2018} } ```
```

