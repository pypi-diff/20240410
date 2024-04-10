# Comparing `tmp/deepepochs-0.5.8.tar.gz` & `tmp/deepepochs-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepepochs-0.5.8.tar", last modified: Wed Nov 29 15:11:58 2023, max compression
+gzip compressed data, was "deepepochs-0.5.9.tar", last modified: Thu Nov 30 06:34:33 2023, max compression
```

## Comparing `deepepochs-0.5.8.tar` & `deepepochs-0.5.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-29 15:11:58.860694 deepepochs-0.5.8/
--rw-r--r--   0 lic        (501) staff       (20)     1073 2023-10-19 06:32:23.000000 deepepochs-0.5.8/LICENSE
--rw-r--r--   0 lic        (501) staff       (20)     7418 2023-11-29 15:11:58.860570 deepepochs-0.5.8/PKG-INFO
--rw-r--r--   0 lic        (501) staff       (20)     6905 2023-11-26 06:29:15.000000 deepepochs-0.5.8/README.md
-drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-29 15:11:58.857891 deepepochs-0.5.8/deepepochs/
--rw-r--r--   0 lic        (501) staff       (20)      344 2023-11-29 14:04:24.000000 deepepochs-0.5.8/deepepochs/__init__.py
-drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-29 15:11:58.860228 deepepochs-0.5.8/deepepochs/callbacks/
--rw-r--r--   0 lic        (501) staff       (20)      279 2023-11-21 05:59:20.000000 deepepochs-0.5.8/deepepochs/callbacks/__init__.py
--rw-r--r--   0 lic        (501) staff       (20)     4555 2023-11-16 00:25:40.000000 deepepochs-0.5.8/deepepochs/callbacks/analyze.py
--rw-r--r--   0 lic        (501) staff       (20)    10035 2023-11-25 03:08:20.000000 deepepochs-0.5.8/deepepochs/callbacks/callback.py
--rw-r--r--   0 lic        (501) staff       (20)     5712 2023-11-29 07:41:31.000000 deepepochs-0.5.8/deepepochs/callbacks/check.py
--rw-r--r--   0 lic        (501) staff       (20)     5523 2023-11-29 08:04:20.000000 deepepochs-0.5.8/deepepochs/callbacks/default.py
--rw-r--r--   0 lic        (501) staff       (20)     5488 2023-11-21 02:55:23.000000 deepepochs-0.5.8/deepepochs/callbacks/interprete.py
--rw-r--r--   0 lic        (501) staff       (20)     4047 2023-11-25 16:19:53.000000 deepepochs-0.5.8/deepepochs/callbacks/log.py
--rw-r--r--   0 lic        (501) staff       (20)     1761 2023-11-16 00:22:52.000000 deepepochs-0.5.8/deepepochs/callbacks/lr_find.py
--rw-r--r--   0 lic        (501) staff       (20)     8573 2023-11-29 15:11:11.000000 deepepochs-0.5.8/deepepochs/loops.py
--rw-r--r--   0 lic        (501) staff       (20)     5421 2023-11-16 12:15:59.000000 deepepochs-0.5.8/deepepochs/metrics.py
--rw-r--r--   0 lic        (501) staff       (20)     2970 2023-11-15 03:43:00.000000 deepepochs-0.5.8/deepepochs/optimizer.py
--rw-r--r--   0 lic        (501) staff       (20)    12869 2023-11-25 05:41:57.000000 deepepochs-0.5.8/deepepochs/patches.py
--rw-r--r--   0 lic        (501) staff       (20)     8098 2023-11-16 12:52:06.000000 deepepochs-0.5.8/deepepochs/tools.py
--rw-r--r--   0 lic        (501) staff       (20)    25404 2023-11-29 07:37:57.000000 deepepochs-0.5.8/deepepochs/trainer.py
-drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-29 15:11:58.858484 deepepochs-0.5.8/deepepochs.egg-info/
--rw-r--r--   0 lic        (501) staff       (20)     7418 2023-11-29 15:11:58.000000 deepepochs-0.5.8/deepepochs.egg-info/PKG-INFO
--rw-r--r--   0 lic        (501) staff       (20)      603 2023-11-29 15:11:58.000000 deepepochs-0.5.8/deepepochs.egg-info/SOURCES.txt
--rw-r--r--   0 lic        (501) staff       (20)        1 2023-11-29 15:11:58.000000 deepepochs-0.5.8/deepepochs.egg-info/dependency_links.txt
--rw-r--r--   0 lic        (501) staff       (20)       72 2023-11-29 15:11:58.000000 deepepochs-0.5.8/deepepochs.egg-info/requires.txt
--rw-r--r--   0 lic        (501) staff       (20)       11 2023-11-29 15:11:58.000000 deepepochs-0.5.8/deepepochs.egg-info/top_level.txt
--rw-r--r--   0 lic        (501) staff       (20)       38 2023-11-29 15:11:58.860731 deepepochs-0.5.8/setup.cfg
--rw-r--r--   0 lic        (501) staff       (20)     1048 2023-11-25 03:52:53.000000 deepepochs-0.5.8/setup.py
+drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-30 06:34:33.987997 deepepochs-0.5.9/
+-rw-r--r--   0 lic        (501) staff       (20)     1073 2023-10-19 06:32:23.000000 deepepochs-0.5.9/LICENSE
+-rw-r--r--   0 lic        (501) staff       (20)     7418 2023-11-30 06:34:33.987877 deepepochs-0.5.9/PKG-INFO
+-rw-r--r--   0 lic        (501) staff       (20)     6905 2023-11-26 06:29:15.000000 deepepochs-0.5.9/README.md
+drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-30 06:34:33.986211 deepepochs-0.5.9/deepepochs/
+-rw-r--r--   0 lic        (501) staff       (20)      321 2023-11-30 06:34:24.000000 deepepochs-0.5.9/deepepochs/__init__.py
+drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-30 06:34:33.987725 deepepochs-0.5.9/deepepochs/callbacks/
+-rw-r--r--   0 lic        (501) staff       (20)      279 2023-11-21 05:59:20.000000 deepepochs-0.5.9/deepepochs/callbacks/__init__.py
+-rw-r--r--   0 lic        (501) staff       (20)     4555 2023-11-16 00:25:40.000000 deepepochs-0.5.9/deepepochs/callbacks/analyze.py
+-rw-r--r--   0 lic        (501) staff       (20)    11025 2023-11-30 05:23:23.000000 deepepochs-0.5.9/deepepochs/callbacks/callback.py
+-rw-r--r--   0 lic        (501) staff       (20)     5712 2023-11-29 07:41:31.000000 deepepochs-0.5.9/deepepochs/callbacks/check.py
+-rw-r--r--   0 lic        (501) staff       (20)     5523 2023-11-30 03:19:57.000000 deepepochs-0.5.9/deepepochs/callbacks/default.py
+-rw-r--r--   0 lic        (501) staff       (20)     5542 2023-11-30 05:31:28.000000 deepepochs-0.5.9/deepepochs/callbacks/interprete.py
+-rw-r--r--   0 lic        (501) staff       (20)     4047 2023-11-25 16:19:53.000000 deepepochs-0.5.9/deepepochs/callbacks/log.py
+-rw-r--r--   0 lic        (501) staff       (20)     1761 2023-11-16 00:22:52.000000 deepepochs-0.5.9/deepepochs/callbacks/lr_find.py
+-rw-r--r--   0 lic        (501) staff       (20)     8998 2023-11-30 04:56:49.000000 deepepochs-0.5.9/deepepochs/loops.py
+-rw-r--r--   0 lic        (501) staff       (20)     5421 2023-11-16 12:15:59.000000 deepepochs-0.5.9/deepepochs/metrics.py
+-rw-r--r--   0 lic        (501) staff       (20)     2970 2023-11-15 03:43:00.000000 deepepochs-0.5.9/deepepochs/optimizer.py
+-rw-r--r--   0 lic        (501) staff       (20)    12876 2023-11-30 03:53:34.000000 deepepochs-0.5.9/deepepochs/patches.py
+-rw-r--r--   0 lic        (501) staff       (20)     8098 2023-11-16 12:52:06.000000 deepepochs-0.5.9/deepepochs/tools.py
+-rw-r--r--   0 lic        (501) staff       (20)    29109 2023-11-30 06:32:40.000000 deepepochs-0.5.9/deepepochs/trainer.py
+drwxr-xr-x   0 lic        (501) staff       (20)        0 2023-11-30 06:34:33.986768 deepepochs-0.5.9/deepepochs.egg-info/
+-rw-r--r--   0 lic        (501) staff       (20)     7418 2023-11-30 06:34:33.000000 deepepochs-0.5.9/deepepochs.egg-info/PKG-INFO
+-rw-r--r--   0 lic        (501) staff       (20)      603 2023-11-30 06:34:33.000000 deepepochs-0.5.9/deepepochs.egg-info/SOURCES.txt
+-rw-r--r--   0 lic        (501) staff       (20)        1 2023-11-30 06:34:33.000000 deepepochs-0.5.9/deepepochs.egg-info/dependency_links.txt
+-rw-r--r--   0 lic        (501) staff       (20)       72 2023-11-30 06:34:33.000000 deepepochs-0.5.9/deepepochs.egg-info/requires.txt
+-rw-r--r--   0 lic        (501) staff       (20)       11 2023-11-30 06:34:33.000000 deepepochs-0.5.9/deepepochs.egg-info/top_level.txt
+-rw-r--r--   0 lic        (501) staff       (20)       38 2023-11-30 06:34:33.988035 deepepochs-0.5.9/setup.cfg
+-rw-r--r--   0 lic        (501) staff       (20)     1048 2023-11-25 03:52:53.000000 deepepochs-0.5.9/setup.py
```

### Comparing `deepepochs-0.5.8/LICENSE` & `deepepochs-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/PKG-INFO` & `deepepochs-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepepochs
-Version: 0.5.8
+Version: 0.5.9
 Summary: An easy-to-use tool for training Pytorch deep learning models
 Home-page: https://github.com/hitlic/deepepochs
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deepepochs-0.5.8/README.md` & `deepepochs-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/analyze.py` & `deepepochs-0.5.9/deepepochs/callbacks/analyze.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/callback.py` & `deepepochs-0.5.9/deepepochs/callbacks/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,45 @@
         on_before_fit
             on_before_epoch
                 on_before_train_epochs   # 多个训练任务
                     on_before_train_epoch
                         on_before_train_batch
                             on_before_train_forward
                             on_after_train_forward
-                            on_before_backward
-                            on_after_backward
-                            on_train_prediction
+                            on_before_train_loss
+                                on_before_backward
+                                on_after_backward
+                            on_after_train_loss
                         on_after_train_batch
                         ...
                     on_after_train_epoch
                 ...
                 on_after_train_epochs
                 on_before_val_epochs     # 多个验证任务
                     on_before_val_epoch
                         on_before_val_batch
                             on_before_val_forward
                             on_after_val_forward
-                            on_val_prediction
+                            on_before_val_loss
+                            on_after_val_loss
                         on_after_val_batch
                         ...
                     on_after_val_epoch
                     ...
                 on_after_val_epochs
             on_after_epoch
             ...
         on_after_fit
         on_before_test_epochs
             on_before_test_epoch
                 on_before_test_batch
                     on_before_test_forward
                     on_after_test_forward
-                    on_test_prediction
+                    on_before_test_loss
+                    on_after_test_loss
                 on_after_test_batch
                 ...
             on_after_test_epoch
             ...
         on_after_test_epochs
     """
     def __init__(self, priority=1):
@@ -113,27 +116,38 @@
     def on_after_train_forward(self, trainer, model_out):
         """
         Args:
             trainer:    Trainer
             model_out:  模型前向预测输出
         """
 
+    def on_before_train_loss(self, trainer, model_out, targets, task):
+        """
+        Args:
+            trainer:    Trainer
+            model_out:  模型前向预测输出
+            targets:    标签
+            task:       当前的EpochTask
+        """
+
     def on_before_backward(self, trainer, loss):
         """
         Args:
             trainer:  Trainer
+            loss:     loss
         """
 
     def on_after_backward(self, trainer, loss):
         """
         Args:
             trainer:  Trainer
+            loss:     loss
         """
 
-    def on_train_prediction(self, trainer, loss, model_out, targets, task):
+    def on_after_train_loss(self, trainer, loss, model_out, targets, task):
         """
         Args:
             trainer:    Trainer
             loss:       当前batch的损失
             model_out:  模型前向预测输出
             targets:    标签
             task:       当前的EpochTask
@@ -197,15 +211,24 @@
     def on_after_val_forward(self, trainer, model_out):
         """
         Args:
             trainer:    Trainer
             model_out:  模型前向预测输出
         """
 
-    def on_val_prediction(self, trainer, loss, model_out, targets, task):
+    def on_before_val_loss(self, trainer, model_out, targets, task):
+        """
+        Args:
+            trainer:    Trainer
+            model_out:  模型前向预测输出
+            targets:    标签
+            task:       当前的EpochTask
+        """
+
+    def on_after_val_loss(self, trainer, loss, model_out, targets, task):
         """
         Args:
             trainer:    Trainer
             loss:       当前batch的损失
             model_out:  模型前向预测输出
             targets:    标签
             task:       当前的EpochTask
@@ -281,15 +304,24 @@
     def on_after_test_forward(self, trainer, model_out):
         """
         Args:
             trainer:    Trainer
             model_out:  模型前向预测输出
         """
 
-    def on_test_prediction(self, trainer, loss, model_out, targets, task):
+    def on_before_test_loss(self, trainer, model_out, targets, task):
+        """
+        Args:
+            trainer:    Trainer
+            model_out:  模型前向预测输出
+            targets:    标签
+            task:       当前的EpochTask
+        """
+
+    def on_after_test_loss(self, trainer, loss, model_out, targets, task):
         """
         Args:
             trainer:    Trainer
             loss:       当前batch的损失
             model_out:  模型前向预测输出
             targets:    标签
             task:       当前的EpochTask
```

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/check.py` & `deepepochs-0.5.9/deepepochs/callbacks/check.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/default.py` & `deepepochs-0.5.9/deepepochs/callbacks/default.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,23 +70,23 @@
         self.global_test_epoch_idx += 1
 
     def on_after_test_batch(self, trainer, metrics, batch_idx):
         self.global_test_batch_idx += 1
         if self.log_batch and trainer.main_process:
             log_batch(metrics, self.global_test_epoch_idx+1, self.total_test_epochs, self.global_test_batch_idx, self.total_test_batchs, 'TEST', self.epoch_width, self.batch_width, self.round_to)
 
-    def on_train_prediction(self, trainer, loss, model_out, targets, task):
+    def on_after_train_loss(self, trainer, loss, model_out, targets, task):
         """当前task的每个指标构建Patch，并注入task.batch_patch_dict"""
         task.batch_patch_dict = self.make_patch_dict(trainer, loss, model_out, targets, task.metrics, 'train')
 
-    def on_val_prediction(self, trainer, loss, model_out, targets, task):
+    def on_after_val_loss(self, trainer, loss, model_out, targets, task):
         """当前task的每个指标构建Patch，并注入task.batch_patch_dict"""
         task.batch_patch_dict = self.make_patch_dict(trainer, loss, model_out, targets, task.metrics, 'val')
 
-    def on_test_prediction(self, trainer, loss, model_out, targets, task):
+    def on_after_test_loss(self, trainer, loss, model_out, targets, task):
         """当前task的每个指标构建Patch，并注入task.batch_patch_dict"""
         task.batch_patch_dict = self.make_patch_dict(trainer, loss, model_out, targets, task.metrics, 'test')
 
     def make_patch_dict(self, trainer, loss, model_out, targets, metrics, stage):
         b_size = torch.tensor(batch_size(model_out)).to(trainer.device)
         # Accelerate 分布式训练时，获取各Process的数据
         if trainer.accelerator is not None and stage!='train':  # 训练时仅在主线程上计算指标
```

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/interprete.py` & `deepepochs-0.5.9/deepepochs/callbacks/interprete.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,23 +70,23 @@
     def update_confusion_matrix(self, model_out):
         """更新混淆矩阵"""
         if self.confusion_matrix is None:
             self.confusion_matrix = confusion_matrix(model_out, self.batch_y, self.class_num)
         else:
             self.confusion_matrix += confusion_matrix(model_out, self.batch_y, self.class_num)
 
-    def on_after_train_forward(self, trainer, model_out):
+    def on_after_train_loss(self, trainer, loss, model_out, targets, task):
         if 'train' in self.stages:
             self.update_confusion_matrix(model_out)
 
-    def on_after_val_forward(self, trainer, model_out):
+    def on_after_val_loss(self, trainer, loss, model_out, targets, task):
         if 'val' in self.stages:
             self.update_confusion_matrix(model_out)
 
-    def on_after_test_forward(self, trainer, model_out):
+    def on_after_test_loss(self, trainer, loss, model_out, targets, task):
         if 'test' in self.stages:
             self.put_queue(model_out, self.batch_y, self.batch_x)
             self.update_confusion_matrix(model_out)
 
     def on_after_train_epochs(self, trainer, tasks, metrics, epoch_idx):
         if 'train' in self.stages:
             fig = self.plot_confusion(show=False)
```

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/log.py` & `deepepochs-0.5.9/deepepochs/callbacks/log.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/callbacks/lr_find.py` & `deepepochs-0.5.9/deepepochs/callbacks/lr_find.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/loops.py` & `deepepochs-0.5.9/deepepochs/loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,21 @@
         del self.__dict__[key]
 
     def __deepcopy__(self, memo=None, _nil=[]):  # pylint: disable=W0102
         dd = dict(self)
         return deepcopy(dd)
 
 
+def concat(datas):
+    if isinstance(datas[0], (list, tuple)):
+        return TensorTuple([torch.concat(ds, dim=0) if ds[0].dim()> 1 else torch.concat(ds) for ds in zip(*datas)])
+    else:
+        return torch.concat(datas, dim=0) if datas[0].dim() > 1 else torch.concat(datas)
+
+
 class TensorTuple(tuple):
     """
     tuple of tensors
     """
     def __new__(cls, tensors):
         if isinstance(tensors, torch.Tensor):
             tensors=(tensors,)
@@ -157,53 +164,57 @@
         batch_idx:   当前batch index
         batchs:      总batch数量
         stage:       train、val或test
         epoch_width: epoch的显示宽度
         batch_width: batch的显示宽度
         round_to:    指标值的小说保留位数
     """
+    if not metrics:  # metrics为空则不输出
+        return
     batch_info = info(metrics, round_to)
     epoch_width = 4 if epoch_width==0 else epoch_width
     batch_width = 4 if batch_width==0 else batch_width
     epoch_idx, epochs = str(epoch_idx).rjust(epoch_width), str(epochs).ljust(epoch_width)
     batch_idx, batchs = str(batch_idx).rjust(batch_width), str(batchs).ljust(batch_width)
-    print_out(f'E {epoch_idx}/{epochs}  B {batch_idx}/{batchs}  {stage}> {batch_info}{" "*10}', end='   ')  # 清除光标至行末字符
+    print_out(f'E {epoch_idx}/{epochs}  B {batch_idx}/{batchs}  {stage}> {batch_info}{" "*20}', end='   ')  # 清除光标至行末字符
 
 
 def log_epoch(stages_metrics, epoch_idx, epochs, epoch_width=0, round_to=4):
     """输出epoch指标值"""
+    if not stages_metrics:  # stages_metrics为空则不输出
+        return
     epoch_width = 4 if epoch_width==0 else epoch_width
     epoch_idx, epochs = str(epoch_idx).rjust(epoch_width), str(epochs).ljust(epoch_width)
 
     train_metrics = stages_metrics.get('train')
     val_metrics = stages_metrics.get('val')
     test_metrics = stages_metrics.get('test')
     if train_metrics is not None:
         train_info = info(train_metrics, round_to)
         val_info = ''
         if val_metrics is not None:
             val_info = info(val_metrics, round_to)
             val_info = '  VAL> ' + val_info
-        print_out(f'E {epoch_idx}/{epochs}  TRAIN> {train_info}{val_info}', end='   \n')  # 清除光标至行末字符
+        print_out(f'E {epoch_idx}/{epochs}  TRAIN> {train_info}{val_info}', end='\n')  # 清除光标至行末字符
     elif test_metrics is not None:
         test_info = info(test_metrics, round_to)
-        print_out(f'E {epoch_idx}/{epochs}  TEST> {test_info}{" "*20}', end='   \n')  # 清除光标至行末字符
+        print_out(f'E {epoch_idx}/{epochs}  TEST> {test_info}{" "*20}', end='\n')  # 清除光标至行末字符
     else:
         raise ValueError("log_epoch 参数错误!")
 
 
 def info(m_dict, round_to):
     def v_str(v):
         v = v.item() if isinstance(v, torch.Tensor) else v
         return f'{{:.{round_to}f}}'.format(v).ljust(round_to+3)
     return ' '.join([f'{k:>}: {v_str(v):<}' for k, v in m_dict.items()])
 
 
 def print_out(content, end='\n'):
-    print(end='\r\x1b[2K\r')  # \x1b[1K 清除行首至光标位置字符
+    print(end='\x1b[2K\r')  # \x1b[1K 清除行首至光标位置字符
     print(content, flush=True, sep='', end=end)
 
 
 def concat_dicts(dicts, to_np=True):
     if to_np:
         return {k: [to_numpy(d.get(k, 0)) for d in dicts] for k in keyset(dicts)}
     else:
```

### Comparing `deepepochs-0.5.8/deepepochs/metrics.py` & `deepepochs-0.5.9/deepepochs/metrics.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/optimizer.py` & `deepepochs-0.5.9/deepepochs/optimizer.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/patches.py` & `deepepochs-0.5.9/deepepochs/patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def run_patch_dicts(patch_dicts):
     """
     计算Patch字典的列表的指标值（计算Epoch指标）
     """
     if len(patch_dicts) == 0:
         return None
-    return {patch_name(k, patch_dicts[0][k]): sum(dic[k] for dic in patch_dicts)() for k in keyset(patch_dicts)}
+    return {patch_name(k, patch_dicts[0][k]): sum(dic[k] for dic in patch_dicts if dic)() for k in keyset(patch_dicts)}
 
 
 class PatchBase(abc.ABC):
     """
     所有Patch对象的基类
     """
     def __init__(self, name=None):
```

### Comparing `deepepochs-0.5.8/deepepochs/tools.py` & `deepepochs-0.5.9/deepepochs/tools.py`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/deepepochs/trainer.py` & `deepepochs-0.5.9/deepepochs/trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 @author: hitlic
 """
 from typing import List, Dict, Callable
 import torch
 from torch.optim import Adam
 from .loops import (StopLoopException, LoopException, TensorTuple,
-                    flatten_dict, default_loss, concat_dicts, to_numpy, listify)
+                    flatten_dict, default_loss, concat_dicts, to_numpy, listify, batch_size, concat)
+from .tools import batches
 from .optimizer import Optimizer, Optimizers
 from .patches import PatchBase, MeanPatch, TensorPatch, run_patch_dict, run_patch_dicts
 from collections import defaultdict
 from .callbacks import CallbackPool, DefaultCallback, CallbackException
 from torch.utils.data import DataLoader
 from datetime import datetime
 import time
@@ -177,14 +178,15 @@
         self.loss_fn = loss_fn
         self.trainer = trainer
         self.stage = None
         self.do_loss = None
         self.task = None
 
     def __call__(self, model_out, targets):
+        self.trainer.callbacks.trigger(f'before_{self.stage}_loss', trainer=self.trainer, model_out=model_out, targets=targets, task=self.task)
         if self.stage == 'train':
             self.trainer.opt.zero_grad()
             loss = self.loss_fn(model_out, targets)
             self.trainer.callbacks.trigger('before_backward', trainer=self, loss=loss)
             if self.trainer.accelerator is None:
                 loss.backward()
             else:       # accelerate的backward
@@ -194,15 +196,16 @@
         else:
             if self.do_loss:
                 loss = self.loss_fn(model_out, targets)
             else:
                 loss = None
         loss = None if loss is None else loss.detach().clone()
         model_out = TensorTuple(model_out).detach().clone()
-        self.trainer.callbacks.trigger(f'{self.stage}_prediction', trainer=self.trainer, loss=loss, model_out=model_out, targets=targets, task=self.task)
+        model_out = model_out[0] if len(model_out)==1 else model_out
+        self.trainer.callbacks.trigger(f'after_{self.stage}_loss', trainer=self.trainer, loss=loss, model_out=model_out, targets=targets, task=self.task)
         return loss
 
 
 class TrainerBase:
     def __init__(self, model,
                  loss=None,
                  opt=None,
@@ -514,15 +517,14 @@
               或
             dict: 键为指标名，值为封装了数据和指标函数的PatchBase子类对象
         """
         model_out = self.model(*batch_x)
         # self.loss是对Trainer中loss参数的封装，会自动调用opt.zero_grad、loss.backward、opt.step等方法
         self.loss(model_out, batch_y)
 
-
     def evaluate_step(self,
                       batch_x:[torch.Tensor, List[torch.Tensor]],
                       batch_y:[torch.Tensor, List[torch.Tensor]],
                       **step_args
                       ) -> Dict[str, PatchBase]:
         """
         TODO: 非常规验证或测试可修改本方法中的代码。也可以定义val_step方法或test_step方法。
@@ -535,7 +537,71 @@
               或
             dict: 键为指标名，值为封装了数据和指标函数的PatchBase子类对象
         """
         # self.model是对Trainer中model参数的封装，
         model_out = self.model(*batch_x)
         # self.loss是对Trainer中loss参数的封装，会自动调用opt.zero_grad、loss.backward、opt.step等方法
         self.loss(model_out, batch_y)
+
+
+class GradAccumulateTask(EpochTask):
+    """
+    累积梯度
+    """
+    def __init__(self, dataloader, accumulate_steps, metrics=None, do_loss=True, **step_args):
+        """
+        Args:
+            dataloader:       pytorch Dataloader
+            accumulate_steps: 梯度累积步数
+            metrics:          指标函数列表
+            do_loss:          验证和测试中是否计算据损失
+            step_args:        其他需要传递给`step`、`train_step`、`val_step`、`test_step`和`evaluate`方法的参数
+        """
+        super().__init__(dataloader, metrics, do_loss, **step_args)
+        if dataloader.batch_size % accumulate_steps != 0:
+            raise LoopException("batch_size必须能被accumulate_steps整除！")
+        self.dl_batch_size = dataloader.batch_size
+
+    def check(self):
+        if self.trainer.accelerator is not None:
+            accumulate_steps = self.trainer.accelerator.gradient_accumulation_steps
+        self.accumulate_steps = accumulate_steps
+        self.sub_batch_size = self.dl_batch_size//accumulate_steps
+
+    def step(self, batch_x, batch_y):
+        self.check()
+        loss_fn = self.trainer.loss.loss_fn
+        total_loss = 0
+        model_out_s = []
+
+        if self.trainer.accelerator is not None and self.stage == 'train':  # 使用accelerate实现
+            for sub_batch_x, sub_batch_y in zip(batches(batch_x, self.sub_batch_size), batches(batch_y, self.sub_batch_size)):
+                with self.trainer.accelerator.accumulate(self.trainer.model.model):
+                    model_out = self.model(*sub_batch_x)
+                    model_out_s.append(model_out)
+                    loss = loss_fn(model_out, sub_batch_y)
+                    self.trainer.accelerator.backward(loss)
+                    self.trainer.opt.step()
+                    self.trainer.opt.zero_grad()
+                    total_loss += loss.detach().clone() * batch_size(sub_batch_x)
+                    sub_loss = loss/self.accumulate_steps
+        else:                                                               # 实现
+            for sub_batch_x, sub_batch_y in zip(batches(batch_x, self.sub_batch_size), batches(batch_y, self.sub_batch_size)):
+                model_out = self.model(*sub_batch_x)
+                model_out_s.append(model_out)
+                if self.do_loss:
+                    loss = loss_fn(model_out, sub_batch_y)
+                    sub_loss = loss/self.accumulate_steps
+                    total_loss += loss.detach().clone() * batch_size(sub_batch_x)
+                if self.stage == 'train':
+                    sub_loss.backward()
+            if self.stage == 'train':
+                self.trainer.opt.step()
+                self.trainer.opt.zero_grad()
+
+        avg_loss = total_loss/batch_size(batch_x) if self.do_loss else None
+        model_outs = concat(model_out_s)
+        self.trainer.callbacks.trigger(f'before_{self.stage}_loss', trainer=self.trainer, model_out=model_outs, targets=batch_y, task=self)
+        if self.stage == 'train':
+            self.trainer.callbacks.trigger('after_backward', trainer=self, loss=avg_loss)
+            self.trainer.callbacks.trigger('before_backward', trainer=self, loss=avg_loss)
+        self.trainer.callbacks.trigger(f'after_{self.stage}_loss', trainer=self.trainer, loss=avg_loss, model_out=model_outs, targets=batch_y, task=self)
```

### Comparing `deepepochs-0.5.8/deepepochs.egg-info/PKG-INFO` & `deepepochs-0.5.9/deepepochs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepepochs
-Version: 0.5.8
+Version: 0.5.9
 Summary: An easy-to-use tool for training Pytorch deep learning models
 Home-page: https://github.com/hitlic/deepepochs
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deepepochs-0.5.8/deepepochs.egg-info/SOURCES.txt` & `deepepochs-0.5.9/deepepochs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepepochs-0.5.8/setup.py` & `deepepochs-0.5.9/setup.py`

 * *Files identical despite different names*

