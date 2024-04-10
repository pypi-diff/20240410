# Comparing `tmp/pybts-1.3.6.tar.gz` & `tmp/pybts-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.3.6.tar", max compression
+gzip compressed data, was "pybts-1.3.7.tar", max compression
```

## Comparing `pybts-1.3.6.tar` & `pybts-1.3.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0   157658 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-09 16:43:21.380304 pybts-1.3.6/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-09 16:43:21.380304 pybts-1.3.6/README.md
--rw-r--r--   0        0        0      423 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/board.py
--rw-r--r--   0        0        0     9589 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/board/server.py
--rw-r--r--   0        0        0     5897 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/builder.py
--rw-r--r--   0        0        0      548 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8666 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/composite.py
--rw-r--r--   0        0        0     2118 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5661 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/parallel.py
--rw-r--r--   0        0        0      944 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/selector.py
--rw-r--r--   0        0        0     2541 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/sequence.py
--rw-r--r--   0        0        0      182 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/composites/template.py
--rw-r--r--   0        0        0     3242 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/constants.py
--rw-r--r--   0        0        0     2482 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    16301 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/main.py
--rw-r--r--   0        0        0     6679 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/node.py
--rw-r--r--   0        0        0     1097 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/ref_file.py
--rw-r--r--   0        0        0      166 2024-04-09 16:43:21.384304 pybts-1.3.6/pybts/rl/__init__.py
--rw-r--r--   0        0        0      234 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/common.py
--rw-r--r--   0        0        0     2689 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/nodes.py
--rw-r--r--   0        0        0    13874 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/on_policy.py
--rw-r--r--   0        0        0      991 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-09 16:43:21.388304 pybts-1.3.6/pybts/templates/index.html
--rw-r--r--   0        0        0  1966405 2024-04-09 16:43:21.396304 pybts-1.3.6/pybts/templates/static/index-BUWP2os5.js
--rw-r--r--   0        0        0   320362 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/templates/static/index-BXdrQGHp.css
--rw-r--r--   0        0        0     1553 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/tree.py
--rw-r--r--   0        0        0     9006 2024-04-09 16:43:21.400304 pybts-1.3.6/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-09 16:43:21.400304 pybts-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-09 19:25:58.664790 pybts-1.3.7/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-09 19:25:58.664790 pybts-1.3.7/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-09 19:25:58.664790 pybts-1.3.7/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-09 19:25:58.664790 pybts-1.3.7/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-09 19:25:58.668789 pybts-1.3.7/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-09 19:25:58.668789 pybts-1.3.7/README.md
+-rw-r--r--   0        0        0      423 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/board/board.py
+-rw-r--r--   0        0        0     9589 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/board/server.py
+-rw-r--r--   0        0        0     5947 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/builder.py
+-rw-r--r--   0        0        0      548 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8666 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2118 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5661 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      944 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2541 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/sequence.py
+-rw-r--r--   0        0        0      182 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/composites/template.py
+-rw-r--r--   0        0        0     3243 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/constants.py
+-rw-r--r--   0        0        0     2579 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-09 19:25:58.668789 pybts-1.3.7/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    19885 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/main.py
+-rw-r--r--   0        0        0     7177 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/node.py
+-rw-r--r--   0        0        0     1097 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/ref_file.py
+-rw-r--r--   0        0        0      166 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/__init__.py
+-rw-r--r--   0        0        0      268 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/common.py
+-rw-r--r--   0        0        0     3810 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/nodes.py
+-rw-r--r--   0        0        0    13874 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0      991 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-09 19:25:58.672790 pybts-1.3.7/pybts/templates/index.html
+-rw-r--r--   0        0        0  1966405 2024-04-09 19:25:58.680790 pybts-1.3.7/pybts/templates/static/index-BUWP2os5.js
+-rw-r--r--   0        0        0   320362 2024-04-09 19:25:58.684790 pybts-1.3.7/pybts/templates/static/index-BXdrQGHp.css
+-rw-r--r--   0        0        0     1553 2024-04-09 19:25:58.684790 pybts-1.3.7/pybts/tree.py
+-rw-r--r--   0        0        0     9920 2024-04-09 19:25:58.684790 pybts-1.3.7/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-09 19:25:58.684790 pybts-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.3.7/PKG-INFO
```

### Comparing `pybts-1.3.6/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.3.7/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/README.assets/image-20240329031220580.png` & `pybts-1.3.7/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/README.assets/image-20240329031233459.png` & `pybts-1.3.7/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/README.assets/image-20240401211552611.png` & `pybts-1.3.7/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/README.assets/image-20240401211609525.png` & `pybts-1.3.7/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/README.md` & `pybts-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/board/board.py` & `pybts-1.3.7/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/board/server.py` & `pybts-1.3.7/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/builder.py` & `pybts-1.3.7/pybts/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,16 @@
                 Count,
                 RunningIsFailure,
                 RunningIsSuccess,
                 FailureIsSuccess,
                 FailureIsRunning,
                 SuccessIsFailure,
                 SuccessIsRunning,
+                Timeout,
+                Throttle
         )
 
         self.register_node(RefFile)
 
         # 且或非
         self.register('And', Sequence)
         self.register('Or', Selector)
```

### Comparing `pybts-1.3.6/pybts/composites/__init__.py` & `pybts-1.3.7/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/composite.py` & `pybts-1.3.7/pybts/composites/composite.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/condition_branch.py` & `pybts-1.3.7/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/parallel.py` & `pybts-1.3.7/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/ppa.py` & `pybts-1.3.7/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/selector.py` & `pybts-1.3.7/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/composites/sequence.py` & `pybts-1.3.7/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/constants.py` & `pybts-1.3.7/pybts/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,10 +106,10 @@
     预设键
     """
     ID = 'id'
     TYPE = 'type'
     STATUS = 'status'
     TAG = 'tag'
     BLACKBOARD = 'blackboard'
-    FEEDBACK_MESSAGES = 'feedback_message'
+    FEEDBACK_MESSAGES = 'feedback_messages'
     NAME = 'name'
     CHILDREN_COUNT = 'children_count'
```

### Comparing `pybts-1.3.6/pybts/converter.py` & `pybts-1.3.7/pybts/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         ctx = { }
         if self.node.context is not None:
             ctx.update(self.node.context)
         if self.node.attrs is not None:
             ctx.update(self.node.attrs)
         if context is not None:
             ctx.update(context)
+        for key in ctx:
+            if callable(ctx[key]):
+                ctx[key] = ctx[key]()
         return jinja2.Template(value).render(ctx)
 
     def list(self, value: typing.Any) -> typing.List[typing.Any]:
         if isinstance(value, str):
             return eval(self.render(value))
         elif isinstance(value, list):
             return value
```

### Comparing `pybts-1.3.6/pybts/decorators/nodes.py` & `pybts-1.3.7/pybts/decorators/nodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         Tick the child or bounce back with the original status if already completed.
 
         Yields:
             a reference to itself or a behaviour in it's child subtree
         """
         if self.final_status:
             # ignore the child
-            for node in py_trees.behaviour.Behaviour.tick(self):
+            for node in Node.tick(self):
                 yield node
         else:
             # tick the child
             for node in Decorator.tick(self):
                 yield node
 
     def terminate(self, new_status: Status) -> None:
@@ -250,14 +250,84 @@
             self.final_status = new_status
         else:
             self.logger.debug(
                     "{}.terminate({})".format(self.__class__.__name__, new_status)
             )
 
 
+class Timeout(Decorator):
+    """
+    Executes a child/subtree with a timeout.
+
+    A decorator that applies a timeout pattern to an existing behaviour.
+    If the timeout is reached, the encapsulated behaviour's
+    :meth:`~py_trees.behaviour.Behaviour.stop` method is called with
+    status :data:`~py_trees.common.Status.FAILURE` otherwise it will
+    simply directly tick and return with the same status
+    as that of it's encapsulated behaviour.
+    """
+
+    def __init__(self, duration: float = 5.0, **kwargs):
+        """
+        Init with the decorated child and a timeout duration.
+
+        Args:
+            child: the child behaviour or subtree
+            name: the decorator name
+            duration: timeout length in seconds
+        """
+        super(Timeout, self).__init__(**kwargs)
+        self.duration = duration
+        self.finish_time = 0.0
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.duration = self.converter.float(self.duration)
+
+    def reset(self):
+        super().reset()
+        self.finish_time = 0
+
+    def initialise(self) -> None:
+        """Reset the feedback message and finish time on behaviour entry."""
+        self.finish_time = self.get_time() + self.duration
+        self.feedback_message = ""
+
+    def update(self) -> Status:
+        """
+        Fail on timeout, or block / reflect the child's result accordingly.
+
+        Terminate the child and return
+        :data:`~py_trees.common.Status.FAILURE`
+        if the timeout is exceeded.
+
+        Returns:
+            the behaviour's new status :class:`~py_trees.common.Status`
+        """
+        current_time = self.get_time()
+        if (
+                self.decorated.status == Status.RUNNING
+                and current_time > self.finish_time
+        ):
+            self.feedback_message = "timed out"
+            self.logger.debug(
+                    "{}.update() {}".format(self.__class__.__name__, self.feedback_message)
+            )
+            # invalidate the decorated (i.e. cancel it), could also put this logic in a terminate() method
+            self.decorated.stop(Status.INVALID)
+            return Status.FAILURE
+        if self.decorated.status == Status.RUNNING:
+            self.feedback_message = "time still ticking ... [remaining: {}s]".format(
+                    self.finish_time - current_time
+            )
+        else:
+            self.feedback_message = "child finished before timeout triggered"
+        return self.decorated.status
+
+
 class Count(Decorator):
     """
     Count the number of times it's child has been ticked.
 
     This increments counters tracking the total number of times
     it's child has been ticked as well as the number of times it
     has landed in each respective state.
@@ -470,7 +540,46 @@
         if self.decorated.status == Status.SUCCESS:
             self.feedback_message = (
                     "success is running [%s]" % self.decorated.feedback_message
             )
             return Status.RUNNING
         self.feedback_message = self.decorated.feedback_message
         return self.decorated.status
+
+
+class Throttle(Decorator):
+    """
+    每隔一段时间才会触发一次子节点，其他时间直接返回之前的状态
+    """
+
+    def __init__(self, duration: float | str = 5.0, **kwargs):
+        """
+        Init with the decorated child and a timeout duration.
+
+        Args:
+            child: the child behaviour or subtree
+            name: the decorator name
+            duration: timeout length in seconds
+        """
+        super().__init__(**kwargs)
+        self.duration = duration
+        self.last_time = -float('inf')
+
+    def reset(self):
+        super().reset()
+        self.last_time = -float('inf')
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.duration = self.converter.float(self.duration)
+
+    def update(self) -> Status:
+        return self.decorated.status
+
+    def tick(self):
+        now_time = self.get_time()
+        if now_time - self.last_time >= self.duration:
+            self.last_time = now_time
+            yield from Decorator.tick(self)
+        else:
+            yield from Node.tick(self)
+
```

### Comparing `pybts-1.3.6/pybts/display.py` & `pybts-1.3.7/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/main.py` & `pybts-1.3.7/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/node.py` & `pybts-1.3.7/pybts/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -158,14 +158,25 @@
             return f'<{self.name} {attrs_str}/>'
         else:
             return f'<{self.name} {attrs_str}/>({len(self.children)})'
 
     def __repr__(self):
         return self.__str__()
 
+    def get_time(self) -> float:
+        """获取行为树时间，时间可以由context传入，可以是一个函数"""
+        if self.context is not None and 'time' in self.context:
+            if callable(self.context['time']):
+                return self.context['time']()
+            # 在context传递了time的情况下使用context里的时间，方便使用游戏时间
+            return self.context['time']
+        else:
+            import time
+            return time.monotonic()
+
 
 class Action(Node, ABC):
     """
     行为节点
     """
 
     def __init__(self, **kwargs):
```

### Comparing `pybts-1.3.6/pybts/ref_file.py` & `pybts-1.3.7/pybts/ref_file.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/rl/on_policy.py` & `pybts-1.3.7/pybts/rl/on_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/rl/tree.py` & `pybts-1.3.7/pybts/rl/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/templates/favicon.ico` & `pybts-1.3.7/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/templates/static/index-BUWP2os5.js` & `pybts-1.3.7/pybts/templates/static/index-BUWP2os5.js`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/templates/static/index-BXdrQGHp.css` & `pybts-1.3.7/pybts/templates/static/index-BXdrQGHp.css`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/tree.py` & `pybts-1.3.7/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.3.6/pybts/utility.py` & `pybts-1.3.7/pybts/utility.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,37 +36,51 @@
         return BT_NODE_TYPE.DECORATOR
     elif isinstance(node, Condition):
         return BT_NODE_TYPE.CONDITION
     else:
         return BT_NODE_TYPE.ACTION
 
 
-def bt_to_json(node: py_trees.behaviour.Behaviour, ignore_children: bool = False) -> dict:
+def bt_to_json(node: py_trees.behaviour.Behaviour,
+               ignore_children: bool = False,
+               ignore_attrs: list = None,
+               ignore_to_data: bool = False) -> dict:
     info = {
         'tag'     : node.__class__.__name__,
         'children': [],
         'data'    : {
             BT_PRESET_DATA_KEY.ID               : node.id.hex,
             BT_PRESET_DATA_KEY.STATUS           : node.status.name,
             BT_PRESET_DATA_KEY.TYPE             : bt_to_node_type(node),
             BT_PRESET_DATA_KEY.TAG              : node.__class__.__name__,
             BT_PRESET_DATA_KEY.FEEDBACK_MESSAGES: node.feedback_message,
             BT_PRESET_DATA_KEY.NAME             : node.name,
-            BT_PRESET_DATA_KEY.CHILDREN_COUNT   : len(node.children)
         },
     }
 
     if isinstance(node, Node):
         info['data'] = {
-            **info['data'],
-            **node.to_data(),
+            **info['data'], **node.attrs,
         }
+        if not ignore_to_data:
+            info['data'] = {
+                **info['data'],
+                **node.to_data(),
+            }
+
+    if ignore_attrs:
+        # 忽略某些键
+        for key in ignore_attrs:
+            if key in info['data']:
+                del info['data'][key]
 
     if not ignore_children:
-        info['children'] = [bt_to_json(child, ignore_children=ignore_children) for child in node.children]
+        info['children'] = [
+            bt_to_json(child, ignore_children=ignore_children, ignore_to_data=ignore_to_data, ignore_attrs=ignore_attrs)
+            for child in node.children]
     return info
 
 
 def bt_to_echarts_json(node: dict | py_trees.behaviour.Behaviour | ET.Element, ignore_children: bool = False) -> dict:
     if isinstance(node, py_trees.behaviour.Behaviour):
         node = bt_to_json(node, ignore_children=ignore_children)
     if isinstance(node, ET.Element):
@@ -95,33 +109,41 @@
     }
 
     if not ignore_children:
         d['children'] = [bt_to_echarts_json(child, ignore_children) for child in node['children']]
     return d
 
 
-def bt_to_xml_node(node: dict | py_trees.behaviour.Behaviour, ignore_children=False) -> ET.Element:
+def bt_to_xml_node(node: dict | py_trees.behaviour.Behaviour, ignore_children=False,
+                   ignore_attrs: list = None,
+                   ignore_to_data: bool = False) -> ET.Element:
     if isinstance(node, py_trees.behaviour.Behaviour):
-        node = bt_to_json(node, ignore_children=ignore_children)
+        node = bt_to_json(node, ignore_children=ignore_children, ignore_attrs=ignore_attrs,
+                          ignore_to_data=ignore_to_data)
     attribs = { key: str(value) for key, value in node['data'].items() }
     xml_node = ET.Element(node['tag'], attrib=attribs)
     if not ignore_children:
         for child in node['children']:
-            xml_node.append(bt_to_xml_node(child, ignore_children=ignore_children))
+            xml_node.append(bt_to_xml_node(child, ignore_children=ignore_children, ignore_attrs=ignore_attrs,
+                                           ignore_to_data=ignore_to_data))
     return xml_node
 
 
 def xml_node_to_string(xml_node: ET.Element) -> str:
     text = ET.tostring(xml_node, encoding='utf-8').decode('utf-8')
     text = minidom.parseString(text).toprettyxml(indent='    ').replace('<?xml version="1.0" ?>', '').strip()
     return text
 
 
-def bt_to_xml(node: dict | py_trees.behaviour.Behaviour, ignore_children=False) -> str:
-    xml_node = bt_to_xml_node(node, ignore_children=ignore_children)
+def bt_to_xml(node: dict | py_trees.behaviour.Behaviour, ignore_children=False,
+              ignore_attrs: list = None,
+              ignore_to_data: bool = False
+              ) -> str:
+    xml_node = bt_to_xml_node(node, ignore_children=ignore_children, ignore_attrs=ignore_attrs,
+                              ignore_to_data=ignore_to_data)
     return xml_node_to_string(xml_node)
 
 
 def xml_to_json(xml_node: ET.Element | str, ignore_children=False) -> dict:
     if isinstance(xml_node, str):
         xml_node = ET.fromstring(xml_node)
 
@@ -180,14 +202,16 @@
             return list(obj)  # Convert tuple to list
         elif isinstance(obj, uuid.UUID):
             return obj.hex  # Convert UUID to string
         elif isinstance(obj, set):
             return list(set)
         elif isinstance(obj, Status):
             return obj.value
+        elif callable(obj):
+            return obj()
         else:
             try:
                 import numpy as np
                 if isinstance(obj, np.integer):
                     return int(obj)
                 elif isinstance(obj, np.floating):
                     return float(obj)
@@ -254,9 +278,7 @@
 def camel_case_to_snake_case(name):
     """
     驼峰转蛇形
     :param name:
     :return:
     """
     return ''.join(['_' + i.lower() if i.isupper() else i for i in name]).lstrip('_')
-
-
```

### Comparing `pybts-1.3.6/pyproject.toml` & `pybts-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.3.6"
+version = "1.3.7"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.3.6/PKG-INFO` & `pybts-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.3.6
+Version: 1.3.7
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

