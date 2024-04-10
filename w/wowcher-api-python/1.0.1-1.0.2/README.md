# Comparing `tmp/wowcher_api_python-1.0.1.tar.gz` & `tmp/wowcher_api_python-1.0.2.tar.gz`

## Comparing `wowcher_api_python-1.0.1.tar` & `wowcher_api_python-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/requirements.txt
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/wowcher-api-python.iml
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/api.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/frame.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/mock/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/mock/api_mock.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/src/wowcher/mock/frame_mock.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/tests/test_api_methods.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/tests/test_payment_frame.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    11189 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/wowcher-api-python.iml
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/copilot/chatSessions/00000000000.xd
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/copilot/chatSessions/xd.lck
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/copilot/chatSessions/blobs/version
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/api.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/frame.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/mock/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/mock/api_mock.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/src/wowcher/mock/frame_mock.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/tests/test_api_methods.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/tests/test_payment_frame.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 wowcher_api_python-1.0.2/PKG-INFO
```

### Comparing `wowcher_api_python-1.0.1/.idea/workspace.xml` & `wowcher_api_python-1.0.2/.idea/workspace.xml`

 * *Files 10% similar despite different names*

#### Comparing `wowcher_api_python-1.0.1/.idea/workspace.xml` & `wowcher_api_python-1.0.2/.idea/workspace.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="609d03ef-8509-40dc-a5de-f71a89af005c" name="Changes" comment="v1.0.0"/>
+    <list default="true" id="609d03ef-8509-40dc-a5de-f71a89af005c" name="Changes" comment="v1.0.1"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -28,33 +28,33 @@
 }</component>
   <component name="ProjectId" id="2cuAhCcfsqqCxBbCmDmNfy1q9qn"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "Python tests.Python tests for test_api_methods.test_activate_voucher.executor": "Run",
-    "Python tests.Python tests for test_api_methods.test_activate_vouchers.executor": "Run",
-    "Python tests.Python tests for test_api_methods.test_activate_vouchers_400.executor": "Run",
-    "Python tests.Python tests for test_api_methods.test_activate_vouchers_500.executor": "Run",
-    "Python tests.Python tests for test_api_methods.test_activate_vouchers_list.executor": "Run",
-    "Python tests.Python tests for test_api_methods.test_activate_vouchers_without_error_message.executor": "Run",
-    "Python tests.Python tests for test_payment_frame.test_get_frame_url.executor": "Run",
-    "Python tests.Python tests in test_api_methods.py.executor": "Run",
-    "Python tests.Python tests in tests.executor": "Run",
-    "Python.test_api_methods.executor": "Run",
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "git-widget-placeholder": "master",
-    "last_opened_file_path": "/Users/sergeygavrilov/Work/wowcher/wowcher-api-python/src/wowcher-api-python",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;Python tests.Python tests for test_api_methods.test_activate_voucher.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_api_methods.test_activate_vouchers.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_api_methods.test_activate_vouchers_400.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_api_methods.test_activate_vouchers_500.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_api_methods.test_activate_vouchers_list.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_api_methods.test_activate_vouchers_without_error_message.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests for test_payment_frame.test_get_frame_url.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests in test_api_methods.py.executor&quot;: &quot;Run&quot;,
+    &quot;Python tests.Python tests in tests.executor&quot;: &quot;Run&quot;,
+    &quot;Python.test_api_methods.executor&quot;: &quot;Run&quot;,
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;master&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/sergeygavrilov/Work/wowcher/wowcher-api-python/src/wowcher-api-python&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/wowcher-api-python"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/wowcher/mock"/>
     </key>
@@ -181,28 +181,35 @@
       <option name="closed" value="true"/>
       <created>1711637609892</created>
       <option name="number" value="00003"/>
       <option name="presentableId" value="LOCAL-00003"/>
       <option name="project" value="LOCAL"/>
       <updated>1711637609892</updated>
     </task>
-    <option name="localTasksCounter" value="4"/>
+    <task id="LOCAL-00004" summary="add mock currency in response">
+      <option name="closed" value="true"/>
+      <created>1711638594410</created>
+      <option name="number" value="00004"/>
+      <option name="presentableId" value="LOCAL-00004"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1711638594410</updated>
+    </task>
+    <task id="LOCAL-00005" summary="v1.0.1">
+      <option name="closed" value="true"/>
+      <created>1711638639238</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1711638639238</updated>
+    </task>
+    <option name="localTasksCounter" value="6"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="init"/>
     <MESSAGE value="build fix"/>
     <MESSAGE value="v1.0.0"/>
-    <option name="LAST_COMMIT_MESSAGE" value="v1.0.0"/>
-  </component>
-  <component name="XDebuggerManager">
-    <breakpoint-manager>
-      <breakpoints>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/tests/test_api_methods.py</url>
-          <line>30</line>
-          <option name="timeStamp" value="3"/>
-        </line-breakpoint>
-      </breakpoints>
-    </breakpoint-manager>
+    <MESSAGE value="add mock currency in response"/>
+    <MESSAGE value="v1.0.1"/>
+    <option name="LAST_COMMIT_MESSAGE" value="v1.0.1"/>
   </component>
 </project>
```

### Comparing `wowcher_api_python-1.0.1/.idea/wowcher-api-python.iml` & `wowcher_api_python-1.0.2/.idea/wowcher-api-python.iml`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/.idea/copilot/chatSessions/00000000000.xd` & `wowcher_api_python-1.0.2/.idea/copilot/chatSessions/00000000000.xd`

 * *Files 4% similar despite different names*

```diff
@@ -335,8 +335,38 @@
 000014e0: 300d 380d 400d 480d 500d 580d 600d 680d  0.8.@.H.P.X.`.h.
 000014f0: 700d 780d 800d 880d 9014 6e00 8200 b00d  p.x.......n.....
 00001500: 980d b40d d80d f40e 180e 3700 d400 f501  ..........7.....
 00001510: 1e01 3d0e 560e 720e 960e ba0e d60e fa0f  ..=.V.r.........
 00001520: 1e0f 3f0f 680f 9414 760f c00f ec10 1810  ..?.h...v.......
 00001530: 4410 7010 9c10 c810 e911 1211 3f11 6b01  D.p.........?.k.
 00001540: 6401 8e01 c001 e311 9702 0e81 8085 23a9  d.............#.
-00001550: a913 ab                                  ...
+00001550: a913 ab86 aa84 8100 628a 82aa 8581 8202  ........b.......
+00001560: 1553 8681 8582 102a 5aaa 8681 918d 6578  .S.....*Z.....ex
+00001570: 6f64 7573 2e67 632e 7570 0000 80aa 8281  odus.gc.up......
+00001580: 2881 d224 8102 144b 0046 0c91 0c98 1452  (..$...K.F.....R
+00001590: 1459 0cad 0cb4 0070 0076 05f0 0cbb 1460  .Y.....p.v.....`
+000015a0: 1467 0cd0 0cd8 0ce0 0ce8 0cf0 0cf8 0d00  .g..............
+000015b0: 0d08 0d10 0d18 0d20 12b8 0d30 0d38 0d40  ....... ...0.8.@
+000015c0: 0d48 0d50 0d58 0d60 0d68 0d70 0d78 0d80  .H.P.X.`.h.p.x..
+000015d0: 0d88 0d90 146e 1562 0082 00b0 0d98 0db4  .....n.b........
+000015e0: 0dd8 0df4 0e18 0e37 00d4 00f5 011e 013d  .......7.......=
+000015f0: 0e56 0e72 0e96 0eba 0ed6 0efa 0f1e 0f3f  .V.r...........?
+00001600: 0f68 0f94 1476 0fc0 0fec 1018 1044 1070  .h...v.......D.p
+00001610: 109c 10c8 10e9 1112 113f 116b 0164 018e  .........?.k.d..
+00001620: 01c0 01e3 1197 156a 020e 8180 857e aaaa  .......j.....~..
+00001630: 6fac 868e 8c82 0006 8180 0001 8ec8 3df7  o.............=.
+00001640: de82 8e95 8992 0209 0c09 3809 6a09 7909  ..........8.j.y.
+00001650: 9309 a216 3209 c013 f786 9b8a 8880 0001  ....2...........
+00001660: 8ec8 3df7 de00 829b 8581 8202 1659 8681  ..=..........Y..
+00001670: 8481 0e41 ac86 8185 8210 1b66 ac82 8128  ...A.......f...(
+00001680: 81d2 2481 0214 4b00 460c 910c 9814 5214  ..$...K.F.....R.
+00001690: 590c ad0c b400 7000 7605 f00c bb16 6e14  Y.....p.v.....n.
+000016a0: 670c d00c d80c e00c e80c f00c f80d 000d  g...............
+000016b0: 080d 100d 180d 2016 750d 300d 380d 400d  ...... .u.0.8.@.
+000016c0: 480d 500d 580d 600d 680d 700d 780d 800d  H.P.X.`.h.p.x...
+000016d0: 880d 9014 6e15 6200 8200 b00d 980d b40d  ....n.b.........
+000016e0: d80d f40e 180e 3700 d400 f501 1e01 3d0e  ......7.......=.
+000016f0: 560e 720e 960e ba0e d60e fa0f 1e0f 3f0f  V.r...........?.
+00001700: 680f 9414 760f c00f ec10 1810 4410 7010  h...v.......D.p.
+00001710: 9c10 c810 e911 1211 3f11 6b01 6401 8e01  ........?.k.d...
+00001720: c001 e311 9715 6a02 0e81 8085 7dac aa6e  ......j.....}..n
+00001730: ae                                       .
```

### Comparing `wowcher_api_python-1.0.1/.idea/copilot/chatSessions/xd.lck` & `wowcher_api_python-1.0.2/.idea/copilot/chatSessions/xd.lck`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Private property of Exodus: 99878@MacBook-Pro-Sergey.local
+Private property of Exodus: 2163@MacBook-Pro-Sergey.local
 
 jetbrains.exodus.io.LockingManager.lock(LockingManager.kt:88)
 jetbrains.exodus.io.LockingManager.lock(LockingManager.kt:39)
 jetbrains.exodus.io.FileDataWriter.lock(FileDataWriter.kt:70)
 jetbrains.exodus.log.Log.tryLock(Log.kt:804)
 jetbrains.exodus.log.Log.<init>(Log.kt:117)
 jetbrains.exodus.env.Environments.newLogInstance(Environments.kt:117)
```

### Comparing `wowcher_api_python-1.0.1/.idea/inspectionProfiles/Project_Default.xml` & `wowcher_api_python-1.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/src/wowcher/api.py` & `wowcher_api_python-1.0.2/src/wowcher/api.py`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/tests/test_api_methods.py` & `wowcher_api_python-1.0.2/tests/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/tests/test_payment_frame.py` & `wowcher_api_python-1.0.2/tests/test_payment_frame.py`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/LICENSE` & `wowcher_api_python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wowcher_api_python-1.0.1/pyproject.toml` & `wowcher_api_python-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wowcher-api-python"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Self", email = "dev@self.team" },
 ]
 description = "Library for integration with Wowcher.App api application"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wowcher_api_python-1.0.1/PKG-INFO` & `wowcher_api_python-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wowcher-api-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for integration with Wowcher.App api application
 Project-URL: Homepage, https://github.com/dev-self-team/wowcher-api-python
 Project-URL: Issues, https://github.com/dev-self-team/wowcher-api-python/issues
 Author-email: Self <dev@self.team>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

